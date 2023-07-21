# Comparing `tmp/MTGProxyPrinter-0.24.1.tar.gz` & `tmp/MTGProxyPrinter-0.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MTGProxyPrinter-0.24.1.tar", last modified: Tue Jun 27 15:48:00 2023, max compression
+gzip compressed data, was "MTGProxyPrinter-0.25.0.tar", last modified: Fri Jul 21 11:42:30 2023, max compression
```

## Comparing `MTGProxyPrinter-0.24.1.tar` & `MTGProxyPrinter-0.25.0.tar`

### file list

```diff
@@ -1,265 +1,265 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/LICENSE.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.24.1/MANIFEST.in
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13399 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/entry_points.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      224 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-06-27 15:48:00.000000 MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8781 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/README.md
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/ThirdPartyLicenses.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/doc/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    44070 2023-06-27 15:46:22.000000 MTGProxyPrinter-0.24.1/doc/changelog.md
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3255 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/__main__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1437 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/app_dirs.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11170 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/application.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/argument_parser.py
--rw-r--r--   0 thomas    (1000) thomas    (1000)    34320 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/card_info_downloader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16632 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_downloader.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.057226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/csv_parsers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/re_parsers.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/_interface.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11404 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/card_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/compact_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/edit_document_settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/import_deck_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/load_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/move_cards.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/new_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/page_actions.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/replace_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4094 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/shuffle_document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/downloader_base.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/http_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2726 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/logger.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-06-27 15:47:02.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/meta_data.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/metered_file.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/missing_images_manager.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11180 2023-06-27 15:32:36.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/card_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    46173 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8066 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    32805 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb_migrations.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v2.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v3.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v4.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v5.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2023-05-03 12:03:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v6.sql
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    24223 2023-06-27 15:32:36.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    26031 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_loader.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1685 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    19124 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/imagedb.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/string_list.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/natsort.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/print.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2175 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/progress_meter.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.053226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.053226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.061226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      490 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.065227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      441 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.065227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/index.theme
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.053226 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/16/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/22/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7302 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/resources.qrc
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7266 2022-10-03 10:12:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/about_dialog.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6278 2022-04-03 09:13:06.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5746 2022-03-27 19:48:38.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3533 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5290 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1119 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4226 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4081 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3703 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5018 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3115 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    20314 2023-04-18 12:59:51.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10907 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/main_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1884 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_dialog.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16376 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_widget.ui
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8075 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    10340 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    25603 2022-10-31 20:16:56.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17043 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/settings.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8583 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/sqlite_helpers.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/stop_thread.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.069227 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    12951 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/add_card.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    21267 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/cache_cleanup_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14900 2023-06-27 15:34:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/central_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3626 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/common.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    31709 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/deck_import_wizard.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    11677 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/dialogs.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8278 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/about_dialog.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8445 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     8009 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4488 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5958 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1666 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5497 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/columnar.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5224 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/grouped.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4125 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     6843 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4337 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17319 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    14308 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1821 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_dialog.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    16398 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_widget.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13255 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    13804 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    30085 2023-06-27 15:47:53.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3670 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/item_delegates.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    26406 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/main_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7234 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_config_widget.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    24943 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_renderer.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5903 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/printing_filter_widgets.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)    17242 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/settings_window.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3913 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/units_and_sizes.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/mtg_proxy_printer/update_checker.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5835 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/pyproject.toml
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-06-27 15:48:00.073228 MTGProxyPrinter-0.24.1/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-06-27 13:00:20.000000 MTGProxyPrinter-0.24.1/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:30.002209 MTGProxyPrinter-0.25.0/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    34993 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.25.0/LICENSE.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      237 2022-10-15 17:05:45.000000 MTGProxyPrinter-0.25.0/MANIFEST.in
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.962209 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-07-21 11:42:29.000000 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13411 2023-07-21 11:42:29.000000 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-07-21 11:42:29.000000 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       66 2023-07-21 11:42:29.000000 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/entry_points.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      224 2023-07-21 11:42:29.000000 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       18 2023-07-21 11:42:29.000000 MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10237 2023-07-21 11:42:30.002209 MTGProxyPrinter-0.25.0/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8781 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/README.md
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    27152 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/ThirdPartyLicenses.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.962209 MTGProxyPrinter-0.25.0/doc/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    46542 2023-07-21 11:40:49.000000 MTGProxyPrinter-0.25.0/doc/changelog.md
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.962209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      746 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3259 2023-07-21 09:02:27.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/__main__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1437 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/app_dirs.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11435 2023-07-21 09:02:27.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/application.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2249 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/argument_parser.py
+-rw-r--r--   0 thomas    (1000) thomas    (1000)    34320 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/card_info_downloader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    16632 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_downloader.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.962209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-03-16 10:13:43.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8224 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10420 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/csv_parsers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11291 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/re_parsers.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.962209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       58 2023-01-19 15:35:22.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2515 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/_interface.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11725 2023-07-20 13:52:58.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/card_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/compact_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4742 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/edit_document_settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2287 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/import_deck_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2877 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/load_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5788 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/move_cards.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2922 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/new_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7232 2023-02-11 12:12:35.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/page_actions.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4449 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/replace_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4096 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/shuffle_document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3227 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/downloader_base.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9787 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/http_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2726 2023-05-23 12:22:18.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/logger.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      978 2023-07-21 11:40:48.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/meta_data.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3946 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/metered_file.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2792 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/missing_images_manager.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.966209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11685 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/card_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    47914 2023-07-21 11:17:01.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/carddb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8066 2023-06-27 12:52:01.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/carddb.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    32805 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/carddb_migrations.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      999 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v2.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1117 2022-03-31 17:25:56.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v3.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1784 2022-09-15 19:32:37.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v4.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1881 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v5.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1280 2023-05-03 12:03:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v6.sql
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    24988 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    28273 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document_loader.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1715 2023-07-21 11:17:01.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    19134 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/imagedb.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2452 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/string_list.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2484 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/natsort.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6761 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/print.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2175 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/progress_meter.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.966209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.958209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.966209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.958209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.990209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      457 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      766 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      504 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      652 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      573 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      546 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1010 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      689 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      543 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      942 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      507 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      917 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1336 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      417 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      695 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      694 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      423 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20688 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1248 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      490 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      644 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      263 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.994209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      904 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      567 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      555 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      472 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      755 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      807 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      498 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      450 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      955 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      465 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1179 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      788 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1182 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      432 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      596 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      667 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      663 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      495 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23995 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      500 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      503 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4255 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      441 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      914 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      413 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.994209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      478 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      938 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      996 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      601 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      698 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      589 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      664 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      506 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      789 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      841 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      532 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      484 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      989 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      499 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1213 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      822 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1216 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      466 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      630 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      701 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      697 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      529 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    23996 2022-09-15 19:31:29.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      534 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      537 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4289 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/list-add.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      948 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      447 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/viewpdf.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.994209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      421 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/application-exit.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      728 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      733 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      355 2022-04-03 17:17:45.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-ok.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      569 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      605 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      475 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-new.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      391 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-open.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      798 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      531 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      616 2022-03-07 18:29:18.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      973 2021-04-12 09:15:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      496 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-revert.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1094 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      665 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-delete.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      482 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-redo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      497 2022-04-03 13:05:49.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      332 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      331 2021-03-27 13:29:06.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      962 2022-10-02 19:41:47.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3231 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/index.theme
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.958209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.994209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/16/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      603 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/22/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      602 2022-03-02 10:53:38.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7302 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/resources.qrc
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7286 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/about_dialog.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6300 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5764 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3464 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5223 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1044 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4242 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4095 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3715 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5022 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3117 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20414 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1948 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/document_settings_dialog.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10905 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/main_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17516 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/page_config_widget.ui
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     7986 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    10303 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    25860 2023-07-19 21:18:39.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17474 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/settings.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8583 2023-06-27 10:53:13.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/sqlite_helpers.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1403 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/stop_thread.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2021-02-23 13:46:10.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    13006 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/add_card.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    20508 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    15066 2023-07-21 11:17:01.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/central_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5806 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/common.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    30980 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/deck_import_wizard.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    11649 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/dialogs.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8403 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/about_dialog.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/add_card_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8808 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8306 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4482 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6029 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1605 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:29.998209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5665 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5357 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/grouped.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4215 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:30.002209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     6923 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/load_list_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4360 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    18009 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2083 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/document_settings_dialog.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14224 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17110 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/page_config_widget.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:30.002209 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        0 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    12690 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/format_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    14717 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    31026 2023-07-21 11:42:20.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4139 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/item_delegates.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    26496 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/main_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     8099 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/page_config_widget.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    30428 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/page_renderer.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5824 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/printing_filter_widgets.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)    17229 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/settings_window.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     3913 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/units_and_sizes.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     9233 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/mtg_proxy_printer/update_checker.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     5835 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/pyproject.toml
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-07-21 11:42:30.002209 MTGProxyPrinter-0.25.0/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2832 2023-07-20 13:45:16.000000 MTGProxyPrinter-0.25.0/setup.py
```

### Comparing `MTGProxyPrinter-0.24.1/LICENSE.md` & `MTGProxyPrinter-0.25.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/PKG-INFO` & `MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.24.1
+Version: 0.25.0
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MTGProxyPrinter-0.24.1/MTGProxyPrinter.egg-info/SOURCES.txt` & `MTGProxyPrinter-0.25.0/MTGProxyPrinter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -172,16 +172,16 @@
 mtg_proxy_printer/resources/icons/breeze/actions/32/edit-undo.svg
 mtg_proxy_printer/resources/icons/breeze/actions/32/go-next.svg
 mtg_proxy_printer/resources/icons/breeze/actions/32/go-previous.svg
 mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg
 mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg
 mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg
 mtg_proxy_printer/resources/ui/about_dialog.ui
+mtg_proxy_printer/resources/ui/document_settings_dialog.ui
 mtg_proxy_printer/resources/ui/main_window.ui
-mtg_proxy_printer/resources/ui/page_config_dialog.ui
 mtg_proxy_printer/resources/ui/page_config_widget.ui
 mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui
 mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui
 mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui
 mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui
 mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui
 mtg_proxy_printer/resources/ui/central_widget/columnar.ui
@@ -204,16 +204,16 @@
 mtg_proxy_printer/ui/main_window.py
 mtg_proxy_printer/ui/page_config_widget.py
 mtg_proxy_printer/ui/page_renderer.py
 mtg_proxy_printer/ui/printing_filter_widgets.py
 mtg_proxy_printer/ui/settings_window.py
 mtg_proxy_printer/ui/generated/__init__.py
 mtg_proxy_printer/ui/generated/about_dialog.py
+mtg_proxy_printer/ui/generated/document_settings_dialog.py
 mtg_proxy_printer/ui/generated/main_window.py
-mtg_proxy_printer/ui/generated/page_config_dialog.py
 mtg_proxy_printer/ui/generated/page_config_widget.py
 mtg_proxy_printer/ui/generated/add_card_widget/__init__.py
 mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py
 mtg_proxy_printer/ui/generated/add_card_widget/vertical.py
 mtg_proxy_printer/ui/generated/cache_cleanup_wizard/__init__.py
 mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py
 mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py
```

### Comparing `MTGProxyPrinter-0.24.1/PKG-INFO` & `MTGProxyPrinter-0.25.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MTGProxyPrinter
-Version: 0.24.1
+Version: 0.25.0
 Summary: MTGProxyPrinter allows efficient printing of Magic: The Gathering cards for playtesting purposes.
 Author-email: Thomas Hess <thomas.hess@udo.edu>
 License: GNU GPLv3+, see LICENSE.md or https://www.gnu.org/licenses/gpl-3.0.html for details
 Project-URL: Homepage, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/index
 Project-URL: Bug tracker, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/ticket
 Project-URL: Changelog, https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter/doc/trunk/doc/changelog.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MTGProxyPrinter-0.24.1/README.md` & `MTGProxyPrinter-0.25.0/README.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/ThirdPartyLicenses.md` & `MTGProxyPrinter-0.25.0/ThirdPartyLicenses.md`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/doc/changelog.md` & `MTGProxyPrinter-0.25.0/doc/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,49 @@
 # Changelog
 
+# Version 0.25.0 (2023-07-21)  <a name="v0_25_0"></a>
+
+## New features
+
+- It is now possible to set a document name in the document settings.
+  If set, it is printed below the card images on each page.
+  This can help distinguish multiple stacks of uncut printed sheets.
+  (Long names may be truncated, if they do not fit on the page.)
+- Added option to print page numbers on each page. It is printed as `page-number / total-pages`, e.g. `2/3`.
+  You can use this to verify that a stack of uncut printed sheets is complete.
+  - This can be enabled by default for all documents in the application settings.
+- Translate cards already added to the document.
+    - You can now double-click the language cells in the table showing the cards on the current page to 
+      translate card in the document to another language.
+    - The opened drop-down menu will only show languages for which a printing is available.
+    - The translation tries to keep the same set and collector number, if available in the desired language,
+      otherwise falls back to a printing in another set. 
+
+## Changed features
+
+- Updated the print guessing heuristic in the deck import wizard that is used when it has to choose a printing
+  among multiple choices (for example, when requesting “`1 Island`”).
+  Now, it prefers slightly older printings with high-resolution 
+  images over the absolutely newest printings that do not yet have high-resolution scans available.
+  This should get better results for reprinted cards during “spoiler season”.
+- The Undo and Redo actions now have keyboard shortcuts assigned. They use the system-default shortcuts for
+  those actions, which are Ctrl+Z and Ctrl+Y on most systems and locales.  
+
+## Fixed issues
+
+- Fixed wrong cards being deleted when cards were selected from bottom to top and then deleted. Now, the selected cards
+  are removed regardless of selection order.
+- It is now possible to save and load documents containing DFC check cards. 
+  Those are no longer implicitly converted to the card front face in the saved document.
+  Loading documents containing DFC check cards with older program versions will fail.
+- Improvements/fixes for the multi-page wizards, like the deck import wizards
+    - Wizards now have a consistent style on Windows (7) and are properly centered above the main window
+    - Wizards are no longer placed partially out of the screen under some edge cases.  
+      The window title bar is now always visible.
+
 # Version 0.24.1 (2023-06-27)  <a name="v0_24_1"></a>
 
 ## Fixed issues
 
 - Fixed broken check card generation and addition of related cards. Both features failed to fetch the required images,
   rendering the cards as white rectangles, instead of the expected card images.
 - Fixed display of the 5th column in the table showing the cards on the current page. It shows whether the image is
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/__init__.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/__main__.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,28 @@
         import certifi
         logger.info("Use certifi library as SSL trust store for HTTPS connections")
         os.environ["SSL_CERT_FILE"] =  certifi.where()
 
 
 def main():
     global _app
-    mtg_proxy_printer.app_dirs.migrate_from_old_appdirs()
     arguments = mtg_proxy_printer.argument_parser.parse_args()
+    mtg_proxy_printer.app_dirs.migrate_from_old_appdirs()
     mtg_proxy_printer.logger.configure_root_logger()
     handle_ssl_certificates()
     # According to https://doc.qt.io/qt-5/qt.html#ApplicationAttribute-enum,
     # Qt.AA_EnableHighDpiScaling has to be set prior to creating the QApplication instance
     QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
     _app = mtg_proxy_printer.application.Application(arguments)
     if arguments.test_exit_on_launch:
         logger.info("Skipping startup tasks, because immediate application exit was requested.")
         QTimer.singleShot(0, _app.main_window.on_action_quit_triggered)
     else:
         logger.debug("Enqueueing startup tasks.")
-        _app.run_startup_tasks(arguments)
+        _app.enqueue_startup_tasks(arguments)
     logger.debug("Initialisation done. Starting event loop.")
     _app.exec_()
     logger.debug("Left event loop.")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/app_dirs.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/app_dirs.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/application.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 class Application(QApplication):
 
     def __init__(self, args: Namespace, argv: typing.List[str] = None):
         if argv is None:
             argv = sys.argv
-        logger.info("Starting MTGProxyPrinter")
+        logger.info(f"Starting MTGProxyPrinter version {meta_data.__version__}")
         if not os.getenv("QT_QPA_PLUGIN") and "-platform" not in argv and platform.system() == "Windows":
             logger.info("Running on Windows without explicit platform override. Enabling dark mode rendering.")
             # The explicit set platform and parameters overwrite the environment, so set these options iff neither
             # present as parameters nor environment variables.
             argv.append("-platform")
             argv.append("windows:darkmode=1")
         super(Application, self).__init__(argv)
@@ -74,18 +74,19 @@
         self.main_window.ui.action_download_card_data.setEnabled(self.card_db.allow_updating_card_data())
         self.settings_window = self._create_settings_window(
             self.language_model, self.document, self.main_window, self.card_info_downloader)
         self.main_window.show()
         self.update_checker = self._create_update_checker(args)
         self.main_window.should_update_languages.emit()
 
-    def run_startup_tasks(self, args: Namespace):
+    def enqueue_startup_tasks(self, args: Namespace):
         """
         Enqueues all tasks that should run in the Qt event loop at application start.
         Includes
+        - Settings migration and change-log display after application updates
         - checking for updates or undecided update policy settings
         - notifying on empty card database
         - running the card data import, if a JSON card data document is given as a command line argument
         - opening a document given via command line arguments
         - etc…
         """
         if settings.was_application_updated():
@@ -182,25 +183,28 @@
         # QIcon.fallbackThemeName() to be used.
         # On platforms without native icon theme support, both QIcon.themeName() and QIcon.fallbackThemeName()
         # return an empty string and no icons will load. These platforms require an explicit theme name set.
 
         # To test if the current platform has native icon theme support, check, if QIcon.fallbackThemeName() returns
         # a non-empty string. If it is empty, explicitly set the name of the internal icon theme. This will load the
         # internal icons.
-        if not QIcon.fallbackThemeName():
+        fallback_icon_theme = QIcon.fallbackThemeName()
+        if not fallback_icon_theme:
             logger.info(
                 "No native icon theme support or no system theme set, defaulting to internal icons."
             )
             if not mtg_proxy_printer.ui.common.HAS_COMPILED_RESOURCES:
                 # If the compiled resources are available, the default search path ":/icons" is sufficient. Only append
                 # the resources directory file system path, if directly running from the source distribution.
                 theme_search_paths = QIcon.themeSearchPaths()
                 theme_search_paths.append(mtg_proxy_printer.ui.common.ICON_PATH_PREFIX)
                 QIcon.setThemeSearchPaths(theme_search_paths)
             QIcon.setThemeName("breeze")
+        else:
+            logger.debug(f"Using system-provided icon theme '{fallback_icon_theme}'")
 
         self.setAttribute(Qt.AA_UseHighDpiPixmaps)
 
     @Slot()
     def quit(self):
         logger.info("About to exit.")
         self.update_checker.stop_background_worker()
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/argument_parser.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/argument_parser.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/card_info_downloader.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/card_info_downloader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_downloader.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_downloader.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/common.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/common.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/csv_parsers.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/csv_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/decklist_parser/re_parsers.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/decklist_parser/re_parsers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/_interface.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/_interface.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/card_actions.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/card_actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import functools
 import itertools
 import math
 import typing
 
-from mtg_proxy_printer.model.carddb import Card, CheckCard
+from mtg_proxy_printer.model.carddb import Card, AnyCardType
 if typing.TYPE_CHECKING:
     from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.model.document_page import CardContainer
 from ._interface import DocumentAction, IllegalStateError, Self
 from .page_actions import ActionNewPage, ActionRemovePage
 from mtg_proxy_printer.logger import get_logger
 
@@ -38,15 +38,15 @@
     """
     Add an amount of copies of a card to a document page. If the count exceeds the available space on that page,
     distribute the remainder across free spots on later pages or append new pages to the document end.
     """
 
     COMPARISON_ATTRIBUTES = ["card", "count", "added_new_pages", "added_cards_to_existing_pages"]
 
-    def __init__(self, card: typing.Union[Card, CheckCard], count: int = 1):
+    def __init__(self, card: AnyCardType, count: int = 1):
         self.card = card
         self.count = count
         self.added_new_pages: int = 0
         self.first_added_page: int = 0
         self.added_cards_to_existing_pages: typing.List[typing.Tuple[int, int]] = []
 
     def apply(self, document: "Document") -> Self:
@@ -163,14 +163,18 @@
     """Deletes one or more cards from a page. The cards are given as an ascendingly sorted sequence of array indices."""
 
     COMPARISON_ATTRIBUTES = ["card_ranges_to_remove", "page_number", "removed_cards"]
 
     def __init__(self, cards_to_remove: typing.Sequence[int], page_number: int = None):
         if not cards_to_remove:
             raise ValueError("Parameter cards_to_remove must not be empty")
+        # The source of the input row sequence is a Qt multi-selection, which is unordered.
+        # The individual selections are ordered, but the selection groups are not. To not break the algorithm,
+        # if the user selects cards from bottom to top, the rows have to be sorted.
+        cards_to_remove = sorted(cards_to_remove)
         self.card_ranges_to_remove = self.to_list_of_ranges(cards_to_remove)
         self.page_number = page_number
         self.removed_cards: typing.List[typing.List[CardContainer]] = []
 
     def apply(self, document: "Document") -> Self:
         if self.page_number is None:
             self.page_number = document.find_page_list_index(document.currently_edited_page)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/compact_document.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/compact_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/edit_document_settings.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/edit_document_settings.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/import_deck_list.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/import_deck_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/load_document.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/load_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/move_cards.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/move_cards.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/new_document.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/new_document.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/page_actions.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/page_actions.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/replace_card.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/replace_card.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/document_controller/shuffle_document.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/document_controller/shuffle_document.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from mtg_proxy_printer.model.document_page import CardContainer
 from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.units_and_sizes import PageType
 
 __all__ = [
     "ActionShuffleDocument",
 ]
-
+ItemDataRole = Qt.ItemDataRole
 IndexedCards = typing.List[typing.Tuple[int, Card]]
 ModelIndexList = typing.List[QModelIndex]
 
 
 class ActionShuffleDocument(DocumentAction):
     """
     Shuffle the cards in the current document.
@@ -58,15 +58,15 @@
         for page_type in (PageType.REGULAR, PageType.OVERSIZED):
             self._shuffle_pages_of_type(document, shuffler, page_type)
         return super().apply(document)
 
     def _shuffle_pages_of_type(self, document: Document, shuffler: Random, page_type: PageType):
         model_indices = list(document.get_card_indices_of_type(page_type))
         cards: IndexedCards = list(
-            enumerate(index.internalPointer().card for index in model_indices)  # The index holds the card container
+            enumerate(index.data(ItemDataRole.UserRole) for index in model_indices)
         )
         shuffler.shuffle(cards)
         self._swap_cards(document, model_indices, cards)
         self.shuffle_order[page_type] = [old_position for old_position, _ in cards]
 
     def undo(self, document: Document) -> Self:
         for page_type in (PageType.REGULAR, PageType.OVERSIZED):
@@ -75,15 +75,15 @@
         self.shuffle_order.clear()
         return self
 
     def _undo_shuffle_of_type(self, document: Document, page_type: PageType):
         model_indices = list(document.get_card_indices_of_type(page_type))
         cards: IndexedCards = list(zip(
             self.shuffle_order[page_type],
-            (index.internalPointer().card for index in model_indices)  # The index holds the card container
+            (index.data(ItemDataRole.UserRole) for index in model_indices)  # The index holds the card container
         ))
         cards.sort()
         self._swap_cards(document, model_indices, cards)
 
     @staticmethod
     def _swap_cards(document: Document, model_indices: ModelIndexList, cards: IndexedCards):
         rightmost_column = len(PageColumns)-1
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/downloader_base.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/downloader_base.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/http_file.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/http_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/logger.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/logger.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/meta_data.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/meta_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 PROGRAMNAME = "MTGProxyPrinter"
-__version__ = "0.24.1"
+__version__ = "0.25.0"
 COPYRIGHT = "(C) 2019-2023 Thomas Hess"
 HOME_PAGE = "https://chiselapp.com/user/luziferius/repository/MTGProxyPrinter"
 
 DOWNLOAD_WEB_PAGE = f"{HOME_PAGE}/uv/download.html"
 USER_AGENT = f"{PROGRAMNAME}/{__version__} ({HOME_PAGE})"
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/metered_file.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/metered_file.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/missing_images_manager.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/missing_images_manager.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/card_list.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/card_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import enum
 import itertools
 import typing
 
 from PyQt5.QtCore import QAbstractTableModel, QModelIndex, Qt, pyqtSlot as Slot, pyqtSignal as Signal, QItemSelection
 from PyQt5.QtGui import QIcon
 
-from mtg_proxy_printer.model.carddb import Card, CardIdentificationData, CardDatabase
+from mtg_proxy_printer.model.carddb import Card, CardIdentificationData, CardDatabase, AnyCardType
 from mtg_proxy_printer.logger import get_logger
 
 logger = get_logger(__name__)
 del get_logger
 CardList = typing.List[Card]
 
 __all__ = [
@@ -51,15 +51,15 @@
     header = {
         PageColumns.CardName: "Card name",
         PageColumns.Set: "Set",
         PageColumns.CollectorNumber: "Collector #",
         PageColumns.Language: "Language",
         PageColumns.IsFront: "Side",
     }
-    EDITABLE_COLUMNS = {PageColumns.Set, PageColumns.CollectorNumber}
+    EDITABLE_COLUMNS = {PageColumns.Set, PageColumns.CollectorNumber, PageColumns.Language}
 
     oversized_card_count_changed = Signal(int)
 
     def __init__(self, card_db: CardDatabase, *args, **kwargs):
         super(CardListModel, self).__init__(*args, **kwargs)
         self.card_db = card_db
         self.cards: CardList = []
@@ -70,14 +70,16 @@
         return 0 if parent.isValid() else len(self.cards)
 
     def columnCount(self, parent: QModelIndex = INVALID_INDEX) -> int:
         return 0 if parent.isValid() else len(CardListModel.header)
 
     def data(self, index: QModelIndex, role: int = Qt.DisplayRole) -> typing.Any:
         card = self.cards[index.row()]
+        if role == Qt.ItemDataRole.UserRole:
+            return card
         if role in (Qt.DisplayRole, Qt.EditRole):
             if index.column() == PageColumns.CardName:
                 return card.name
             elif index.column() == PageColumns.Set:
                 if role == Qt.EditRole:
                     return card.set.code
                 else:
@@ -99,35 +101,46 @@
     def flags(self, index: QModelIndex) -> Qt.ItemFlags:
         flags = super(CardListModel, self).flags(index)
         if index.column() in self.EDITABLE_COLUMNS:
             flags |= Qt.ItemIsEditable
         return flags
 
     def setData(self, index: QModelIndex, value: typing.Any, role: int = Qt.EditRole) -> bool:
-        if role == Qt.EditRole and index.column() in self.EDITABLE_COLUMNS:
-            logger.debug(f"Setting card list model data for column {index.column()} to {value}")
+        column = index.column()
+        if role == Qt.EditRole and column in self.EDITABLE_COLUMNS:
+            logger.debug(f"Setting card list model data for column {column} to {value}")
             card = self.cards[index.row()]
-            if index.column() == PageColumns.CollectorNumber:
+            if column == PageColumns.CollectorNumber:
                 card_data = CardIdentificationData(
                     card.language, card.name, card.set.code, value, is_front=card.is_front)
-            else:
+            elif column == PageColumns.Set:
                 card_data = CardIdentificationData(
                     card.language, card.name, value, is_front=card.is_front
                 )
+            else:
+                card_data = self.card_db.translate_card(card, value)
+                if card_data == card:
+                    return False
             return self._request_replacement_card(index, card_data)
         return False
 
-    def _request_replacement_card(self, index: QModelIndex, card_data: CardIdentificationData):
-        if result := self.card_db.get_cards_from_data(card_data):
+    def _request_replacement_card(
+            self, index: QModelIndex, card_data: typing.Union[CardIdentificationData, AnyCardType]):
+        if isinstance(card_data, CardIdentificationData):
             logger.debug(f"Requesting replacement for {card_data}")
+            result = self.card_db.get_cards_from_data(card_data)
+        else:
+            result = [card_data]
+        if result:
             # Simply choose the first match. The user can’t make a choice at this point, so just use one of
             # the results.
             new_card = result[0]
+            logger.debug(f"Replacing with {new_card}")
             top_left = index.sibling(index.row(), index.column())
-            bottom_right = top_left.siblingAtColumn(PageColumns.CollectorNumber)
+            bottom_right = top_left.siblingAtColumn(len(PageColumns)-2)
             old_card = self.cards[index.row()]
             self.cards[index.row()] = new_card
             self.dataChanged.emit(top_left, bottom_right, (Qt.DisplayRole, Qt.EditRole, Qt.ToolTipRole))
             # Oversized card count changes, iff the flags differ
             if old_card.is_oversized and not new_card.is_oversized:
                 self._remove_card_handle_oversized_flag(old_card)
             elif new_card.is_oversized and not old_card.is_oversized:
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/carddb.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 MINIMUM_REFRESH_DELAY = datetime.timedelta(days=14)
 
 __all__ = [
     "CardIdentificationData",
     "MTGSet",
     "CheckCard",
     "Card",
+    "AnyCardType",
     "CardCorner",
     "CardDatabase",
     "cached_dedent",
     "CardList",
     "OLD_DATABASE_LOCATION",
     "DEFAULT_DATABASE_LOCATION",
 ]
@@ -261,14 +262,18 @@
     visible: typing.List[typing.Tuple[Card, "CacheContent"]] = []
     hidden: typing.List[typing.Tuple[Card, "CacheContent"]] = []
     unknown: typing.List["CacheContent"] = []
 
 
 OptionalCard = typing.Optional[Card]
 CardList = typing.List[Card]
+AnyCardType = typing.Union[Card, CheckCard]
+# Py3.8 compatibility hack, because isinstance(a, AnyCardType) fails on 3.8
+AnyCardTypeForTypeCheck = typing.get_args(AnyCardType)
+T = typing.TypeVar("T", Card, CheckCard)
 
 
 @functools.lru_cache(None)
 def cached_dedent(text: str):
     """Wraps textwrap.dedent() in an LRU cache."""
     return textwrap.dedent(text)
 
@@ -470,14 +475,15 @@
             where_parameters.append(card.oracle_id)
         where_clause.append("")  # Insert final newline after joining
         query += "\n    ".join(where_clause)
         order_by_terms = []
         if order_by_print_count:
             order_by_terms.append("LastImageUseTimestamps.usage_count DESC NULLS LAST")
         order_by_terms.append("wackiness_score ASC")
+        order_by_terms.append("highres_image DESC")
         order_by_terms.append("release_date DESC")
         query += "ORDER BY " + "\n    ,".join(order_by_terms)
         result = self._get_cards_from_data(query, where_parameters)
         return result
 
     def get_replacement_card_for_unknown_printing(
             self, card: CardIdentificationData, /, *, order_by_print_count: bool = False) -> CardList:
@@ -700,24 +706,34 @@
             -- Assume English by default to not match other languages in case their entry misses the proper
             -- localisation and uses the English name as a fallback.
             ORDER BY "language" = 'en' DESC;
         ''')
         return self._read_optional_scalar_from_db(query, (name,))
 
     def is_known_language(self, language: str) -> bool:
-        """Returns true, if the given two-letter code is a known language. Returns False otherwise."""
+        """Returns True, if the given two-letter code is a known language. Returns False otherwise."""
         query = cached_dedent('''
         SELECT EXISTS( -- is_known_language()
             SELECT *
             FROM PrintLanguage
             WHERE "language" = ?
         )
         ''')
         return bool(self._read_optional_scalar_from_db(query, (language,)))
 
+    def is_dfc(self, scryfall_id: str) -> bool:
+        """Returns True, if the given card is a DFC, False otherwise."""
+        # This query returns two values for DFC cards, but that does not pose any issue
+        query = cached_dedent('''
+        SELECT is_dfc -- is_dfc()
+          FROM AllPrintings
+          WHERE "scryfall_id" = ?
+        ''')
+        return bool(self._read_optional_scalar_from_db(query, (scryfall_id,)))
+
     def translate_card_name(self, card_data: CardIdentificationData, target_language: str) -> OptionalString:
         """
         Translates a card into the target_language. Uses the language in the card data as the source language, if given.
         If not, card names across all languages are searched.
 
         :return: String with the translated card name, or None, if either unknown or unavailable in the target language.
         """
@@ -728,16 +744,16 @@
         # So if no context is given, this query performs a majority vote, because that is the most likely expected
         # result. But if context is given, either by the scryfall id or the set code, the exact, set-specific
         # translation is returned.
         query = cached_dedent("""\
         WITH  -- translate_card_name()
           source_context (source_scryfall_id, source_set_code) AS (SELECT ?, ?),
           source_oracle_id (oracle_id, face_number, source_likeliness, source_set_code) AS (
-            SELECT oracle_id, face_number, (
-                SELECT count() FROM Card)
+            SELECT oracle_id, face_number,
+                (SELECT count() FROM Card)
                   * (COALESCE(scryfall_id = source_scryfall_id, 0)
                      OR COALESCE(set_code = source_set_code, 0))
                   + count(oracle_id) AS source_likeliness,
                 set_code AS source_set_code
             FROM FaceName
             JOIN PrintLanguage USING (language_id)
             JOIN CardFace USING (face_name_id)
@@ -756,18 +772,36 @@
           WHERE language = ?
           GROUP BY card_name
           -- Some localized names were updated to fix typos and similar, so prefer the newest, matched name
           ORDER BY source_likeliness DESC, set_code = source_set_code DESC, release_date DESC
           LIMIT 1
         ;
         """)
-        return self._read_optional_scalar_from_db(
-            query,
-            (card_data.scryfall_id, card_data.set_code, card_data.name, card_data.language, target_language)
-        )
+        parameters = card_data.scryfall_id, card_data.set_code, card_data.name, card_data.language, target_language
+        return self._read_optional_scalar_from_db(query, parameters)
+
+    def get_available_languages_for_card(self, card: Card) -> StringList:
+        """
+        Returns the sorted list of languages the given card is available in.
+        This is used as the data source for the ComboBoxItemDelegate model
+        to generate the choices for translating cards in the document.
+        """
+        query = cached_dedent("""\
+        SELECT DISTINCT language 
+          FROM Card
+          JOIN Printing USING (card_id)
+          JOIN CardFace USING (printing_id)
+          JOIN FaceName USING (face_name_id)
+          JOIN PrintLanguage USING (language_id)
+          WHERE oracle_id = ?
+            AND Printing.is_hidden IS FALSE
+          ORDER BY language ASC;
+        """)
+        result = [item for item, in self.db.execute(query, (card.oracle_id,))]
+        return result
 
     def _read_optional_scalar_from_db(self, query: str, parameters: typing.Sequence[typing.Any]):
         if result := self.db.execute(query, parameters).fetchone():
             return result[0]
         else:
             return None
 
@@ -830,29 +864,34 @@
         query = cached_dedent("""\
         SELECT MAX(update_id), reported_card_count -- get_total_cards_in_last_update()
             FROM LastDatabaseUpdate
         """)
         id_, total_cards_in_last_update = self.db.execute(query).fetchone()
         return 0 if id_ is None else total_cards_in_last_update
 
-    def translate_card(self, to_translate: Card, target_language: str = None) -> Card:
+    def translate_card(self, to_translate: T, target_language: str = None) -> T:
         """
         Returns a new card object representing the card translated into the target language.
 
         The translation step tries to be as faithful as possible to the original printing by matching as many
         properties as possible, but may have to choose a printing another Magic set, if the source set does not
         contain the card in the desired language. For example, translating an Alpha printing of a card will always
         yield a Card in a different set. Also, multi-language support for printings of promotional cards in the Scryfall
         database is limited.
 
         If no translation is available, or the target language is equal to the source language, returns the given
         card instance unaltered.
         """
         if target_language is None or target_language == to_translate.language:
             return to_translate
+        if isinstance(to_translate, CheckCard):
+            return CheckCard(
+                (front := self.translate_card(to_translate.front, target_language)),
+                self.get_opposing_face(front)
+            )
         if (result := self._translate_card(to_translate, target_language)) is not None:
             return result
         return to_translate
 
     def _translate_card(self, card: Card, language_override: str) -> OptionalCard:
         """
         Tries to translate the given card into the given language.
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb.sql` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/carddb.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/carddb_migrations.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/carddb_migrations.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v2.sql` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v2.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v3.sql` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v3.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v4.sql` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v4.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v5.sql` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v5.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document-v6.sql` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document-v6.sql`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,36 +15,42 @@
 
 import collections
 import dataclasses
 import enum
 import itertools
 import math
 import pathlib
+import sys
 import textwrap
 import typing
 
 from PyQt5.QtCore import QAbstractItemModel, QModelIndex, Qt, pyqtSlot as Slot, pyqtSignal as Signal,\
     QPersistentModelIndex
 
 import mtg_proxy_printer.sqlite_helpers
 from mtg_proxy_printer.model.document_page import CardContainer, Page, PageList
 from mtg_proxy_printer.units_and_sizes import PageType
-from mtg_proxy_printer.model.carddb import Card, CardDatabase, CardIdentificationData
+from mtg_proxy_printer.model.carddb import AnyCardType, CardDatabase, CardIdentificationData
 from mtg_proxy_printer.model.card_list import PageColumns
 from mtg_proxy_printer.model.document_loader import DocumentLoader, DocumentSaveFormat, PageLayoutSettings, \
     CardType
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.logger import get_logger
 
 from mtg_proxy_printer.document_controller import DocumentAction
 from mtg_proxy_printer.document_controller.replace_card import ActionReplaceCard
 
 logger = get_logger(__name__)
 del get_logger
 
+if sys.version_info[:2] >= (3, 9):
+    Counter = collections.Counter
+else:
+    Counter = typing.Counter
+
 __all__ = [
     "Document",
 ]
 
 
 class DocumentColumns(enum.IntEnum):
     Page = 0
@@ -76,15 +82,15 @@
         PageColumns.CardName: "Card name",
         PageColumns.Set: "Set",
         PageColumns.CollectorNumber: "Collector #",
         PageColumns.Language: "Language",
         PageColumns.Image: "Image",
         PageColumns.IsFront: "Side",
     }
-    EDITABLE_COLUMNS = {PageColumns.Set, PageColumns.CollectorNumber}
+    EDITABLE_COLUMNS = {PageColumns.Set, PageColumns.CollectorNumber, PageColumns.Language}
 
     def __init__(self, card_db: CardDatabase, image_db: ImageDatabase, *args, **kwargs):
         super(Document, self).__init__(*args, **kwargs)
         self.undo_stack: ActionStack = collections.deque()
         self.redo_stack: ActionStack = collections.deque()
         self.save_file_path: typing.Optional[pathlib.Path] = None
         self.card_db = card_db
@@ -93,14 +99,16 @@
         self.loader.loading_state_changed.connect(self.loading_state_changed)
         self.loader.load_requested.connect(self.apply)
         self.pages: PageList = [first_page := Page()]
         # Mapping from page id() to list index in the page list
         self.page_index_cache: typing.Dict[int, int] = {id(first_page): 0}
         self.currently_edited_page = first_page
         self.page_layout = PageLayoutSettings.create_from_settings()
+        logger.debug(f"Loaded document settings from configuration file: {self.page_layout}")
+        logger.info(f"Created {self.__class__.__name__} instance")
 
     @Slot(DocumentAction)
     def apply(self, action: DocumentAction):
         if self.redo_stack:
             # Do not discard the rest redo stack if the top is equal to the given action
             if self.redo_stack.pop() != action:
                 self.redo_stack.clear()
@@ -212,32 +220,41 @@
             flags |= Qt.ItemIsEditable
         return flags
 
     def setData(self, index: QModelIndex, value: typing.Any, role: int = Qt.EditRole) -> bool:
         data = index.internalPointer()
         if isinstance(data, CardContainer) and role == Qt.EditRole and index.column() in self.EDITABLE_COLUMNS:
             logger.debug(f"Setting model data for column {index.column()} to {value}")
-            card: Card = index.internalPointer().card
-            if index.column() == PageColumns.CollectorNumber:
+            card = data.card
+            column = index.column()
+            if column == PageColumns.CollectorNumber:
                 card_data = CardIdentificationData(
                     card.language, card.name, card.set.code, value, is_front=card.is_front)
-            else:
+            elif column == PageColumns.Set:
                 card_data = CardIdentificationData(
                     card.language, card.name, value, is_front=card.is_front
                 )
+            else:
+                replacement = self.card_db.translate_card(card, value)
+                if replacement != card:
+                    action = ActionReplaceCard(replacement, index.parent().row(), index.row())
+                    self.request_fill_image_for_action.emit(action)
+                    return True
+                return False
             return self._request_replacement_card(index, card_data)
         return False
 
     def _request_replacement_card(self, index: QModelIndex, card_data: CardIdentificationData):
         if result := self.card_db.get_cards_from_data(card_data):
             logger.debug(f"Requesting replacement for card '{card_data.name}' in set {card_data.set_code}")
             # Simply choose the first match. The user can’t make a choice at this point, so just use one of
             # the results.
             new_card = result[0]
-            self.request_fill_image_for_action.emit(ActionReplaceCard(new_card, index.parent().row(), index.row()))
+            action = ActionReplaceCard(new_card, index.parent().row(), index.row())
+            self.request_fill_image_for_action.emit(action)
             return True
         return False
 
     def _data_page(self, index: QModelIndex, role: int = Qt.DisplayRole) -> typing.Any:
         """Returns the requested data for an index pointing to a page of Cards."""
         if index.row() >= self.rowCount():
             logger.error(f"Invalid index: {index.row()=}, {index.column()=}, {self.rowCount()=}, {index.isValid()=}")
@@ -256,15 +273,17 @@
         """Returns the requested data for an index pointing to a single Card."""
         parent = index.parent()
         if index.row() >= self.rowCount(parent) or index.column() >= self.columnCount(parent):
             logger.error(
                 f"Invalid index: {index.row()=}, {index.column()=}, "
                 f"{self.rowCount(index.parent())=}, {index.isValid()=}")
             return None
-        card: Card = index.internalPointer().card
+        card: AnyCardType = index.internalPointer().card
+        if role == Qt.ItemDataRole.UserRole:
+            return card
         if role in {Qt.DisplayRole, Qt.EditRole}:
             if index.column() == PageColumns.CardName:
                 return card.name
             elif index.column() == PageColumns.Set:
                 return card.set.data(role)
             elif index.column() == PageColumns.CollectorNumber:
                 return card.collector_number
@@ -294,28 +313,28 @@
         self.save_file_path = path
         self.save_to_disk()
 
     def save_to_disk(self):
         """Save the document at the internally remembered save path. Raises a RuntimeError, if no such path is set."""
         if self.save_file_path is None:
             raise RuntimeError("Cannot save without a file path!")
+        pages = enumerate(self.pages, start=1)
         cards = (
             zip(itertools.repeat(page_index), enumerate((
-                (container.card.scryfall_id, container.card.is_front) for container in page), start=1))
-            for page_index, page in enumerate(self.pages, start=1)
+                container.card for container in page), start=1))
+            for page_index, page in pages
         )
-        regular_card = CardType("r")
-        flattened_data: DocumentSaveFormat = (
-            (page, slot, scryfall_id, is_front, regular_card)
-            for (page, (slot, (scryfall_id, is_front)))
+        flattened_data: DocumentSaveFormat = [
+            (page, slot, card.scryfall_id, card.is_front, CardType.from_card(card))
+            for (page, (slot, card))
             in itertools.chain.from_iterable(cards)
             # TODO: For now, custom cards have an empty id. Until saving them is implemented, skip custom cards
             #   so that the document can still be loaded
-            if scryfall_id
-        )
+            if card.scryfall_id
+        ]
         with mtg_proxy_printer.sqlite_helpers.open_database(
                 self.save_file_path, "document-v6", self.loader.MIN_SUPPORTED_SQLITE_VERSION) as db:
             db.execute("BEGIN TRANSACTION")
             _migrate_database(db)
             db.execute("DELETE FROM Card")
             db.executemany(
                 "INSERT INTO Card (page, slot, scryfall_id, is_front, type) VALUES (?, ?, ?, ?, ?)",
@@ -333,15 +352,15 @@
             db.execute("VACUUM")
         logger.debug("Database saved and closed.")
 
     def compute_pages_saved_by_compacting(self) -> int:
         """
         Computes the number of pages that can be saved by compacting the document.
         """
-        cards = collections.Counter()
+        cards: Counter[PageType] = collections.Counter()
         for page in self.pages:
             cards[page.page_type()] += len(page)
         required_pages = (
             math.ceil(cards[PageType.OVERSIZED] / self.page_layout.compute_page_card_capacity(PageType.OVERSIZED))
             + math.ceil(cards[PageType.REGULAR] / self.page_layout.compute_page_card_capacity(PageType.REGULAR))
         ) or 1
         result = self.rowCount() - required_pages
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_loader.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,48 +21,59 @@
 import pathlib
 import sqlite3
 import textwrap
 import typing
 
 from PyQt5.QtCore import QObject, pyqtSignal as Signal, QThread
 from hamcrest import assert_that, all_of, instance_of, greater_than_or_equal_to, matches_regexp, is_in, \
-    has_properties, greater_than, is_
+    has_properties, greater_than, is_, equal_to
 
 try:
     from hamcrest import contains_exactly
 except ImportError:
     # Compatibility with PyHamcrest < 1.10
     from hamcrest import contains as contains_exactly
 
 import mtg_proxy_printer.settings
 import mtg_proxy_printer.sqlite_helpers
-from mtg_proxy_printer.model.carddb import CardDatabase, CardIdentificationData, CardList
+from mtg_proxy_printer.model.carddb import CardDatabase, CardIdentificationData, CardList, Card, CheckCard, AnyCardType
 from mtg_proxy_printer.model.imagedb import ImageDatabase, ImageDownloader
 from mtg_proxy_printer.stop_thread import stop_thread
 from mtg_proxy_printer.logger import get_logger
 from mtg_proxy_printer.units_and_sizes import PageType, CardSize, CardSizes
 from mtg_proxy_printer.document_controller import DocumentAction
 
 if typing.TYPE_CHECKING:
     from mtg_proxy_printer.model.document import Document
 logger = get_logger(__name__)
 del get_logger
 
 __all__ = [
     "DocumentSaveFormat",
     "DocumentLoader",
-    "PageLayoutSettings"
+    "PageLayoutSettings",
+    "CardType",
 ]
 
 # ASCII encoded 'MTGP' for 'MTG proxies'. Stored in the Application ID file header field of the created save files
 SAVE_FILE_MAGIC_NUMBER = 41325044
 
 
 class CardType(str, enum.Enum):
     REGULAR = "r"
+    CHECK_CARD = "d"
+
+    @classmethod
+    def from_card(cls, card: AnyCardType) -> "CardType":
+        if isinstance(card, Card):
+            return cls.REGULAR
+        elif isinstance(card, CheckCard):
+            return cls.CHECK_CARD
+        else:
+            raise NotImplementedError()
 
 
 DocumentSaveFormat = typing.List[typing.Tuple[int, int, str, bool, CardType]]
 T = typing.TypeVar("T")
 
 
 def split_iterable(iterable: typing.Iterable[T], chunk_size: int, /) -> typing.Iterable[typing.Tuple[T, ...]]:
@@ -70,30 +81,34 @@
     iterable = iter(iterable)
     return iter(lambda: tuple(itertools.islice(iterable, chunk_size)), ())
 
 
 @dataclasses.dataclass
 class PageLayoutSettings:
     """Stores all page layout attributes, like paper size, margins and spacings"""
+    document_name: str = ""
     draw_cut_markers: bool = False
+    draw_page_numbers: bool = False
     draw_sharp_corners: bool = False
     image_spacing_horizontal: int = 0
     image_spacing_vertical: int = 0
     margin_bottom: int = 0
     margin_left: int = 0
     margin_right: int = 0
     margin_top: int = 0
     page_height: int = 0
     page_width: int = 0
 
     @classmethod
     def create_from_settings(cls):
         document_settings = mtg_proxy_printer.settings.settings["documents"]
         return cls(
+            document_settings["default-document-name"],
             document_settings.getboolean("print-cut-marker"),
+            document_settings.getboolean("print-page-numbers"),
             document_settings.getboolean("print-sharp-corners"),
             document_settings.getint("image-spacing-horizontal-mm"),
             document_settings.getint("image-spacing-vertical-mm"),
             document_settings.getint("margin-bottom-mm"),
             document_settings.getint("margin-left-mm"),
             document_settings.getint("margin-right-mm"),
             document_settings.getint("margin-top-mm"),
@@ -219,14 +234,15 @@
         self.worker.cancel_running_operations()
 
     def quit_background_thread(self):
         if self.worker_thread.isRunning():
             logger.info(f"Quitting {self.__class__.__name__} background worker thread")
             stop_thread(self.worker_thread, logger)
 
+
 class Worker(QObject):
     """
     This is the worker object that runs inside the DocumentLoader’s internal QThread.
     It creates ActionLoadDocument instances from saved documents.
     """
 
     finished = Signal()
@@ -306,23 +322,33 @@
             "prefer-already-downloaded-images")
 
         current_page_index = 1
         unknown_ids = 0
         migrated_ids = 0
         pages: typing.List[CardList] = [[]]
         current_page = pages[-1]
-        for page_number, slot, scryfall_id, is_front, _ in card_data:
+        for page_number, slot, scryfall_id, is_front, card_type in card_data:
             if not self.should_run:
                 logger.info("Cancel request received, stop processing the card list.")
                 return unknown_ids, migrated_ids
             if current_page_index != page_number:
                 current_page_index = page_number
                 current_page: CardList = []
                 pages.append(current_page)
-            card = self.card_db.get_card_with_scryfall_id(scryfall_id, is_front)
+            if card_type == CardType.CHECK_CARD:
+                if not self.card_db.is_dfc(scryfall_id):
+                    logger.warning("Requested loading check card for non-DFC card, skipping it.")
+                    self.unknown_ids += 1
+                    continue
+                card = CheckCard(
+                    self.card_db.get_card_with_scryfall_id(scryfall_id, True),
+                    self.card_db.get_card_with_scryfall_id(scryfall_id, False)
+                )
+            else:
+                card = self.card_db.get_card_with_scryfall_id(scryfall_id, is_front)
             if card is None:
                 card = self._find_replacement_card(scryfall_id, is_front, prefer_already_downloaded)
                 if card:
                     migrated_ids += 1
                 else:
                     # If the save file was tampered with or the database used to save contained more cards than the
                     # currently used one, the save may contain unknown Scryfall IDs. So skip all unknown data.
@@ -419,83 +445,105 @@
         elif user_version == 6:
             query = textwrap.dedent("""\
                 SELECT page, slot, scryfall_id, is_front, type
                     FROM Card
                     ORDER BY page ASC, slot ASC""")
         else:
             raise AssertionError(f"Unknown database schema version: {user_version}")
+        supported_card_types: typing.List[str] = list(item.value for item in CardType)
         for row_number, row_data in enumerate(db.execute(query)):
             assert_that(row_data, contains_exactly(
                 all_of(instance_of(int), greater_than_or_equal_to(0)),
                 all_of(instance_of(int), greater_than_or_equal_to(0)),
                 all_of(instance_of(str), matches_regexp(r"[0-9a-f]{8}-([0-9a-f]{4}-){3}[0-9a-f]{12}")),
                 is_in((0, 1)),
-                is_in(("r",))  # Currently only regular cards (r) supported
+                is_in(supported_card_types)
             ), f"Invalid data found in the save data at row {row_number}. Aborting")
             page, slot, scryfall_id, is_front, card_type = row_data
             card_data.append((page, slot, scryfall_id, bool(is_front), CardType(card_type)))
         return card_data
 
     @staticmethod
     def _read_page_layout_data_from_database(db, user_version):
         default_settings = PageLayoutSettings.create_from_settings()
         if user_version in {4, 5}:
-            settings = Worker._read_document_settings_version_4_5(db, default_settings, user_version)
+            settings = Worker._read_document_settings_version_4_5(db, default_settings)
         elif user_version == 6:
             settings = Worker._read_document_settings_version_6(db, default_settings)
         else:
             settings = default_settings
+        logger.debug(f"Loaded document settings: {settings}")
         return settings
 
     @staticmethod
     def _read_document_settings_version_4_5(
-            db: sqlite3.Connection, default_settings: PageLayoutSettings, user_version: int) -> PageLayoutSettings:
+            db: sqlite3.Connection, default_settings: PageLayoutSettings) -> PageLayoutSettings:
+        logger.debug("Reading legacy document settings …")
+        stored_keys_query = textwrap.dedent("""\
+        SELECT p.name AS column_name  -- _read_document_settings_version_4_5
+            FROM sqlite_schema AS s
+            JOIN pragma_table_info(s.name) AS p
+            WHERE s.type = 'table'
+              AND s.name = ?
+              AND column_name <> 'rowid'
+        """)
+        required_keys = default_settings.__annotations__.keys()
+        stored_keys = {
+            key for key, in db.execute(stored_keys_query, ('DocumentSettings',))
+            if key in default_settings.__annotations__  # Ignore potentially dropped settings
+        }
+        # Use the actual column names found in the save database, use ? for all settings not stored, so that they can
+        # be substituted with the defaults
+        query_columns = ((key if key in stored_keys else '?') for key in required_keys)
+        # Default values for settings not found in the save file
+        default_values_for_settings_not_in_the_save_file = list(
+            getattr(default_settings, key) for key in required_keys if key not in stored_keys)
         document_settings_query = textwrap.dedent(f"""\
-            SELECT
-                draw_cut_markers, 
-                {int(default_settings.draw_sharp_corners) if user_version == 4 else 'draw_sharp_corners'},
-                image_spacing_horizontal, image_spacing_vertical, 
-                margin_bottom, margin_left, margin_right, margin_top,
-                page_height, page_width
-                FROM DocumentSettings
-                WHERE rowid == 1
-            """)
+            SELECT {', '.join(query_columns)}
+              FROM DocumentSettings
+              WHERE rowid == 1
+        """)
         assert_that(
             db.execute("SELECT COUNT(*) FROM DocumentSettings").fetchone(),
             contains_exactly(1),
         )
-        settings = PageLayoutSettings(*db.execute(document_settings_query).fetchone())
+        settings = PageLayoutSettings(*db.execute(
+            document_settings_query, default_values_for_settings_not_in_the_save_file).fetchone())
         assert_that(
             settings,
             has_properties(
+                document_name=equal_to(default_settings.document_name),
                 page_height=all_of(instance_of(int), greater_than(0)),
                 page_width=all_of(instance_of(int), greater_than(0)),
                 margin_top=all_of(instance_of(int), greater_than_or_equal_to(0)),
                 margin_bottom=all_of(instance_of(int), greater_than_or_equal_to(0)),
                 margin_left=all_of(instance_of(int), greater_than_or_equal_to(0)),
                 margin_right=all_of(instance_of(int), greater_than_or_equal_to(0)),
                 image_spacing_horizontal=all_of(instance_of(int), greater_than_or_equal_to(0)),
                 image_spacing_vertical=all_of(instance_of(int), greater_than_or_equal_to(0)),
                 draw_cut_markers=is_in((0, 1)),
                 draw_sharp_corners=is_in((0, 1)),
+                draw_page_numbers=is_in((0, 1)),
             ),
             "Document settings contain invalid data or data types"
         )
         assert_that(
             settings.compute_page_card_capacity(),
             is_(greater_than_or_equal_to(1)),
             "Document settings invalid: At least one card has to fit on a page."
         )
-        settings.draw_cut_markers = bool(settings.draw_cut_markers)
-        settings.draw_sharp_corners = bool(settings.draw_sharp_corners)
+        for key, expected_type in settings.__annotations__.items():
+            if expected_type is bool:
+                setattr(settings, key, bool(getattr(settings, key)))
         return settings
 
     @staticmethod
     def _read_document_settings_version_6(
             db: sqlite3.Connection, default_settings: PageLayoutSettings) -> PageLayoutSettings:
+        logger.debug("Reading document settings …")
         keys = ", ".join(map("'{}'".format, default_settings.__annotations__.keys()))
         document_settings_query = textwrap.dedent(f"""\
             SELECT key, value
                 FROM DocumentSettings
                 WHERE key in ({keys})
                 ORDER BY key ASC
             """)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/document_page.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/document_page.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,36 +12,36 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import dataclasses
 import typing
 
-from mtg_proxy_printer.model.carddb import Card, CheckCard
+from mtg_proxy_printer.model.carddb import AnyCardType, AnyCardTypeForTypeCheck
 from mtg_proxy_printer.units_and_sizes import PageType
 
 
 @dataclasses.dataclass
 class CardContainer:
     parent: "Page"
-    card: Card
+    card: AnyCardType
 
 
 class Page(typing.List[CardContainer]):
 
     def page_type(self) -> PageType:
         if not self:
             return PageType.UNDETERMINED
         found_types = set(container.card.requested_page_type() for container in self)
         if found_types == {PageType.REGULAR}:
             return PageType.REGULAR
         if found_types == {PageType.OVERSIZED}:
             return PageType.OVERSIZED
         return PageType.MIXED
 
-    def accepts_card(self, card: typing.Union[Card, CheckCard, PageType]) -> bool:
-        other_type = card.requested_page_type() if isinstance(card, (Card, CheckCard)) else card
+    def accepts_card(self, card: typing.Union[AnyCardType, PageType]) -> bool:
+        other_type = card.requested_page_type() if isinstance(card, AnyCardTypeForTypeCheck) else card
         own_page_type = self.page_type()
         return other_type == own_page_type or own_page_type is PageType.UNDETERMINED
 
 
 PageList = typing.List[Page]
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/imagedb.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/imagedb.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,31 +21,31 @@
 import pathlib
 import shutil
 import socket
 import string
 import typing
 import urllib.error
 
-from PyQt5.QtCore import QObject, pyqtSignal as Signal, pyqtSlot as Slot, QThread, QSize, QModelIndex
+from PyQt5.QtCore import QObject, pyqtSignal as Signal, pyqtSlot as Slot, QThread, QSize, QModelIndex, Qt
 from PyQt5.QtGui import QPixmap, QColor
 
 from mtg_proxy_printer.document_controller.card_actions import ActionAddCard
 from mtg_proxy_printer.document_controller.replace_card import ActionReplaceCard
 from mtg_proxy_printer.document_controller.import_deck_list import ActionImportDeckList
 from mtg_proxy_printer.document_controller import DocumentAction
 import mtg_proxy_printer.app_dirs
 import mtg_proxy_printer.downloader_base
 import mtg_proxy_printer.http_file
-from mtg_proxy_printer.model.carddb import Card, CheckCard
+from mtg_proxy_printer.model.carddb import Card, CheckCard, AnyCardType
 from mtg_proxy_printer.stop_thread import stop_thread
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
-
+ItemDataRole = Qt.ItemDataRole
 DEFAULT_DATABASE_LOCATION = mtg_proxy_printer.app_dirs.data_directories.user_cache_path / "CardImages"
 __all__ = [
     "ImageDatabase",
     "ImageDownloader",
     "CacheContent",
     "ImageKey",
 ]
@@ -272,16 +272,16 @@
 
     @Slot(list)
     def obtain_missing_images(self, card_indices: typing.List[QModelIndex]):
         logger.debug(f"Requesting {len(card_indices)} missing images")
         blank = self.image_database.blank_image
         self.update_batch_processing_state(True)
         for index in card_indices:
-            card = index.internalPointer().card
-            self.get_image_synchronous(index.internalPointer().card)
+            card = index.data(ItemDataRole.UserRole)
+            self.get_image_synchronous(card)
             if card.image_file is not blank:
                 self.missing_image_obtained.emit(index)
         self.update_batch_processing_state(False)
         logger.debug("Done fetching missing images.")
         self.missing_images_obtained.emit()
 
     @Slot(bool)
@@ -300,15 +300,15 @@
             f"Image download failed for card {card}, reason is \"{reason_str}\". Using blank replacement image.")
         # Only return the error message for storage, if the queue currently processes a batch job.
         # Otherwise, it’ll be re-raised if a batch job starts right after a singular request failed.
         if not self.batch_processing_state:
             self.network_error_occurred.emit(reason_str)
         return reason_str
 
-    def get_image_synchronous(self, card: typing.Union[Card, CheckCard]):
+    def get_image_synchronous(self, card: AnyCardType):
         try:
             if isinstance(card, CheckCard):
                 self._get_image_synchronous(card.front)
                 self._get_image_synchronous(card.back)
             else:
                 self._get_image_synchronous(card)
         except urllib.error.URLError as e:
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/model/string_list.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/model/string_list.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/natsort.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/natsort.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/print.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/print.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/progress_meter.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/progress_meter.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-open.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/16/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/22/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/dialog-ok.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-new.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-clear-history.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-download.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/format-align-vertical-top.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/globe.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-next.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/go-previous.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/help-contents.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/24/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/configure.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/dialog-cancel.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-close.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-import.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print-direct.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-print.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-properties.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-replace.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/document-save.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/actions/32/shuffle.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/index.theme` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/index.theme`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/16/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/icons/breeze/status/22/data-warning.svg`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/resources.qrc` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/resources.qrc`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/about_dialog.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/about_dialog.ui`

 * *Files 0% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/about_dialog.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/about_dialog.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>Dialog</class>
-  <widget class="QDialog" name="Dialog">
+  <class>AboutDialog</class>
+  <widget class="QDialog" name="AboutDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>800</width>
         <height>600</height>
       </rect>
@@ -186,15 +186,15 @@
     </layout>
   </widget>
   <resources/>
   <connections>
     <connection>
       <sender>buttonBox</sender>
       <signal>accepted()</signal>
-      <receiver>Dialog</receiver>
+      <receiver>AboutDialog</receiver>
       <slot>accept()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>248</x>
           <y>254</y>
         </hint>
         <hint type="destinationlabel">
@@ -202,15 +202,15 @@
           <y>274</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>buttonBox</sender>
       <signal>rejected()</signal>
-      <receiver>Dialog</receiver>
+      <receiver>AboutDialog</receiver>
       <slot>reject()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>316</x>
           <y>260</y>
         </hint>
         <hint type="destinationlabel">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/horizontal.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>AddCardWidget</class>
-  <widget class="QWidget" name="AddCardWidget">
+  <class>AddCardWidget_Horizontal</class>
+  <widget class="QWidget" name="AddCardWidget_Horizontal">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>1242</width>
         <height>292</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/add_card_widget/vertical.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>AddCardWidget</class>
-  <widget class="QWidget" name="AddCardWidget">
+  <class>AddCardWidget_Vertical</class>
+  <widget class="QWidget" name="AddCardWidget_Vertical">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>349</width>
         <height>715</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui`

 * *Files 6% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/card_filter_page.ui`

```diff
@@ -1,22 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WizardPage</class>
-  <widget class="QWizardPage" name="WizardPage">
+  <class>CardFilterPage</class>
+  <widget class="QWizardPage" name="CardFilterPage">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>406</width>
         <height>568</height>
       </rect>
     </property>
-    <property name="windowTitle">
-      <string>WizardPage</string>
-    </property>
     <property name="title">
       <string>Select images for removal</string>
     </property>
     <property name="subTitle">
       <string>Click on entries in the tables below to mark or un-mark them for removal. All selected entries will be removed.</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout_3">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui`

 * *Files 5% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/filter_setup_page.ui`

```diff
@@ -1,22 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WizardPage</class>
-  <widget class="QWizardPage" name="WizardPage">
+  <class>FilterSetupPage</class>
+  <widget class="QWizardPage" name="FilterSetupPage">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>417</width>
         <height>186</height>
       </rect>
     </property>
-    <property name="windowTitle">
-      <string>WizardPage</string>
-    </property>
     <property name="title">
       <string>Cleanup locally stored card images</string>
     </property>
     <property name="subTitle">
       <string>This wizard can be used to remove unwanted card images currently stored on your computer. You can enable automatic cleanup conditions below, to preselect images for removal.</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui`

 * *Files 14% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/cache_cleanup_wizard/summary_page.ui`

```diff
@@ -1,22 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WizardPage</class>
-  <widget class="QWizardPage" name="WizardPage">
+  <class>SummaryPage</class>
+  <widget class="QWizardPage" name="SummaryPage">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>266</width>
         <height>90</height>
       </rect>
     </property>
-    <property name="windowTitle">
-      <string>WizardPage</string>
-    </property>
     <property name="title">
       <string>Summary</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
         <widget class="QLabel" name="image_count_summary">
           <property name="text">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/columnar.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/columnar.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/columnar.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>central_widget</class>
-  <widget class="QWidget" name="central_widget">
+  <class>CentralWidget_Columnar</class>
+  <widget class="QWidget" name="CentralWidget_Columnar">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>888</width>
         <height>258</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/grouped.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui`

 * *Files 6% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/grouped.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/grouped.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>central_widget</class>
-  <widget class="QWidget" name="central_widget">
+  <class>CentralWidget_Grouped</class>
+  <widget class="QWidget" name="CentralWidget_Grouped">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>580</width>
         <height>539</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui`

 * *Files 10% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>central_widget</class>
-  <widget class="QWidget" name="central_widget">
+  <class>CentralWidget_Tabbed</class>
+  <widget class="QWidget" name="CentralWidget_Tabbed">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>454</width>
         <height>765</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/load_list_page.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WizardPage</class>
-  <widget class="QWizardPage" name="WizardPage">
+  <class>LoadListPage</class>
+  <widget class="QWizardPage" name="LoadListPage">
     <property name="enabled">
       <bool>true</bool>
     </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/parser_result_page.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WizardPage</class>
-  <widget class="QWizardPage" name="WizardPage">
+  <class>SummaryPage</class>
+  <widget class="QWizardPage" name="SummaryPage">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>440</width>
         <height>278</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui`

 * *Files 2% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/deck_import_wizard/select_deck_parser_page.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>WizardPage</class>
-  <widget class="QWizardPage" name="WizardPage">
+  <class>SelectDeckParserPage</class>
+  <widget class="QWizardPage" name="SelectDeckParserPage">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>767</width>
         <height>596</height>
       </rect>
@@ -333,15 +333,15 @@
           <y>261</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_mtg_arena</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>20</x>
           <y>20</y>
         </hint>
         <hint type="destinationlabel">
@@ -349,15 +349,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_mtg_online</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>26</x>
           <y>51</y>
         </hint>
         <hint type="destinationlabel">
@@ -365,15 +365,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_scryfall_csv</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>32</x>
           <y>139</y>
         </hint>
         <hint type="destinationlabel">
@@ -381,15 +381,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_custom_re</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>44</x>
           <y>223</y>
         </hint>
         <hint type="destinationlabel">
@@ -397,15 +397,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_xmage</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>32</x>
           <y>111</y>
         </hint>
         <hint type="destinationlabel">
@@ -413,15 +413,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>custom_re_input</sender>
       <signal>textChanged(QString)</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>247</x>
           <y>261</y>
         </hint>
         <hint type="destinationlabel">
@@ -429,15 +429,15 @@
           <y>114</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_tappedout_csv</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>145</x>
           <y>167</y>
         </hint>
         <hint type="destinationlabel">
@@ -573,15 +573,15 @@
           <y>342</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>select_parser_magic_workstation</sender>
       <signal>clicked()</signal>
-      <receiver>WizardPage</receiver>
+      <receiver>SelectDeckParserPage</receiver>
       <slot>isComplete()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>383</x>
           <y>72</y>
         </hint>
         <hint type="destinationlabel">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/main_window.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/main_window.ui`

 * *Files 2% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/main_window.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/main_window.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>main_window</class>
-  <widget class="QMainWindow" name="main_window">
+  <class>MainWindow</class>
+  <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>1050</width>
         <height>700</height>
       </rect>
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_dialog.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/document_settings_dialog.ui`

 * *Files 5% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_dialog.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/document_settings_dialog.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>Dialog</class>
-  <widget class="QDialog" name="Dialog">
+  <class>DocumentSettingsDialog</class>
+  <widget class="QDialog" name="DocumentSettingsDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>501</width>
         <height>300</height>
       </rect>
@@ -42,15 +42,15 @@
     </customwidget>
   </customwidgets>
   <resources/>
   <connections>
     <connection>
       <sender>button_box</sender>
       <signal>accepted()</signal>
-      <receiver>Dialog</receiver>
+      <receiver>DocumentSettingsDialog</receiver>
       <slot>accept()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>248</x>
           <y>254</y>
         </hint>
         <hint type="destinationlabel">
@@ -58,15 +58,15 @@
           <y>274</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>button_box</sender>
       <signal>rejected()</signal>
-      <receiver>Dialog</receiver>
+      <receiver>DocumentSettingsDialog</receiver>
       <slot>reject()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>316</x>
           <y>260</y>
         </hint>
         <hint type="destinationlabel">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_widget.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/page_config_widget.ui`

 * *Files 4% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/page_config_widget.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/page_config_widget.ui`

```diff
@@ -1,316 +1,358 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>page_configuration_group_box</class>
-  <widget class="QGroupBox" name="page_configuration_group_box">
+  <class>PageConfigWidget</class>
+  <widget class="QGroupBox" name="PageConfigWidget">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>642</width>
         <height>475</height>
       </rect>
     </property>
     <property name="title">
       <string>Default settings for new documents</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
-      <item row="10" column="1">
-        <widget class="QLabel" name="page_height_label">
-          <property name="text">
-            <string>Page height</string>
-          </property>
-          <property name="buddy">
-            <cstring>page_height</cstring>
-          </property>
-        </widget>
-      </item>
       <item row="17" column="3">
-        <widget class="QSpinBox" name="margin_right">
+        <widget class="QSpinBox" name="page_height">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the right paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+            <string>Default paper height in millimeters</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="12" column="3">
-        <widget class="QSpinBox" name="page_width">
-          <property name="sizePolicy">
-            <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
-              <horstretch>0</horstretch>
-              <verstretch>0</verstretch>
-            </sizepolicy>
-          </property>
+      <item row="1" column="3">
+        <widget class="QCheckBox" name="draw_page_numbers">
           <property name="toolTip">
-            <string>Default paper width in millimeters</string>
+            <string>If enabled, the page number is printed on each page. Makes it easier to notice missing pages in a stack.</string>
           </property>
-          <property name="suffix">
-            <string>mm</string>
+          <property name="text">
+            <string>Print page numbers</string>
           </property>
-          <property name="maximum">
-            <number>10000</number>
+        </widget>
+      </item>
+      <item row="27" column="1">
+        <widget class="QLabel" name="page_capacity_label">
+          <property name="text">
+            <string>Resulting page capacity:</string>
           </property>
         </widget>
       </item>
-      <item row="0" column="3">
+      <item row="2" column="3">
         <widget class="QCheckBox" name="draw_cut_markers">
           <property name="toolTip">
             <string>Enable printing additional lines to aid cutting the printed sheets.</string>
           </property>
           <property name="text">
             <string>Print cut markers</string>
           </property>
         </widget>
       </item>
-      <item row="10" column="3">
-        <widget class="QSpinBox" name="page_height">
+      <item row="20" column="3">
+        <widget class="QSpinBox" name="margin_top">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>Default paper height in millimeters</string>
+            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the top paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="13" column="1">
-        <widget class="QLabel" name="margin_top_label">
+      <item row="24" column="1">
+        <widget class="QLabel" name="margin_right_label">
           <property name="text">
-            <string>Top margin</string>
+            <string>Right margin</string>
           </property>
           <property name="buddy">
-            <cstring>margin_top</cstring>
+            <cstring>margin_right</cstring>
           </property>
         </widget>
       </item>
-      <item row="14" column="3">
-        <widget class="QSpinBox" name="margin_bottom">
+      <item row="25" column="3">
+        <widget class="QSpinBox" name="image_spacing_horizontal">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the bottom paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Space left and right of images. Images are this many millimeters apart.&lt;/p&gt;&lt;p&gt;If set to zero, you only need one cut to separate two images, otherwise you need two cuts but require less precision hitting the exact middle.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="14" column="1">
+      <item row="20" column="1">
+        <widget class="QLabel" name="margin_top_label">
+          <property name="text">
+            <string>Top margin</string>
+          </property>
+          <property name="buddy">
+            <cstring>margin_top</cstring>
+          </property>
+        </widget>
+      </item>
+      <item row="21" column="1">
         <widget class="QLabel" name="margin_bottom_label">
           <property name="text">
             <string>Bottom Margin</string>
           </property>
           <property name="buddy">
             <cstring>margin_bottom</cstring>
           </property>
         </widget>
       </item>
-      <item row="8" column="1" colspan="3">
-        <widget class="Line" name="line">
-          <property name="orientation">
-            <enum>Qt::Horizontal</enum>
+      <item row="19" column="1">
+        <widget class="QLabel" name="page_width_label">
+          <property name="text">
+            <string>Page width</string>
+          </property>
+          <property name="buddy">
+            <cstring>page_width</cstring>
           </property>
         </widget>
       </item>
-      <item row="20" column="3">
-        <widget class="QLabel" name="page_capacity">
-          <property name="toolTip">
-            <string>Number of regular-size cards fitting on each page,
-based on the page size and spacings configured</string>
-          </property>
+      <item row="23" column="1">
+        <widget class="QLabel" name="margin_left_label">
           <property name="text">
-            <string/>
+            <string>Left margin</string>
+          </property>
+          <property name="buddy">
+            <cstring>margin_left</cstring>
           </property>
         </widget>
       </item>
-      <item row="17" column="1">
-        <widget class="QLabel" name="margin_right_label">
+      <item row="25" column="1">
+        <widget class="QLabel" name="image_spacing_horizontal_label">
           <property name="text">
-            <string>Right margin</string>
+            <string>Horizontal image spacing</string>
           </property>
           <property name="buddy">
-            <cstring>margin_right</cstring>
+            <cstring>image_spacing_horizontal</cstring>
           </property>
         </widget>
       </item>
-      <item row="19" column="1">
+      <item row="26" column="1">
         <widget class="QLabel" name="image_spacing_vertical_label">
           <property name="text">
             <string>Vertical image spacing</string>
           </property>
           <property name="buddy">
             <cstring>image_spacing_vertical</cstring>
           </property>
         </widget>
       </item>
-      <item row="16" column="3">
-        <widget class="QSpinBox" name="margin_left">
+      <item row="24" column="3">
+        <widget class="QSpinBox" name="margin_right">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the left paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the right paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="18" column="1">
-        <widget class="QLabel" name="image_spacing_horizontal_label">
-          <property name="text">
-            <string>Horizontal image spacing</string>
+      <item row="21" column="3">
+        <widget class="QSpinBox" name="margin_bottom">
+          <property name="sizePolicy">
+            <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
+              <horstretch>0</horstretch>
+              <verstretch>0</verstretch>
+            </sizepolicy>
           </property>
-          <property name="buddy">
-            <cstring>image_spacing_horizontal</cstring>
+          <property name="toolTip">
+            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the bottom paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
-        </widget>
-      </item>
-      <item row="20" column="1">
-        <widget class="QLabel" name="page_capacity_label">
-          <property name="text">
-            <string>Resulting page capacity:</string>
+          <property name="suffix">
+            <string>mm</string>
+          </property>
+          <property name="maximum">
+            <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="13" column="3">
-        <widget class="QSpinBox" name="margin_top">
+      <item row="26" column="3">
+        <widget class="QSpinBox" name="image_spacing_vertical">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the top paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Space above and below images. Images are this many millimeters apart.&lt;/p&gt;&lt;p&gt;If set to zero, you only need one cut to separate two images, otherwise you need two cuts but require less precision hitting the exact middle.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="19" column="3">
-        <widget class="QSpinBox" name="image_spacing_vertical">
+      <item row="15" column="1" colspan="3">
+        <widget class="Line" name="line">
+          <property name="orientation">
+            <enum>Qt::Horizontal</enum>
+          </property>
+        </widget>
+      </item>
+      <item row="27" column="3">
+        <widget class="QLabel" name="page_capacity">
+          <property name="toolTip">
+            <string>Number of regular-size cards fitting on each page,
+based on the page size and spacings configured</string>
+          </property>
+          <property name="text">
+            <string/>
+          </property>
+        </widget>
+      </item>
+      <item row="23" column="3">
+        <widget class="QSpinBox" name="margin_left">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Space above and below images. Images are this many millimeters apart.&lt;/p&gt;&lt;p&gt;If set to zero, you only need one cut to separate two images, otherwise you need two cuts but require less precision hitting the exact middle.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Minimum margin between the left paper border and the page content.&lt;/p&gt;&lt;p&gt;Most printers have a minimum printing margin of 3 to 5 mm.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="16" column="1">
-        <widget class="QLabel" name="margin_left_label">
+      <item row="17" column="1">
+        <widget class="QLabel" name="page_height_label">
           <property name="text">
-            <string>Left margin</string>
+            <string>Page height</string>
           </property>
           <property name="buddy">
-            <cstring>margin_left</cstring>
+            <cstring>page_height</cstring>
           </property>
         </widget>
       </item>
-      <item row="18" column="3">
-        <widget class="QSpinBox" name="image_spacing_horizontal">
+      <item row="3" column="3">
+        <widget class="QCheckBox" name="draw_sharp_corners">
+          <property name="text">
+            <string>Draw 90° card corners, instead of round ones</string>
+          </property>
+        </widget>
+      </item>
+      <item row="19" column="3">
+        <widget class="QSpinBox" name="page_width">
           <property name="sizePolicy">
             <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
               <horstretch>0</horstretch>
               <verstretch>0</verstretch>
             </sizepolicy>
           </property>
           <property name="toolTip">
-            <string>&lt;html&gt;&lt;head/&gt;&lt;body&gt;&lt;p&gt;Space left and right of images. Images are this many millimeters apart.&lt;/p&gt;&lt;p&gt;If set to zero, you only need one cut to separate two images, otherwise you need two cuts but require less precision hitting the exact middle.&lt;/p&gt;&lt;/body&gt;&lt;/html&gt;</string>
+            <string>Default paper width in millimeters</string>
           </property>
           <property name="suffix">
             <string>mm</string>
           </property>
           <property name="maximum">
             <number>10000</number>
           </property>
         </widget>
       </item>
-      <item row="12" column="1">
-        <widget class="QLabel" name="page_width_label">
-          <property name="text">
-            <string>Page width</string>
+      <item row="0" column="3">
+        <widget class="QLineEdit" name="document_name">
+          <property name="toolTip">
+            <string>The document name is printed on each page and can help you keeping track
+of different printed sheets and to which deck they belong.
+
+Leave empty to disable.</string>
           </property>
-          <property name="buddy">
-            <cstring>page_width</cstring>
+          <property name="maxLength">
+            <number>200</number>
+          </property>
+          <property name="placeholderText">
+            <string>Document/deck name</string>
+          </property>
+          <property name="clearButtonEnabled">
+            <bool>true</bool>
           </property>
         </widget>
       </item>
-      <item row="1" column="3">
-        <widget class="QCheckBox" name="draw_sharp_corners">
+      <item row="0" column="1">
+        <widget class="QLabel" name="document_name_label">
           <property name="text">
-            <string>Draw 90° card corners, instead of round ones</string>
+            <string>Document name</string>
+          </property>
+          <property name="buddy">
+            <cstring>document_name</cstring>
           </property>
         </widget>
       </item>
     </layout>
   </widget>
   <tabstops>
+    <tabstop>document_name</tabstop>
+    <tabstop>draw_page_numbers</tabstop>
     <tabstop>draw_cut_markers</tabstop>
+    <tabstop>draw_sharp_corners</tabstop>
     <tabstop>page_height</tabstop>
     <tabstop>page_width</tabstop>
     <tabstop>margin_top</tabstop>
     <tabstop>margin_bottom</tabstop>
     <tabstop>margin_left</tabstop>
     <tabstop>margin_right</tabstop>
     <tabstop>image_spacing_horizontal</tabstop>
     <tabstop>image_spacing_vertical</tabstop>
   </tabstops>
   <resources/>
   <connections>
     <connection>
       <sender>page_height</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>89</y>
         </hint>
         <hint type="destinationlabel">
@@ -318,15 +360,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>page_height</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>89</y>
         </hint>
         <hint type="destinationlabel">
@@ -334,15 +376,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>page_width</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>126</y>
         </hint>
         <hint type="destinationlabel">
@@ -350,15 +392,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>page_width</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>126</y>
         </hint>
         <hint type="destinationlabel">
@@ -366,15 +408,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_top</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>163</y>
         </hint>
         <hint type="destinationlabel">
@@ -382,15 +424,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_top</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>163</y>
         </hint>
         <hint type="destinationlabel">
@@ -398,15 +440,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_bottom</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>200</y>
         </hint>
         <hint type="destinationlabel">
@@ -414,15 +456,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_bottom</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>200</y>
         </hint>
         <hint type="destinationlabel">
@@ -430,15 +472,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_left</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>237</y>
         </hint>
         <hint type="destinationlabel">
@@ -446,15 +488,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_left</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>237</y>
         </hint>
         <hint type="destinationlabel">
@@ -462,15 +504,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_right</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>274</y>
         </hint>
         <hint type="destinationlabel">
@@ -478,15 +520,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>margin_right</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>274</y>
         </hint>
         <hint type="destinationlabel">
@@ -494,15 +536,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>image_spacing_horizontal</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>311</y>
         </hint>
         <hint type="destinationlabel">
@@ -510,15 +552,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>image_spacing_horizontal</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>311</y>
         </hint>
         <hint type="destinationlabel">
@@ -526,15 +568,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>image_spacing_vertical</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>validate_paper_size_settings()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>348</y>
         </hint>
         <hint type="destinationlabel">
@@ -542,15 +584,15 @@
           <y>20</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>image_spacing_vertical</sender>
       <signal>valueChanged(int)</signal>
-      <receiver>page_configuration_group_box</receiver>
+      <receiver>PageConfigWidget</receiver>
       <slot>page_layout_setting_changed()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>200</x>
           <y>348</y>
         </hint>
         <hint type="destinationlabel">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/format_printing_filter.ui`

```diff
@@ -1,22 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>card_download_format_settings</class>
-  <widget class="QGroupBox" name="card_download_format_settings">
+  <class>FormatPrintingFilter</class>
+  <widget class="QGroupBox" name="FormatPrintingFilter">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>400</width>
         <height>300</height>
       </rect>
     </property>
-    <property name="windowTitle">
-      <string>Form</string>
-    </property>
     <property name="title">
       <string>Hide cards banned in specific Formats</string>
     </property>
     <layout class="QGridLayout" name="format_filter_layout">
       <item row="4" column="0">
         <widget class="QCheckBox" name="hide_banned_in_modern">
           <property name="text">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui`

 * *Files 1% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/general_printing_filter.ui`

```diff
@@ -1,22 +1,19 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>Form</class>
-  <widget class="QGroupBox" name="Form">
+  <class>GeneralPrintingFilter</class>
+  <widget class="QGroupBox" name="GeneralPrintingFilter">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>487</width>
         <height>302</height>
       </rect>
     </property>
-    <property name="windowTitle">
-      <string>Form</string>
-    </property>
     <property name="title">
       <string>General printing filters</string>
     </property>
     <layout class="QGridLayout" name="gridLayout">
       <item row="5" column="0">
         <widget class="QCheckBox" name="hide_gold_bordered_cards">
           <property name="toolTip">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui`

 * *Files 2% similar despite different names*

#### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/resources/ui/settings_window/settings_window.ui`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <ui version="4.0">
-  <class>Dialog</class>
-  <widget class="QDialog" name="Dialog">
+  <class>SettingsWindow</class>
+  <widget class="QDialog" name="SettingsWindow">
     <property name="windowModality">
       <enum>Qt::ApplicationModal</enum>
     </property>
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
@@ -73,16 +73,17 @@
                         <property name="sizePolicy">
                           <sizepolicy hsizetype="Expanding" vsizetype="Fixed">
                             <horstretch>0</horstretch>
                             <verstretch>0</verstretch>
                           </sizepolicy>
                         </property>
                         <property name="toolTip">
-                          <string>Horizontal adds a wide search area above the currently edited page.
-Vertical adds a tall search area between the page list and the currently edited page.</string>
+                          <string>Horizontal adds a wide, horizontal search area above the currently edited page, and is best for taller screens, like 4:3 or 3:2.
+Columnar organizes the main window content in four columns, and is best for (ultra-)wide screens.
+Tabbed uses tabs to only show parts of the main window at a time. Best used with small screens in portrait mode (i.e. 9:16), otherwise not recommended.</string>
                         </property>
                       </widget>
                     </item>
                   </layout>
                 </widget>
               </item>
               <item row="3" column="0" colspan="2">
@@ -658,15 +659,15 @@
     <tabstop>pdf_page_count_limit</tabstop>
   </tabstops>
   <resources/>
   <connections>
     <connection>
       <sender>button_box</sender>
       <signal>accepted()</signal>
-      <receiver>Dialog</receiver>
+      <receiver>SettingsWindow</receiver>
       <slot>accept()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>284</x>
           <y>643</y>
         </hint>
         <hint type="destinationlabel">
@@ -674,15 +675,15 @@
           <y>274</y>
         </hint>
       </hints>
     </connection>
     <connection>
       <sender>button_box</sender>
       <signal>rejected()</signal>
-      <receiver>Dialog</receiver>
+      <receiver>SettingsWindow</receiver>
       <slot>reject()</slot>
       <hints>
         <hint type="sourcelabel">
           <x>352</x>
           <y>643</y>
         </hint>
         <hint type="destinationlabel">
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/settings.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,16 @@
     "margin-left-mm": "7",
     "margin-right-mm": "7",
     "image-spacing-horizontal-mm": "0",
     "image-spacing-vertical-mm": "0",
     "print-cut-marker": "False",
     "pdf-page-count-limit": "0",
     "print-sharp-corners": "False",
+    "print-page-numbers": "False",
+    "default-document-name": "",
 }
 DEFAULT_SETTINGS["default-filesystem-paths"] = {
     "document-save-path": QStandardPaths.locate(QStandardPaths.DocumentsLocation, "", QStandardPaths.LocateDirectory),
     "pdf-export-path": QStandardPaths.locate(QStandardPaths.DocumentsLocation, "", QStandardPaths.LocateDirectory),
     "deck-list-search-path": QStandardPaths.locate(QStandardPaths.DownloadLocation, "", QStandardPaths.LocateDirectory),
 }
 DEFAULT_SETTINGS["gui"] = {
@@ -126,14 +128,15 @@
     "remove-snow-basics": "False",
 }
 DEFAULT_SETTINGS["application"] = {
     "last-used-version": mtg_proxy_printer.meta_data.__version__,
     "check-for-application-updates": "None",
     "check-for-card-data-updates": "None",
 }
+MAX_DOCUMENT_NAME_LENGTH = 200
 
 
 def read_settings_from_file():
     global settings, DEFAULT_SETTINGS
     settings.clear()
     if not config_file_path.exists():
         settings.read_dict(DEFAULT_SETTINGS)
@@ -217,20 +220,25 @@
 
 
 def _validate_documents_section(settings: configparser.ConfigParser, section_name: str = "documents"):
     card_size = mtg_proxy_printer.units_and_sizes.CardSizes.OVERSIZED
     card_height = card_size.as_mm(card_size.height)
     card_width = card_size.as_mm(card_size.width)
     section = settings[section_name]
+    if (document_name := section["default-document-name"]) and len(document_name) > MAX_DOCUMENT_NAME_LENGTH:
+        section["default-document-name"] = document_name[:MAX_DOCUMENT_NAME_LENGTH-1] + "…"
     defaults = DEFAULT_SETTINGS[section_name]
-    boolean_settings = {"print-cut-marker", "print-sharp-corners"}
+    boolean_settings = {"print-cut-marker", "print-sharp-corners", "print-page-numbers", }
+    string_settings = {"default-document-name", }
     # Check syntax
     for key in section.keys():
         if key in boolean_settings:
             _validate_boolean(section, defaults, key)
+        elif key in string_settings:
+            pass
         else:
             _validate_non_negative_int(section, defaults, key)
     # Check some semantic properties
     available_height = section.getint("paper-height-mm") - \
         (section.getint("margin-top-mm") + section.getint("margin-bottom-mm"))
     available_width = section.getint("paper-width-mm") - \
         (section.getint("margin-left-mm") + section.getint("margin-right-mm"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/sqlite_helpers.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/sqlite_helpers.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/stop_thread.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/stop_thread.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/add_card.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/add_card.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
-import typing
+from typing import Union, Type, Optional
 
 from PyQt5.QtCore import QStringListModel, pyqtSlot as Slot, pyqtSignal as Signal, Qt, QItemSelectionModel, QItemSelection
 from PyQt5.QtWidgets import QWidget, QDialogButtonBox
 from PyQt5.QtGui import QIcon
 
 from mtg_proxy_printer.document_controller.card_actions import ActionAddCard
 import mtg_proxy_printer.model.string_list
@@ -27,28 +27,28 @@
 from mtg_proxy_printer.ui.common import load_ui_from_file
 
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
 try:
-    from mtg_proxy_printer.ui.generated.add_card_widget.vertical import Ui_AddCardWidget as Ui_vertical
-    from mtg_proxy_printer.ui.generated.add_card_widget.horizontal import Ui_AddCardWidget as Ui_horizontal
+    from mtg_proxy_printer.ui.generated.add_card_widget.vertical import Ui_AddCardWidget_Vertical
+    from mtg_proxy_printer.ui.generated.add_card_widget.horizontal import Ui_AddCardWidget_Horizontal
 except ModuleNotFoundError:
-    Ui_vertical = load_ui_from_file("add_card_widget/vertical")
-    Ui_horizontal = load_ui_from_file("add_card_widget/horizontal")
+    Ui_AddCardWidget_Vertical = load_ui_from_file("add_card_widget/vertical")
+    Ui_AddCardWidget_Horizontal = load_ui_from_file("add_card_widget/horizontal")
 
 
 __all__ = [
     "AddCardWidget",
     "VerticalAddCardWidget",
     "HorizontalAddCardWidget",
 ]
 
-UiTypes = typing.Union[typing.Type[Ui_horizontal], typing.Type[Ui_horizontal]]
+UiTypes = Union[Type[Ui_AddCardWidget_Vertical], Type[Ui_AddCardWidget_Horizontal]]
 
 
 class AddCardWidget(QWidget):
 
     request_action = Signal(ActionAddCard)
 
     def __init__(self, ui_class: UiTypes, parent: QWidget = None):
@@ -248,40 +248,40 @@
         self.ui.copies_input.setValue(1)
 
     @property
     def current_language(self) -> str:
         return self.ui.language_combo_box.currentText()
 
     @property
-    def current_card_name(self) -> typing.Optional[str]:
+    def current_card_name(self) -> Optional[str]:
         selected = self.ui.card_name_list.selectedIndexes()
         if selected:
             return selected[0].data(Qt.DisplayRole)
         else:
             return None
 
     @property
-    def current_set_name(self) -> typing.Optional[str]:
+    def current_set_name(self) -> Optional[str]:
         selected = self.ui.set_name_list.selectedIndexes()
         if selected:
             return selected[0].data(Qt.EditRole)
         else:
             return None
 
     @property
-    def current_collector_number(self) -> typing.Optional[str]:
+    def current_collector_number(self) -> Optional[str]:
         selected = self.ui.collector_number_list.selectedIndexes()
         if selected:
             return selected[0].data(Qt.DisplayRole)
         else:
             return None
 
 
 class VerticalAddCardWidget(AddCardWidget):
 
     def __init__(self, parent: QWidget = None):
-        super().__init__(Ui_vertical, parent)
+        super().__init__(Ui_AddCardWidget_Vertical, parent)
 
 
 class HorizontalAddCardWidget(AddCardWidget):
     def __init__(self, parent: QWidget = None):
-        super().__init__(Ui_horizontal, parent)
+        super().__init__(Ui_AddCardWidget_Horizontal, parent)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/cache_cleanup_wizard.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/cache_cleanup_wizard.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 import datetime
 import enum
 import functools
 import math
 import pathlib
 import typing
 
-from PyQt5.QtCore import QAbstractTableModel, Qt, QModelIndex, QObject, QBuffer, QIODevice, QItemSelectionModel
+from PyQt5.QtCore import QAbstractTableModel, Qt, QModelIndex, QObject, QBuffer, QIODevice, QItemSelectionModel, QSize
 from PyQt5.QtGui import QIcon, QPixmap
 from PyQt5.QtWidgets import QWidget, QWizard, QTableView, QWizardPage
 
 from mtg_proxy_printer.natsort import NaturallySortedSortFilterProxyModel
 from mtg_proxy_printer.model.carddb import CardDatabase, Card, MTGSet
 from mtg_proxy_printer.model.imagedb import ImageDatabase, CacheContent as ImageCacheContent, ImageKey
-from mtg_proxy_printer.ui.common import load_ui_from_file, format_size
+from mtg_proxy_printer.ui.common import load_ui_from_file, format_size, WizardBase
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
 try:
-    from mtg_proxy_printer.ui.generated.cache_cleanup_wizard.card_filter_page import Ui_WizardPage as Ui_CardFilterPage
-    from mtg_proxy_printer.ui.generated.cache_cleanup_wizard.filter_setup_page import Ui_WizardPage as Ui_FilterSetupPage
-    from mtg_proxy_printer.ui.generated.cache_cleanup_wizard.summary_page import Ui_WizardPage as Ui_SummaryPage
+    from mtg_proxy_printer.ui.generated.cache_cleanup_wizard.card_filter_page import Ui_CardFilterPage
+    from mtg_proxy_printer.ui.generated.cache_cleanup_wizard.filter_setup_page import Ui_FilterSetupPage
+    from mtg_proxy_printer.ui.generated.cache_cleanup_wizard.summary_page import Ui_SummaryPage
 except ModuleNotFoundError:
     Ui_CardFilterPage = load_ui_from_file("cache_cleanup_wizard/card_filter_page")
     Ui_FilterSetupPage = load_ui_from_file("cache_cleanup_wizard/filter_setup_page")
     Ui_SummaryPage = load_ui_from_file("cache_cleanup_wizard/summary_page")
 
 __all__ = [
     "CacheCleanupWizard",
@@ -312,16 +312,15 @@
         sort_model.setSourceModel(card_image_model)
         # Use the EditRole for sorting, as this returns the raw data.
         # Makes it possible to sort the file sizes correctly.
         sort_model.setSortRole(Qt.EditRole)
         return sort_model
 
     def _setup_card_image_view(self, model: NaturallySortedSortFilterProxyModel):
-        view: QTableView = self.ui.card_image_view
-        view: QTableView
+        view = self.ui.card_image_view
         view.setModel(model)
         view.setSortingEnabled(True)
         view.sortByColumn(KnownCardColumns.Name, Qt.AscendingOrder)
         view.setColumnHidden(KnownCardColumns.ScryfallId, True)
         for column, scaling_factor in (
                 (KnownCardColumns.Name, 2),
                 (KnownCardColumns.Set, 2.5),
@@ -416,49 +415,32 @@
         indices = self.field("selected-images")
         disk_space_freed = format_size(sum(size_bytes for _, _, _, size_bytes in indices))
         self.ui.image_count_summary.setText(f"Images about to be deleted: {len(indices)}")
         self.ui.filesize_summary.setText(f"Disk space that will be freed: {disk_space_freed}")
         logger.debug(f"{self.__class__.__name__} populated.")
 
 
-class CacheCleanupWizard(QWizard):
+class CacheCleanupWizard(WizardBase):
+    BUTTON_ICONS = {
+        QWizard.WizardButton.FinishButton: "edit-delete",
+        QWizard.WizardButton.CancelButton: "dialog-cancel",
+        QWizard.WizardButton.HelpButton: "help-contents",
+    }
 
-    def __init__(self, card_db: CardDatabase, image_db: ImageDatabase, *args, **kwargs):
-        super(CacheCleanupWizard, self).__init__(*args, **kwargs)
+    def __init__(self, card_db: CardDatabase, image_db: ImageDatabase,
+                 parent: QWidget = None, flags = Qt.WindowFlags()):
+        super().__init__(QSize(1024, 768), parent, flags)
         self.image_db = image_db
         self.addPage(FilterSetupPage(self))
         self.addPage(CardFilterPage(card_db, image_db, self))
         self.addPage(SummaryPage(self))
         self.setWindowTitle("Cleanup locally stored card images")
         self.setWindowIcon(QIcon.fromTheme("edit-clear-history"))
-        self._setup_button_icons()
-        self._set_default_size()
         logger.info(f"Created {self.__class__.__name__} instance.")
 
-    def _set_default_size(self):
-        new_width, new_height = 1024, 768
-        if (parent := self.parent()) is not None:
-            parent_pos = parent.mapToGlobal(parent.pos())
-            self.setGeometry(
-                parent_pos.x() + parent.width()//2 - new_width//2,
-                parent_pos.y() + parent.height()//2 - new_height//2,
-                new_width, new_height
-            )
-        else:
-            self.resize(new_width, new_height)
-
-    def _setup_button_icons(self):
-        buttons_with_icons: typing.List[typing.Tuple[QWizard.WizardButton, str]] = [
-            (QWizard.CancelButton, "dialog-cancel"),
-            (QWizard.HelpButton, "help-contents"),
-            (QWizard.FinishButton, "edit-delete"),
-        ]
-        for button, icon_name in buttons_with_icons:
-            self.button(button).setIcon(QIcon.fromTheme(icon_name))
-
     def accept(self) -> None:
         super(CacheCleanupWizard, self).accept()
         logger.info("User accepted the wizard, deleting entries from the cache.")
         self.image_db.delete_disk_cache_entries((
             ImageKey(scryfall_id, is_front, is_high_resolution)
             for scryfall_id, is_front, is_high_resolution, _ in self.field("selected-images")
         ))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/central_widget.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/central_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,52 +13,52 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import functools
 import math
 import operator
 import pathlib
-import typing
+from typing import Union, Type, Optional
 
 from PyQt5.QtCore import pyqtSignal as Signal, pyqtSlot as Slot, QPersistentModelIndex, QItemSelectionModel, \
-    QModelIndex, QPoint
+    QModelIndex, QPoint, Qt
 from PyQt5.QtGui import QIcon
 from PyQt5.QtWidgets import QWidget, QAction, QMenu, QInputDialog, QFileDialog
 
 import mtg_proxy_printer.app_dirs
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.model.card_list import PageColumns
 from mtg_proxy_printer.model.document import Document
-from mtg_proxy_printer.model.carddb import CardDatabase, Card, CardList, CheckCard
+from mtg_proxy_printer.model.carddb import CardDatabase, Card, CardList, CheckCard, AnyCardType, AnyCardTypeForTypeCheck
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.document_controller import DocumentAction
 from mtg_proxy_printer.document_controller.card_actions import ActionRemoveCards, ActionAddCard
 from mtg_proxy_printer.ui.item_delegates import ComboBoxItemDelegate
 
 try:
-    from mtg_proxy_printer.ui.generated.central_widget.columnar import Ui_central_widget as Ui_Columnar
-    from mtg_proxy_printer.ui.generated.central_widget.grouped import Ui_central_widget as Ui_Grouped
-    from mtg_proxy_printer.ui.generated.central_widget.tabbed_vertical import Ui_central_widget as Ui_TabbedVertical
+    from mtg_proxy_printer.ui.generated.central_widget.columnar import Ui_CentralWidget_Columnar
+    from mtg_proxy_printer.ui.generated.central_widget.grouped import Ui_CentralWidget_Grouped
+    from mtg_proxy_printer.ui.generated.central_widget.tabbed_vertical import Ui_CentralWidget_Tabbed
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
-    Ui_Columnar = load_ui_from_file("central_widget/columnar")
-    Ui_Grouped = load_ui_from_file("central_widget/grouped")
-    Ui_TabbedVertical = load_ui_from_file("central_widget/tabbed_vertical")
+    Ui_CentralWidget_Columnar = load_ui_from_file("central_widget/columnar")
+    Ui_CentralWidget_Grouped = load_ui_from_file("central_widget/grouped")
+    Ui_CentralWidget_Tabbed = load_ui_from_file("central_widget/tabbed_vertical")
 
 
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
 del get_logger
 
 
 __all__ = [
     "CentralWidget",
 ]
 
-UiType = typing.Union[typing.Type[Ui_Grouped], typing.Type[Ui_Columnar], typing.Type[Ui_TabbedVertical]]
+UiType = Union[Type[Ui_CentralWidget_Grouped], Type[Ui_CentralWidget_Columnar], Type[Ui_CentralWidget_Tabbed]]
 
 
 class CentralWidget(QWidget):
 
     request_action = Signal(DocumentAction)
     obtain_card_image = Signal(ActionAddCard)
 
@@ -76,14 +76,15 @@
         logger.info(f"Created {self.__class__.__name__} instance.")
 
     def _setup_page_card_table_view(self) -> ComboBoxItemDelegate:
         self.ui.page_card_table_view.customContextMenuRequested.connect(self.page_table_context_menu_requested)
         combo_box_delegate = ComboBoxItemDelegate(self.ui.page_card_table_view)
         self.ui.page_card_table_view.setItemDelegateForColumn(PageColumns.CollectorNumber, combo_box_delegate)
         self.ui.page_card_table_view.setItemDelegateForColumn(PageColumns.Set, combo_box_delegate)
+        self.ui.page_card_table_view.setItemDelegateForColumn(PageColumns.Language, combo_box_delegate)
         return combo_box_delegate
 
     def set_data(self, document: Document, card_db: CardDatabase, image_db: ImageDatabase):
         self.document = document
         self.card_db = card_db
         self.image_db = image_db
         self.obtain_card_image.connect(image_db.download_worker.fill_document_action_image)
@@ -111,38 +112,38 @@
     def page_table_context_menu_requested(self, pos: QPoint):
         view = self.ui.page_card_table_view
         if not (index := view.indexAt(pos)).isValid():
             logger.debug("Right clicked empty space in the page card table view, ignoring event")
             return
         logger.info(f"Page card table requests context menu at x={pos.x()}, y={pos.y()}, row={index.row()}")
         menu = QMenu(view)
-        card: Card = index.internalPointer().card
+        card: Card = index.data(Qt.ItemDataRole.UserRole)
         menu.addActions(self._create_add_copies_actions(card))
         if card.is_dfc:
             menu.addSeparator()
             self._create_add_check_card_actions(menu, card)
         if related_cards := self.card_db.find_related_cards(card):
             menu.addSeparator()
             self._create_add_related_actions(menu, related_cards)
         self._add_save_image_action(menu, card)
         menu.popup(view.viewport().mapToGlobal(pos))
 
-    def _create_add_copies_actions(self, card: typing.Union[Card, CardList], add_4th: bool = False):
+    def _create_add_copies_actions(self, card: Union[AnyCardType, CardList], add_4th: bool = False):
         actions = [
             self._create_add_copies_action("Add 1 copy", 1, card),
             self._create_add_copies_action("Add 2 copies", 2, card),
             self._create_add_copies_action("Add 3 copies", 3, card),
             self._create_add_copies_action("Add copies …", None, card)
         ]
         if add_4th:
             actions.insert(-1, self._create_add_copies_action("Add 4 copies", 4, card),)
         return actions
 
-    def _create_add_copies_action(self, label: str, count: typing.Optional[int],
-                                  card: typing.Union[Card, CheckCard, CardList]):
+    def _create_add_copies_action(self, label: str, count: Optional[int],
+                                  card: Union[AnyCardType, CardList]):
         action = QAction(QIcon.fromTheme("list-add"), label, self.ui.page_card_table_view)
         action.triggered.connect(functools.partial(self._add_copies, card, count))
         return action
 
     def _create_add_check_card_actions(self, parent: QMenu, card: Card):
         other_face = self.card_db.get_opposing_face(card)
         front, back = sorted([card, other_face], key=operator.attrgetter("is_front"), reverse=True)
@@ -158,40 +159,40 @@
 
     def _create_add_related_actions(self, parent: QMenu, related_cards: CardList) -> None:
         logger.debug(f"Found {len(related_cards)} related cards. Adding them to the context menu")
         parent.addMenu("All related cards").addActions(self._create_add_copies_actions(related_cards, True))
         for card in related_cards:
             parent.addMenu(card.name).addActions(self._create_add_copies_actions(card, True))
 
-    def _add_copies(self, card: typing.Union[Card, CheckCard, CardList], count: typing.Optional[int]):
+    def _add_copies(self, card: Union[AnyCardType, CardList], count: Optional[int]):
         nl = '\n'
-        card_name = card.name if isinstance(card, (Card, CheckCard)) else nl + nl.join(item.name for item in card)
+        card_name = card.name if isinstance(card, AnyCardTypeForTypeCheck) else nl + nl.join(item.name for item in card)
         if count is None:
             count, success = QInputDialog.getInt(self, "Add copies", f"Add copies of {card_name}", 1, 1, 100)
             if not success:
                 logger.info("User cancelled adding card copies")
                 return
         logger.info(f"Add {count} × {card_name.replace(nl, ',')} via the context menu action")
-        if isinstance(card, (Card, CheckCard)):
+        if isinstance(card, AnyCardTypeForTypeCheck):
             self._request_action_add_card(card, count)
         else:
             for item in card:
                 self._request_action_add_card(item, count)
 
-    def _request_action_add_card(self, card: typing.Union[Card, CheckCard], count: int):
+    def _request_action_add_card(self, card: AnyCardType, count: int):
         # If cards have images, request the action directly. This happens when adding copies of already added cards
         # and is required for custom cards. Otherwise, request the image from the image database. Cards without images
         # at this point are CheckCards or related cards.
         action = ActionAddCard(card, count)
         if card.image_file is None:
             self.obtain_card_image.emit(action)
         else:
             self.request_action.emit(action)
 
-    def _add_save_image_action(self, parent: QMenu, card: typing.Union[Card, CheckCard]):
+    def _add_save_image_action(self, parent: QMenu, card: AnyCardType):
         action = QAction(QIcon.fromTheme("document-save"), "Export image", parent)
         action.setData(card)
         action.triggered.connect(self._on_save_image_action_triggered)
         parent.addSeparator()
         parent.addAction(action)
 
     @Slot()
@@ -282,11 +283,11 @@
             self.document.on_ui_selects_new_page(new_selection)
 
 
 def get_configured_central_widget_layout_class() -> UiType:
     gui_settings = mtg_proxy_printer.settings.settings["gui"]
     configured_layout = gui_settings["central-widget-layout"]
     if configured_layout == "horizontal":
-        return Ui_Grouped
+        return Ui_CentralWidget_Grouped
     if configured_layout == "columnar":
-        return Ui_Columnar
-    return Ui_TabbedVertical
+        return Ui_CentralWidget_Columnar
+    return Ui_CentralWidget_Tabbed
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/deck_import_wizard.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/deck_import_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 import itertools
 import math
 import pathlib
 import re
 import typing
 
 from PyQt5.QtCore import pyqtSlot as Slot, pyqtSignal as Signal, pyqtProperty as Property, QStringListModel, Qt, \
-    QItemSelection, QAbstractTableModel
+    QItemSelection, QAbstractTableModel, QSize
 from PyQt5.QtGui import QValidator, QIcon
-from PyQt5.QtWidgets import QWizard, QFileDialog, QMessageBox, QWizardPage
+from PyQt5.QtWidgets import QWizard, QFileDialog, QMessageBox, QWizardPage, QWidget
 
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.decklist_parser import re_parsers, common, csv_parsers
 from mtg_proxy_printer.decklist_downloader import IsIdentifyingDeckUrlValidator, AVAILABLE_DOWNLOADERS, \
     get_downloader_class
 from mtg_proxy_printer.model.carddb import CardDatabase
 from mtg_proxy_printer.model.imagedb import ImageDatabase
 from mtg_proxy_printer.model.card_list import CardListModel, PageColumns
 from mtg_proxy_printer.natsort import NaturallySortedSortFilterProxyModel
-from mtg_proxy_printer.ui.common import load_ui_from_file, format_size
+from mtg_proxy_printer.ui.common import load_ui_from_file, format_size, WizardBase
 from mtg_proxy_printer.ui.item_delegates import ComboBoxItemDelegate
 from mtg_proxy_printer.document_controller.import_deck_list import ActionImportDeckList
 
 try:
-    from mtg_proxy_printer.ui.generated.deck_import_wizard.load_list_page import Ui_WizardPage as Ui_LoadListPage
-    from mtg_proxy_printer.ui.generated.deck_import_wizard.parser_result_page import Ui_WizardPage as Ui_SummaryPage
-    from mtg_proxy_printer.ui.generated.deck_import_wizard.select_deck_parser_page import Ui_WizardPage as Ui_SelectDeckParserPage
+    from mtg_proxy_printer.ui.generated.deck_import_wizard.load_list_page import Ui_LoadListPage
+    from mtg_proxy_printer.ui.generated.deck_import_wizard.parser_result_page import Ui_SummaryPage
+    from mtg_proxy_printer.ui.generated.deck_import_wizard.select_deck_parser_page import Ui_SelectDeckParserPage
 except ModuleNotFoundError:
     Ui_LoadListPage = load_ui_from_file("deck_import_wizard/load_list_page")
     Ui_SummaryPage = load_ui_from_file("deck_import_wizard/parser_result_page")
     Ui_SelectDeckParserPage = load_ui_from_file("deck_import_wizard/select_deck_parser_page")
 
 from mtg_proxy_printer.logger import get_logger
 logger = get_logger(__name__)
@@ -385,15 +385,16 @@
         super(SummaryPage, self).__init__(*args, **kwargs)
         self.ui = Ui_SummaryPage()
         self.ui.setupUi(self)
         self.setCommitPage(True)
         self.card_list = CardListModel(card_db, self)
         self.card_list_sort_model = self._create_sort_model(self.card_list)
         self.card_list.oversized_card_count_changed.connect(self._update_accept_button_on_oversized_card_count_changed)
-        self.combo_box_delegate = self._setup_parsed_cards_table(self.card_list_sort_model)
+        self.ui.parsed_cards_table.setModel(self.card_list_sort_model)
+        self.combo_box_delegate = self._setup_parsed_cards_table()
         self.selected_cells_count = 0
         self.registerField("should_replace_document", self.ui.should_replace_document)
         self.ui.should_replace_document.toggled[bool].connect(
             self._update_accept_button_on_replace_document_option_toggled)
         logger.info(f"Created {self.__class__.__name__} instance.")
 
     def _create_sort_model(self, source_model: CardListModel) -> NaturallySortedSortFilterProxyModel:
@@ -426,20 +427,20 @@
         if enabled:
             accept_button.setIcon(QIcon.fromTheme("document-replace"))
             accept_button.setToolTip("Replace document content with the identified cards")
         else:
             accept_button.setIcon(QIcon.fromTheme("dialog-ok"))
             accept_button.setToolTip("Append identified cards to the document")
 
-    def _setup_parsed_cards_table(self, model: QAbstractTableModel) -> ComboBoxItemDelegate:
-        self.ui.parsed_cards_table.setModel(model)
+    def _setup_parsed_cards_table(self) -> ComboBoxItemDelegate:
         self.ui.parsed_cards_table.selectionModel().selectionChanged.connect(self.parsed_cards_table_selection_changed)
         delegate = ComboBoxItemDelegate(self.ui.parsed_cards_table)
         self.ui.parsed_cards_table.setItemDelegateForColumn(PageColumns.Set, delegate)
         self.ui.parsed_cards_table.setItemDelegateForColumn(PageColumns.CollectorNumber, delegate)
+        self.ui.parsed_cards_table.setItemDelegateForColumn(PageColumns.Language, delegate)
         for column, scaling_factor in (
                 (PageColumns.CardName, 2),
                 (PageColumns.Set, 2.75),
                 (PageColumns.CollectorNumber, 0.95),
                 (PageColumns.Language, 0.9)):
             new_size = math.floor(self.ui.parsed_cards_table.columnWidth(column) * scaling_factor)
             self.ui.parsed_cards_table.setColumnWidth(column, new_size)
@@ -463,15 +464,15 @@
         )
         self.card_list.add_cards(parsed_deck)
         self.ui.unparsed_lines_text.setPlainText("\n".join(unidentified_lines))
         self._initialize_custom_buttons()
         logger.debug(f"Initialized {self.__class__.__name__}")
 
     def _initialize_custom_buttons(self):
-        wizard: QWizard = self.wizard()
+        wizard = self.wizard()
         wizard.customButtonClicked.connect(self.custom_button_clicked)
         wizard.setOption(QWizard.HaveCustomButton1, True)
         decklist_import_section = mtg_proxy_printer.settings.settings["decklist-import"]
         remove_basic_lands_button = wizard.button(QWizard.CustomButton1)
         remove_basic_lands_button.setEnabled(self.card_list.has_basic_lands(
             decklist_import_section.getboolean("remove-basic-wastes"),
             decklist_import_section.getboolean("remove-snow-basics")))
@@ -484,34 +485,34 @@
         remove_selected_cards_button.setText("Remove selected")
         remove_selected_cards_button.setToolTip("Remove all selected cards in the deck list above")
         remove_selected_cards_button.setIcon(QIcon.fromTheme("edit-delete"))
 
     def cleanupPage(self):
         self.card_list.clear()
         super(SummaryPage, self).cleanupPage()
-        wizard: QWizard = self.wizard()
+        wizard = self.wizard()
         wizard.customButtonClicked.disconnect(self.custom_button_clicked)
         wizard.setOption(QWizard.HaveCustomButton1, False)
         wizard.setOption(QWizard.HaveCustomButton2, False)
         logger.debug(f"Cleaned up {self.__class__.__name__}")
 
     @Slot()
     def isComplete(self) -> bool:
         return self.card_list.rowCount() > 0
 
     @Slot(QItemSelection, QItemSelection)
     def parsed_cards_table_selection_changed(self, selected: QItemSelection, deselected: QItemSelection):
         self.selected_cells_count += selected.count() - deselected.count()
         logger.debug(f"Selection changed: Currently selected cells: {self.selected_cells_count}")
-        wizard: QWizard = self.wizard()
+        wizard = self.wizard()
         wizard.button(QWizard.CustomButton2).setEnabled(self.selected_cells_count > 0)
 
     @Slot(int)
     def custom_button_clicked(self, button_id: int):
-        wizard: QWizard = self.wizard()
+        wizard = self.wizard()
         if button_id == QWizard.CustomButton1:
             wizard.button(button_id).setEnabled(False)
             logger.info("User requests to remove all basic lands")
             decklist_import_section = mtg_proxy_printer.settings.settings["decklist-import"]
             self.card_list.remove_all_basic_lands(
                 decklist_import_section.getboolean("remove-basic-wastes"),
                 decklist_import_section.getboolean("remove-snow-basics"))
@@ -526,55 +527,35 @@
             self.ui.parsed_cards_table.selectionModel().selection())
         self.card_list.remove_multi_selection(selection_mapped_to_source)
         if not self.card_list.rowCount():
             # User deleted everything, so nothing left to complete the wizard. This’ll disable the Finish button.
             self.completeChanged.emit()
 
 
-class DeckImportWizard(QWizard):
+class DeckImportWizard(WizardBase):
     request_action = Signal(ActionImportDeckList)
+    BUTTON_ICONS = {
+        QWizard.WizardButton.FinishButton: "dialog-ok",
+        QWizard.WizardButton.CancelButton: "dialog-cancel",
+    }
 
     def __init__(self, card_db: CardDatabase, image_db: ImageDatabase,
-                 language_model: QStringListModel, *args, **kwargs):
-        super(DeckImportWizard, self).__init__(*args, **kwargs)
+                 language_model: QStringListModel, parent: QWidget = None, flags = Qt.WindowFlags()):
+        super().__init__(QSize(800, 600), parent, flags)
         self.card_db = card_db
         self.select_deck_parser_page = SelectDeckParserPage(card_db, image_db, self)
         self.load_list_page = LoadListPage(language_model, self)
         self.summary_page = SummaryPage(card_db, self)
         self.addPage(self.load_list_page)
         self.addPage(self.select_deck_parser_page)
         self.addPage(self.summary_page)
         self.setWindowIcon(QIcon.fromTheme("document-import"))
-        self._set_default_size()
         self.setWindowTitle("Import a deck list")
-        self._setup_dialog_button_icons()
         logger.info(f"Created {self.__class__.__name__} instance.")
 
-    def _set_default_size(self):
-        new_width, new_height = 800, 600
-        if (parent := self.parent()) is not None:
-            parent_pos = parent.mapToGlobal(parent.pos())
-            self.setGeometry(
-                parent_pos.x() + parent.width()//2 - new_width//2,
-                parent_pos.y() + parent.height()//2 - new_height//2,
-                new_width, new_height
-            )
-        else:
-            self.resize(new_width, new_height)
-
-    def _setup_dialog_button_icons(self):
-        buttons_with_icons = [
-            (QWizard.FinishButton, "dialog-ok"),
-            (QWizard.CancelButton, "dialog-cancel"),
-        ]
-        for role, icon in buttons_with_icons:
-            button = self.button(role)
-            if button.icon().isNull():
-                button.setIcon(QIcon.fromTheme(icon))
-
     def accept(self):
         if not self._ask_about_oversized_cards():
             logger.info("Aborting accept(), because oversized cards are present "
                         "in the deck list and the user chose to go back.")
             return
         super(DeckImportWizard, self).accept()
         logger.info("User finished the import wizard, performing the requested actions")
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/dialogs.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 import mtg_proxy_printer.ui.common
 import mtg_proxy_printer.meta_data
 from mtg_proxy_printer.units_and_sizes import DEFAULT_SAVE_SUFFIX
 from mtg_proxy_printer.document_controller.edit_document_settings import ActionEditDocumentSettings
 from mtg_proxy_printer.logger import get_logger
 
 try:
-    from mtg_proxy_printer.ui.generated.about_dialog import Ui_Dialog as Ui_AboutDialog
-    from mtg_proxy_printer.ui.generated.page_config_dialog import Ui_Dialog as Ui_PageConfigDialog
+    from mtg_proxy_printer.ui.generated.about_dialog import Ui_AboutDialog
+    from mtg_proxy_printer.ui.generated.document_settings_dialog import Ui_DocumentSettingsDialog
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_AboutDialog = load_ui_from_file("about_dialog")
-    Ui_PageConfigDialog = load_ui_from_file("page_config_dialog")
+    Ui_DocumentSettingsDialog = load_ui_from_file("document_settings_dialog")
 
 logger = get_logger(__name__)
 del get_logger
 
 __all__ = [
     "SavePDFDialog",
     "SaveDocumentAsDialog",
@@ -142,15 +142,15 @@
     def on_reject(self):
         logger.debug("User aborted loading. Doing nothing.")
 
 
 class AboutMTGProxyPrinterDialog(QDialog):
 
     def __init__(self, *args, **kwargs):
-        super(AboutMTGProxyPrinterDialog, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.ui = Ui_AboutDialog()
         self.ui.setupUi(self)
         self._setup_about_text()
         self._setup_changelog_text()
         self._setup_license_text()
         self._setup_third_party_license_text()
         self.ui.mtg_proxy_printer_version_label.setText(mtg_proxy_printer.meta_data.__version__)
@@ -225,15 +225,15 @@
         logger.info(f"Created {self.__class__.__name__} instance.")
 
 
 class DocumentSettingsDialog(QDialog):
 
     def __init__(self, document: mtg_proxy_printer.model.document.Document, parent: QWidget = None):
         super(DocumentSettingsDialog, self).__init__(parent)
-        self.ui = Ui_PageConfigDialog()
+        self.ui = Ui_DocumentSettingsDialog()
         self.ui.setupUi(self)
         self.setModal(True)
         self.document = document
         self.ui.page_config_groupbox.load_from_page_layout(document.page_layout)
         self.ui.page_config_groupbox.setTitle("These settings only affect the current document")
         self._setup_button_box()
         self.accepted.connect(self.on_accept)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/about_dialog.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/about_dialog.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Dialog(object):
-    def setupUi(self, Dialog):
-        Dialog.setObjectName("Dialog")
-        Dialog.resize(800, 600)
-        Dialog.setModal(True)
-        self.verticalLayout = QtWidgets.QVBoxLayout(Dialog)
+class Ui_AboutDialog(object):
+    def setupUi(self, AboutDialog):
+        AboutDialog.setObjectName("AboutDialog")
+        AboutDialog.resize(800, 600)
+        AboutDialog.setModal(True)
+        self.verticalLayout = QtWidgets.QVBoxLayout(AboutDialog)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.tab_widget = QtWidgets.QTabWidget(Dialog)
+        self.tab_widget = QtWidgets.QTabWidget(AboutDialog)
         self.tab_widget.setObjectName("tab_widget")
         self.tab_about = QtWidgets.QWidget()
         self.tab_about.setObjectName("tab_about")
         self.tab_about_layout = QtWidgets.QGridLayout(self.tab_about)
         self.tab_about_layout.setObjectName("tab_about_layout")
         self.python_version_label = QtWidgets.QLabel(self.tab_about)
         self.python_version_label.setTextInteractionFlags(QtCore.Qt.TextSelectableByMouse)
@@ -76,33 +76,33 @@
         self.tab_widget.addTab(self.license_text_browser, "")
         self.third_party_license_text_browser = QtWidgets.QTextBrowser()
         self.third_party_license_text_browser.setTextInteractionFlags(QtCore.Qt.LinksAccessibleByKeyboard|QtCore.Qt.LinksAccessibleByMouse|QtCore.Qt.TextBrowserInteraction|QtCore.Qt.TextSelectableByKeyboard|QtCore.Qt.TextSelectableByMouse)
         self.third_party_license_text_browser.setOpenExternalLinks(True)
         self.third_party_license_text_browser.setObjectName("third_party_license_text_browser")
         self.tab_widget.addTab(self.third_party_license_text_browser, "")
         self.verticalLayout.addWidget(self.tab_widget)
-        self.buttonBox = QtWidgets.QDialogButtonBox(Dialog)
+        self.buttonBox = QtWidgets.QDialogButtonBox(AboutDialog)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Close)
         self.buttonBox.setObjectName("buttonBox")
         self.verticalLayout.addWidget(self.buttonBox)
 
-        self.retranslateUi(Dialog)
+        self.retranslateUi(AboutDialog)
         self.tab_widget.setCurrentIndex(0)
-        self.buttonBox.accepted.connect(Dialog.accept) # type: ignore
-        self.buttonBox.rejected.connect(Dialog.reject) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(Dialog)
+        self.buttonBox.accepted.connect(AboutDialog.accept) # type: ignore
+        self.buttonBox.rejected.connect(AboutDialog.reject) # type: ignore
+        QtCore.QMetaObject.connectSlotsByName(AboutDialog)
 
-    def retranslateUi(self, Dialog):
+    def retranslateUi(self, AboutDialog):
         _translate = QtCore.QCoreApplication.translate
-        Dialog.setWindowTitle(_translate("Dialog", "About MTGProxyPrinter"))
-        self.mtg_proxy_printer_name.setText(_translate("Dialog", "<html><head/><body><p><span style=\" font-size:xx-large; font-weight:600;\">MTGProxyPrinter</span></p><p><br/></p></body></html>"))
-        self.mtg_proxy_printer_version_header_label.setText(_translate("Dialog", "Version:"))
-        self.python_version_header_label.setText(_translate("Dialog", "Python Version:"))
-        self.about_text.setMarkdown(_translate("Dialog", "{application_name} allows printing \n"
+        AboutDialog.setWindowTitle(_translate("AboutDialog", "About MTGProxyPrinter"))
+        self.mtg_proxy_printer_name.setText(_translate("AboutDialog", "<html><head/><body><p><span style=\" font-size:xx-large; font-weight:600;\">MTGProxyPrinter</span></p><p><br/></p></body></html>"))
+        self.mtg_proxy_printer_version_header_label.setText(_translate("AboutDialog", "Version:"))
+        self.python_version_header_label.setText(_translate("AboutDialog", "Python Version:"))
+        self.about_text.setMarkdown(_translate("AboutDialog", "{application_name} allows printing \n"
 "[Magic: The Gathering](https://magic.wizards.com/) cards for play-testing\n"
 "purposes.\n"
 "\n"
 "{application_name} is unofficial Fan Content permitted under the \n"
 "[Fan Content Policy](https://company.wizards.com/fancontentpolicy). Not\n"
 "approved/endorsed by Wizards. Portions of the materials used are property of\n"
 "Wizards of the Coast. ©[Wizards of the Coast LLC](https://company.wizards.com/).\n"
@@ -111,12 +111,12 @@
 "this program, including the card database content and downloaded card images,\n"
 "nor any documents created, both in digital and physical form.\n"
 "\n"
 "Project Website: \n"
 "[{application_name} home page]({application_home_page})\n"
 "\n"
 ""))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_about), _translate("Dialog", "About"))
-        self.changelog_text_browser.setDocumentTitle(_translate("Dialog", "Changelog"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.changelog_text_browser), _translate("Dialog", "Changelog"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.license_text_browser), _translate("Dialog", "License"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.third_party_license_text_browser), _translate("Dialog", "Third party licenses"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_about), _translate("AboutDialog", "About"))
+        self.changelog_text_browser.setDocumentTitle(_translate("AboutDialog", "Changelog"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.changelog_text_browser), _translate("AboutDialog", "Changelog"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.license_text_browser), _translate("AboutDialog", "License"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.third_party_license_text_browser), _translate("AboutDialog", "Third party licenses"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/add_card_widget/horizontal.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_AddCardWidget(object):
-    def setupUi(self, AddCardWidget):
-        AddCardWidget.setObjectName("AddCardWidget")
-        AddCardWidget.resize(1242, 292)
-        self.gridLayout = QtWidgets.QGridLayout(AddCardWidget)
+class Ui_AddCardWidget_Horizontal(object):
+    def setupUi(self, AddCardWidget_Horizontal):
+        AddCardWidget_Horizontal.setObjectName("AddCardWidget_Horizontal")
+        AddCardWidget_Horizontal.resize(1242, 292)
+        self.gridLayout = QtWidgets.QGridLayout(AddCardWidget_Horizontal)
         self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.language_label = QtWidgets.QLabel(AddCardWidget)
+        self.language_label = QtWidgets.QLabel(AddCardWidget_Horizontal)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.language_label.sizePolicy().hasHeightForWidth())
         self.language_label.setSizePolicy(sizePolicy)
         self.language_label.setObjectName("language_label")
         self.gridLayout.addWidget(self.language_label, 7, 5, 1, 1)
-        self.card_name_box = QtWidgets.QGroupBox(AddCardWidget)
+        self.card_name_box = QtWidgets.QGroupBox(AddCardWidget_Horizontal)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(7)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.card_name_box.sizePolicy().hasHeightForWidth())
         self.card_name_box.setSizePolicy(sizePolicy)
         self.card_name_box.setObjectName("card_name_box")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.card_name_box)
@@ -41,15 +41,15 @@
         self.verticalLayout.addWidget(self.card_name_filter)
         self.card_name_list = QtWidgets.QListView(self.card_name_box)
         self.card_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.card_name_list.setAlternatingRowColors(True)
         self.card_name_list.setObjectName("card_name_list")
         self.verticalLayout.addWidget(self.card_name_list)
         self.gridLayout.addWidget(self.card_name_box, 7, 1, 9, 1)
-        self.set_name_box = QtWidgets.QGroupBox(AddCardWidget)
+        self.set_name_box = QtWidgets.QGroupBox(AddCardWidget_Horizontal)
         self.set_name_box.setEnabled(False)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(7)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.set_name_box.sizePolicy().hasHeightForWidth())
         self.set_name_box.setSizePolicy(sizePolicy)
         self.set_name_box.setObjectName("set_name_box")
@@ -61,15 +61,15 @@
         self.verticalLayout_2.addWidget(self.set_name_filter)
         self.set_name_list = QtWidgets.QListView(self.set_name_box)
         self.set_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.set_name_list.setAlternatingRowColors(True)
         self.set_name_list.setObjectName("set_name_list")
         self.verticalLayout_2.addWidget(self.set_name_list)
         self.gridLayout.addWidget(self.set_name_box, 7, 2, 9, 1)
-        self.collector_number_box = QtWidgets.QGroupBox(AddCardWidget)
+        self.collector_number_box = QtWidgets.QGroupBox(AddCardWidget_Horizontal)
         self.collector_number_box.setEnabled(False)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(5)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.collector_number_box.sizePolicy().hasHeightForWidth())
         self.collector_number_box.setSizePolicy(sizePolicy)
         self.collector_number_box.setObjectName("collector_number_box")
@@ -77,56 +77,56 @@
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.collector_number_list = QtWidgets.QListView(self.collector_number_box)
         self.collector_number_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.collector_number_list.setAlternatingRowColors(True)
         self.collector_number_list.setObjectName("collector_number_list")
         self.verticalLayout_3.addWidget(self.collector_number_list)
         self.gridLayout.addWidget(self.collector_number_box, 7, 3, 9, 1)
-        self.language_combo_box = QtWidgets.QComboBox(AddCardWidget)
+        self.language_combo_box = QtWidgets.QComboBox(AddCardWidget_Horizontal)
         self.language_combo_box.setObjectName("language_combo_box")
         self.gridLayout.addWidget(self.language_combo_box, 8, 5, 1, 1)
-        self.copies_label = QtWidgets.QLabel(AddCardWidget)
+        self.copies_label = QtWidgets.QLabel(AddCardWidget_Horizontal)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.copies_label.sizePolicy().hasHeightForWidth())
         self.copies_label.setSizePolicy(sizePolicy)
         self.copies_label.setObjectName("copies_label")
         self.gridLayout.addWidget(self.copies_label, 9, 5, 1, 1)
-        self.copies_input = QtWidgets.QSpinBox(AddCardWidget)
+        self.copies_input = QtWidgets.QSpinBox(AddCardWidget_Horizontal)
         self.copies_input.setMinimum(1)
         self.copies_input.setObjectName("copies_input")
         self.gridLayout.addWidget(self.copies_input, 10, 5, 1, 1)
-        self.button_box = QtWidgets.QDialogButtonBox(AddCardWidget)
+        self.button_box = QtWidgets.QDialogButtonBox(AddCardWidget_Horizontal)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.button_box.sizePolicy().hasHeightForWidth())
         self.button_box.setSizePolicy(sizePolicy)
         self.button_box.setOrientation(QtCore.Qt.Vertical)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Ok|QtWidgets.QDialogButtonBox.Reset)
         self.button_box.setObjectName("button_box")
         self.gridLayout.addWidget(self.button_box, 11, 5, 5, 1)
         self.language_label.setBuddy(self.language_combo_box)
         self.copies_label.setBuddy(self.copies_input)
 
-        self.retranslateUi(AddCardWidget)
-        QtCore.QMetaObject.connectSlotsByName(AddCardWidget)
-        AddCardWidget.setTabOrder(self.card_name_filter, self.card_name_list)
-        AddCardWidget.setTabOrder(self.card_name_list, self.set_name_filter)
-        AddCardWidget.setTabOrder(self.set_name_filter, self.set_name_list)
-        AddCardWidget.setTabOrder(self.set_name_list, self.collector_number_list)
-        AddCardWidget.setTabOrder(self.collector_number_list, self.language_combo_box)
-        AddCardWidget.setTabOrder(self.language_combo_box, self.copies_input)
+        self.retranslateUi(AddCardWidget_Horizontal)
+        QtCore.QMetaObject.connectSlotsByName(AddCardWidget_Horizontal)
+        AddCardWidget_Horizontal.setTabOrder(self.card_name_filter, self.card_name_list)
+        AddCardWidget_Horizontal.setTabOrder(self.card_name_list, self.set_name_filter)
+        AddCardWidget_Horizontal.setTabOrder(self.set_name_filter, self.set_name_list)
+        AddCardWidget_Horizontal.setTabOrder(self.set_name_list, self.collector_number_list)
+        AddCardWidget_Horizontal.setTabOrder(self.collector_number_list, self.language_combo_box)
+        AddCardWidget_Horizontal.setTabOrder(self.language_combo_box, self.copies_input)
 
-    def retranslateUi(self, AddCardWidget):
+    def retranslateUi(self, AddCardWidget_Horizontal):
         _translate = QtCore.QCoreApplication.translate
-        self.language_label.setText(_translate("AddCardWidget", "Language:"))
-        self.card_name_box.setTitle(_translate("AddCardWidget", "Card Name"))
-        self.card_name_filter.setToolTip(_translate("AddCardWidget", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
-        self.card_name_filter.setPlaceholderText(_translate("AddCardWidget", "Filter card names"))
-        self.card_name_list.setToolTip(_translate("AddCardWidget", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
-        self.set_name_box.setToolTip(_translate("AddCardWidget", "The sets in which the currently selected card was printed."))
-        self.set_name_box.setTitle(_translate("AddCardWidget", "Set"))
-        self.set_name_filter.setPlaceholderText(_translate("AddCardWidget", "Filter set names"))
-        self.collector_number_box.setTitle(_translate("AddCardWidget", "Collector Number"))
-        self.copies_label.setText(_translate("AddCardWidget", "Copies"))
+        self.language_label.setText(_translate("AddCardWidget_Horizontal", "Language:"))
+        self.card_name_box.setTitle(_translate("AddCardWidget_Horizontal", "Card Name"))
+        self.card_name_filter.setToolTip(_translate("AddCardWidget_Horizontal", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
+        self.card_name_filter.setPlaceholderText(_translate("AddCardWidget_Horizontal", "Filter card names"))
+        self.card_name_list.setToolTip(_translate("AddCardWidget_Horizontal", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
+        self.set_name_box.setToolTip(_translate("AddCardWidget_Horizontal", "The sets in which the currently selected card was printed."))
+        self.set_name_box.setTitle(_translate("AddCardWidget_Horizontal", "Set"))
+        self.set_name_filter.setPlaceholderText(_translate("AddCardWidget_Horizontal", "Filter set names"))
+        self.collector_number_box.setTitle(_translate("AddCardWidget_Horizontal", "Collector Number"))
+        self.copies_label.setText(_translate("AddCardWidget_Horizontal", "Copies"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/add_card_widget/vertical.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_AddCardWidget(object):
-    def setupUi(self, AddCardWidget):
-        AddCardWidget.setObjectName("AddCardWidget")
-        AddCardWidget.resize(349, 715)
-        self.gridLayout = QtWidgets.QGridLayout(AddCardWidget)
+class Ui_AddCardWidget_Vertical(object):
+    def setupUi(self, AddCardWidget_Vertical):
+        AddCardWidget_Vertical.setObjectName("AddCardWidget_Vertical")
+        AddCardWidget_Vertical.resize(349, 715)
+        self.gridLayout = QtWidgets.QGridLayout(AddCardWidget_Vertical)
         self.gridLayout.setObjectName("gridLayout")
-        self.set_name_box = QtWidgets.QGroupBox(AddCardWidget)
+        self.set_name_box = QtWidgets.QGroupBox(AddCardWidget_Vertical)
         self.set_name_box.setEnabled(False)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(7)
         sizePolicy.setHeightForWidth(self.set_name_box.sizePolicy().hasHeightForWidth())
         self.set_name_box.setSizePolicy(sizePolicy)
         self.set_name_box.setObjectName("set_name_box")
@@ -33,15 +33,15 @@
         self.verticalLayout_2.addWidget(self.set_name_filter)
         self.set_name_list = QtWidgets.QListView(self.set_name_box)
         self.set_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.set_name_list.setAlternatingRowColors(True)
         self.set_name_list.setObjectName("set_name_list")
         self.verticalLayout_2.addWidget(self.set_name_list)
         self.gridLayout.addWidget(self.set_name_box, 3, 0, 1, 3)
-        self.collector_number_box = QtWidgets.QGroupBox(AddCardWidget)
+        self.collector_number_box = QtWidgets.QGroupBox(AddCardWidget_Vertical)
         self.collector_number_box.setEnabled(False)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(2)
         sizePolicy.setHeightForWidth(self.collector_number_box.sizePolicy().hasHeightForWidth())
         self.collector_number_box.setSizePolicy(sizePolicy)
         self.collector_number_box.setObjectName("collector_number_box")
@@ -49,15 +49,15 @@
         self.verticalLayout_3.setObjectName("verticalLayout_3")
         self.collector_number_list = QtWidgets.QListView(self.collector_number_box)
         self.collector_number_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.collector_number_list.setAlternatingRowColors(True)
         self.collector_number_list.setObjectName("collector_number_list")
         self.verticalLayout_3.addWidget(self.collector_number_list)
         self.gridLayout.addWidget(self.collector_number_box, 10, 0, 1, 3)
-        self.card_name_box = QtWidgets.QGroupBox(AddCardWidget)
+        self.card_name_box = QtWidgets.QGroupBox(AddCardWidget_Vertical)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(7)
         sizePolicy.setHeightForWidth(self.card_name_box.sizePolicy().hasHeightForWidth())
         self.card_name_box.setSizePolicy(sizePolicy)
         self.card_name_box.setObjectName("card_name_box")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.card_name_box)
@@ -68,58 +68,58 @@
         self.verticalLayout.addWidget(self.card_name_filter)
         self.card_name_list = QtWidgets.QListView(self.card_name_box)
         self.card_name_list.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
         self.card_name_list.setAlternatingRowColors(True)
         self.card_name_list.setObjectName("card_name_list")
         self.verticalLayout.addWidget(self.card_name_list)
         self.gridLayout.addWidget(self.card_name_box, 2, 0, 1, 3)
-        self.language_combo_box = QtWidgets.QComboBox(AddCardWidget)
+        self.language_combo_box = QtWidgets.QComboBox(AddCardWidget_Vertical)
         self.language_combo_box.setObjectName("language_combo_box")
         self.gridLayout.addWidget(self.language_combo_box, 0, 1, 1, 2)
-        self.language_label = QtWidgets.QLabel(AddCardWidget)
+        self.language_label = QtWidgets.QLabel(AddCardWidget_Vertical)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Maximum, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.language_label.sizePolicy().hasHeightForWidth())
         self.language_label.setSizePolicy(sizePolicy)
         self.language_label.setObjectName("language_label")
         self.gridLayout.addWidget(self.language_label, 0, 0, 1, 1)
-        self.copies_label = QtWidgets.QLabel(AddCardWidget)
+        self.copies_label = QtWidgets.QLabel(AddCardWidget_Vertical)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Preferred, QtWidgets.QSizePolicy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.copies_label.sizePolicy().hasHeightForWidth())
         self.copies_label.setSizePolicy(sizePolicy)
         self.copies_label.setObjectName("copies_label")
         self.gridLayout.addWidget(self.copies_label, 11, 0, 1, 1)
-        self.copies_input = QtWidgets.QSpinBox(AddCardWidget)
+        self.copies_input = QtWidgets.QSpinBox(AddCardWidget_Vertical)
         self.copies_input.setMinimum(1)
         self.copies_input.setObjectName("copies_input")
         self.gridLayout.addWidget(self.copies_input, 11, 1, 1, 2)
-        self.button_box = QtWidgets.QDialogButtonBox(AddCardWidget)
+        self.button_box = QtWidgets.QDialogButtonBox(AddCardWidget_Vertical)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Ok|QtWidgets.QDialogButtonBox.Reset)
         self.button_box.setObjectName("button_box")
         self.gridLayout.addWidget(self.button_box, 12, 0, 1, 3)
         self.language_label.setBuddy(self.language_combo_box)
         self.copies_label.setBuddy(self.copies_input)
 
-        self.retranslateUi(AddCardWidget)
-        QtCore.QMetaObject.connectSlotsByName(AddCardWidget)
-        AddCardWidget.setTabOrder(self.language_combo_box, self.card_name_filter)
-        AddCardWidget.setTabOrder(self.card_name_filter, self.card_name_list)
-        AddCardWidget.setTabOrder(self.card_name_list, self.set_name_filter)
-        AddCardWidget.setTabOrder(self.set_name_filter, self.set_name_list)
-        AddCardWidget.setTabOrder(self.set_name_list, self.collector_number_list)
-        AddCardWidget.setTabOrder(self.collector_number_list, self.copies_input)
+        self.retranslateUi(AddCardWidget_Vertical)
+        QtCore.QMetaObject.connectSlotsByName(AddCardWidget_Vertical)
+        AddCardWidget_Vertical.setTabOrder(self.language_combo_box, self.card_name_filter)
+        AddCardWidget_Vertical.setTabOrder(self.card_name_filter, self.card_name_list)
+        AddCardWidget_Vertical.setTabOrder(self.card_name_list, self.set_name_filter)
+        AddCardWidget_Vertical.setTabOrder(self.set_name_filter, self.set_name_list)
+        AddCardWidget_Vertical.setTabOrder(self.set_name_list, self.collector_number_list)
+        AddCardWidget_Vertical.setTabOrder(self.collector_number_list, self.copies_input)
 
-    def retranslateUi(self, AddCardWidget):
+    def retranslateUi(self, AddCardWidget_Vertical):
         _translate = QtCore.QCoreApplication.translate
-        self.set_name_box.setToolTip(_translate("AddCardWidget", "The sets in which the currently selected card was printed."))
-        self.set_name_box.setTitle(_translate("AddCardWidget", "Set"))
-        self.set_name_filter.setPlaceholderText(_translate("AddCardWidget", "Filter set names"))
-        self.collector_number_box.setTitle(_translate("AddCardWidget", "Collector Number"))
-        self.card_name_box.setTitle(_translate("AddCardWidget", "Card Name"))
-        self.card_name_filter.setToolTip(_translate("AddCardWidget", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
-        self.card_name_filter.setPlaceholderText(_translate("AddCardWidget", "Filter card names"))
-        self.card_name_list.setToolTip(_translate("AddCardWidget", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
-        self.language_label.setText(_translate("AddCardWidget", "Language:"))
-        self.copies_label.setText(_translate("AddCardWidget", "Copies:"))
+        self.set_name_box.setToolTip(_translate("AddCardWidget_Vertical", "The sets in which the currently selected card was printed."))
+        self.set_name_box.setTitle(_translate("AddCardWidget_Vertical", "Set"))
+        self.set_name_filter.setPlaceholderText(_translate("AddCardWidget_Vertical", "Filter set names"))
+        self.collector_number_box.setTitle(_translate("AddCardWidget_Vertical", "Collector Number"))
+        self.card_name_box.setTitle(_translate("AddCardWidget_Vertical", "Card Name"))
+        self.card_name_filter.setToolTip(_translate("AddCardWidget_Vertical", "Filter the list below. Use  % (Percent signs) as wildcards matching any number of characters."))
+        self.card_name_filter.setPlaceholderText(_translate("AddCardWidget_Vertical", "Filter card names"))
+        self.card_name_list.setToolTip(_translate("AddCardWidget_Vertical", "The filtered list of card names in the currently selected language. Click on an entry to select it and choose a printing."))
+        self.language_label.setText(_translate("AddCardWidget_Vertical", "Language:"))
+        self.copies_label.setText(_translate("AddCardWidget_Vertical", "Copies:"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/card_filter_page.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_WizardPage(object):
-    def setupUi(self, WizardPage):
-        WizardPage.setObjectName("WizardPage")
-        WizardPage.resize(406, 568)
-        self.verticalLayout_3 = QtWidgets.QVBoxLayout(WizardPage)
+class Ui_CardFilterPage(object):
+    def setupUi(self, CardFilterPage):
+        CardFilterPage.setObjectName("CardFilterPage")
+        CardFilterPage.resize(406, 568)
+        self.verticalLayout_3 = QtWidgets.QVBoxLayout(CardFilterPage)
         self.verticalLayout_3.setObjectName("verticalLayout_3")
-        self.splitter = QtWidgets.QSplitter(WizardPage)
+        self.splitter = QtWidgets.QSplitter(CardFilterPage)
         self.splitter.setOrientation(QtCore.Qt.Vertical)
         self.splitter.setObjectName("splitter")
         self.verticalLayoutWidget = QtWidgets.QWidget(self.splitter)
         self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.verticalLayoutWidget)
         self.verticalLayout.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout.setObjectName("verticalLayout")
@@ -54,18 +54,17 @@
         self.unknown_image_view.horizontalHeader().setStretchLastSection(True)
         self.unknown_image_view.verticalHeader().setVisible(False)
         self.verticalLayout_2.addWidget(self.unknown_image_view)
         self.verticalLayout_3.addWidget(self.splitter)
         self.card_image_view_label.setBuddy(self.card_image_view)
         self.unknown_images_view_label.setBuddy(self.unknown_image_view)
 
-        self.retranslateUi(WizardPage)
-        QtCore.QMetaObject.connectSlotsByName(WizardPage)
+        self.retranslateUi(CardFilterPage)
+        QtCore.QMetaObject.connectSlotsByName(CardFilterPage)
 
-    def retranslateUi(self, WizardPage):
+    def retranslateUi(self, CardFilterPage):
         _translate = QtCore.QCoreApplication.translate
-        WizardPage.setWindowTitle(_translate("WizardPage", "WizardPage"))
-        WizardPage.setTitle(_translate("WizardPage", "Select images for removal"))
-        WizardPage.setSubTitle(_translate("WizardPage", "Click on entries in the tables below to mark or un-mark them for removal. All selected entries will be removed."))
-        self.card_image_view_label.setText(_translate("WizardPage", "All images currently stored on disk:"))
-        self.unknown_images_view_label.setToolTip(_translate("WizardPage", "Images found on disk that can not be associated with any card."))
-        self.unknown_images_view_label.setText(_translate("WizardPage", "Unknown images:"))
+        CardFilterPage.setTitle(_translate("CardFilterPage", "Select images for removal"))
+        CardFilterPage.setSubTitle(_translate("CardFilterPage", "Click on entries in the tables below to mark or un-mark them for removal. All selected entries will be removed."))
+        self.card_image_view_label.setText(_translate("CardFilterPage", "All images currently stored on disk:"))
+        self.unknown_images_view_label.setToolTip(_translate("CardFilterPage", "Images found on disk that can not be associated with any card."))
+        self.unknown_images_view_label.setText(_translate("CardFilterPage", "Unknown images:"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/filter_setup_page.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_WizardPage(object):
-    def setupUi(self, WizardPage):
-        WizardPage.setObjectName("WizardPage")
-        WizardPage.resize(417, 186)
-        self.verticalLayout = QtWidgets.QVBoxLayout(WizardPage)
+class Ui_FilterSetupPage(object):
+    def setupUi(self, FilterSetupPage):
+        FilterSetupPage.setObjectName("FilterSetupPage")
+        FilterSetupPage.resize(417, 186)
+        self.verticalLayout = QtWidgets.QVBoxLayout(FilterSetupPage)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.delete_everything_checkbox = QtWidgets.QCheckBox(WizardPage)
+        self.delete_everything_checkbox = QtWidgets.QCheckBox(FilterSetupPage)
         icon = QtGui.QIcon.fromTheme("edit-delete")
         self.delete_everything_checkbox.setIcon(icon)
         self.delete_everything_checkbox.setObjectName("delete_everything_checkbox")
         self.verticalLayout.addWidget(self.delete_everything_checkbox)
-        self.individual_filter_group = QtWidgets.QGroupBox(WizardPage)
+        self.individual_filter_group = QtWidgets.QGroupBox(FilterSetupPage)
         self.individual_filter_group.setObjectName("individual_filter_group")
         self.gridLayout_2 = QtWidgets.QGridLayout(self.individual_filter_group)
         self.gridLayout_2.setObjectName("gridLayout_2")
         self.count_filter_enabled_checkbox = QtWidgets.QCheckBox(self.individual_filter_group)
         self.count_filter_enabled_checkbox.setObjectName("count_filter_enabled_checkbox")
         self.gridLayout_2.addWidget(self.count_filter_enabled_checkbox, 1, 0, 1, 1)
         self.time_filter_enabled_checkbox = QtWidgets.QCheckBox(self.individual_filter_group)
@@ -47,35 +47,34 @@
         self.remove_unknown_cards_checkbox = QtWidgets.QCheckBox(self.individual_filter_group)
         self.remove_unknown_cards_checkbox.setObjectName("remove_unknown_cards_checkbox")
         self.gridLayout_2.addWidget(self.remove_unknown_cards_checkbox, 2, 0, 1, 2)
         self.verticalLayout.addWidget(self.individual_filter_group)
         spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout.addItem(spacerItem)
 
-        self.retranslateUi(WizardPage)
+        self.retranslateUi(FilterSetupPage)
         self.time_filter_enabled_checkbox.toggled['bool'].connect(self.time_filter_value_spinbox.setEnabled) # type: ignore
         self.count_filter_enabled_checkbox.toggled['bool'].connect(self.count_filter_value_spinbox.setEnabled) # type: ignore
         self.delete_everything_checkbox.toggled['bool'].connect(self.individual_filter_group.setDisabled) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(WizardPage)
-        WizardPage.setTabOrder(self.delete_everything_checkbox, self.time_filter_enabled_checkbox)
-        WizardPage.setTabOrder(self.time_filter_enabled_checkbox, self.time_filter_value_spinbox)
-        WizardPage.setTabOrder(self.time_filter_value_spinbox, self.count_filter_enabled_checkbox)
-        WizardPage.setTabOrder(self.count_filter_enabled_checkbox, self.count_filter_value_spinbox)
-        WizardPage.setTabOrder(self.count_filter_value_spinbox, self.remove_unknown_cards_checkbox)
+        QtCore.QMetaObject.connectSlotsByName(FilterSetupPage)
+        FilterSetupPage.setTabOrder(self.delete_everything_checkbox, self.time_filter_enabled_checkbox)
+        FilterSetupPage.setTabOrder(self.time_filter_enabled_checkbox, self.time_filter_value_spinbox)
+        FilterSetupPage.setTabOrder(self.time_filter_value_spinbox, self.count_filter_enabled_checkbox)
+        FilterSetupPage.setTabOrder(self.count_filter_enabled_checkbox, self.count_filter_value_spinbox)
+        FilterSetupPage.setTabOrder(self.count_filter_value_spinbox, self.remove_unknown_cards_checkbox)
 
-    def retranslateUi(self, WizardPage):
+    def retranslateUi(self, FilterSetupPage):
         _translate = QtCore.QCoreApplication.translate
-        WizardPage.setWindowTitle(_translate("WizardPage", "WizardPage"))
-        WizardPage.setTitle(_translate("WizardPage", "Cleanup locally stored card images"))
-        WizardPage.setSubTitle(_translate("WizardPage", "This wizard can be used to remove unwanted card images currently stored on your computer. You can enable automatic cleanup conditions below, to preselect images for removal."))
-        self.delete_everything_checkbox.setText(_translate("WizardPage", "Delete everything"))
-        self.individual_filter_group.setToolTip(_translate("WizardPage", "Select images for removal based on any matching criterion."))
-        self.individual_filter_group.setTitle(_translate("WizardPage", "Select images for deletion, if …"))
-        self.count_filter_enabled_checkbox.setText(_translate("WizardPage", "Used in prints and PDFs less often than:"))
-        self.time_filter_enabled_checkbox.setText(_translate("WizardPage", "Not used in the last:"))
-        self.time_filter_value_spinbox.setSuffix(_translate("WizardPage", " days"))
-        self.count_filter_value_spinbox.setSuffix(_translate("WizardPage", " times"))
-        self.remove_unknown_cards_checkbox.setToolTip(_translate("WizardPage", "Card images may become unknown, if printings are removed by Scryfall.\n"
+        FilterSetupPage.setTitle(_translate("FilterSetupPage", "Cleanup locally stored card images"))
+        FilterSetupPage.setSubTitle(_translate("FilterSetupPage", "This wizard can be used to remove unwanted card images currently stored on your computer. You can enable automatic cleanup conditions below, to preselect images for removal."))
+        self.delete_everything_checkbox.setText(_translate("FilterSetupPage", "Delete everything"))
+        self.individual_filter_group.setToolTip(_translate("FilterSetupPage", "Select images for removal based on any matching criterion."))
+        self.individual_filter_group.setTitle(_translate("FilterSetupPage", "Select images for deletion, if …"))
+        self.count_filter_enabled_checkbox.setText(_translate("FilterSetupPage", "Used in prints and PDFs less often than:"))
+        self.time_filter_enabled_checkbox.setText(_translate("FilterSetupPage", "Not used in the last:"))
+        self.time_filter_value_spinbox.setSuffix(_translate("FilterSetupPage", " days"))
+        self.count_filter_value_spinbox.setSuffix(_translate("FilterSetupPage", " times"))
+        self.remove_unknown_cards_checkbox.setToolTip(_translate("FilterSetupPage", "Card images may become unknown, if printings are removed by Scryfall.\n"
 "This filter also applies to cards and printings hidden by a card filter in the settings.\n"
 "For example, if you downloaded images of silver-bordered cards and then configured the program to hide those,\n"
 "all these images become hidden and will be removed."))
-        self.remove_unknown_cards_checkbox.setText(_translate("WizardPage", "Remove unknown images and images of hidden printings"))
+        self.remove_unknown_cards_checkbox.setText(_translate("FilterSetupPage", "Remove unknown images and images of hidden printings"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/cache_cleanup_wizard/summary_page.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_WizardPage(object):
-    def setupUi(self, WizardPage):
-        WizardPage.setObjectName("WizardPage")
-        WizardPage.resize(266, 90)
-        self.verticalLayout = QtWidgets.QVBoxLayout(WizardPage)
+class Ui_SummaryPage(object):
+    def setupUi(self, SummaryPage):
+        SummaryPage.setObjectName("SummaryPage")
+        SummaryPage.resize(266, 90)
+        self.verticalLayout = QtWidgets.QVBoxLayout(SummaryPage)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.image_count_summary = QtWidgets.QLabel(WizardPage)
+        self.image_count_summary = QtWidgets.QLabel(SummaryPage)
         self.image_count_summary.setText("")
         self.image_count_summary.setObjectName("image_count_summary")
         self.verticalLayout.addWidget(self.image_count_summary)
-        self.filesize_summary = QtWidgets.QLabel(WizardPage)
+        self.filesize_summary = QtWidgets.QLabel(SummaryPage)
         self.filesize_summary.setText("")
         self.filesize_summary.setObjectName("filesize_summary")
         self.verticalLayout.addWidget(self.filesize_summary)
         spacerItem = QtWidgets.QSpacerItem(20, 27, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.verticalLayout.addItem(spacerItem)
 
-        self.retranslateUi(WizardPage)
-        QtCore.QMetaObject.connectSlotsByName(WizardPage)
+        self.retranslateUi(SummaryPage)
+        QtCore.QMetaObject.connectSlotsByName(SummaryPage)
 
-    def retranslateUi(self, WizardPage):
+    def retranslateUi(self, SummaryPage):
         _translate = QtCore.QCoreApplication.translate
-        WizardPage.setWindowTitle(_translate("WizardPage", "WizardPage"))
-        WizardPage.setTitle(_translate("WizardPage", "Summary"))
+        SummaryPage.setTitle(_translate("SummaryPage", "Summary"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/columnar.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/tabbed_vertical.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,90 +1,72 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/columnar.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/tabbed_vertical.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_central_widget(object):
-    def setupUi(self, central_widget):
-        central_widget.setObjectName("central_widget")
-        central_widget.resize(888, 258)
-        self.gridLayout = QtWidgets.QGridLayout(central_widget)
-        self.gridLayout.setContentsMargins(-1, -1, -1, 0)
+class Ui_CentralWidget_Tabbed(object):
+    def setupUi(self, CentralWidget_Tabbed):
+        CentralWidget_Tabbed.setObjectName("CentralWidget_Tabbed")
+        CentralWidget_Tabbed.resize(454, 765)
+        self.gridLayout = QtWidgets.QGridLayout(CentralWidget_Tabbed)
+        self.gridLayout.setContentsMargins(0, 0, 0, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.page_renderer = PageRenderer(central_widget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(9)
-        sizePolicy.setVerticalStretch(1)
-        sizePolicy.setHeightForWidth(self.page_renderer.sizePolicy().hasHeightForWidth())
-        self.page_renderer.setSizePolicy(sizePolicy)
-        self.page_renderer.setAcceptDrops(False)
-        self.page_renderer.setRenderHints(QtGui.QPainter.Antialiasing|QtGui.QPainter.HighQualityAntialiasing)
-        self.page_renderer.setObjectName("page_renderer")
-        self.gridLayout.addWidget(self.page_renderer, 4, 3, 3, 1)
-        self.page_card_table_view = QtWidgets.QTableView(central_widget)
+        self.tab_widget = QtWidgets.QTabWidget(CentralWidget_Tabbed)
+        self.tab_widget.setObjectName("tab_widget")
+        self.document_view = QtWidgets.QListView()
+        self.document_view.setObjectName("document_view")
+        self.tab_widget.addTab(self.document_view, "")
+        self.add_card_widget = VerticalAddCardWidget()
+        self.add_card_widget.setObjectName("add_card_widget")
+        self.tab_widget.addTab(self.add_card_widget, "")
+        self.tab = QtWidgets.QWidget()
+        self.tab.setObjectName("tab")
+        self.verticalLayout = QtWidgets.QVBoxLayout(self.tab)
+        self.verticalLayout.setContentsMargins(0, 0, 0, 0)
+        self.verticalLayout.setObjectName("verticalLayout")
+        self.page_card_table_view = QtWidgets.QTableView(self.tab)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(9)
-        sizePolicy.setVerticalStretch(1)
+        sizePolicy.setHorizontalStretch(5)
+        sizePolicy.setVerticalStretch(10)
         sizePolicy.setHeightForWidth(self.page_card_table_view.sizePolicy().hasHeightForWidth())
         self.page_card_table_view.setSizePolicy(sizePolicy)
         self.page_card_table_view.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.page_card_table_view.setLineWidth(0)
         self.page_card_table_view.setAlternatingRowColors(True)
         self.page_card_table_view.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
         self.page_card_table_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.page_card_table_view.setObjectName("page_card_table_view")
         self.page_card_table_view.verticalHeader().setVisible(False)
-        self.gridLayout.addWidget(self.page_card_table_view, 4, 2, 2, 1)
-        self.document_view_label = QtWidgets.QLabel(central_widget)
-        self.document_view_label.setObjectName("document_view_label")
-        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 1)
-        self.page_view_label = QtWidgets.QLabel(central_widget)
-        self.page_view_label.setObjectName("page_view_label")
-        self.gridLayout.addWidget(self.page_view_label, 0, 2, 1, 2)
-        self.delete_selected_images_button = QtWidgets.QPushButton(central_widget)
+        self.verticalLayout.addWidget(self.page_card_table_view)
+        self.delete_selected_images_button = QtWidgets.QPushButton(self.tab)
         self.delete_selected_images_button.setEnabled(False)
         icon = QtGui.QIcon.fromTheme("edit-delete")
         self.delete_selected_images_button.setIcon(icon)
         self.delete_selected_images_button.setObjectName("delete_selected_images_button")
-        self.gridLayout.addWidget(self.delete_selected_images_button, 6, 2, 1, 1)
-        self.add_card_widget_label = QtWidgets.QLabel(central_widget)
-        self.add_card_widget_label.setObjectName("add_card_widget_label")
-        self.gridLayout.addWidget(self.add_card_widget_label, 0, 1, 1, 1)
-        self.add_card_widget = VerticalAddCardWidget(central_widget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(1)
-        sizePolicy.setHeightForWidth(self.add_card_widget.sizePolicy().hasHeightForWidth())
-        self.add_card_widget.setSizePolicy(sizePolicy)
-        self.add_card_widget.setObjectName("add_card_widget")
-        self.gridLayout.addWidget(self.add_card_widget, 4, 1, 3, 1)
-        self.document_view = QtWidgets.QListView(central_widget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(4)
-        sizePolicy.setVerticalStretch(1)
-        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
-        self.document_view.setSizePolicy(sizePolicy)
-        self.document_view.setAlternatingRowColors(True)
-        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
-        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
-        self.document_view.setObjectName("document_view")
-        self.gridLayout.addWidget(self.document_view, 4, 0, 3, 1)
+        self.verticalLayout.addWidget(self.delete_selected_images_button)
+        self.tab_widget.addTab(self.tab, "")
+        self.page_renderer = PageRenderer()
+        self.page_renderer.setObjectName("page_renderer")
+        self.tab_widget.addTab(self.page_renderer, "")
+        self.gridLayout.addWidget(self.tab_widget, 4, 0, 2, 2)
 
-        self.retranslateUi(central_widget)
-        QtCore.QMetaObject.connectSlotsByName(central_widget)
+        self.retranslateUi(CentralWidget_Tabbed)
+        self.tab_widget.setCurrentIndex(0)
+        QtCore.QMetaObject.connectSlotsByName(CentralWidget_Tabbed)
 
-    def retranslateUi(self, central_widget):
+    def retranslateUi(self, CentralWidget_Tabbed):
         _translate = QtCore.QCoreApplication.translate
-        self.document_view_label.setText(_translate("central_widget", "All pages:"))
-        self.page_view_label.setText(_translate("central_widget", "Current page:"))
-        self.delete_selected_images_button.setText(_translate("central_widget", "Remove selected"))
-        self.add_card_widget_label.setText(_translate("central_widget", "Add new cards:"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.document_view), _translate("CentralWidget_Tabbed", "All pages"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.add_card_widget), _translate("CentralWidget_Tabbed", "Add new cards"))
+        self.delete_selected_images_button.setText(_translate("CentralWidget_Tabbed", "Remove selected"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab), _translate("CentralWidget_Tabbed", "Current page"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.page_renderer), _translate("CentralWidget_Tabbed", "Preview"))
 from mtg_proxy_printer.ui.add_card import VerticalAddCardWidget
 from mtg_proxy_printer.ui.page_renderer import PageRenderer
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/central_widget/grouped.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/central_widget/columnar.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,90 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/grouped.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/central_widget/columnar.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_central_widget(object):
-    def setupUi(self, central_widget):
-        central_widget.setObjectName("central_widget")
-        central_widget.resize(580, 539)
-        self.gridLayout = QtWidgets.QGridLayout(central_widget)
+class Ui_CentralWidget_Columnar(object):
+    def setupUi(self, CentralWidget_Columnar):
+        CentralWidget_Columnar.setObjectName("CentralWidget_Columnar")
+        CentralWidget_Columnar.resize(888, 258)
+        self.gridLayout = QtWidgets.QGridLayout(CentralWidget_Columnar)
         self.gridLayout.setContentsMargins(-1, -1, -1, 0)
         self.gridLayout.setObjectName("gridLayout")
-        self.page_renderer = PageRenderer(central_widget)
+        self.page_renderer = PageRenderer(CentralWidget_Columnar)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(10)
+        sizePolicy.setHorizontalStretch(9)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(self.page_renderer.sizePolicy().hasHeightForWidth())
         self.page_renderer.setSizePolicy(sizePolicy)
         self.page_renderer.setAcceptDrops(False)
         self.page_renderer.setRenderHints(QtGui.QPainter.Antialiasing|QtGui.QPainter.HighQualityAntialiasing)
         self.page_renderer.setObjectName("page_renderer")
-        self.gridLayout.addWidget(self.page_renderer, 5, 3, 3, 1)
-        self.document_view = QtWidgets.QListView(central_widget)
-        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(3)
-        sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
-        self.document_view.setSizePolicy(sizePolicy)
-        self.document_view.setAlternatingRowColors(True)
-        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
-        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
-        self.document_view.setObjectName("document_view")
-        self.gridLayout.addWidget(self.document_view, 1, 0, 7, 2)
-        self.delete_selected_images_button = QtWidgets.QPushButton(central_widget)
-        self.delete_selected_images_button.setEnabled(False)
-        icon = QtGui.QIcon.fromTheme("edit-delete")
-        self.delete_selected_images_button.setIcon(icon)
-        self.delete_selected_images_button.setObjectName("delete_selected_images_button")
-        self.gridLayout.addWidget(self.delete_selected_images_button, 7, 2, 1, 1)
-        self.page_card_table_view = QtWidgets.QTableView(central_widget)
+        self.gridLayout.addWidget(self.page_renderer, 4, 3, 3, 1)
+        self.page_card_table_view = QtWidgets.QTableView(CentralWidget_Columnar)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
-        sizePolicy.setHorizontalStretch(8)
-        sizePolicy.setVerticalStretch(10)
+        sizePolicy.setHorizontalStretch(9)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(self.page_card_table_view.sizePolicy().hasHeightForWidth())
         self.page_card_table_view.setSizePolicy(sizePolicy)
         self.page_card_table_view.setContextMenuPolicy(QtCore.Qt.CustomContextMenu)
         self.page_card_table_view.setLineWidth(0)
         self.page_card_table_view.setAlternatingRowColors(True)
         self.page_card_table_view.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
         self.page_card_table_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
         self.page_card_table_view.setObjectName("page_card_table_view")
         self.page_card_table_view.verticalHeader().setVisible(False)
-        self.gridLayout.addWidget(self.page_card_table_view, 5, 2, 2, 1)
-        self.add_card_widget = HorizontalAddCardWidget(central_widget)
+        self.gridLayout.addWidget(self.page_card_table_view, 4, 2, 2, 1)
+        self.document_view_label = QtWidgets.QLabel(CentralWidget_Columnar)
+        self.document_view_label.setObjectName("document_view_label")
+        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 1)
+        self.page_view_label = QtWidgets.QLabel(CentralWidget_Columnar)
+        self.page_view_label.setObjectName("page_view_label")
+        self.gridLayout.addWidget(self.page_view_label, 0, 2, 1, 2)
+        self.delete_selected_images_button = QtWidgets.QPushButton(CentralWidget_Columnar)
+        self.delete_selected_images_button.setEnabled(False)
+        icon = QtGui.QIcon.fromTheme("edit-delete")
+        self.delete_selected_images_button.setIcon(icon)
+        self.delete_selected_images_button.setObjectName("delete_selected_images_button")
+        self.gridLayout.addWidget(self.delete_selected_images_button, 6, 2, 1, 1)
+        self.add_card_widget_label = QtWidgets.QLabel(CentralWidget_Columnar)
+        self.add_card_widget_label.setObjectName("add_card_widget_label")
+        self.gridLayout.addWidget(self.add_card_widget_label, 0, 1, 1, 1)
+        self.add_card_widget = VerticalAddCardWidget(CentralWidget_Columnar)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(7)
-        sizePolicy.setVerticalStretch(6)
+        sizePolicy.setVerticalStretch(1)
         sizePolicy.setHeightForWidth(self.add_card_widget.sizePolicy().hasHeightForWidth())
         self.add_card_widget.setSizePolicy(sizePolicy)
         self.add_card_widget.setObjectName("add_card_widget")
-        self.gridLayout.addWidget(self.add_card_widget, 1, 2, 2, 2)
-        self.document_view_label = QtWidgets.QLabel(central_widget)
-        self.document_view_label.setObjectName("document_view_label")
-        self.gridLayout.addWidget(self.document_view_label, 0, 0, 1, 2)
-        self.add_card_widget_label = QtWidgets.QLabel(central_widget)
-        self.add_card_widget_label.setObjectName("add_card_widget_label")
-        self.gridLayout.addWidget(self.add_card_widget_label, 0, 2, 1, 2)
+        self.gridLayout.addWidget(self.add_card_widget, 4, 1, 3, 1)
+        self.document_view = QtWidgets.QListView(CentralWidget_Columnar)
+        sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
+        sizePolicy.setHorizontalStretch(4)
+        sizePolicy.setVerticalStretch(1)
+        sizePolicy.setHeightForWidth(self.document_view.sizePolicy().hasHeightForWidth())
+        self.document_view.setSizePolicy(sizePolicy)
+        self.document_view.setAlternatingRowColors(True)
+        self.document_view.setSelectionMode(QtWidgets.QAbstractItemView.SingleSelection)
+        self.document_view.setSelectionBehavior(QtWidgets.QAbstractItemView.SelectRows)
+        self.document_view.setObjectName("document_view")
+        self.gridLayout.addWidget(self.document_view, 4, 0, 3, 1)
 
-        self.retranslateUi(central_widget)
-        QtCore.QMetaObject.connectSlotsByName(central_widget)
+        self.retranslateUi(CentralWidget_Columnar)
+        QtCore.QMetaObject.connectSlotsByName(CentralWidget_Columnar)
 
-    def retranslateUi(self, central_widget):
+    def retranslateUi(self, CentralWidget_Columnar):
         _translate = QtCore.QCoreApplication.translate
-        self.delete_selected_images_button.setText(_translate("central_widget", "Remove selected"))
-        self.document_view_label.setText(_translate("central_widget", "All pages:"))
-        self.add_card_widget_label.setText(_translate("central_widget", "Add new cards:"))
-from mtg_proxy_printer.ui.add_card import HorizontalAddCardWidget
+        self.document_view_label.setText(_translate("CentralWidget_Columnar", "All pages:"))
+        self.page_view_label.setText(_translate("CentralWidget_Columnar", "Current page:"))
+        self.delete_selected_images_button.setText(_translate("CentralWidget_Columnar", "Remove selected"))
+        self.add_card_widget_label.setText(_translate("CentralWidget_Columnar", "Add new cards:"))
+from mtg_proxy_printer.ui.add_card import VerticalAddCardWidget
 from mtg_proxy_printer.ui.page_renderer import PageRenderer
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/parser_result_page.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,61 +7,61 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_WizardPage(object):
-    def setupUi(self, WizardPage):
-        WizardPage.setObjectName("WizardPage")
-        WizardPage.resize(440, 278)
-        self.verticalLayout = QtWidgets.QVBoxLayout(WizardPage)
+class Ui_SummaryPage(object):
+    def setupUi(self, SummaryPage):
+        SummaryPage.setObjectName("SummaryPage")
+        SummaryPage.resize(440, 278)
+        self.verticalLayout = QtWidgets.QVBoxLayout(SummaryPage)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.should_replace_document = QtWidgets.QCheckBox(WizardPage)
+        self.should_replace_document = QtWidgets.QCheckBox(SummaryPage)
         icon = QtGui.QIcon.fromTheme("document-replace")
         self.should_replace_document.setIcon(icon)
         self.should_replace_document.setObjectName("should_replace_document")
         self.verticalLayout.addWidget(self.should_replace_document)
-        self.parsed_cards_label = QtWidgets.QLabel(WizardPage)
+        self.parsed_cards_label = QtWidgets.QLabel(SummaryPage)
         self.parsed_cards_label.setObjectName("parsed_cards_label")
         self.verticalLayout.addWidget(self.parsed_cards_label)
-        self.parsed_cards_table = QtWidgets.QTableView(WizardPage)
+        self.parsed_cards_table = QtWidgets.QTableView(SummaryPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(65)
         sizePolicy.setHeightForWidth(self.parsed_cards_table.sizePolicy().hasHeightForWidth())
         self.parsed_cards_table.setSizePolicy(sizePolicy)
         self.parsed_cards_table.setSizeAdjustPolicy(QtWidgets.QAbstractScrollArea.AdjustToContents)
         self.parsed_cards_table.setAlternatingRowColors(True)
         self.parsed_cards_table.setSortingEnabled(True)
         self.parsed_cards_table.setObjectName("parsed_cards_table")
         self.parsed_cards_table.horizontalHeader().setDefaultSectionSize(110)
         self.verticalLayout.addWidget(self.parsed_cards_table)
-        self.unsuccessful_lines_label = QtWidgets.QLabel(WizardPage)
+        self.unsuccessful_lines_label = QtWidgets.QLabel(SummaryPage)
         self.unsuccessful_lines_label.setObjectName("unsuccessful_lines_label")
         self.verticalLayout.addWidget(self.unsuccessful_lines_label)
-        self.unparsed_lines_text = QtWidgets.QTextBrowser(WizardPage)
+        self.unparsed_lines_text = QtWidgets.QTextBrowser(SummaryPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Expanding)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(35)
         sizePolicy.setHeightForWidth(self.unparsed_lines_text.sizePolicy().hasHeightForWidth())
         self.unparsed_lines_text.setSizePolicy(sizePolicy)
         self.unparsed_lines_text.setSizeAdjustPolicy(QtWidgets.QAbstractScrollArea.AdjustToContents)
         self.unparsed_lines_text.setAcceptRichText(False)
         self.unparsed_lines_text.setOpenLinks(False)
         self.unparsed_lines_text.setObjectName("unparsed_lines_text")
         self.verticalLayout.addWidget(self.unparsed_lines_text)
 
-        self.retranslateUi(WizardPage)
-        QtCore.QMetaObject.connectSlotsByName(WizardPage)
+        self.retranslateUi(SummaryPage)
+        QtCore.QMetaObject.connectSlotsByName(SummaryPage)
 
-    def retranslateUi(self, WizardPage):
+    def retranslateUi(self, SummaryPage):
         _translate = QtCore.QCoreApplication.translate
-        WizardPage.setTitle(_translate("WizardPage", "Import a deck list for printing"))
-        WizardPage.setSubTitle(_translate("WizardPage", "The table below shows all identified cards. Double-clicking the Set or Collector# cells to change the selected printing. The text field shows all lines from the input that were not identified as cards."))
-        self.should_replace_document.setToolTip(_translate("WizardPage", "If checked, clear all cards in the current document, replacing everything with the list below.\n"
+        SummaryPage.setTitle(_translate("SummaryPage", "Import a deck list for printing"))
+        SummaryPage.setSubTitle(_translate("SummaryPage", "The table below shows all identified cards. Double-clicking the Set or Collector# cells to change the selected printing. The text field shows all lines from the input that were not identified as cards."))
+        self.should_replace_document.setToolTip(_translate("SummaryPage", "If checked, clear all cards in the current document, replacing everything with the list below.\n"
 "If unchecked, append the cards found below to the document."))
-        self.should_replace_document.setText(_translate("WizardPage", "Replace the current document content with the found cards"))
-        self.parsed_cards_label.setText(_translate("WizardPage", "These cards were successfully identified:"))
-        self.unsuccessful_lines_label.setText(_translate("WizardPage", "These lines from the deck list were not identified as cards:"))
-        self.unparsed_lines_text.setPlaceholderText(_translate("WizardPage", "Nothing. All cards were successfully identified!"))
+        self.should_replace_document.setText(_translate("SummaryPage", "Replace the current document content with the found cards"))
+        self.parsed_cards_label.setText(_translate("SummaryPage", "These cards were successfully identified:"))
+        self.unsuccessful_lines_label.setText(_translate("SummaryPage", "These lines from the deck list were not identified as cards:"))
+        self.unparsed_lines_text.setPlaceholderText(_translate("SummaryPage", "Nothing. All cards were successfully identified!"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/deck_import_wizard/select_deck_parser_page.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,170 +7,170 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_WizardPage(object):
-    def setupUi(self, WizardPage):
-        WizardPage.setObjectName("WizardPage")
-        WizardPage.resize(767, 596)
-        self.gridLayout = QtWidgets.QGridLayout(WizardPage)
+class Ui_SelectDeckParserPage(object):
+    def setupUi(self, SelectDeckParserPage):
+        SelectDeckParserPage.setObjectName("SelectDeckParserPage")
+        SelectDeckParserPage.resize(767, 596)
+        self.gridLayout = QtWidgets.QGridLayout(SelectDeckParserPage)
         self.gridLayout.setObjectName("gridLayout")
-        self.select_parser_xmage = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_xmage = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_xmage.setObjectName("select_parser_xmage")
         self.gridLayout.addWidget(self.select_parser_xmage, 3, 1, 1, 4)
-        self.tappedout_include_acquire_board = QtWidgets.QCheckBox(WizardPage)
+        self.tappedout_include_acquire_board = QtWidgets.QCheckBox(SelectDeckParserPage)
         self.tappedout_include_acquire_board.setEnabled(False)
         self.tappedout_include_acquire_board.setObjectName("tappedout_include_acquire_board")
         self.gridLayout.addWidget(self.tappedout_include_acquire_board, 6, 3, 1, 1)
-        self.select_parser_mtg_online = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_mtg_online = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_mtg_online.setObjectName("select_parser_mtg_online")
         self.gridLayout.addWidget(self.select_parser_mtg_online, 1, 1, 1, 4)
         spacerItem = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
         self.gridLayout.addItem(spacerItem, 11, 1, 1, 1)
         spacerItem1 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
         self.gridLayout.addItem(spacerItem1, 9, 1, 1, 1)
-        self.tappedout_include_maybe_board = QtWidgets.QCheckBox(WizardPage)
+        self.tappedout_include_maybe_board = QtWidgets.QCheckBox(SelectDeckParserPage)
         self.tappedout_include_maybe_board.setEnabled(False)
         self.tappedout_include_maybe_board.setObjectName("tappedout_include_maybe_board")
         self.gridLayout.addWidget(self.tappedout_include_maybe_board, 6, 2, 1, 1)
-        self.select_parser_scryfall_csv = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_scryfall_csv = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_scryfall_csv.setObjectName("select_parser_scryfall_csv")
         self.gridLayout.addWidget(self.select_parser_scryfall_csv, 4, 1, 1, 4)
         spacerItem2 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
         self.gridLayout.addItem(spacerItem2, 14, 1, 1, 4)
-        self.select_parser_tappedout_csv = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_tappedout_csv = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_tappedout_csv.setObjectName("select_parser_tappedout_csv")
         self.gridLayout.addWidget(self.select_parser_tappedout_csv, 5, 1, 1, 4)
         self.sample_buttons_layout = QtWidgets.QGridLayout()
         self.sample_buttons_layout.setObjectName("sample_buttons_layout")
-        self.insert_set_code_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
+        self.insert_set_code_matcher_sample_button = QtWidgets.QPushButton(SelectDeckParserPage)
         self.insert_set_code_matcher_sample_button.setEnabled(False)
         self.insert_set_code_matcher_sample_button.setObjectName("insert_set_code_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_set_code_matcher_sample_button, 0, 1, 1, 1)
-        self.insert_collector_number_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
+        self.insert_collector_number_matcher_sample_button = QtWidgets.QPushButton(SelectDeckParserPage)
         self.insert_collector_number_matcher_sample_button.setEnabled(False)
         self.insert_collector_number_matcher_sample_button.setObjectName("insert_collector_number_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_collector_number_matcher_sample_button, 0, 2, 1, 1)
-        self.insert_copies_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
+        self.insert_copies_matcher_sample_button = QtWidgets.QPushButton(SelectDeckParserPage)
         self.insert_copies_matcher_sample_button.setEnabled(False)
         self.insert_copies_matcher_sample_button.setObjectName("insert_copies_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_copies_matcher_sample_button, 1, 0, 1, 1)
-        self.insert_name_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
+        self.insert_name_matcher_sample_button = QtWidgets.QPushButton(SelectDeckParserPage)
         self.insert_name_matcher_sample_button.setEnabled(False)
         self.insert_name_matcher_sample_button.setObjectName("insert_name_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_name_matcher_sample_button, 0, 0, 1, 1)
-        self.insert_scryfall_id_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
+        self.insert_scryfall_id_matcher_sample_button = QtWidgets.QPushButton(SelectDeckParserPage)
         self.insert_scryfall_id_matcher_sample_button.setEnabled(False)
         self.insert_scryfall_id_matcher_sample_button.setObjectName("insert_scryfall_id_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_scryfall_id_matcher_sample_button, 1, 2, 1, 1)
-        self.insert_language_matcher_sample_button = QtWidgets.QPushButton(WizardPage)
+        self.insert_language_matcher_sample_button = QtWidgets.QPushButton(SelectDeckParserPage)
         self.insert_language_matcher_sample_button.setEnabled(False)
         self.insert_language_matcher_sample_button.setObjectName("insert_language_matcher_sample_button")
         self.sample_buttons_layout.addWidget(self.insert_language_matcher_sample_button, 1, 1, 1, 1)
         self.gridLayout.addLayout(self.sample_buttons_layout, 11, 2, 1, 3)
-        self.select_parser_custom_re = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_custom_re = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_custom_re.setObjectName("select_parser_custom_re")
         self.gridLayout.addWidget(self.select_parser_custom_re, 8, 1, 1, 4)
         spacerItem3 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Minimum)
         self.gridLayout.addItem(spacerItem3, 6, 1, 1, 1)
         spacerItem4 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
         self.gridLayout.addItem(spacerItem4, 6, 4, 1, 1)
-        self.select_parser_mtg_arena = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_mtg_arena = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_mtg_arena.setObjectName("select_parser_mtg_arena")
         self.gridLayout.addWidget(self.select_parser_mtg_arena, 0, 1, 1, 4)
-        self.custom_re_input = QtWidgets.QLineEdit(WizardPage)
+        self.custom_re_input = QtWidgets.QLineEdit(SelectDeckParserPage)
         self.custom_re_input.setEnabled(False)
         self.custom_re_input.setClearButtonEnabled(True)
         self.custom_re_input.setObjectName("custom_re_input")
         self.gridLayout.addWidget(self.custom_re_input, 9, 2, 1, 3)
-        self.select_parser_magic_workstation = QtWidgets.QRadioButton(WizardPage)
+        self.select_parser_magic_workstation = QtWidgets.QRadioButton(SelectDeckParserPage)
         self.select_parser_magic_workstation.setObjectName("select_parser_magic_workstation")
         self.gridLayout.addWidget(self.select_parser_magic_workstation, 2, 1, 1, 4)
 
-        self.retranslateUi(WizardPage)
+        self.retranslateUi(SelectDeckParserPage)
         self.select_parser_custom_re.toggled['bool'].connect(self.custom_re_input.setEnabled) # type: ignore
-        self.select_parser_mtg_arena.clicked.connect(WizardPage.isComplete) # type: ignore
-        self.select_parser_mtg_online.clicked.connect(WizardPage.isComplete) # type: ignore
-        self.select_parser_scryfall_csv.clicked.connect(WizardPage.isComplete) # type: ignore
-        self.select_parser_custom_re.clicked.connect(WizardPage.isComplete) # type: ignore
-        self.select_parser_xmage.clicked.connect(WizardPage.isComplete) # type: ignore
-        self.custom_re_input.textChanged['QString'].connect(WizardPage.isComplete) # type: ignore
-        self.select_parser_tappedout_csv.clicked.connect(WizardPage.isComplete) # type: ignore
+        self.select_parser_mtg_arena.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
+        self.select_parser_mtg_online.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
+        self.select_parser_scryfall_csv.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
+        self.select_parser_custom_re.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
+        self.select_parser_xmage.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
+        self.custom_re_input.textChanged['QString'].connect(SelectDeckParserPage.isComplete) # type: ignore
+        self.select_parser_tappedout_csv.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
         self.select_parser_tappedout_csv.toggled['bool'].connect(self.tappedout_include_maybe_board.setEnabled) # type: ignore
         self.select_parser_tappedout_csv.toggled['bool'].connect(self.tappedout_include_acquire_board.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_name_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_collector_number_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_scryfall_id_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_set_code_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_copies_matcher_sample_button.setEnabled) # type: ignore
         self.select_parser_custom_re.toggled['bool'].connect(self.insert_language_matcher_sample_button.setEnabled) # type: ignore
-        self.select_parser_magic_workstation.clicked.connect(WizardPage.isComplete) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(WizardPage)
+        self.select_parser_magic_workstation.clicked.connect(SelectDeckParserPage.isComplete) # type: ignore
+        QtCore.QMetaObject.connectSlotsByName(SelectDeckParserPage)
 
-    def retranslateUi(self, WizardPage):
+    def retranslateUi(self, SelectDeckParserPage):
         _translate = QtCore.QCoreApplication.translate
-        WizardPage.setTitle(_translate("WizardPage", "Import a deck list for printing"))
-        WizardPage.setSubTitle(_translate("WizardPage", "Select which kind of deck list you want to import."))
-        self.select_parser_xmage.setToolTip(_translate("WizardPage", "Decklist files, stored in XMage’s native format.\n"
+        SelectDeckParserPage.setTitle(_translate("SelectDeckParserPage", "Import a deck list for printing"))
+        SelectDeckParserPage.setSubTitle(_translate("SelectDeckParserPage", "Select which kind of deck list you want to import."))
+        self.select_parser_xmage.setToolTip(_translate("SelectDeckParserPage", "Decklist files, stored in XMage’s native format.\n"
 "Because XMage closely follows Scryfall regarding Magic sets,\n"
 "this should give very accurate results."))
-        self.select_parser_xmage.setText(_translate("WizardPage", "XMage"))
-        self.tappedout_include_acquire_board.setToolTip(_translate("WizardPage", "This is a Tappedout-specific section of the deck.\n"
+        self.select_parser_xmage.setText(_translate("SelectDeckParserPage", "XMage"))
+        self.tappedout_include_acquire_board.setToolTip(_translate("SelectDeckParserPage", "This is a Tappedout-specific section of the deck.\n"
 "It may contain the decklist author’s buylist or anything else."))
-        self.tappedout_include_acquire_board.setText(_translate("WizardPage", "Include “Acquire-Board”"))
-        self.select_parser_mtg_online.setToolTip(_translate("WizardPage", "The simplistic format used by Magic Online. It does not specify exact printings, so may not give the best results."))
-        self.select_parser_mtg_online.setText(_translate("WizardPage", "Magic Online"))
-        self.tappedout_include_maybe_board.setToolTip(_translate("WizardPage", "This is a Tappedout-specific section of the deck.\n"
+        self.tappedout_include_acquire_board.setText(_translate("SelectDeckParserPage", "Include “Acquire-Board”"))
+        self.select_parser_mtg_online.setToolTip(_translate("SelectDeckParserPage", "The simplistic format used by Magic Online. It does not specify exact printings, so may not give the best results."))
+        self.select_parser_mtg_online.setText(_translate("SelectDeckParserPage", "Magic Online"))
+        self.tappedout_include_maybe_board.setToolTip(_translate("SelectDeckParserPage", "This is a Tappedout-specific section of the deck.\n"
 "It may contain cards that the decklist creator considers for inclusion, based on the meta\n"
 "or any other preference, like card price."))
-        self.tappedout_include_maybe_board.setText(_translate("WizardPage", "Include “Maybe-Board”"))
-        self.select_parser_scryfall_csv.setToolTip(_translate("WizardPage", "CSV exports from Scryfall’s own deck builder.\n"
+        self.tappedout_include_maybe_board.setText(_translate("SelectDeckParserPage", "Include “Maybe-Board”"))
+        self.select_parser_scryfall_csv.setToolTip(_translate("SelectDeckParserPage", "CSV exports from Scryfall’s own deck builder.\n"
 "Gives very accurate results, unless the imported deck list contains ignored items\n"
 "matching a configured download filter."))
-        self.select_parser_scryfall_csv.setText(_translate("WizardPage", "Scryfall.com deck lists (CSV export)"))
-        self.select_parser_tappedout_csv.setToolTip(_translate("WizardPage", "CSV exports can be downloaded from Tappedout by choosing the appropriate deck export option."))
-        self.select_parser_tappedout_csv.setText(_translate("WizardPage", "tappedout.net deck list (CSV export)"))
-        self.insert_set_code_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a sample matcher for a set code to the input field above."))
-        self.insert_set_code_matcher_sample_button.setText(_translate("WizardPage", "Set code matcher"))
-        self.insert_collector_number_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a sample matcher for a collector number to the input field above"))
-        self.insert_collector_number_matcher_sample_button.setText(_translate("WizardPage", "Collector number matcher"))
-        self.insert_copies_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for the number of card copies to the input field above.\n"
+        self.select_parser_scryfall_csv.setText(_translate("SelectDeckParserPage", "Scryfall.com deck lists (CSV export)"))
+        self.select_parser_tappedout_csv.setToolTip(_translate("SelectDeckParserPage", "CSV exports can be downloaded from Tappedout by choosing the appropriate deck export option."))
+        self.select_parser_tappedout_csv.setText(_translate("SelectDeckParserPage", "tappedout.net deck list (CSV export)"))
+        self.insert_set_code_matcher_sample_button.setToolTip(_translate("SelectDeckParserPage", "Appends a sample matcher for a set code to the input field above."))
+        self.insert_set_code_matcher_sample_button.setText(_translate("SelectDeckParserPage", "Set code matcher"))
+        self.insert_collector_number_matcher_sample_button.setToolTip(_translate("SelectDeckParserPage", "Appends a sample matcher for a collector number to the input field above"))
+        self.insert_collector_number_matcher_sample_button.setText(_translate("SelectDeckParserPage", "Collector number matcher"))
+        self.insert_copies_matcher_sample_button.setToolTip(_translate("SelectDeckParserPage", "Appends a matcher for the number of card copies to the input field above.\n"
 "If a card count field is not present in the deck list, 1 card copy per line is assumed"))
-        self.insert_copies_matcher_sample_button.setText(_translate("WizardPage", "Copies matcher"))
-        self.insert_name_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for a card name to the input field above."))
-        self.insert_name_matcher_sample_button.setText(_translate("WizardPage", "Card name matcher"))
-        self.insert_scryfall_id_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for the Scryfall ID to the input field above.\n"
+        self.insert_copies_matcher_sample_button.setText(_translate("SelectDeckParserPage", "Copies matcher"))
+        self.insert_name_matcher_sample_button.setToolTip(_translate("SelectDeckParserPage", "Appends a matcher for a card name to the input field above."))
+        self.insert_name_matcher_sample_button.setText(_translate("SelectDeckParserPage", "Card name matcher"))
+        self.insert_scryfall_id_matcher_sample_button.setToolTip(_translate("SelectDeckParserPage", "Appends a matcher for the Scryfall ID to the input field above.\n"
 "This may be used by deck lists that closely integrate with the Scryfall website.\n"
 "Most deck lists won’t use this."))
-        self.insert_scryfall_id_matcher_sample_button.setText(_translate("WizardPage", "Scryfall ID matcher"))
-        self.insert_language_matcher_sample_button.setToolTip(_translate("WizardPage", "Appends a matcher for the  card language to the input field above.\n"
+        self.insert_scryfall_id_matcher_sample_button.setText(_translate("SelectDeckParserPage", "Scryfall ID matcher"))
+        self.insert_language_matcher_sample_button.setToolTip(_translate("SelectDeckParserPage", "Appends a matcher for the  card language to the input field above.\n"
 "If a language field is not present in the deck list, the card language is guessed."))
-        self.insert_language_matcher_sample_button.setText(_translate("WizardPage", "Language matcher"))
-        self.select_parser_custom_re.setToolTip(_translate("WizardPage", "Specify a custom regular expression in the input field below. It will be used to parse each deck list line.\n"
+        self.insert_language_matcher_sample_button.setText(_translate("SelectDeckParserPage", "Language matcher"))
+        self.select_parser_custom_re.setToolTip(_translate("SelectDeckParserPage", "Specify a custom regular expression in the input field below. It will be used to parse each deck list line.\n"
 "You can use the buttons below to insert basic building blocks.\n"
 "You have to separate them with the “control structures”, like spaces, as used in your deck list."))
-        self.select_parser_custom_re.setText(_translate("WizardPage", "Custom regular expression based parser:"))
-        self.select_parser_mtg_arena.setToolTip(_translate("WizardPage", "Magic Arena and exports from compatible websites, like moxfield.com\n"
+        self.select_parser_custom_re.setText(_translate("SelectDeckParserPage", "Custom regular expression based parser:"))
+        self.select_parser_mtg_arena.setToolTip(_translate("SelectDeckParserPage", "Magic Arena and exports from compatible websites, like moxfield.com\n"
 "Note that this option is not limited to cards in Standard/Historic,\n"
 "as the format works for any card."))
-        self.select_parser_mtg_arena.setText(_translate("WizardPage", "MTG Arena"))
-        self.custom_re_input.setToolTip(_translate("WizardPage", "Use this regular expression to parse the deck list file. See the context help (?-Button) for more detailes."))
-        self.custom_re_input.setWhatsThis(_translate("WizardPage", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
+        self.select_parser_mtg_arena.setText(_translate("SelectDeckParserPage", "MTG Arena"))
+        self.custom_re_input.setToolTip(_translate("SelectDeckParserPage", "Use this regular expression to parse the deck list file. See the context help (?-Button) for more detailes."))
+        self.custom_re_input.setWhatsThis(_translate("SelectDeckParserPage", "<!DOCTYPE HTML PUBLIC \"-//W3C//DTD HTML 4.0//EN\" \"http://www.w3.org/TR/REC-html40/strict.dtd\">\n"
 "<html><head><meta name=\"qrichtext\" content=\"1\" /><style type=\"text/css\">\n"
 "p, li { white-space: pre-wrap; }\n"
 "</style></head><body style=\" font-family:\'Ubuntu\'; font-size:10pt; font-weight:400; font-style:normal;\">\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">You can enter a custom Regular Expression (in Python syntax) to parse the lines of your deck list. Use <span style=\" font-style:italic;\">named groups</span> to extract the individual card properties from the individual lines of the deck list.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">A named group looks like this <span style=\" font-weight:600;\">(?P&lt;GroupName&gt;RE)</span>, where RE is a Regular Expression matching the part you want to extract.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">This program recognises these group names:</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">copies</span>: The number of card copies. Defaults to 1, if not present</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">name</span>: The card name</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">set_code</span>: The 3 (or more) letter code identifying the set.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">collector_number</span>: The collector number of the card</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">- <span style=\" font-weight:600;\">language</span>: The card language, using a two-letter language code. If not given, the importer tries to determine the language from the card name. Defaults to &quot;en&quot; for English, if not possible.<br /></p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">Not all groups are required for a successful match. For example, <span style=\" font-weight:600;\">set_code</span> and <span style=\" font-weight:600;\">collector_number</span> is sufficient for exact identification most of the time.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\">Hint: You may want to use an online Regular Expression editor, like <a href=\"https://regex101.com/\"><span style=\" text-decoration: underline; color:#2980b9;\">https://regex101.com/</span></a>, for example.</p>\n"
 "<p style=\" margin-top:12px; margin-bottom:12px; margin-left:0px; margin-right:0px; -qt-block-indent:0; text-indent:0px;\"><br /></p></body></html>"))
-        self.custom_re_input.setPlaceholderText(_translate("WizardPage", "(?P<copies>\\w+) (?P<name>.+) \\((?P<set_code>\\w+)\\) (?P<collector_number>\\d+)"))
-        self.select_parser_magic_workstation.setText(_translate("WizardPage", "Magic Workstation Deck Data (mwDeck)"))
+        self.custom_re_input.setPlaceholderText(_translate("SelectDeckParserPage", "(?P<copies>\\w+) (?P<name>.+) \\((?P<set_code>\\w+)\\) (?P<collector_number>\\d+)"))
+        self.select_parser_magic_workstation.setText(_translate("SelectDeckParserPage", "Magic Workstation Deck Data (mwDeck)"))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/main_window.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/main_window.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,127 +7,127 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_main_window(object):
-    def setupUi(self, main_window):
-        main_window.setObjectName("main_window")
-        main_window.resize(1050, 700)
-        main_window.setToolButtonStyle(QtCore.Qt.ToolButtonFollowStyle)
-        self.central_widget = CentralWidget(main_window)
+class Ui_MainWindow(object):
+    def setupUi(self, MainWindow):
+        MainWindow.setObjectName("MainWindow")
+        MainWindow.resize(1050, 700)
+        MainWindow.setToolButtonStyle(QtCore.Qt.ToolButtonFollowStyle)
+        self.central_widget = CentralWidget(MainWindow)
         self.central_widget.setObjectName("central_widget")
-        self.menubar = QtWidgets.QMenuBar(main_window)
+        self.menubar = QtWidgets.QMenuBar(MainWindow)
         self.menubar.setGeometry(QtCore.QRect(0, 0, 1050, 28))
         self.menubar.setObjectName("menubar")
         self.menu_file = QtWidgets.QMenu(self.menubar)
         self.menu_file.setObjectName("menu_file")
         self.menu_settings = QtWidgets.QMenu(self.menubar)
         self.menu_settings.setObjectName("menu_settings")
         self.menu_edit = QtWidgets.QMenu(self.menubar)
         self.menu_edit.setObjectName("menu_edit")
-        main_window.setMenuBar(self.menubar)
-        self.statusbar = QtWidgets.QStatusBar(main_window)
+        MainWindow.setMenuBar(self.menubar)
+        self.statusbar = QtWidgets.QStatusBar(MainWindow)
         self.statusbar.setObjectName("statusbar")
-        main_window.setStatusBar(self.statusbar)
-        self.toolBar = QtWidgets.QToolBar(main_window)
+        MainWindow.setStatusBar(self.statusbar)
+        self.toolBar = QtWidgets.QToolBar(MainWindow)
         self.toolBar.setToolButtonStyle(QtCore.Qt.ToolButtonTextBesideIcon)
         self.toolBar.setObjectName("toolBar")
-        main_window.addToolBar(QtCore.Qt.TopToolBarArea, self.toolBar)
-        self.action_quit = QtWidgets.QAction(main_window)
+        MainWindow.addToolBar(QtCore.Qt.TopToolBarArea, self.toolBar)
+        self.action_quit = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("application-exit")
         self.action_quit.setIcon(icon)
         self.action_quit.setMenuRole(QtWidgets.QAction.QuitRole)
         self.action_quit.setObjectName("action_quit")
-        self.action_print = QtWidgets.QAction(main_window)
+        self.action_print = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-print-direct")
         self.action_print.setIcon(icon)
         self.action_print.setObjectName("action_print")
-        self.action_print_preview = QtWidgets.QAction(main_window)
+        self.action_print_preview = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-print-preview")
         self.action_print_preview.setIcon(icon)
         self.action_print_preview.setObjectName("action_print_preview")
-        self.action_print_pdf = QtWidgets.QAction(main_window)
+        self.action_print_pdf = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("viewpdf")
         self.action_print_pdf.setIcon(icon)
         self.action_print_pdf.setObjectName("action_print_pdf")
-        self.action_discard_page = QtWidgets.QAction(main_window)
+        self.action_discard_page = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-close")
         self.action_discard_page.setIcon(icon)
         self.action_discard_page.setObjectName("action_discard_page")
-        self.action_show_settings = QtWidgets.QAction(main_window)
+        self.action_show_settings = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("configure")
         self.action_show_settings.setIcon(icon)
         self.action_show_settings.setMenuRole(QtWidgets.QAction.PreferencesRole)
         self.action_show_settings.setObjectName("action_show_settings")
-        self.action_download_card_data = QtWidgets.QAction(main_window)
+        self.action_download_card_data = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("edit-download")
         self.action_download_card_data.setIcon(icon)
         self.action_download_card_data.setObjectName("action_download_card_data")
-        self.action_new_page = QtWidgets.QAction(main_window)
+        self.action_new_page = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-new")
         self.action_new_page.setIcon(icon)
         self.action_new_page.setObjectName("action_new_page")
-        self.action_save_document = QtWidgets.QAction(main_window)
+        self.action_save_document = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-save")
         self.action_save_document.setIcon(icon)
         self.action_save_document.setObjectName("action_save_document")
-        self.action_new_document = QtWidgets.QAction(main_window)
+        self.action_new_document = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-replace")
         self.action_new_document.setIcon(icon)
         self.action_new_document.setObjectName("action_new_document")
-        self.action_load_document = QtWidgets.QAction(main_window)
+        self.action_load_document = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-open")
         self.action_load_document.setIcon(icon)
         self.action_load_document.setObjectName("action_load_document")
-        self.action_save_as = QtWidgets.QAction(main_window)
+        self.action_save_as = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-save-as")
         self.action_save_as.setIcon(icon)
         self.action_save_as.setObjectName("action_save_as")
-        self.action_show_about_dialog = QtWidgets.QAction(main_window)
+        self.action_show_about_dialog = QtWidgets.QAction(MainWindow)
         self.action_show_about_dialog.setMenuRole(QtWidgets.QAction.AboutRole)
         self.action_show_about_dialog.setObjectName("action_show_about_dialog")
-        self.action_show_changelog = QtWidgets.QAction(main_window)
+        self.action_show_changelog = QtWidgets.QAction(MainWindow)
         self.action_show_changelog.setObjectName("action_show_changelog")
-        self.action_compact_document = QtWidgets.QAction(main_window)
+        self.action_compact_document = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("format-align-vertical-top")
         self.action_compact_document.setIcon(icon)
         self.action_compact_document.setObjectName("action_compact_document")
-        self.action_edit_document_settings = QtWidgets.QAction(main_window)
+        self.action_edit_document_settings = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-properties")
         self.action_edit_document_settings.setIcon(icon)
         self.action_edit_document_settings.setObjectName("action_edit_document_settings")
-        self.action_import_deck_list = QtWidgets.QAction(main_window)
+        self.action_import_deck_list = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("document-import")
         self.action_import_deck_list.setIcon(icon)
         self.action_import_deck_list.setObjectName("action_import_deck_list")
-        self.action_cleanup_local_image_cache = QtWidgets.QAction(main_window)
+        self.action_cleanup_local_image_cache = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("edit-clear-history")
         self.action_cleanup_local_image_cache.setIcon(icon)
         self.action_cleanup_local_image_cache.setObjectName("action_cleanup_local_image_cache")
-        self.action_show_toolbar = QtWidgets.QAction(main_window)
+        self.action_show_toolbar = QtWidgets.QAction(MainWindow)
         self.action_show_toolbar.setCheckable(True)
         self.action_show_toolbar.setChecked(True)
         self.action_show_toolbar.setObjectName("action_show_toolbar")
-        self.action_download_missing_card_images = QtWidgets.QAction(main_window)
+        self.action_download_missing_card_images = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("edit-download")
         self.action_download_missing_card_images.setIcon(icon)
         self.action_download_missing_card_images.setObjectName("action_download_missing_card_images")
-        self.action_shuffle_document = QtWidgets.QAction(main_window)
+        self.action_shuffle_document = QtWidgets.QAction(MainWindow)
         icon = QtGui.QIcon.fromTheme("shuffle")
         self.action_shuffle_document.setIcon(icon)
         self.action_shuffle_document.setObjectName("action_shuffle_document")
-        self.action_undo = QtWidgets.QAction(main_window)
+        self.action_undo = QtWidgets.QAction(MainWindow)
         self.action_undo.setEnabled(False)
         icon = QtGui.QIcon.fromTheme("edit-undo")
         self.action_undo.setIcon(icon)
         self.action_undo.setObjectName("action_undo")
-        self.action_redo = QtWidgets.QAction(main_window)
+        self.action_redo = QtWidgets.QAction(MainWindow)
         self.action_redo.setEnabled(False)
         icon = QtGui.QIcon.fromTheme("edit-redo")
         self.action_redo.setIcon(icon)
         self.action_redo.setObjectName("action_redo")
         self.menu_file.addAction(self.action_new_document)
         self.menu_file.addAction(self.action_load_document)
         self.menu_file.addAction(self.action_save_document)
@@ -168,61 +168,61 @@
         self.toolBar.addAction(self.action_print_preview)
         self.toolBar.addAction(self.action_print)
         self.toolBar.addAction(self.action_print_pdf)
         self.toolBar.addSeparator()
         self.toolBar.addAction(self.action_new_page)
         self.toolBar.addAction(self.action_discard_page)
 
-        self.retranslateUi(main_window)
+        self.retranslateUi(MainWindow)
         self.action_show_toolbar.toggled['bool'].connect(self.toolBar.setVisible) # type: ignore
         self.toolBar.visibilityChanged['bool'].connect(self.action_show_toolbar.setChecked) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(main_window)
+        QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
-    def retranslateUi(self, main_window):
+    def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
-        main_window.setWindowTitle(_translate("main_window", "MTGProxyPrinter"))
-        self.menu_file.setTitle(_translate("main_window", "Fi&le"))
-        self.menu_settings.setTitle(_translate("main_window", "Settings"))
-        self.menu_edit.setTitle(_translate("main_window", "Edit"))
-        self.toolBar.setWindowTitle(_translate("main_window", "Show toolbar"))
-        self.action_quit.setText(_translate("main_window", "&Quit"))
-        self.action_quit.setShortcut(_translate("main_window", "Ctrl+Q"))
-        self.action_print.setText(_translate("main_window", "&Print"))
-        self.action_print.setToolTip(_translate("main_window", "Print the current documents"))
-        self.action_print.setShortcut(_translate("main_window", "Ctrl+P"))
-        self.action_print_preview.setText(_translate("main_window", "&Show print preview"))
-        self.action_print_preview.setToolTip(_translate("main_window", "Show print preview window"))
-        self.action_print_pdf.setText(_translate("main_window", "&Create PDF"))
-        self.action_print_pdf.setToolTip(_translate("main_window", "Create a PDF document"))
-        self.action_discard_page.setText(_translate("main_window", "Discard page"))
-        self.action_discard_page.setToolTip(_translate("main_window", "Discard this page."))
-        self.action_show_settings.setText(_translate("main_window", "Settings"))
-        self.action_download_card_data.setText(_translate("main_window", "Download card data"))
-        self.action_new_page.setText(_translate("main_window", "New Page"))
-        self.action_new_page.setToolTip(_translate("main_window", "Add a new, empty page."))
-        self.action_save_document.setText(_translate("main_window", "Save"))
-        self.action_save_document.setShortcut(_translate("main_window", "Ctrl+S"))
-        self.action_new_document.setText(_translate("main_window", "New"))
-        self.action_new_document.setShortcut(_translate("main_window", "Ctrl+N"))
-        self.action_load_document.setText(_translate("main_window", "Load"))
-        self.action_load_document.setShortcut(_translate("main_window", "Ctrl+L"))
-        self.action_save_as.setText(_translate("main_window", "Save as …"))
-        self.action_show_about_dialog.setText(_translate("main_window", "About…"))
-        self.action_show_changelog.setText(_translate("main_window", "Show Changelog"))
-        self.action_compact_document.setText(_translate("main_window", "Compact document"))
-        self.action_compact_document.setToolTip(_translate("main_window", "Minimize page count: Fill empty slots on pages by moving cards from the end of the document"))
-        self.action_edit_document_settings.setText(_translate("main_window", "Edit document settings"))
-        self.action_edit_document_settings.setToolTip(_translate("main_window", "Configure page size, margins, image spacings for the currently edited document."))
-        self.action_import_deck_list.setText(_translate("main_window", "Import Deck list"))
-        self.action_import_deck_list.setToolTip(_translate("main_window", "Import a deck list from online sources"))
-        self.action_cleanup_local_image_cache.setText(_translate("main_window", "Cleanup card images"))
-        self.action_cleanup_local_image_cache.setToolTip(_translate("main_window", "Delete locally stored card images you no longer need."))
-        self.action_show_toolbar.setText(_translate("main_window", "Show toolbar"))
-        self.action_show_toolbar.setShortcut(_translate("main_window", "Ctrl+M"))
-        self.action_download_missing_card_images.setText(_translate("main_window", "Download missing card images"))
-        self.action_shuffle_document.setText(_translate("main_window", "Shuffle document"))
-        self.action_shuffle_document.setToolTip(_translate("main_window", "Randomly rearrange all card image.\n"
+        MainWindow.setWindowTitle(_translate("MainWindow", "MTGProxyPrinter"))
+        self.menu_file.setTitle(_translate("MainWindow", "Fi&le"))
+        self.menu_settings.setTitle(_translate("MainWindow", "Settings"))
+        self.menu_edit.setTitle(_translate("MainWindow", "Edit"))
+        self.toolBar.setWindowTitle(_translate("MainWindow", "Show toolbar"))
+        self.action_quit.setText(_translate("MainWindow", "&Quit"))
+        self.action_quit.setShortcut(_translate("MainWindow", "Ctrl+Q"))
+        self.action_print.setText(_translate("MainWindow", "&Print"))
+        self.action_print.setToolTip(_translate("MainWindow", "Print the current documents"))
+        self.action_print.setShortcut(_translate("MainWindow", "Ctrl+P"))
+        self.action_print_preview.setText(_translate("MainWindow", "&Show print preview"))
+        self.action_print_preview.setToolTip(_translate("MainWindow", "Show print preview window"))
+        self.action_print_pdf.setText(_translate("MainWindow", "&Create PDF"))
+        self.action_print_pdf.setToolTip(_translate("MainWindow", "Create a PDF document"))
+        self.action_discard_page.setText(_translate("MainWindow", "Discard page"))
+        self.action_discard_page.setToolTip(_translate("MainWindow", "Discard this page."))
+        self.action_show_settings.setText(_translate("MainWindow", "Settings"))
+        self.action_download_card_data.setText(_translate("MainWindow", "Download card data"))
+        self.action_new_page.setText(_translate("MainWindow", "New Page"))
+        self.action_new_page.setToolTip(_translate("MainWindow", "Add a new, empty page."))
+        self.action_save_document.setText(_translate("MainWindow", "Save"))
+        self.action_save_document.setShortcut(_translate("MainWindow", "Ctrl+S"))
+        self.action_new_document.setText(_translate("MainWindow", "New"))
+        self.action_new_document.setShortcut(_translate("MainWindow", "Ctrl+N"))
+        self.action_load_document.setText(_translate("MainWindow", "Load"))
+        self.action_load_document.setShortcut(_translate("MainWindow", "Ctrl+L"))
+        self.action_save_as.setText(_translate("MainWindow", "Save as …"))
+        self.action_show_about_dialog.setText(_translate("MainWindow", "About…"))
+        self.action_show_changelog.setText(_translate("MainWindow", "Show Changelog"))
+        self.action_compact_document.setText(_translate("MainWindow", "Compact document"))
+        self.action_compact_document.setToolTip(_translate("MainWindow", "Minimize page count: Fill empty slots on pages by moving cards from the end of the document"))
+        self.action_edit_document_settings.setText(_translate("MainWindow", "Edit document settings"))
+        self.action_edit_document_settings.setToolTip(_translate("MainWindow", "Configure page size, margins, image spacings for the currently edited document."))
+        self.action_import_deck_list.setText(_translate("MainWindow", "Import Deck list"))
+        self.action_import_deck_list.setToolTip(_translate("MainWindow", "Import a deck list from online sources"))
+        self.action_cleanup_local_image_cache.setText(_translate("MainWindow", "Cleanup card images"))
+        self.action_cleanup_local_image_cache.setToolTip(_translate("MainWindow", "Delete locally stored card images you no longer need."))
+        self.action_show_toolbar.setText(_translate("MainWindow", "Show toolbar"))
+        self.action_show_toolbar.setShortcut(_translate("MainWindow", "Ctrl+M"))
+        self.action_download_missing_card_images.setText(_translate("MainWindow", "Download missing card images"))
+        self.action_shuffle_document.setText(_translate("MainWindow", "Shuffle document"))
+        self.action_shuffle_document.setToolTip(_translate("MainWindow", "Randomly rearrange all card image.\n"
 "If you want to quickly print a full deck for playing,\n"
 "use this to reduce the initial deck shuffling required"))
-        self.action_undo.setText(_translate("main_window", "Undo"))
-        self.action_redo.setText(_translate("main_window", "Redo"))
+        self.action_undo.setText(_translate("MainWindow", "Undo"))
+        self.action_redo.setText(_translate("MainWindow", "Redo"))
 from mtg_proxy_printer.ui.central_widget import CentralWidget
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/page_config_dialog.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/document_settings_dialog.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # -*- coding: utf-8 -*-
 
-# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/page_config_dialog.ui'
+# Form implementation generated from reading ui file '/mnt/Daten/Projekte/MTGProxyPrinter/mtg_proxy_printer/resources/ui/document_settings_dialog.ui'
 #
 # Created by: PyQt5 UI code generator 5.15.9
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Dialog(object):
-    def setupUi(self, Dialog):
-        Dialog.setObjectName("Dialog")
-        Dialog.resize(501, 300)
-        self.verticalLayout = QtWidgets.QVBoxLayout(Dialog)
+class Ui_DocumentSettingsDialog(object):
+    def setupUi(self, DocumentSettingsDialog):
+        DocumentSettingsDialog.setObjectName("DocumentSettingsDialog")
+        DocumentSettingsDialog.resize(501, 300)
+        self.verticalLayout = QtWidgets.QVBoxLayout(DocumentSettingsDialog)
         self.verticalLayout.setObjectName("verticalLayout")
-        self.page_config_groupbox = PageConfigWidget(Dialog)
+        self.page_config_groupbox = PageConfigWidget(DocumentSettingsDialog)
         self.page_config_groupbox.setObjectName("page_config_groupbox")
         self.verticalLayout.addWidget(self.page_config_groupbox)
-        self.button_box = QtWidgets.QDialogButtonBox(Dialog)
+        self.button_box = QtWidgets.QDialogButtonBox(DocumentSettingsDialog)
         self.button_box.setOrientation(QtCore.Qt.Horizontal)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Reset|QtWidgets.QDialogButtonBox.RestoreDefaults|QtWidgets.QDialogButtonBox.Save)
         self.button_box.setObjectName("button_box")
         self.verticalLayout.addWidget(self.button_box)
 
-        self.retranslateUi(Dialog)
-        self.button_box.accepted.connect(Dialog.accept) # type: ignore
-        self.button_box.rejected.connect(Dialog.reject) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(Dialog)
+        self.retranslateUi(DocumentSettingsDialog)
+        self.button_box.accepted.connect(DocumentSettingsDialog.accept) # type: ignore
+        self.button_box.rejected.connect(DocumentSettingsDialog.reject) # type: ignore
+        QtCore.QMetaObject.connectSlotsByName(DocumentSettingsDialog)
 
-    def retranslateUi(self, Dialog):
+    def retranslateUi(self, DocumentSettingsDialog):
         _translate = QtCore.QCoreApplication.translate
-        Dialog.setWindowTitle(_translate("Dialog", "Set Document settings"))
-        self.page_config_groupbox.setTitle(_translate("Dialog", "GroupBox"))
+        DocumentSettingsDialog.setWindowTitle(_translate("DocumentSettingsDialog", "Set Document settings"))
+        self.page_config_groupbox.setTitle(_translate("DocumentSettingsDialog", "GroupBox"))
 from mtg_proxy_printer.ui.page_config_widget import PageConfigWidget
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/general_printing_filter.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,187 +7,186 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Form(object):
-    def setupUi(self, Form):
-        Form.setObjectName("Form")
-        Form.resize(487, 302)
-        self.gridLayout = QtWidgets.QGridLayout(Form)
+class Ui_GeneralPrintingFilter(object):
+    def setupUi(self, GeneralPrintingFilter):
+        GeneralPrintingFilter.setObjectName("GeneralPrintingFilter")
+        GeneralPrintingFilter.resize(487, 302)
+        self.gridLayout = QtWidgets.QGridLayout(GeneralPrintingFilter)
         self.gridLayout.setObjectName("gridLayout")
-        self.hide_gold_bordered_cards = QtWidgets.QCheckBox(Form)
+        self.hide_gold_bordered_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_gold_bordered_cards.setObjectName("hide_gold_bordered_cards")
         self.gridLayout.addWidget(self.hide_gold_bordered_cards, 5, 0, 1, 1)
-        self.hide_cards_depicting_racism = QtWidgets.QCheckBox(Form)
+        self.hide_cards_depicting_racism = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_cards_depicting_racism.setObjectName("hide_cards_depicting_racism")
         self.gridLayout.addWidget(self.hide_cards_depicting_racism, 1, 0, 1, 1)
-        self.view_funny_cards = QtWidgets.QPushButton(Form)
+        self.view_funny_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_funny_cards.sizePolicy().hasHeightForWidth())
         self.view_funny_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_funny_cards.setIcon(icon)
         self.view_funny_cards.setObjectName("view_funny_cards")
         self.gridLayout.addWidget(self.view_funny_cards, 7, 1, 1, 1)
-        self.hide_funny_cards = QtWidgets.QCheckBox(Form)
+        self.hide_funny_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_funny_cards.setObjectName("hide_funny_cards")
         self.gridLayout.addWidget(self.hide_funny_cards, 7, 0, 1, 1)
-        self.hide_cards_without_images = QtWidgets.QCheckBox(Form)
+        self.hide_cards_without_images = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_cards_without_images.setObjectName("hide_cards_without_images")
         self.gridLayout.addWidget(self.hide_cards_without_images, 2, 0, 1, 1)
-        self.view_white_bordered_cards = QtWidgets.QPushButton(Form)
+        self.view_white_bordered_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_white_bordered_cards.sizePolicy().hasHeightForWidth())
         self.view_white_bordered_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_white_bordered_cards.setIcon(icon)
         self.view_white_bordered_cards.setObjectName("view_white_bordered_cards")
         self.gridLayout.addWidget(self.view_white_bordered_cards, 4, 1, 1, 1)
-        self.hide_token = QtWidgets.QCheckBox(Form)
+        self.hide_token = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_token.setObjectName("hide_token")
         self.gridLayout.addWidget(self.hide_token, 1, 2, 1, 1)
-        self.view_cards_depicting_racism = QtWidgets.QPushButton(Form)
+        self.view_cards_depicting_racism = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_cards_depicting_racism.sizePolicy().hasHeightForWidth())
         self.view_cards_depicting_racism.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_cards_depicting_racism.setIcon(icon)
         self.view_cards_depicting_racism.setObjectName("view_cards_depicting_racism")
         self.gridLayout.addWidget(self.view_cards_depicting_racism, 1, 1, 1, 1)
-        self.view_token = QtWidgets.QPushButton(Form)
+        self.view_token = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_token.sizePolicy().hasHeightForWidth())
         self.view_token.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_token.setIcon(icon)
         self.view_token.setObjectName("view_token")
         self.gridLayout.addWidget(self.view_token, 1, 3, 1, 1)
-        self.hide_digital_cards = QtWidgets.QCheckBox(Form)
+        self.hide_digital_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_digital_cards.setObjectName("hide_digital_cards")
         self.gridLayout.addWidget(self.hide_digital_cards, 2, 2, 1, 1)
-        self.hide_oversized_cards = QtWidgets.QCheckBox(Form)
+        self.hide_oversized_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_oversized_cards.setObjectName("hide_oversized_cards")
         self.gridLayout.addWidget(self.hide_oversized_cards, 3, 0, 1, 1)
-        self.hide_white_bordered_cards = QtWidgets.QCheckBox(Form)
+        self.hide_white_bordered_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_white_bordered_cards.setObjectName("hide_white_bordered_cards")
         self.gridLayout.addWidget(self.hide_white_bordered_cards, 4, 0, 1, 1)
-        self.view_digital_cards = QtWidgets.QPushButton(Form)
+        self.view_digital_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_digital_cards.sizePolicy().hasHeightForWidth())
         self.view_digital_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_digital_cards.setIcon(icon)
         self.view_digital_cards.setObjectName("view_digital_cards")
         self.gridLayout.addWidget(self.view_digital_cards, 2, 3, 1, 1)
-        self.view_cards_without_images = QtWidgets.QPushButton(Form)
+        self.view_cards_without_images = QtWidgets.QPushButton(GeneralPrintingFilter)
         self.view_cards_without_images.setEnabled(False)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_cards_without_images.sizePolicy().hasHeightForWidth())
         self.view_cards_without_images.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_cards_without_images.setIcon(icon)
         self.view_cards_without_images.setObjectName("view_cards_without_images")
         self.gridLayout.addWidget(self.view_cards_without_images, 2, 1, 1, 1)
-        self.view_oversized_cards = QtWidgets.QPushButton(Form)
+        self.view_oversized_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_oversized_cards.sizePolicy().hasHeightForWidth())
         self.view_oversized_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_oversized_cards.setIcon(icon)
         self.view_oversized_cards.setObjectName("view_oversized_cards")
         self.gridLayout.addWidget(self.view_oversized_cards, 3, 1, 1, 1)
-        self.view_gold_bordered_cards = QtWidgets.QPushButton(Form)
+        self.view_gold_bordered_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_gold_bordered_cards.sizePolicy().hasHeightForWidth())
         self.view_gold_bordered_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_gold_bordered_cards.setIcon(icon)
         self.view_gold_bordered_cards.setObjectName("view_gold_bordered_cards")
         self.gridLayout.addWidget(self.view_gold_bordered_cards, 5, 1, 1, 1)
-        self.hide_borderless_cards = QtWidgets.QCheckBox(Form)
+        self.hide_borderless_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_borderless_cards.setObjectName("hide_borderless_cards")
         self.gridLayout.addWidget(self.hide_borderless_cards, 6, 0, 1, 1)
-        self.view_borderless_cards = QtWidgets.QPushButton(Form)
+        self.view_borderless_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_borderless_cards.sizePolicy().hasHeightForWidth())
         self.view_borderless_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_borderless_cards.setIcon(icon)
         self.view_borderless_cards.setObjectName("view_borderless_cards")
         self.gridLayout.addWidget(self.view_borderless_cards, 6, 1, 1, 1)
-        self.hide_reversible_cards = QtWidgets.QCheckBox(Form)
+        self.hide_reversible_cards = QtWidgets.QCheckBox(GeneralPrintingFilter)
         self.hide_reversible_cards.setObjectName("hide_reversible_cards")
         self.gridLayout.addWidget(self.hide_reversible_cards, 3, 2, 1, 1)
-        self.view_reversible_cards = QtWidgets.QPushButton(Form)
+        self.view_reversible_cards = QtWidgets.QPushButton(GeneralPrintingFilter)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Fixed, QtWidgets.QSizePolicy.Fixed)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(self.view_reversible_cards.sizePolicy().hasHeightForWidth())
         self.view_reversible_cards.setSizePolicy(sizePolicy)
         icon = QtGui.QIcon.fromTheme("globe")
         self.view_reversible_cards.setIcon(icon)
         self.view_reversible_cards.setObjectName("view_reversible_cards")
         self.gridLayout.addWidget(self.view_reversible_cards, 3, 3, 1, 1)
 
-        self.retranslateUi(Form)
-        QtCore.QMetaObject.connectSlotsByName(Form)
+        self.retranslateUi(GeneralPrintingFilter)
+        QtCore.QMetaObject.connectSlotsByName(GeneralPrintingFilter)
 
-    def retranslateUi(self, Form):
+    def retranslateUi(self, GeneralPrintingFilter):
         _translate = QtCore.QCoreApplication.translate
-        Form.setWindowTitle(_translate("Form", "Form"))
-        Form.setTitle(_translate("Form", "General printing filters"))
-        self.hide_gold_bordered_cards.setToolTip(_translate("Form", "<html><head/><body><p>Some “collectible” sets, like full reprints of tournament-winning decks were printed with golden borders. Many also have printed signatures of the involved players in the text box.</p><p>These are not tournament legal.</p></body></html>"))
-        self.hide_gold_bordered_cards.setText(_translate("Form", "Hide gold-bordered cards"))
-        self.hide_cards_depicting_racism.setToolTip(_translate("Form", "<html><head/><body><p>Hide cards banned for depicting racism.</p><p>Background:</p><p>Some cards were banned by Wizards of the Coast, because they depict references to controversial real-world events, religion or contain combinations of card effect, name and artwork that, when viewed together, depict racism. These cards are banned in all sanctioned tournament formats and several community formats like Commander, Oathbreaker and others.</p></body></html>"))
-        self.hide_cards_depicting_racism.setText(_translate("Form", "Hide cards depicting racism"))
-        self.view_funny_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.hide_funny_cards.setToolTip(_translate("Form", "“Funny” cards, not legal in any constructed format.\n"
+        GeneralPrintingFilter.setTitle(_translate("GeneralPrintingFilter", "General printing filters"))
+        self.hide_gold_bordered_cards.setToolTip(_translate("GeneralPrintingFilter", "<html><head/><body><p>Some “collectible” sets, like full reprints of tournament-winning decks were printed with golden borders. Many also have printed signatures of the involved players in the text box.</p><p>These are not tournament legal.</p></body></html>"))
+        self.hide_gold_bordered_cards.setText(_translate("GeneralPrintingFilter", "Hide gold-bordered cards"))
+        self.hide_cards_depicting_racism.setToolTip(_translate("GeneralPrintingFilter", "<html><head/><body><p>Hide cards banned for depicting racism.</p><p>Background:</p><p>Some cards were banned by Wizards of the Coast, because they depict references to controversial real-world events, religion or contain combinations of card effect, name and artwork that, when viewed together, depict racism. These cards are banned in all sanctioned tournament formats and several community formats like Commander, Oathbreaker and others.</p></body></html>"))
+        self.hide_cards_depicting_racism.setText(_translate("GeneralPrintingFilter", "Hide cards depicting racism"))
+        self.view_funny_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.hide_funny_cards.setToolTip(_translate("GeneralPrintingFilter", "“Funny” cards, not legal in any constructed format.\n"
 "This includes full-art Contraptions from Unstable,\n"
 "cards with acorn-shaped security stamps from Unfinity (and newer Un-Sets),\n"
 "some black-bordered promotional cards with non-standard back faces,\n"
 "and all silver-bordered cards."))
-        self.hide_funny_cards.setText(_translate("Form", "Hide “funny” cards"))
-        self.hide_cards_without_images.setToolTip(_translate("Form", "Hide non-English cards with low-resolution,\n"
+        self.hide_funny_cards.setText(_translate("GeneralPrintingFilter", "Hide “funny” cards"))
+        self.hide_cards_without_images.setToolTip(_translate("GeneralPrintingFilter", "Hide non-English cards with low-resolution,\n"
 "English placeholder images with an overlay text stating\n"
 "“This card is not available in the selected language.”"))
-        self.hide_cards_without_images.setText(_translate("Form", "Hide cards with placeholder images"))
-        self.view_white_bordered_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.hide_token.setText(_translate("Form", "Hide Token cards"))
-        self.view_cards_depicting_racism.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.view_token.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.hide_digital_cards.setToolTip(_translate("Form", "Hide cards and printings that are only available on digital platforms. This includes all kinds of digital printings."))
-        self.hide_digital_cards.setText(_translate("Form", "Hide digital cards"))
-        self.hide_oversized_cards.setToolTip(_translate("Form", "These cards are larger than regular Magic cards and can’t be included in decks.\n"
+        self.hide_cards_without_images.setText(_translate("GeneralPrintingFilter", "Hide cards with placeholder images"))
+        self.view_white_bordered_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.hide_token.setText(_translate("GeneralPrintingFilter", "Hide Token cards"))
+        self.view_cards_depicting_racism.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.view_token.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.hide_digital_cards.setToolTip(_translate("GeneralPrintingFilter", "Hide cards and printings that are only available on digital platforms. This includes all kinds of digital printings."))
+        self.hide_digital_cards.setText(_translate("GeneralPrintingFilter", "Hide digital cards"))
+        self.hide_oversized_cards.setToolTip(_translate("GeneralPrintingFilter", "These cards are larger than regular Magic cards and can’t be included in decks.\n"
 "Includes Archenemy schemes, Planechase planes and\n"
 "oversized commander creature or Planeswalker cards included in some pre-constructed Commander decks."))
-        self.hide_oversized_cards.setText(_translate("Form", "Hide oversized cards"))
-        self.hide_white_bordered_cards.setText(_translate("Form", "Hide white-bordered cards"))
-        self.view_digital_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.view_oversized_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.view_gold_bordered_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.hide_borderless_cards.setText(_translate("Form", "Hide borderless cards"))
-        self.view_borderless_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
-        self.hide_reversible_cards.setToolTip(_translate("Form", "Some single-sided cards are re-printed as two-sided, reversible cards in some Secret Lair releases.\n"
+        self.hide_oversized_cards.setText(_translate("GeneralPrintingFilter", "Hide oversized cards"))
+        self.hide_white_bordered_cards.setText(_translate("GeneralPrintingFilter", "Hide white-bordered cards"))
+        self.view_digital_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.view_oversized_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.view_gold_bordered_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.hide_borderless_cards.setText(_translate("GeneralPrintingFilter", "Hide borderless cards"))
+        self.view_borderless_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
+        self.hide_reversible_cards.setToolTip(_translate("GeneralPrintingFilter", "Some single-sided cards are re-printed as two-sided, reversible cards in some Secret Lair releases.\n"
 "This filter hides those."))
-        self.hide_reversible_cards.setText(_translate("Form", "Hide reversible cards"))
-        self.view_reversible_cards.setToolTip(_translate("Form", "View cards hidden by this filter on the Scryfall website."))
+        self.hide_reversible_cards.setText(_translate("GeneralPrintingFilter", "Hide reversible cards"))
+        self.view_reversible_cards.setToolTip(_translate("GeneralPrintingFilter", "View cards hidden by this filter on the Scryfall website."))
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/generated/settings_window/settings_window.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/generated/settings_window/settings_window.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 # WARNING: Any manual changes made to this file will be lost when pyuic5 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
-class Ui_Dialog(object):
-    def setupUi(self, Dialog):
-        Dialog.setObjectName("Dialog")
-        Dialog.setWindowModality(QtCore.Qt.ApplicationModal)
-        Dialog.resize(612, 650)
-        self.dialog_layout = QtWidgets.QVBoxLayout(Dialog)
+class Ui_SettingsWindow(object):
+    def setupUi(self, SettingsWindow):
+        SettingsWindow.setObjectName("SettingsWindow")
+        SettingsWindow.setWindowModality(QtCore.Qt.ApplicationModal)
+        SettingsWindow.resize(612, 650)
+        self.dialog_layout = QtWidgets.QVBoxLayout(SettingsWindow)
         self.dialog_layout.setObjectName("dialog_layout")
-        self.tab_widget = QtWidgets.QTabWidget(Dialog)
+        self.tab_widget = QtWidgets.QTabWidget(SettingsWindow)
         self.tab_widget.setObjectName("tab_widget")
         self.tab_general = QtWidgets.QWidget()
         self.tab_general.setObjectName("tab_general")
         self.gridLayout = QtWidgets.QGridLayout(self.tab_general)
         self.gridLayout.setObjectName("gridLayout")
         self.preferred_language_label = QtWidgets.QLabel(self.tab_general)
         self.preferred_language_label.setObjectName("preferred_language_label")
@@ -240,128 +240,129 @@
         self.debug_download_card_data_as_file = QtWidgets.QPushButton(self.tab_debug)
         icon = QtGui.QIcon.fromTheme("edit-download")
         self.debug_download_card_data_as_file.setIcon(icon)
         self.debug_download_card_data_as_file.setObjectName("debug_download_card_data_as_file")
         self.gridLayout_7.addWidget(self.debug_download_card_data_as_file, 8, 1, 1, 1)
         self.tab_widget.addTab(self.tab_debug, "")
         self.dialog_layout.addWidget(self.tab_widget)
-        self.button_box = QtWidgets.QDialogButtonBox(Dialog)
+        self.button_box = QtWidgets.QDialogButtonBox(SettingsWindow)
         self.button_box.setOrientation(QtCore.Qt.Horizontal)
         self.button_box.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Reset|QtWidgets.QDialogButtonBox.RestoreDefaults|QtWidgets.QDialogButtonBox.Save)
         self.button_box.setObjectName("button_box")
         self.dialog_layout.addWidget(self.button_box)
         self.preferred_language_label.setBuddy(self.preferred_language_combo_box)
         self.add_card_widget_style_label.setBuddy(self.add_card_widget_style_combo_box)
         self.document_save_path_label.setBuddy(self.document_save_path)
         self.pdf_save_path_label.setBuddy(self.pdf_save_path)
         self.pdf_page_count_limit_label.setBuddy(self.pdf_page_count_limit)
         self.log_level_label.setBuddy(self.log_level_combo_box)
 
-        self.retranslateUi(Dialog)
+        self.retranslateUi(SettingsWindow)
         self.tab_widget.setCurrentIndex(0)
-        self.button_box.accepted.connect(Dialog.accept) # type: ignore
-        self.button_box.rejected.connect(Dialog.reject) # type: ignore
-        QtCore.QMetaObject.connectSlotsByName(Dialog)
-        Dialog.setTabOrder(self.add_card_widget_style_combo_box, self.automatically_add_opposing_faces)
-        Dialog.setTabOrder(self.automatically_add_opposing_faces, self.document_save_path)
-        Dialog.setTabOrder(self.document_save_path, self.document_save_path_browse_button)
-        Dialog.setTabOrder(self.document_save_path_browse_button, self.pdf_save_path)
-        Dialog.setTabOrder(self.pdf_save_path, self.pdf_save_path_browse_button)
-        Dialog.setTabOrder(self.pdf_save_path_browse_button, self.check_application_updates_enabled)
-        Dialog.setTabOrder(self.check_application_updates_enabled, self.check_card_data_updates_enabled)
-        Dialog.setTabOrder(self.check_card_data_updates_enabled, self.print_guessing_enable)
-        Dialog.setTabOrder(self.print_guessing_enable, self.print_guessing_prefer_already_downloaded)
-        Dialog.setTabOrder(self.print_guessing_prefer_already_downloaded, self.automatic_deck_list_translation_enable)
-        Dialog.setTabOrder(self.automatic_deck_list_translation_enable, self.pdf_page_count_limit)
+        self.button_box.accepted.connect(SettingsWindow.accept) # type: ignore
+        self.button_box.rejected.connect(SettingsWindow.reject) # type: ignore
+        QtCore.QMetaObject.connectSlotsByName(SettingsWindow)
+        SettingsWindow.setTabOrder(self.add_card_widget_style_combo_box, self.automatically_add_opposing_faces)
+        SettingsWindow.setTabOrder(self.automatically_add_opposing_faces, self.document_save_path)
+        SettingsWindow.setTabOrder(self.document_save_path, self.document_save_path_browse_button)
+        SettingsWindow.setTabOrder(self.document_save_path_browse_button, self.pdf_save_path)
+        SettingsWindow.setTabOrder(self.pdf_save_path, self.pdf_save_path_browse_button)
+        SettingsWindow.setTabOrder(self.pdf_save_path_browse_button, self.check_application_updates_enabled)
+        SettingsWindow.setTabOrder(self.check_application_updates_enabled, self.check_card_data_updates_enabled)
+        SettingsWindow.setTabOrder(self.check_card_data_updates_enabled, self.print_guessing_enable)
+        SettingsWindow.setTabOrder(self.print_guessing_enable, self.print_guessing_prefer_already_downloaded)
+        SettingsWindow.setTabOrder(self.print_guessing_prefer_already_downloaded, self.automatic_deck_list_translation_enable)
+        SettingsWindow.setTabOrder(self.automatic_deck_list_translation_enable, self.pdf_page_count_limit)
 
-    def retranslateUi(self, Dialog):
+    def retranslateUi(self, SettingsWindow):
         _translate = QtCore.QCoreApplication.translate
-        Dialog.setWindowTitle(_translate("Dialog", "Settings"))
-        self.preferred_language_label.setText(_translate("Dialog", "Preferred card language:"))
-        self.preferred_language_combo_box.setToolTip(_translate("Dialog", "Language choices will default to the chosen language here.\n"
+        SettingsWindow.setWindowTitle(_translate("SettingsWindow", "Settings"))
+        self.preferred_language_label.setText(_translate("SettingsWindow", "Preferred card language:"))
+        self.preferred_language_combo_box.setToolTip(_translate("SettingsWindow", "Language choices will default to the chosen language here.\n"
 "\n"
 "Entries use the language codes as listed on Scryfall."))
-        self.look_and_feel_settings_group_box.setTitle(_translate("Dialog", "Look && Feel (Changing this requires an application restart)"))
-        self.add_card_widget_style_label.setText(_translate("Dialog", "Main window layout"))
-        self.add_card_widget_style_combo_box.setToolTip(_translate("Dialog", "Horizontal adds a wide search area above the currently edited page.\n"
-"Vertical adds a tall search area between the page list and the currently edited page."))
-        self.double_faced_cards_group_box.setTitle(_translate("Dialog", "Double-faced cards"))
-        self.automatically_add_opposing_faces.setToolTip(_translate("Dialog", "When adding double-faced cards, automatically add the same number of copies of the other side.\n"
+        self.look_and_feel_settings_group_box.setTitle(_translate("SettingsWindow", "Look && Feel (Changing this requires an application restart)"))
+        self.add_card_widget_style_label.setText(_translate("SettingsWindow", "Main window layout"))
+        self.add_card_widget_style_combo_box.setToolTip(_translate("SettingsWindow", "Horizontal adds a wide, horizontal search area above the currently edited page, and is best for taller screens, like 4:3 or 3:2.\n"
+"Columnar organizes the main window content in four columns, and is best for (ultra-)wide screens.\n"
+"Tabbed uses tabs to only show parts of the main window at a time. Best used with small screens in portrait mode (i.e. 9:16), otherwise not recommended."))
+        self.double_faced_cards_group_box.setTitle(_translate("SettingsWindow", "Double-faced cards"))
+        self.automatically_add_opposing_faces.setToolTip(_translate("SettingsWindow", "When adding double-faced cards, automatically add the same number of copies of the other side.\n"
 "Uses the appropriate, matching other card side.\n"
 "Uncheck to disable this automatism."))
-        self.automatically_add_opposing_faces.setText(_translate("Dialog", "Automatically add the other side of double-faced cards"))
-        self.default_paths_group_box.setToolTip(_translate("Dialog", "These paths are selected by default when browsing the file system for files"))
-        self.default_paths_group_box.setTitle(_translate("Dialog", "Default save paths"))
-        self.pdf_save_path.setToolTip(_translate("Dialog", "If set, use this as the default location for saving exported PDF documents."))
-        self.pdf_save_path.setPlaceholderText(_translate("Dialog", "Path to a directory"))
-        self.document_save_path.setToolTip(_translate("Dialog", "If set, use this as the default location for saving documents."))
-        self.document_save_path.setPlaceholderText(_translate("Dialog", "Path to a directory"))
-        self.pdf_save_path_browse_button.setToolTip(_translate("Dialog", "Browse…"))
-        self.document_save_path_label.setText(_translate("Dialog", "Document save path"))
-        self.pdf_save_path_label.setText(_translate("Dialog", "PDF export path"))
-        self.document_save_path_browse_button.setToolTip(_translate("Dialog", "Browse…"))
-        self.update_check_group_box.setTitle(_translate("Dialog", "Automatic update checks"))
-        self.update_check_label.setText(_translate("Dialog", "Update checks are performed at application start, if enabled."))
-        self.check_application_updates_enabled.setToolTip(_translate("Dialog", "If enabled, check for application updates, and notify if new updates are available for installation."))
-        self.check_application_updates_enabled.setText(_translate("Dialog", "Check for application updates"))
-        self.check_card_data_updates_enabled.setToolTip(_translate("Dialog", "If enabled, query the Scryfall API if new cards are available. If so, offer to update the local card data."))
-        self.check_card_data_updates_enabled.setText(_translate("Dialog", "Check for new card data"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_general), _translate("Dialog", "General"))
-        self.deck_list_search_path.setToolTip(_translate("Dialog", "If set, use this as the default location for loading deck lists. Your webbrowser’s download directorry is a good choice."))
-        self.deck_list_search_path.setPlaceholderText(_translate("Dialog", "Path to a directory"))
-        self.deck_list_search_path_browse_button.setToolTip(_translate("Dialog", "Browse…"))
-        self.label.setText(_translate("Dialog", "These options control the deck list import function."))
-        self.basic_land_removal_group_box.setTitle(_translate("Dialog", "Control the one-click basic land removal"))
-        self.basic_land_removal_label.setText(_translate("Dialog", "These options control, if the automatic removal should also include Wastes or Snow-Covered basic lands."))
-        self.remove_basic_wastes_enable.setWhatsThis(_translate("Dialog", "Include Wastes when removing basic lands."))
-        self.remove_basic_wastes_enable.setText(_translate("Dialog", "Enable removal of Basic Wastes"))
-        self.remove_snow_basics_enable.setWhatsThis(_translate("Dialog", "Include Snow-Covered basic lands when removing basic lands."))
-        self.remove_snow_basics_enable.setText(_translate("Dialog", "Enable removal of Snow-Covered Basic lands"))
-        self.deck_list_search_path_label.setText(_translate("Dialog", "Deck list search path"))
-        self.print_guessing_group_box.setToolTip(_translate("Dialog", "Not all deck list formats always contain complete data.\n"
+        self.automatically_add_opposing_faces.setText(_translate("SettingsWindow", "Automatically add the other side of double-faced cards"))
+        self.default_paths_group_box.setToolTip(_translate("SettingsWindow", "These paths are selected by default when browsing the file system for files"))
+        self.default_paths_group_box.setTitle(_translate("SettingsWindow", "Default save paths"))
+        self.pdf_save_path.setToolTip(_translate("SettingsWindow", "If set, use this as the default location for saving exported PDF documents."))
+        self.pdf_save_path.setPlaceholderText(_translate("SettingsWindow", "Path to a directory"))
+        self.document_save_path.setToolTip(_translate("SettingsWindow", "If set, use this as the default location for saving documents."))
+        self.document_save_path.setPlaceholderText(_translate("SettingsWindow", "Path to a directory"))
+        self.pdf_save_path_browse_button.setToolTip(_translate("SettingsWindow", "Browse…"))
+        self.document_save_path_label.setText(_translate("SettingsWindow", "Document save path"))
+        self.pdf_save_path_label.setText(_translate("SettingsWindow", "PDF export path"))
+        self.document_save_path_browse_button.setToolTip(_translate("SettingsWindow", "Browse…"))
+        self.update_check_group_box.setTitle(_translate("SettingsWindow", "Automatic update checks"))
+        self.update_check_label.setText(_translate("SettingsWindow", "Update checks are performed at application start, if enabled."))
+        self.check_application_updates_enabled.setToolTip(_translate("SettingsWindow", "If enabled, check for application updates, and notify if new updates are available for installation."))
+        self.check_application_updates_enabled.setText(_translate("SettingsWindow", "Check for application updates"))
+        self.check_card_data_updates_enabled.setToolTip(_translate("SettingsWindow", "If enabled, query the Scryfall API if new cards are available. If so, offer to update the local card data."))
+        self.check_card_data_updates_enabled.setText(_translate("SettingsWindow", "Check for new card data"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_general), _translate("SettingsWindow", "General"))
+        self.deck_list_search_path.setToolTip(_translate("SettingsWindow", "If set, use this as the default location for loading deck lists. Your webbrowser’s download directorry is a good choice."))
+        self.deck_list_search_path.setPlaceholderText(_translate("SettingsWindow", "Path to a directory"))
+        self.deck_list_search_path_browse_button.setToolTip(_translate("SettingsWindow", "Browse…"))
+        self.label.setText(_translate("SettingsWindow", "These options control the deck list import function."))
+        self.basic_land_removal_group_box.setTitle(_translate("SettingsWindow", "Control the one-click basic land removal"))
+        self.basic_land_removal_label.setText(_translate("SettingsWindow", "These options control, if the automatic removal should also include Wastes or Snow-Covered basic lands."))
+        self.remove_basic_wastes_enable.setWhatsThis(_translate("SettingsWindow", "Include Wastes when removing basic lands."))
+        self.remove_basic_wastes_enable.setText(_translate("SettingsWindow", "Enable removal of Basic Wastes"))
+        self.remove_snow_basics_enable.setWhatsThis(_translate("SettingsWindow", "Include Snow-Covered basic lands when removing basic lands."))
+        self.remove_snow_basics_enable.setText(_translate("SettingsWindow", "Enable removal of Snow-Covered Basic lands"))
+        self.deck_list_search_path_label.setText(_translate("SettingsWindow", "Deck list search path"))
+        self.print_guessing_group_box.setToolTip(_translate("SettingsWindow", "Not all deck list formats always contain complete data.\n"
 "These options set the default behaviour when encountering ambiguous card"))
-        self.print_guessing_group_box.setTitle(_translate("Dialog", "Control print guessing in ambiguous cases"))
-        self.print_guessing_prefer_already_downloaded.setToolTip(_translate("Dialog", "When guessing a printing, prefer printings with already downloaded images over other possible printings."))
-        self.print_guessing_prefer_already_downloaded.setText(_translate("Dialog", "Prefer printings with already downloaded images"))
-        self.automatic_deck_list_translation_enable.setToolTip(_translate("Dialog", "Always enable automatic deck list translation when importing deck lists.\n"
+        self.print_guessing_group_box.setTitle(_translate("SettingsWindow", "Control print guessing in ambiguous cases"))
+        self.print_guessing_prefer_already_downloaded.setToolTip(_translate("SettingsWindow", "When guessing a printing, prefer printings with already downloaded images over other possible printings."))
+        self.print_guessing_prefer_already_downloaded.setText(_translate("SettingsWindow", "Prefer printings with already downloaded images"))
+        self.automatic_deck_list_translation_enable.setToolTip(_translate("SettingsWindow", "Always enable automatic deck list translation when importing deck lists.\n"
 "This avoids adding foreign language cards, if the deck list happens to contain some."))
-        self.automatic_deck_list_translation_enable.setText(_translate("Dialog", "Enable translating imported deck lists by default"))
-        self.print_guessing_enable.setToolTip(_translate("Dialog", "Not all deck list formats always contain complete data to identify exact printings.\n"
+        self.automatic_deck_list_translation_enable.setText(_translate("SettingsWindow", "Enable translating imported deck lists by default"))
+        self.print_guessing_enable.setToolTip(_translate("SettingsWindow", "Not all deck list formats always contain complete data to identify exact printings.\n"
 "If enabled, choose an arbitrary printing, instead of failing to identify such cards.\n"
 "With some deck list formats, this option is always enabled."))
-        self.print_guessing_enable.setText(_translate("Dialog", "Enable print guessing by default"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_decklist_import), _translate("Dialog", "Deck list import"))
-        self.pdf_page_count_limit.setToolTip(_translate("Dialog", "Automatically split PDF documents, if they get longer than this many pages.\n"
+        self.print_guessing_enable.setText(_translate("SettingsWindow", "Enable print guessing by default"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_decklist_import), _translate("SettingsWindow", "Deck list import"))
+        self.pdf_page_count_limit.setToolTip(_translate("SettingsWindow", "Automatically split PDF documents, if they get longer than this many pages.\n"
 "Set to zero to disable splitting.\n"
 "\n"
 "\n"
 "When printing PDFs using a USB flash drive directly connected to the printer,\n"
 "the printer may refuse to print documents exceeding some arbitrary size limit.\n"
 "To work around this limitation, you can enable this option,\n"
 "and limit the number of pages per PDF. If the document has more pages,\n"
 "it will be exported into multiple PDF documents automatically."))
-        self.pdf_page_count_limit.setSuffix(_translate("Dialog", " pages"))
-        self.pdf_page_count_limit_label.setToolTip(_translate("Dialog", "Automatically split PDF documents, if they get longer than this many pages.\n"
+        self.pdf_page_count_limit.setSuffix(_translate("SettingsWindow", " pages"))
+        self.pdf_page_count_limit_label.setToolTip(_translate("SettingsWindow", "Automatically split PDF documents, if they get longer than this many pages.\n"
 "Set to zero to disable splitting.\n"
 "\n"
 "\n"
 "When printing PDFs using a USB flash drive directly connected to the printer,\n"
 "the printer may refuse to print documents exceeding some arbitrary size limit.\n"
 "To work around this limitation, you can enable this option,\n"
 "and limit the number of pages per PDF. If the document has more pages,\n"
 "it will be exported into multiple PDF documents automatically."))
-        self.pdf_page_count_limit_label.setText(_translate("Dialog", "Split PDF documents longer than"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_page_sizes), _translate("Dialog", "Page size && Printing"))
-        self.card_filter_settings_header_label.setText(_translate("Dialog", "These options allow hiding unwanted cards and printings. Hidden printings are treated as though they don’t exist. They can’t be found in the card search and are automatically replaced in loaded documents or imported deck lists, if possible. If all printings of a card are hidden, it won’t be available at all."))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_card_data_download), _translate("Dialog", "Hide printings"))
-        self.debug_settings_headerlabel.setText(_translate("Dialog", "Debug settings (Changing these require an application restart)"))
-        self.log_level_label.setText(_translate("Dialog", "Event severity that gets logged to file:"))
-        self.open_debug_log_location.setText(_translate("Dialog", "Open debug log directory"))
-        self.log_level_combo_box.setToolTip(_translate("Dialog", "Only write events with the given severity level and higher to the log file."))
-        self.enable_cutelog_integration.setToolTip(_translate("Dialog", "Cutelog is a live log event viewer that can be used to monitor events in real-time."))
-        self.enable_cutelog_integration.setWhatsThis(_translate("Dialog", "<html><head/><body><p>See <a href=\"https://github.com/busimus/cutelog\"><span style=\" text-decoration: underline; color:#2980b9;\">https://github.com/busimus/cutelog</span></a> for details about Cutelog.</p></body></html>"))
-        self.enable_cutelog_integration.setText(_translate("Dialog", "Enable Cutelog integration"))
-        self.enable_write_log_file.setText(_translate("Dialog", "Enable writing a log file to disk"))
-        self.debug_download_card_data_as_file.setText(_translate("Dialog", "Download card data as file"))
-        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_debug), _translate("Dialog", "Debug settings"))
+        self.pdf_page_count_limit_label.setText(_translate("SettingsWindow", "Split PDF documents longer than"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_page_sizes), _translate("SettingsWindow", "Page size && Printing"))
+        self.card_filter_settings_header_label.setText(_translate("SettingsWindow", "These options allow hiding unwanted cards and printings. Hidden printings are treated as though they don’t exist. They can’t be found in the card search and are automatically replaced in loaded documents or imported deck lists, if possible. If all printings of a card are hidden, it won’t be available at all."))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_card_data_download), _translate("SettingsWindow", "Hide printings"))
+        self.debug_settings_headerlabel.setText(_translate("SettingsWindow", "Debug settings (Changing these require an application restart)"))
+        self.log_level_label.setText(_translate("SettingsWindow", "Event severity that gets logged to file:"))
+        self.open_debug_log_location.setText(_translate("SettingsWindow", "Open debug log directory"))
+        self.log_level_combo_box.setToolTip(_translate("SettingsWindow", "Only write events with the given severity level and higher to the log file."))
+        self.enable_cutelog_integration.setToolTip(_translate("SettingsWindow", "Cutelog is a live log event viewer that can be used to monitor events in real-time."))
+        self.enable_cutelog_integration.setWhatsThis(_translate("SettingsWindow", "<html><head/><body><p>See <a href=\"https://github.com/busimus/cutelog\"><span style=\" text-decoration: underline; color:#2980b9;\">https://github.com/busimus/cutelog</span></a> for details about Cutelog.</p></body></html>"))
+        self.enable_cutelog_integration.setText(_translate("SettingsWindow", "Enable Cutelog integration"))
+        self.enable_write_log_file.setText(_translate("SettingsWindow", "Enable writing a log file to disk"))
+        self.debug_download_card_data_as_file.setText(_translate("SettingsWindow", "Download card data as file"))
+        self.tab_widget.setTabText(self.tab_widget.indexOf(self.tab_debug), _translate("SettingsWindow", "Debug settings"))
 from mtg_proxy_printer.ui.page_config_widget import PageConfigWidget
 from mtg_proxy_printer.ui.printing_filter_widgets import FormatPrintingFilterWidget, GeneralPrintingFilterWidget
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/item_delegates.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/item_delegates.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,39 +36,49 @@
     def createEditor(self, parent: QWidget, option: QStyleOptionViewItem, index: QModelIndex) -> QComboBox:
         editor = QComboBox(parent)
         return editor
 
     def setEditorData(self, editor: QComboBox, index: QModelIndex) -> None:
         model: typing.Union[Document, QSortFilterProxyModel] = index.model()
         source_model: Document = model
+        column = index.column()
         while hasattr(source_model, "sourceModel"):  # Resolve the source model to gain access to the card database.
             source_model = source_model.sourceModel()
-        if index.column() == PageColumns.Set:
+        if column == PageColumns.Set:
             matching_sets = source_model.card_db.find_sets_matching(
                 index.siblingAtColumn(PageColumns.CardName).data(Qt.EditRole),
                 index.siblingAtColumn(PageColumns.Language).data(Qt.EditRole),
                 is_front=index.siblingAtColumn(PageColumns.IsFront).data(Qt.EditRole),
             )
             current_set_code = index.data(Qt.EditRole)
             current_set_position = 0
             for position, set_data in enumerate(matching_sets):
                 editor.addItem(set_data.data(Qt.DisplayRole), set_data.data(Qt.EditRole))
                 if set_data.code == current_set_code:
                     current_set_position = position
             editor.setCurrentIndex(current_set_position)
 
-        elif index.column() == PageColumns.CollectorNumber:
+        elif column == PageColumns.CollectorNumber:
             matching_collector_numbers = source_model.card_db.find_collector_numbers_matching(
                 index.siblingAtColumn(PageColumns.CardName).data(Qt.EditRole),
                 index.siblingAtColumn(PageColumns.Set).data(Qt.EditRole),
                 index.siblingAtColumn(PageColumns.Language).data(Qt.EditRole),
             )
             for collector_number in matching_collector_numbers:
                 editor.addItem(collector_number, collector_number)  # Store the key in the UserData role
-            editor.setCurrentIndex(matching_collector_numbers.index(index.data(Qt.EditRole)))
+            if matching_collector_numbers:
+                editor.setCurrentIndex(matching_collector_numbers.index(index.data(Qt.EditRole)))
+
+        elif column == PageColumns.Language:
+            card = index.data(Qt.UserRole)
+            matching_languages = source_model.card_db.get_available_languages_for_card(card)
+            for language in matching_languages:
+                editor.addItem(language, language)
+            if matching_languages:
+                editor.setCurrentIndex(matching_languages.index(index.data(Qt.EditRole)))
 
     def setModelData(self, editor: QComboBox, model: QAbstractItemModel, index: QModelIndex) -> None:
         new_value = editor.currentData(Qt.UserRole)
         previous_value = index.data(Qt.EditRole)
         if new_value != previous_value:
             logger.debug(f"Setting data for column {index.column()} to {new_value}")
             model.setData(index, new_value, Qt.EditRole)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/main_window.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import mtg_proxy_printer.print
 from mtg_proxy_printer.ui.dialogs import SavePDFDialog, SaveDocumentAsDialog, LoadDocumentDialog, \
     AboutMTGProxyPrinterDialog, PrintPreviewDialog, PrintDialog, DocumentSettingsDialog
 from mtg_proxy_printer.ui.cache_cleanup_wizard import CacheCleanupWizard
 from mtg_proxy_printer.ui.deck_import_wizard import DeckImportWizard
 
 try:
-    from mtg_proxy_printer.ui.generated.main_window import Ui_main_window as Ui_MainWindow
+    from mtg_proxy_printer.ui.generated.main_window import Ui_MainWindow
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_MainWindow = load_ui_from_file("main_window")
 
 from mtg_proxy_printer.logger import get_logger
 
 logger = get_logger(__name__)
@@ -110,14 +110,16 @@
             (self.ui.action_new_document, QKeySequence.New),
             (self.ui.action_load_document, QKeySequence.Open),
             (self.ui.action_save_document, QKeySequence.Save),
             (self.ui.action_save_as, QKeySequence.SaveAs),
             (self.ui.action_show_settings, QKeySequence.Preferences),
             (self.ui.action_print, QKeySequence.Print),
             (self.ui.action_quit, QKeySequence.Quit),
+            (self.ui.action_undo, QKeySequence.Undo),
+            (self.ui.action_redo, QKeySequence.Redo),
         ]
         for action, shortcut in actions_with_shortcuts:
             action.setShortcut(shortcut)
 
     def _setup_central_widget(self):
         self.setCentralWidget(self.ui.central_widget)
         self.ui.central_widget.set_data(self.document, self.card_database, self.image_db)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_config_widget.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/page_config_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import configparser
 from functools import partial
 import typing
 
 from PyQt5.QtCore import pyqtSlot as Slot, Qt
-from PyQt5.QtWidgets import QGroupBox, QWidget, QSpinBox, QCheckBox
+from PyQt5.QtWidgets import QGroupBox, QWidget, QSpinBox, QCheckBox, QLineEdit
 
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.ui.common import load_ui_from_file, BlockedSignals
 from mtg_proxy_printer.model.document_loader import PageLayoutSettings
-from mtg_proxy_printer.units_and_sizes import CardSizes, CardSize
+from mtg_proxy_printer.units_and_sizes import CardSizes
 
 try:
-    from mtg_proxy_printer.ui.generated.page_config_widget import Ui_page_configuration_group_box as Ui_PageConfigWidget
+    from mtg_proxy_printer.ui.generated.page_config_widget import Ui_PageConfigWidget
 except ModuleNotFoundError:
     Ui_PageConfigWidget = load_ui_from_file("page_config_widget")
 
 from mtg_proxy_printer.logger import get_logger
 
 logger = get_logger(__name__)
 del get_logger
@@ -59,14 +59,17 @@
         self.ui.image_spacing_horizontal.valueChanged[int].connect(
             partial(setattr, page_layout, "image_spacing_horizontal"))
         self.ui.image_spacing_vertical.valueChanged[int].connect(partial(setattr, page_layout, "image_spacing_vertical"))
         self.ui.draw_cut_markers.stateChanged.connect(
             lambda new: setattr(page_layout, "draw_cut_markers", new == Qt.Checked))
         self.ui.draw_sharp_corners.stateChanged.connect(
             lambda new: setattr(page_layout, "draw_sharp_corners", new == Qt.Checked))
+        self.ui.draw_page_numbers.stateChanged.connect(
+            lambda new: setattr(page_layout, "draw_page_numbers", new == Qt.CheckState.Checked))
+        self.ui.document_name.textChanged.connect(partial(setattr, page_layout, "document_name"))
         return page_layout
 
     @Slot()
     def page_layout_setting_changed(self):
         """
         Recomputes and updates the page capacity value, whenever any page layout widget changes.
         Qt Signal/Slot connections from editor widgets valueChanged[int] signals are defined in the UI file.
@@ -85,46 +88,52 @@
         min_page_height = pl.margin_bottom + pl.margin_top + oversized.as_mm(oversized.height)
         min_page_width = pl.margin_left + pl.margin_right + oversized.as_mm(oversized.width)
         self.ui.page_height.setMinimum(min_page_height)
         self.ui.page_width.setMinimum(min_page_width)
 
     def load_document_settings_from_config(self, settings: configparser.ConfigParser):
         logger.debug(f"About to load document settings from the global settings")
-        document_section = settings["documents"]
+        documents_section = settings["documents"]
         for spinbox, setting in self._get_integer_settings_widgets():
-            spinbox.setValue(document_section.getint(setting))
+            spinbox.setValue(documents_section.getint(setting))
         for checkbox, setting in self._get_boolean_settings_widgets():
-            checkbox.setChecked(document_section.getboolean(setting))
+            checkbox.setChecked(documents_section.getboolean(setting))
+        for line_edit, setting in self._get_string_settings_widgets():
+            line_edit.setText(documents_section[setting])
         logger.debug(f"Loading from settings finished")
 
     def load_from_page_layout(self, other: PageLayoutSettings):
         """Loads the page layout from another PageLayoutSettings instance"""
         logger.debug(f"About to load document settings from a document instance")
         ui = self.ui
         layout = self.page_layout
         for key in layout.__annotations__.keys():
             value = getattr(other, key)
             setattr(self.page_layout, key, value)
             widget = getattr(ui, key)
             with BlockedSignals(widget):  # Don’t call the validation methods in each iteration
                 if isinstance(widget, QSpinBox):
                     widget.setValue(value)
+                elif isinstance(widget, QLineEdit):
+                    widget.setText(value)
                 else:
                     widget.setChecked(value)
         self.validate_paper_size_settings()
         self.page_layout_setting_changed()
         logger.debug(f"Loading from document settings finished")
 
     def save_document_settings_to_config(self):
         logger.info("About to save document settings to the global settings")
         documents_section = mtg_proxy_printer.settings.settings["documents"]
         for spinbox, setting in self._get_integer_settings_widgets():
             documents_section[setting] = str(spinbox.value())
         for checkbox, setting in self._get_boolean_settings_widgets():
             documents_section[setting] = str(checkbox.isChecked())
+        for line_edit, setting in self._get_string_settings_widgets():
+            documents_section[setting] = line_edit.text()
         logger.debug("Saving done.")
 
     def _get_integer_settings_widgets(self):
         widgets_with_settings: typing.List[typing.Tuple[QSpinBox, str]] = [
             (self.ui.page_height, "paper-height-mm"),
             (self.ui.page_width, "paper-width-mm"),
             (self.ui.margin_top, "margin-top-mm"),
@@ -136,9 +145,16 @@
         ]
         return widgets_with_settings
 
     def _get_boolean_settings_widgets(self):
         widgets_with_settings: typing.List[typing.Tuple[QCheckBox, str]] = [
             (self.ui.draw_cut_markers, "print-cut-marker"),
             (self.ui.draw_sharp_corners, "print-sharp-corners"),
+            (self.ui.draw_page_numbers, "print-page-numbers"),
+        ]
+        return widgets_with_settings
+
+    def _get_string_settings_widgets(self):
+        widgets_with_settings: typing.List[typing.Tuple[QLineEdit, str]] = [
+            (self.ui.document_name, "default-document-name")
         ]
         return widgets_with_settings
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/page_renderer.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/page_renderer.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 import itertools
 import functools
 import typing
 
 from PyQt5.QtCore import pyqtSlot as Slot, QRectF, QPointF, QSizeF, Qt, QModelIndex, QPersistentModelIndex, QObject,\
     pyqtSignal as Signal, QEvent
 from PyQt5.QtWidgets import QGraphicsView, QGraphicsScene, QWidget, QAction, \
-    QGraphicsLineItem, QGraphicsItemGroup, QGraphicsItem, QGraphicsRectItem, QGraphicsPixmapItem
-from PyQt5.QtGui import QColor, QWheelEvent, QKeySequence, QPalette, QBrush, QResizeEvent, QPen, QColorConstants
+    QGraphicsLineItem, QGraphicsItemGroup, QGraphicsItem, QGraphicsRectItem, QGraphicsPixmapItem, QGraphicsSimpleTextItem
+from PyQt5.QtGui import QColor, QWheelEvent, QKeySequence, QPalette, QBrush, QResizeEvent, QPen, QColorConstants, \
+    QFontMetrics
 import pint
 
 from mtg_proxy_printer.units_and_sizes import PageType, CardSizes, CardSize, unit_registry, RESOLUTION
 from mtg_proxy_printer.model.document_loader import PageLayoutSettings
 from mtg_proxy_printer.model.document import Document
 from mtg_proxy_printer.model.carddb import Card, CardCorner
 from mtg_proxy_printer.model.card_list import PageColumns
@@ -38,20 +39,22 @@
 
 __all__ = [
     "RenderMode",
     "PageScene",
     "PageRenderer",
 ]
 PixelCache = typing.DefaultDict[PageType, typing.List[float]]
+ItemDataRole = Qt.ItemDataRole
 
 
 @enum.unique
 class RenderLayers(enum.Enum):
     BACKGROUND = -3
     CUT_LINES = -2
+    TEXT = -1
     CARDS = 0
 
 
 @enum.unique
 class ZoomDirection(enum.Enum):
     IN = enum.auto()
     OUT = enum.auto()
@@ -129,14 +132,18 @@
     return isinstance(item, CardItem)
 
 
 def is_cut_line_item(item: QGraphicsItem) -> bool:
     return isinstance(item, QGraphicsLineItem)
 
 
+def is_text_item(item: QGraphicsItem) -> bool:
+    return isinstance(item, QGraphicsSimpleTextItem)
+
+
 class PageScene(QGraphicsScene):
     """This class implements the low-level rendering of the currently selected page on a blank canvas."""
 
     scene_size_changed = Signal()
 
     def __init__(self, document: Document, render_mode: RenderMode, parent: QObject = None):
         """
@@ -152,96 +159,199 @@
         self.document.rowsRemoved.connect(self.on_rows_removed)
         self.document.rowsAboutToBeRemoved.connect(self.on_rows_about_to_be_removed)
         self.document.rowsMoved.connect(self.on_rows_moved)
         self.document.current_page_changed.connect(self.on_current_page_changed)
         self.document.dataChanged.connect(self.on_data_changed)
         self.document.page_type_changed.connect(self.on_page_type_changed)
         self.document.page_layout_changed.connect(self.on_page_layout_changed)
-        self.selected_page: QPersistentModelIndex = self.document.get_current_page_index()
+        self.selected_page = self.document.get_current_page_index()
         self.setBackgroundBrush(QBrush(QColorConstants.White, Qt.SolidPattern))
         self.render_mode = render_mode
         background_color = self.get_background_color(render_mode)
         logger.debug(f"Drawing background rectangle")
         self.background = self.addRect(0, 0, self.width(), self.height(), background_color, background_color)
         self.background.setZValue(RenderLayers.BACKGROUND.value)
         self.horizontal_cut_line_locations: PixelCache = collections.defaultdict(list)
         self.vertical_cut_line_locations: PixelCache = collections.defaultdict(list)
         self._update_cut_marker_positions()
+        self.document_title_text = self._create_text_item()
+        self.page_number_text = self._create_text_item()
+        self._update_text_items(document.page_layout)
         if document.page_layout.draw_cut_markers:
             self.draw_cut_markers()
         logger.info(f"Created {self.__class__.__name__} instance. Render mode: {self.render_mode}")
 
+    @staticmethod
+    def _create_text_item(font_size: float = 40):
+        item = QGraphicsSimpleTextItem()
+        font = item.font()
+        font.setPointSizeF(font_size)
+        item.setFont(font)
+        return item
+
     def get_background_color(self, render_mode: RenderMode) -> QColor:
         if render_mode is RenderMode.ON_PAPER:
             return QColorConstants.Transparent
         return self.palette().color(QPalette.Active, QPalette.Base)
 
     def get_cut_marker_color(self, render_mode: RenderMode) -> QColor:
         if render_mode is RenderMode.ON_PAPER:
             return QColorConstants.Black
         return self.palette().color(QPalette.Active, QPalette.WindowText)
 
+    def get_text_color(self, render_mode: RenderMode) -> QColor:
+        if render_mode is RenderMode.ON_PAPER:
+            return QColorConstants.Black
+        return self.palette().color(QPalette.Active, QPalette.WindowText)
+
     def setPalette(self, palette: QPalette) -> None:
         logger.info("Color palette changed, updating PageScene background and cut line colors.")
         super().setPalette(palette)
         background_color = self.get_background_color(self.render_mode)
         self.background.setPen(background_color)
         self.background.setBrush(background_color)
         cut_line_color = self.get_cut_marker_color(self.render_mode)
+        text_color = self.get_text_color(self.render_mode)
         logger.info(f"Number of cut lines: {len(self.cut_lines)}")
         for line in self.cut_lines:
             line.setPen(cut_line_color)
+        for item in self.text_items:
+            item.setDefaultTextColor(text_color)
 
     @property
     def card_items(self) -> typing.List[CardItem]:
         return list(filter(is_card_item, self.items(Qt.AscendingOrder)))
 
     @property
     def cut_lines(self) -> typing.List[QGraphicsLineItem]:
         return list(filter(is_cut_line_item, self.items(Qt.AscendingOrder)))
 
+    @property
+    def text_items(self) -> typing.List[QGraphicsSimpleTextItem]:
+        return list(filter(is_text_item, self.items(Qt.AscendingOrder)))
+
     @Slot(QPersistentModelIndex)
     def on_current_page_changed(self, selected_page: QPersistentModelIndex):
         """Draws the canvas, when the currently selected page changes."""
         logger.debug(f"Current page changed to page {selected_page.row()}")
         page_types: typing.Set[PageType] = {
-            self.selected_page.data(Qt.UserRole),
-            selected_page.data(Qt.UserRole)
+            self.selected_page.data(ItemDataRole.UserRole),
+            selected_page.data(ItemDataRole.UserRole)
         }
         self.selected_page = selected_page
 
         if PageType.OVERSIZED in page_types and len(page_types) > 1:  # Switching to or from an oversized page
             logger.debug("New page contains cards of different size, re-drawing cut markers")
             self.remove_cut_markers()
             self.draw_cut_markers()
-
         for item in self.card_items:
             self.removeItem(item)
         if self._is_valid_page_index(selected_page):
+            self._update_page_number_text()
+            self._update_page_text_x()
+            self._update_page_text_y()
             self._draw_cards()
 
+    def _update_page_text_y(self):
+        # Put the text labels below the
+        y = 2 + round(max(
+            self.horizontal_cut_line_locations[PageType.REGULAR][-1],
+            self.horizontal_cut_line_locations[PageType.OVERSIZED][-1]
+        ))
+        for item in self.text_items:
+            item.setY(y)
+
+    def _update_page_text_x(self):
+        title_x = self._mm_to_rounded_px(self.document.page_layout.margin_right) + 1
+        self.document_title_text.setX(title_x)
+        font_metrics = QFontMetrics(self.page_number_text.font())
+        text_width = font_metrics.horizontalAdvance(self.page_number_text.text())
+        page_number_x = round(
+            self.width()
+            - self._mm_to_rounded_px(self.document.page_layout.margin_right) - text_width - 2
+        )
+        self.page_number_text.setX(page_number_x)
+
+    def _update_page_number_text(self):
+        model = self.selected_page.model()
+        if self.page_number_text not in self.text_items:
+            return
+        logger.debug("Updating page number text")
+        page = self.selected_page.row() + 1
+        total_pages = model.rowCount()
+        self.page_number_text.setText(f"{page}/{total_pages}")
+
     @Slot(PageLayoutSettings)
     def on_page_layout_changed(self, new_page_layout: PageLayoutSettings):
+        logger.info("Applying new document settings …")
         new_page_size = self.get_document_page_size(new_page_layout)
         old_size = self.sceneRect()
         size_changed = old_size != new_page_size
         if size_changed:
             logger.debug("Page size changed. Adjusting PageScene dimensions")
             self.setSceneRect(new_page_size)
             self.background.setRect(new_page_size)
         self._update_cut_marker_positions()
         self.remove_cut_markers()
         if new_page_layout.draw_cut_markers:
             self.draw_cut_markers()
         self._compute_position_for_image.cache_clear()
         self.update_card_positions()
+        self._update_text_items(new_page_layout)
         if size_changed:
             # Changed paper dimensions very likely caused the page aspect ratio to change. It may no longer fit
             # in the available space or is now too small, so emit a notification to allow the display widget to adjust.
             self.scene_size_changed.emit()
+        logger.info("New document settings applied")
+
+    def _update_text_items(self, page_layout: PageLayoutSettings):
+        self._update_page_number_text()
+        self.document_title_text.setText(self._format_document_title(page_layout.document_name))
+        self._update_text_visibility(self.document_title_text, page_layout.document_name)
+        self._update_text_visibility(self.page_number_text, page_layout.draw_page_numbers)
+        self._update_page_text_x()
+        self._update_page_text_y()
+
+    def _format_document_title(self, title: str) -> str:
+        page_layout = self.document.page_layout
+        font_metrics = QFontMetrics(self.document_title_text.font())
+        space_width_px = font_metrics.horizontalAdvance(" ")
+        margins_px = self._mm_to_rounded_px(page_layout.margin_left+page_layout.margin_right)
+        available_widths_px = itertools.chain(
+            [self.width()-margins_px-QFontMetrics(self.page_number_text.font()).horizontalAdvance("999/999")-4],
+            itertools.repeat(self.width()-margins_px-4)
+        )
+        words = collections.deque(title.split(" "))
+        lines: typing.List[str] = []
+        current_line_words: typing.List[str] = []
+        current_line_available_space = next(available_widths_px)
+        current_line_used_space = 0
+        logger.debug(f"Formatting line {len(lines)+1}, {current_line_available_space=}")
+        while words:
+            word = words.popleft()
+            word_width_px = font_metrics.horizontalAdvance(word)
+            if current_line_used_space + word_width_px + space_width_px <= current_line_available_space:
+                current_line_words.append(word)
+                current_line_used_space += space_width_px + word_width_px
+            else:
+                logger.debug(f"Formatting line {len(lines)+1}, {current_line_available_space=}")
+                current_line_available_space = next(available_widths_px)
+                lines.append(" ".join(current_line_words))
+                current_line_words = [word]
+                current_line_used_space = word_width_px
+        if current_line_words:
+            lines.append(" ".join(current_line_words))
+        return "\n".join(lines)
+
+    def _update_text_visibility(self, item: QGraphicsSimpleTextItem, new_visibility):
+        text_items = self.text_items
+        if item not in text_items and new_visibility:
+            self.addItem(item)
+        elif item in text_items and not new_visibility:
+            self.removeItem(item)
 
     @staticmethod
     def get_document_page_size(page_layout: PageLayoutSettings) -> QRectF:
         height: pint.Quantity = page_layout.page_height * unit_registry.millimeter
         width: pint.Quantity = page_layout.page_width * unit_registry.millimeter
         page_size = QRectF(
             QPointF(0, 0),
@@ -250,86 +360,92 @@
                 (RESOLUTION * height).to("pixel").magnitude
             )
         )
         return page_size
 
     def _draw_cards(self):
         index = self.selected_page.sibling(self.selected_page.row(), 0)
-        page_type: PageType = self.selected_page.data(Qt.UserRole)
+        page_type: PageType = self.selected_page.data(ItemDataRole.UserRole)
         images_to_draw = self.selected_page.model().rowCount(index)
         logger.info(f"Drawing {images_to_draw} cards")
         for row in range(images_to_draw):
             self.draw_card(row, page_type)
 
     def draw_card(self, row: int, page_type: PageType, next_item: CardItem = None):
         index = self.selected_page.child(row, PageColumns.Image)
         position = self._compute_position_for_image(row, page_type)
-        if index.data(Qt.DisplayRole) is not None:  # Card has a QPixmap set
-            card: Card = index.internalPointer().card
+        if index.data(ItemDataRole.DisplayRole) is not None:  # Card has a QPixmap set
+            card: Card = index.data(ItemDataRole.UserRole)
             self.addItem(card_item := CardItem(card, self.document))
             card_item.setPos(position)
             if next_item is not None:
                 # See https://doc.qt.io/qt-6/qgraphicsitem.html#sorting
                 # "You can call stackBefore() to reorder the list of children.
                 # This will directly modify the insertion order."
                 # This is required to keep the card order consistent with the model when inserting cards in the
                 # middle of the page. This can happen when undoing a card removal. The caller has to supply the
                 # item which’s position the new item takes.
                 card_item.stackBefore(next_item)
 
     def update_card_positions(self):
-        page_type: PageType = self.selected_page.data(Qt.UserRole)
+        page_type: PageType = self.selected_page.data(ItemDataRole.UserRole)
         for index, card in enumerate(self.card_items):
             card.setPos(self._compute_position_for_image(index, page_type))
 
     def _is_valid_page_index(self, index: QModelIndex):
         return index.isValid() and not index.parent().isValid() and index.row() < self.document.rowCount()
 
     @Slot(QModelIndex)
     def on_page_type_changed(self, page: QModelIndex):
         if page.row() == self.selected_page.row():
             self.update_card_positions()
             if self.document.page_layout.draw_cut_markers:
                 self.remove_cut_markers()
                 self.draw_cut_markers()
 
-    def on_data_changed(self, top_left: QModelIndex, bottom_right: QModelIndex, roles: typing.List[Qt.ItemDataRole]):
-        if top_left.parent().row() == self.selected_page.row() and Qt.DisplayRole in roles:
-            page_type: PageType = top_left.parent().data(Qt.UserRole)
+    def on_data_changed(self, top_left: QModelIndex, bottom_right: QModelIndex, roles: typing.List[ItemDataRole]):
+        if top_left.parent().row() == self.selected_page.row() and ItemDataRole.DisplayRole in roles:
+            page_type: PageType = top_left.parent().data(ItemDataRole.UserRole)
             card_items = self.card_items
             for row in range(top_left.row(), bottom_right.row()+1):
                 logger.debug(f"Card {row} on the current page was replaced, replacing image.")
                 current_item = card_items[row]
                 self.draw_card(row, page_type, current_item)
                 self.removeItem(current_item)
 
     def on_rows_inserted(self, parent: QModelIndex, first: int, last: int):
         if self._is_valid_page_index(parent) and parent.row() == self.selected_page.row():
             inserted_cards = last-first+1
             needs_reorder = first + inserted_cards < self.document.rowCount(parent)
             next_item = self.card_items[first] if needs_reorder else None
-            page_type: PageType = self.selected_page.data(Qt.EditRole).page_type()
+            page_type: PageType = self.selected_page.data(ItemDataRole.EditRole).page_type()
             logger.debug(f"Added {inserted_cards} cards to the currently shown page, drawing them.")
             for new in range(first, last+1):
                 self.draw_card(new, page_type, next_item)
             if needs_reorder:
                 logger.debug("Cards added in the middle of the page, re-order existing cards.")
                 self.update_card_positions()
+        elif self.selected_page.isValid():
+            # Page inserted. Update the page number text, as it contains the total number of pages
+            self._update_page_number_text()
 
     def on_rows_about_to_be_removed(self, parent: QModelIndex, first: int, last: int):
         if not parent.isValid() and first <= self.selected_page.row() <= last:
             logger.debug("About to delete the currently shown page. Removing the held index.")
             self.selected_page = QPersistentModelIndex()
 
     def on_rows_removed(self, parent: QModelIndex, first: int, last: int):
         if parent.isValid() and parent.row() == self.selected_page.row():
             logger.debug(f"Removing cards {first} to {last} from the current page.")
             for item in self.card_items[first:last+1]:
                 self.removeItem(item)
             self.update_card_positions()
+        elif self.selected_page.isValid():
+            # Page removed. Update the page number text, as it contains the total number of pages
+            self._update_page_number_text()
 
     def on_rows_moved(self, parent: QModelIndex, start: int, end: int, destination: QModelIndex, row: int):
         if parent.isValid() and parent.row() == self.selected_page.row():
             # Cards moved away are treated as if they were deleted
             logger.debug("Cards moved away from the currently shown page, calling card removal handler.")
             self.on_rows_removed(parent, start, end)
         if destination.isValid() and destination.row() == self.selected_page.row():
@@ -367,15 +483,15 @@
 
     def remove_cut_markers(self):
         for line in self.cut_lines:
             self.removeItem(line)
 
     def draw_cut_markers(self):
         """Draws the optional cut markers that extend to the paper border"""
-        page_type: PageType = self.selected_page.data(Qt.EditRole).page_type()
+        page_type: PageType = self.selected_page.data(ItemDataRole.EditRole).page_type()
         if page_type == PageType.MIXED:
             logger.warning("Not drawing cut markers for page with mixed image sizes")
             return
         line_color = self.get_cut_marker_color(self.render_mode)
         logger.info(f"Drawing cut markers")
         self._draw_vertical_markers(line_color, page_type)
         self._draw_horizontal_markers(line_color, page_type)
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/printing_filter_widgets.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/printing_filter_widgets.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,30 @@
 
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 import abc
 import configparser
 import functools
-import typing
+from functools import partial
+from typing import Union, Type, List, Tuple
 
 from PyQt5.QtCore import QUrl
 from PyQt5.QtGui import QDesktopServices
 from PyQt5.QtWidgets import QGroupBox, QWidget, QCheckBox, QPushButton
 
 try:
-    from mtg_proxy_printer.ui.generated.settings_window.format_printing_filter import Ui_card_download_format_settings as Ui_FormatPrintingFilter
-    from mtg_proxy_printer.ui.generated.settings_window.general_printing_filter import Ui_Form as Ui_GeneralPrintingFilter
+    from mtg_proxy_printer.ui.generated.settings_window.format_printing_filter import Ui_FormatPrintingFilter
+    from mtg_proxy_printer.ui.generated.settings_window.general_printing_filter import Ui_GeneralPrintingFilter
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_FormatPrintingFilter = load_ui_from_file("settings_window/format_printing_filter")
     Ui_GeneralPrintingFilter = load_ui_from_file("settings_window/general_printing_filter")
 
-UiTypes = typing.Union[typing.Type[Ui_FormatPrintingFilter], typing.Type[Ui_GeneralPrintingFilter]]
+UiTypes = Union[Type[Ui_FormatPrintingFilter], Type[Ui_GeneralPrintingFilter]]
 
 
 class AbstractPrintingFilterWidget(QGroupBox):
 
     def __init__(self, ui_class: UiTypes, parent: QWidget = None):
         super(AbstractPrintingFilterWidget, self).__init__(parent)
         self.ui = ui_class()
@@ -52,36 +53,36 @@
     @staticmethod
     def view_query_on_scryfall(query: str):
         query_url = QUrl("https://scryfall.com/search", QUrl.StrictMode)
         query_url.setQuery(f"q={query}", QUrl.StrictMode)
         QDesktopServices.openUrl(query_url)
 
     @abc.abstractmethod
-    def _get_widgets_with_keys(self) -> typing.List[typing.Tuple[QCheckBox, str]]:
+    def _get_widgets_with_keys(self) -> List[Tuple[QCheckBox, str]]:
         pass
 
 
 class GeneralPrintingFilterWidget(AbstractPrintingFilterWidget):
     def __init__(self, parent: QWidget = None):
         super().__init__(Ui_GeneralPrintingFilter, parent)
         ui = self.ui
         ui.view_cards_depicting_racism.clicked.connect(
-            lambda: self.view_query_on_scryfall("function:banned-due-to-racist-imagery"))
-        ui.view_oversized_cards.clicked.connect(lambda: self.view_query_on_scryfall("is:oversized"))
-        ui.view_white_bordered_cards.clicked.connect(lambda: self.view_query_on_scryfall("border:white"))
-        ui.view_gold_bordered_cards.clicked.connect(lambda: self.view_query_on_scryfall("border:gold"))
-        ui.view_borderless_cards.clicked.connect(lambda: self.view_query_on_scryfall("border:borderless"))
-        ui.view_funny_cards.clicked.connect(lambda: self.view_query_on_scryfall("is:funny"))
-        ui.view_token.clicked.connect(lambda: self.view_query_on_scryfall("is:token"))
-        ui.view_digital_cards.clicked.connect(lambda: self.view_query_on_scryfall("is:digital"))
-        ui.view_reversible_cards.clicked.connect(lambda: self.view_query_on_scryfall("is:reversible"))
+            partial(self.view_query_on_scryfall, "function:banned-due-to-racist-imagery"))
+        ui.view_oversized_cards.clicked.connect(partial(self.view_query_on_scryfall, "is:oversized"))
+        ui.view_white_bordered_cards.clicked.connect(partial(self.view_query_on_scryfall, "border:white"))
+        ui.view_gold_bordered_cards.clicked.connect(partial(self.view_query_on_scryfall, "border:gold"))
+        ui.view_borderless_cards.clicked.connect(partial(self.view_query_on_scryfall, "border:borderless"))
+        ui.view_funny_cards.clicked.connect(partial(self.view_query_on_scryfall, "is:funny"))
+        ui.view_token.clicked.connect(partial(self.view_query_on_scryfall, "is:token"))
+        ui.view_digital_cards.clicked.connect(partial(self.view_query_on_scryfall, "is:digital"))
+        ui.view_reversible_cards.clicked.connect(partial(self.view_query_on_scryfall, "is:reversible"))
 
-    def _get_widgets_with_keys(self) -> typing.List[typing.Tuple[QCheckBox, str]]:
+    def _get_widgets_with_keys(self) -> List[Tuple[QCheckBox, str]]:
         ui = self.ui
-        widgets_with_settings: typing.List[typing.Tuple[QCheckBox, str]] = [
+        widgets_with_settings: List[Tuple[QCheckBox, str]] = [
             (ui.hide_cards_depicting_racism, "hide-cards-depicting-racism"),
             (ui.hide_cards_without_images, "hide-cards-without-images"),
             (ui.hide_oversized_cards, "hide-oversized-cards"),
             (ui.hide_white_bordered_cards, "hide-white-bordered"),
             (ui.hide_gold_bordered_cards, "hide-gold-bordered"),
             (ui.hide_borderless_cards, "hide-borderless"),
             (ui.hide_funny_cards, "hide-funny-cards"),
@@ -97,20 +98,20 @@
     def __init__(self, parent: QWidget = None):
         super().__init__(Ui_FormatPrintingFilter, parent)
         ui = self.ui
         for _, key in self._get_widgets_with_keys():
             format_name = key.split("-")[-1]
             button: QPushButton = getattr(ui, f"view_banned_in_{format_name}")
             button.clicked.connect(
-                functools.partial(self.view_query_on_scryfall, f"banned:{format_name}")
+                partial(self.view_query_on_scryfall, f"banned:{format_name}")
             )
 
-    def _get_widgets_with_keys(self) -> typing.List[typing.Tuple[QCheckBox, str]]:
+    def _get_widgets_with_keys(self) -> List[Tuple[QCheckBox, str]]:
         ui = self.ui
-        widgets_with_settings: typing.List[typing.Tuple[QCheckBox, str]] = [
+        widgets_with_settings: List[Tuple[QCheckBox, str]] = [
             (ui.hide_banned_in_brawl, "hide-banned-in-brawl"),
             (ui.hide_banned_in_commander, "hide-banned-in-commander"),
             (ui.hide_banned_in_historic, "hide-banned-in-historic"),
             (ui.hide_banned_in_legacy, "hide-banned-in-legacy"),
             (ui.hide_banned_in_modern, "hide-banned-in-modern"),
             (ui.hide_banned_in_pauper, "hide-banned-in-pauper"),
             (ui.hide_banned_in_penny, "hide-banned-in-penny"),
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/ui/settings_window.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/ui/settings_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from mtg_proxy_printer.document_controller.edit_document_settings import ActionEditDocumentSettings
 
 import mtg_proxy_printer.settings
 from mtg_proxy_printer.progress_meter import ProgressMeter
 from mtg_proxy_printer.logger import get_logger
 
 try:
-    from mtg_proxy_printer.ui.generated.settings_window.settings_window import Ui_Dialog as Ui_SettingsWindow
+    from mtg_proxy_printer.ui.generated.settings_window.settings_window import Ui_SettingsWindow
 except ModuleNotFoundError:
     from mtg_proxy_printer.ui.common import load_ui_from_file
     Ui_SettingsWindow = load_ui_from_file("settings_window/settings_window")
 
 logger = get_logger(__name__)
 del get_logger
 __all__ = [
```

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/units_and_sizes.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/units_and_sizes.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/mtg_proxy_printer/update_checker.py` & `MTGProxyPrinter-0.25.0/mtg_proxy_printer/update_checker.py`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/pyproject.toml` & `MTGProxyPrinter-0.25.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `MTGProxyPrinter-0.24.1/setup.py` & `MTGProxyPrinter-0.25.0/setup.py`

 * *Files identical despite different names*

