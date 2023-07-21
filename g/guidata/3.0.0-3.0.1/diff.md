# Comparing `tmp/guidata-3.0.0.tar.gz` & `tmp/guidata-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guidata-3.0.0.tar", last modified: Thu Jul  6 16:25:04 2023, max compression
+gzip compressed data, was "guidata-3.0.1.tar", last modified: Fri Jul 21 16:08:50 2023, max compression
```

## Comparing `guidata-3.0.0.tar` & `guidata-3.0.1.tar`

### file list

```diff
@@ -1,210 +1,178 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.453874 guidata-3.0.0/
--rw-rw-rw-   0        0        0    18426 2023-07-06 14:11:58.000000 guidata-3.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.0/LICENSE
--rw-rw-rw-   0        0        0      186 2023-07-06 16:11:07.000000 guidata-3.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3359 2023-07-06 16:25:03.454875 guidata-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2218 2023-07-06 12:34:12.000000 guidata-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.845870 guidata-3.0.0/doc/
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.847869 guidata-3.0.0/doc/_static/
--rw-rw-rw-   0        0        0    97375 2023-06-30 10:35:52.000000 guidata-3.0.0/doc/_static/favicon.ico
--rw-rw-rw-   0        0        0      734 2023-06-12 16:28:37.000000 guidata-3.0.0/doc/basic_example.py
--rw-rw-rw-   0        0        0     1253 2023-07-06 14:41:46.000000 guidata-3.0.0/doc/conf.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.863871 guidata-3.0.0/doc/dev/
--rw-rw-rw-   0        0        0     1839 2023-07-06 07:59:24.000000 guidata-3.0.0/doc/dev/contribute.rst
--rw-rw-rw-   0        0        0      975 2023-07-06 12:59:03.000000 guidata-3.0.0/doc/dev/howto.rst
--rw-rw-rw-   0        0        0      123 2023-07-06 12:57:35.000000 guidata-3.0.0/doc/dev/index.rst
--rw-rw-rw-   0        0        0     1186 2023-07-06 13:32:10.000000 guidata-3.0.0/doc/dev/v2_to_v3.rst
--rw-rw-rw-   0        0        0     1631 2023-07-06 14:12:31.000000 guidata-3.0.0/doc/examples.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.884868 guidata-3.0.0/doc/images/
--rw-rw-rw-   0        0        0     4718 2023-07-06 12:12:29.000000 guidata-3.0.0/doc/images/basic_example.png
--rw-rw-rw-   0        0        0    16573 2023-07-06 15:02:39.000000 guidata-3.0.0/doc/images/guidata-banner.png
--rw-rw-rw-   0        0        0     6176 2023-06-30 10:38:57.000000 guidata-3.0.0/doc/images/guidata-vertical.png
--rw-rw-rw-   0        0        0    14799 2023-07-06 12:21:56.000000 guidata-3.0.0/doc/images/layout_example.png
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.926867 guidata-3.0.0/doc/images/screenshots/
--rw-rw-rw-   0        0        0    78499 2023-07-06 12:13:38.000000 guidata-3.0.0/doc/images/screenshots/__init__.png
--rw-rw-rw-   0        0        0     4765 2023-07-06 12:14:34.000000 guidata-3.0.0/doc/images/screenshots/activable_dataset.png
--rw-rw-rw-   0        0        0    31447 2023-07-06 12:15:25.000000 guidata-3.0.0/doc/images/screenshots/all_features.png
--rw-rw-rw-   0        0        0    37993 2023-07-06 12:15:56.000000 guidata-3.0.0/doc/images/screenshots/all_items.png
--rw-rw-rw-   0        0        0     8866 2023-07-06 12:16:16.000000 guidata-3.0.0/doc/images/screenshots/bool_selector.png
--rw-rw-rw-   0        0        0    32420 2023-07-06 12:16:41.000000 guidata-3.0.0/doc/images/screenshots/datasetgroup.png
--rw-rw-rw-   0        0        0    20345 2023-07-06 12:17:05.000000 guidata-3.0.0/doc/images/screenshots/editgroupbox.png
--rw-rw-rw-   0        0        0      900 2023-07-06 12:56:58.000000 guidata-3.0.0/doc/index.rst
--rw-rw-rw-   0        0        0      507 2023-07-06 12:07:32.000000 guidata-3.0.0/doc/installation.rst
--rw-rw-rw-   0        0        0     1731 2023-07-06 12:22:51.000000 guidata-3.0.0/doc/overview.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.934867 guidata-3.0.0/doc/reference/
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.974873 guidata-3.0.0/doc/reference/dataset/
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:46.000000 guidata-3.0.0/doc/reference/dataset/dataitems.rst
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:54.000000 guidata-3.0.0/doc/reference/dataset/datatypes.rst
--rw-rw-rw-   0        0        0      137 2023-07-06 12:24:53.000000 guidata-3.0.0/doc/reference/dataset/index.rst
--rw-rw-rw-   0        0        0       43 2023-06-30 13:46:30.000000 guidata-3.0.0/doc/reference/dataset/qtwidgets.rst
--rw-rw-rw-   0        0        0       33 2023-06-30 12:46:29.000000 guidata-3.0.0/doc/reference/guitest.rst
--rw-rw-rw-   0        0        0      133 2023-07-06 12:24:40.000000 guidata-3.0.0/doc/reference/index.rst
--rw-rw-rw-   0        0        0      130 2023-06-30 12:45:12.000000 guidata-3.0.0/doc/reference/utils.rst
--rw-rw-rw-   0        0        0      120 2023-06-30 10:49:38.000000 guidata-3.0.0/doc/reference/widgets.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.993870 guidata-3.0.0/guidata/
--rw-rw-rw-   0        0        0     3004 2023-07-06 14:12:41.000000 guidata-3.0.0/guidata/__init__.py
--rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.0/guidata/config.py
--rw-rw-rw-   0        0        0    14144 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/configtools.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.026870 guidata-3.0.0/guidata/dataset/
--rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/__init__.py
--rw-rw-rw-   0        0        0    33232 2023-07-06 12:39:43.000000 guidata-3.0.0/guidata/dataset/dataitems.py
--rw-rw-rw-   0        0        0    34658 2023-07-06 14:12:57.000000 guidata-3.0.0/guidata/dataset/datatypes.py
--rw-rw-rw-   0        0        0    23498 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/hdf5io.py
--rw-rw-rw-   0        0        0    11586 2023-07-06 12:40:58.000000 guidata-3.0.0/guidata/dataset/iniio.py
--rw-rw-rw-   0        0        0     8371 2023-06-30 12:40:36.000000 guidata-3.0.0/guidata/dataset/jsonio.py
--rw-rw-rw-   0        0        0    40201 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/qtitemwidgets.py
--rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/qtwidgets.py
--rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/dataset/textedit.py
--rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.0/guidata/env.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.029869 guidata-3.0.0/guidata/external/
--rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.042874 guidata-3.0.0/guidata/external/darkdetect/
--rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/__init__.py
--rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_dummy.py
--rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_linux_detect.py
--rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_mac_detect.py
--rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/external/darkdetect/_windows_detect.py
--rw-rw-rw-   0        0        0   361592 2023-07-06 16:24:46.000000 guidata-3.0.0/guidata/guidata.chm
--rw-rw-rw-   0        0        0    11264 2023-07-06 14:13:06.000000 guidata-3.0.0/guidata/guitest.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.128870 guidata-3.0.0/guidata/images/
--rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/apply.png
--rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/arredit.png
--rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/busy.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/cell_edit.png
--rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/copy.png
--rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/delete.png
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/dictedit.png
--rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/dtype.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/edit.png
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.172872 guidata-3.0.0/guidata/images/editors/
--rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/copywop.png
--rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/edit.png
--rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/edit_add.png
--rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editclear.png
--rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editcopy.png
--rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editcut.png
--rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editdelete.png
--rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/editpaste.png
--rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/fileimport.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/filesave.png
--rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/imshow.png
--rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/insert.png
--rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/plot.png
--rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/rename.png
--rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/editors/selectall.png
--rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/exit.png
--rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/expander_down.png
--rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/expander_right.png
--rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/file.png
--rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/fileclose.png
--rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/fileimport.png
--rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filenew.png
--rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/fileopen.png
--rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filesave.png
--rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filesaveas.png
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.255873 guidata-3.0.0/guidata/images/filetypes/
--rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/doc.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/gif.png
--rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/html.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/jpg.png
--rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/pdf.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/png.png
--rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/pps.png
--rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/ps.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/tar.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/tgz.png
--rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/tif.png
--rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/txt.png
--rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/xls.png
--rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/filetypes/zip.png
--rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.0/guidata/images/guidata-banner.svg
--rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.0/guidata/images/guidata-vertical.svg
--rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.0/guidata/images/guidata.svg
--rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/max.png
--rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/min.png
--rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/none.png
--rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/not_found.png
--rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/python.png
--rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/quickview.png
--rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/save_all.png
--rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/selection.png
--rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/settings.png
--rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/shape.png
--rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/xmax.png
--rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/images/xmin.png
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.257873 guidata-3.0.0/guidata/locale/
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:02.792868 guidata-3.0.0/guidata/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.261873 guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.mo
--rw-rw-rw-   0        0        0    20765 2023-06-29 17:09:05.000000 guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.po
--rw-rw-rw-   0        0        0    16593 2023-06-29 17:08:15.000000 guidata-3.0.0/guidata/locale/guidata.pot
--rw-rw-rw-   0        0        0    20476 2023-07-06 12:39:28.000000 guidata-3.0.0/guidata/qthelpers.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.359874 guidata-3.0.0/guidata/tests/
--rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/__init__.py
--rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.0/guidata/tests/_all_tests.py
--rw-rw-rw-   0        0        0      469 2023-06-29 14:36:29.000000 guidata-3.0.0/guidata/tests/conftest.py
--rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.0/guidata/tests/test_activable_dataset.py
--rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.0/guidata/tests/test_activable_items.py
--rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.0/guidata/tests/test_all_features.py
--rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.0/guidata/tests/test_all_items.py
--rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.0/guidata/tests/test_arrayeditor.py
--rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.0/guidata/tests/test_bool_selector.py
--rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.0/guidata/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.0/guidata/tests/test_codeeditor.py
--rw-rw-rw-   0        0        0     3794 2023-07-06 14:14:29.000000 guidata-3.0.0/guidata/tests/test_collectionseditor.py
--rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_config.py
--rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.0/guidata/tests/test_console.py
--rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.0/guidata/tests/test_data.py
--rw-rw-rw-   0        0        0     1944 2023-07-06 14:14:58.000000 guidata-3.0.0/guidata/tests/test_dataframeeditor.py
--rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_datasetgroup.py
--rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.0/guidata/tests/test_disthelpers.py
--rw-rw-rw-   0        0        0     6011 2023-07-06 14:15:08.000000 guidata-3.0.0/guidata/tests/test_editgroupbox.py
--rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.0/guidata/tests/test_importwizard.py
--rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.0/guidata/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.0/guidata/tests/test_item_order.py
--rw-rw-rw-   0        0        0     1112 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_loadsave_hdf5.py
--rw-rw-rw-   0        0        0     1046 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/tests/test_loadsave_json.py
--rw-rw-rw-   0        0        0     1446 2023-07-06 14:15:35.000000 guidata-3.0.0/guidata/tests/test_objecteditor.py
--rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.0/guidata/tests/test_rotatedlabel.py
--rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.0/guidata/tests/test_text.py
--rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.0/guidata/tests/test_translations.py
--rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.0/guidata/tests/test_userconfig_app.py
--rw-rw-rw-   0        0        0    14759 2023-05-22 12:48:41.000000 guidata-3.0.0/guidata/userconfig.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.383872 guidata-3.0.0/guidata/utils/
--rw-rw-rw-   0        0        0     2868 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/utils/__init__.py
--rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.0/guidata/utils/disthelpers.py
--rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/utils/encoding.py
--rw-rw-rw-   0        0        0     2364 2023-07-06 12:05:00.000000 guidata-3.0.0/guidata/utils/genreqs.py
--rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.0/guidata/utils/gettext_helpers.py
--rw-rw-rw-   0        0        0     9067 2023-07-06 12:39:33.000000 guidata-3.0.0/guidata/utils/misc.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.419872 guidata-3.0.0/guidata/widgets/
--rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.0/guidata/widgets/__init__.py
--rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.0/guidata/widgets/arrayeditor.py
--rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.0/guidata/widgets/codeeditor.py
--rw-rw-rw-   0        0        0    55310 2023-06-30 12:28:15.000000 guidata-3.0.0/guidata/widgets/collectionseditor.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.451874 guidata-3.0.0/guidata/widgets/console/
--rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.0/guidata/widgets/console/__init__.py
--rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/console/base.py
--rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/console/calltip.py
--rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.0/guidata/widgets/console/dochelpers.py
--rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.0/guidata/widgets/console/internalshell.py
--rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.0/guidata/widgets/console/interpreter.py
--rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.0/guidata/widgets/console/mixins.py
--rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.0/guidata/widgets/console/shell.py
--rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/console/terminal.py
--rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/dataframeeditor.py
--rw-rw-rw-   0        0        0     3644 2023-07-06 12:41:23.000000 guidata-3.0.0/guidata/widgets/dockable.py
--rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/importwizard.py
--rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/nsview.py
--rw-rw-rw-   0        0        0     3351 2023-06-30 13:19:03.000000 guidata-3.0.0/guidata/widgets/objecteditor.py
--rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.0/guidata/widgets/rotatedlabel.py
--rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/syntaxhighlighters.py
--rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.0/guidata/widgets/texteditor.py
-drwxrwxrwx   0        0        0        0 2023-07-06 16:25:03.005872 guidata-3.0.0/guidata.egg-info/
--rw-rw-rw-   0        0        0     3359 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5585 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-06 16:25:02.000000 guidata-3.0.0/guidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       84 2023-07-06 15:51:24.000000 guidata-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1312 2023-07-06 16:25:04.088819 guidata-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.687090 guidata-3.0.1/
+-rw-rw-rw-   0        0        0     1563 2023-07-06 12:28:58.000000 guidata-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5248 2023-07-21 16:08:50.685076 guidata-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2234 2023-07-18 08:47:02.000000 guidata-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.272077 guidata-3.0.1/guidata/
+-rw-rw-rw-   0        0        0     3004 2023-07-07 13:55:43.000000 guidata-3.0.1/guidata/__init__.py
+-rw-rw-rw-   0        0        0    11296 2023-07-06 14:12:49.000000 guidata-3.0.1/guidata/config.py
+-rw-rw-rw-   0        0        0    13964 2023-07-19 16:04:51.000000 guidata-3.0.1/guidata/configtools.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.299077 guidata-3.0.1/guidata/dataset/
+-rw-rw-rw-   0        0        0      535 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/dataset/__init__.py
+-rw-rw-rw-   0        0        0    33518 2023-07-19 16:11:47.000000 guidata-3.0.1/guidata/dataset/dataitems.py
+-rw-rw-rw-   0        0        0    45137 2023-07-19 16:09:55.000000 guidata-3.0.1/guidata/dataset/datatypes.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.310080 guidata-3.0.1/guidata/dataset/io/
+-rw-rw-rw-   0        0        0     1702 2023-07-19 16:10:46.000000 guidata-3.0.1/guidata/dataset/io/__init__.py
+-rw-rw-rw-   0        0        0     5978 2023-07-19 09:51:48.000000 guidata-3.0.1/guidata/dataset/io/base.py
+-rw-rw-rw-   0        0        0    23319 2023-07-19 16:04:45.000000 guidata-3.0.1/guidata/dataset/io/h5fmt.py
+-rw-rw-rw-   0        0        0     5576 2023-07-19 10:06:28.000000 guidata-3.0.1/guidata/dataset/io/inifmt.py
+-rw-rw-rw-   0        0        0     8428 2023-07-19 09:51:48.000000 guidata-3.0.1/guidata/dataset/io/jsonfmt.py
+-rw-rw-rw-   0        0        0    40609 2023-07-18 14:45:16.000000 guidata-3.0.1/guidata/dataset/qtitemwidgets.py
+-rw-rw-rw-   0        0        0    23426 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/dataset/qtwidgets.py
+-rw-rw-rw-   0        0        0      820 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/dataset/textedit.py
+-rw-rw-rw-   0        0        0     6093 2023-07-06 12:40:25.000000 guidata-3.0.1/guidata/env.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.313093 guidata-3.0.1/guidata/external/
+-rw-rw-rw-   0        0        0        1 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.325077 guidata-3.0.1/guidata/external/darkdetect/
+-rw-rw-rw-   0        0        0     1289 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/__init__.py
+-rw-rw-rw-   0        0        0      377 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_dummy.py
+-rw-rw-rw-   0        0        0      890 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_linux_detect.py
+-rw-rw-rw-   0        0        0     2212 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_mac_detect.py
+-rw-rw-rw-   0        0        0     1257 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/external/darkdetect/_windows_detect.py
+-rw-rw-rw-   0        0        0   394832 2023-07-21 16:08:26.000000 guidata-3.0.1/guidata/guidata.chm
+-rw-rw-rw-   0        0        0    11214 2023-07-19 16:04:52.000000 guidata-3.0.1/guidata/guitest.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.408076 guidata-3.0.1/guidata/images/
+-rw-rw-rw-   0        0        0      785 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/apply.png
+-rw-rw-rw-   0        0        0     1123 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/arredit.png
+-rw-rw-rw-   0        0        0      721 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/busy.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/cell_edit.png
+-rw-rw-rw-   0        0        0      830 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/copy.png
+-rw-rw-rw-   0        0        0      722 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/delete.png
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/dictedit.png
+-rw-rw-rw-   0        0        0      735 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/dtype.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/edit.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.446075 guidata-3.0.1/guidata/images/editors/
+-rw-rw-rw-   0        0        0      911 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/copywop.png
+-rw-rw-rw-   0        0        0      929 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/edit.png
+-rw-rw-rw-   0        0        0     1001 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/edit_add.png
+-rw-rw-rw-   0        0        0     1777 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editclear.png
+-rw-rw-rw-   0        0        0     1048 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editcopy.png
+-rw-rw-rw-   0        0        0      824 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editcut.png
+-rw-rw-rw-   0        0        0     1453 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editdelete.png
+-rw-rw-rw-   0        0        0     1295 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/editpaste.png
+-rw-rw-rw-   0        0        0     2248 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/fileimport.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/filesave.png
+-rw-rw-rw-   0        0        0      727 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/imshow.png
+-rw-rw-rw-   0        0        0      525 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/insert.png
+-rw-rw-rw-   0        0        0      515 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/plot.png
+-rw-rw-rw-   0        0        0      689 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/rename.png
+-rw-rw-rw-   0        0        0     1184 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/editors/selectall.png
+-rw-rw-rw-   0        0        0     1164 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/exit.png
+-rw-rw-rw-   0        0        0      165 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/expander_down.png
+-rw-rw-rw-   0        0        0      432 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/expander_right.png
+-rw-rw-rw-   0        0        0      530 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/file.png
+-rw-rw-rw-   0        0        0     1424 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/fileclose.png
+-rw-rw-rw-   0        0        0     1556 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/fileimport.png
+-rw-rw-rw-   0        0        0      463 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filenew.png
+-rw-rw-rw-   0        0        0     1539 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/fileopen.png
+-rw-rw-rw-   0        0        0     1144 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filesave.png
+-rw-rw-rw-   0        0        0     1443 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filesaveas.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.518077 guidata-3.0.1/guidata/images/filetypes/
+-rw-rw-rw-   0        0        0     1601 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/doc.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/gif.png
+-rw-rw-rw-   0        0        0     1848 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/html.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/jpg.png
+-rw-rw-rw-   0        0        0     1543 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/pdf.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/png.png
+-rw-rw-rw-   0        0        0     1439 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/pps.png
+-rw-rw-rw-   0        0        0     1428 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/ps.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/tar.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/tgz.png
+-rw-rw-rw-   0        0        0     1512 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/tif.png
+-rw-rw-rw-   0        0        0     1801 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/txt.png
+-rw-rw-rw-   0        0        0     1237 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/xls.png
+-rw-rw-rw-   0        0        0     1577 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/filetypes/zip.png
+-rw-rw-rw-   0        0        0    16434 2023-07-06 15:03:14.000000 guidata-3.0.1/guidata/images/guidata-banner.svg
+-rw-rw-rw-   0        0        0    16406 2023-06-30 10:39:39.000000 guidata-3.0.1/guidata/images/guidata-vertical.svg
+-rw-rw-rw-   0        0        0    15818 2023-06-30 10:21:40.000000 guidata-3.0.1/guidata/images/guidata.svg
+-rw-rw-rw-   0        0        0      356 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/max.png
+-rw-rw-rw-   0        0        0      351 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/min.png
+-rw-rw-rw-   0        0        0      331 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/none.png
+-rw-rw-rw-   0        0        0      531 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/not_found.png
+-rw-rw-rw-   0        0        0      887 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/python.png
+-rw-rw-rw-   0        0        0      888 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/quickview.png
+-rw-rw-rw-   0        0        0     1599 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/save_all.png
+-rw-rw-rw-   0        0        0      744 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/selection.png
+-rw-rw-rw-   0        0        0     2445 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/settings.png
+-rw-rw-rw-   0        0        0      361 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/shape.png
+-rw-rw-rw-   0        0        0      354 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/xmax.png
+-rw-rw-rw-   0        0        0      353 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/images/xmin.png
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.224078 guidata-3.0.1/guidata/locale/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.225076 guidata-3.0.1/guidata/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.521093 guidata-3.0.1/guidata/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    10186 2023-06-29 17:09:10.000000 guidata-3.0.1/guidata/locale/fr/LC_MESSAGES/guidata.mo
+-rw-rw-rw-   0        0        0    20476 2023-07-19 16:01:55.000000 guidata-3.0.1/guidata/qthelpers.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.601078 guidata-3.0.1/guidata/tests/
+-rw-rw-rw-   0        0        0      368 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/tests/__init__.py
+-rw-rw-rw-   0        0        0     1709 2023-06-30 14:48:32.000000 guidata-3.0.1/guidata/tests/_all_tests.py
+-rw-rw-rw-   0        0        0      469 2023-07-18 14:57:07.000000 guidata-3.0.1/guidata/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.229076 guidata-3.0.1/guidata/tests/data/
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.606075 guidata-3.0.1/guidata/tests/data/genreqs/
+-rw-rw-rw-   0        0        0     2002 2023-07-21 12:09:05.000000 guidata-3.0.1/guidata/tests/data/genreqs/pyproject.toml
+-rw-rw-rw-   0        0        0     1493 2023-07-21 12:25:47.000000 guidata-3.0.1/guidata/tests/data/genreqs/setup.cfg
+-rw-rw-rw-   0        0        0     1724 2023-07-06 14:13:35.000000 guidata-3.0.1/guidata/tests/test_activable_dataset.py
+-rw-rw-rw-   0        0        0     1153 2023-07-06 14:13:43.000000 guidata-3.0.1/guidata/tests/test_activable_items.py
+-rw-rw-rw-   0        0        0     4858 2023-07-06 14:13:50.000000 guidata-3.0.1/guidata/tests/test_all_features.py
+-rw-rw-rw-   0        0        0     3577 2023-07-06 14:13:57.000000 guidata-3.0.1/guidata/tests/test_all_items.py
+-rw-rw-rw-   0        0        0     2601 2023-07-06 14:14:03.000000 guidata-3.0.1/guidata/tests/test_arrayeditor.py
+-rw-rw-rw-   0        0        0     1932 2023-07-06 14:14:10.000000 guidata-3.0.1/guidata/tests/test_bool_selector.py
+-rw-rw-rw-   0        0        0     2049 2023-07-06 14:14:16.000000 guidata-3.0.1/guidata/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      652 2023-07-06 14:14:23.000000 guidata-3.0.1/guidata/tests/test_codeeditor.py
+-rw-rw-rw-   0        0        0     3955 2023-07-18 15:13:56.000000 guidata-3.0.1/guidata/tests/test_collectionseditor.py
+-rw-rw-rw-   0        0        0     1068 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/tests/test_config.py
+-rw-rw-rw-   0        0        0      598 2023-07-06 14:14:35.000000 guidata-3.0.1/guidata/tests/test_console.py
+-rw-rw-rw-   0        0        0     1413 2023-07-06 14:14:42.000000 guidata-3.0.1/guidata/tests/test_data.py
+-rw-rw-rw-   0        0        0     2104 2023-07-18 14:56:56.000000 guidata-3.0.1/guidata/tests/test_dataframeeditor.py
+-rw-rw-rw-   0        0        0      869 2023-07-06 12:39:33.000000 guidata-3.0.1/guidata/tests/test_datasetgroup.py
+-rw-rw-rw-   0        0        0      962 2023-07-06 12:41:46.000000 guidata-3.0.1/guidata/tests/test_disthelpers.py
+-rw-rw-rw-   0        0        0     6052 2023-07-18 14:11:17.000000 guidata-3.0.1/guidata/tests/test_editgroupbox.py
+-rw-rw-rw-   0        0        0      839 2023-07-21 12:12:15.000000 guidata-3.0.1/guidata/tests/test_genreqs.py
+-rw-rw-rw-   0        0        0      779 2023-07-06 14:15:14.000000 guidata-3.0.1/guidata/tests/test_importwizard.py
+-rw-rw-rw-   0        0        0     1511 2023-07-06 14:15:21.000000 guidata-3.0.1/guidata/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     1321 2023-07-06 14:15:27.000000 guidata-3.0.1/guidata/tests/test_item_order.py
+-rw-rw-rw-   0        0        0     1108 2023-07-19 09:56:40.000000 guidata-3.0.1/guidata/tests/test_loadsave_hdf5.py
+-rw-rw-rw-   0        0        0     1042 2023-07-19 09:55:37.000000 guidata-3.0.1/guidata/tests/test_loadsave_json.py
+-rw-rw-rw-   0        0        0      714 2023-07-07 12:57:07.000000 guidata-3.0.1/guidata/tests/test_no_qt.py
+-rw-rw-rw-   0        0        0     1578 2023-07-18 15:02:08.000000 guidata-3.0.1/guidata/tests/test_objecteditor.py
+-rw-rw-rw-   0        0        0     1361 2023-07-06 14:15:41.000000 guidata-3.0.1/guidata/tests/test_rotatedlabel.py
+-rw-rw-rw-   0        0        0      818 2023-07-06 14:15:48.000000 guidata-3.0.1/guidata/tests/test_text.py
+-rw-rw-rw-   0        0        0      493 2023-07-06 12:40:58.000000 guidata-3.0.1/guidata/tests/test_translations.py
+-rw-rw-rw-   0        0        0      778 2023-06-29 14:26:00.000000 guidata-3.0.1/guidata/tests/test_userconfig_app.py
+-rw-rw-rw-   0        0        0    15176 2023-07-07 14:24:22.000000 guidata-3.0.1/guidata/userconfig.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.628077 guidata-3.0.1/guidata/utils/
+-rw-rw-rw-   0        0        0     2858 2023-07-19 16:04:50.000000 guidata-3.0.1/guidata/utils/__init__.py
+-rw-rw-rw-   0        0        0    43150 2023-07-06 12:41:24.000000 guidata-3.0.1/guidata/utils/disthelpers.py
+-rw-rw-rw-   0        0        0     6408 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/utils/encoding.py
+-rw-rw-rw-   0        0        0     6977 2023-07-21 12:45:00.000000 guidata-3.0.1/guidata/utils/genreqs.py
+-rw-rw-rw-   0        0        0     4025 2023-07-06 12:39:27.000000 guidata-3.0.1/guidata/utils/gettext_helpers.py
+-rw-rw-rw-   0        0        0    10494 2023-07-19 16:04:50.000000 guidata-3.0.1/guidata/utils/misc.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.661076 guidata-3.0.1/guidata/widgets/
+-rw-rw-rw-   0        0        0      729 2023-07-06 12:41:42.000000 guidata-3.0.1/guidata/widgets/__init__.py
+-rw-rw-rw-   0        0        0    33274 2023-06-30 13:14:39.000000 guidata-3.0.1/guidata/widgets/arrayeditor.py
+-rw-rw-rw-   0        0        0    13477 2023-06-30 14:48:54.000000 guidata-3.0.1/guidata/widgets/codeeditor.py
+-rw-rw-rw-   0        0        0    55677 2023-07-18 15:07:59.000000 guidata-3.0.1/guidata/widgets/collectionseditor.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.684075 guidata-3.0.1/guidata/widgets/console/
+-rw-rw-rw-   0        0        0     3257 2023-06-30 12:22:39.000000 guidata-3.0.1/guidata/widgets/console/__init__.py
+-rw-rw-rw-   0        0        0    59019 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/console/base.py
+-rw-rw-rw-   0        0        0    12513 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/console/calltip.py
+-rw-rw-rw-   0        0        0    11610 2023-06-30 15:04:24.000000 guidata-3.0.1/guidata/widgets/console/dochelpers.py
+-rw-rw-rw-   0        0        0    15411 2023-06-30 14:59:03.000000 guidata-3.0.1/guidata/widgets/console/internalshell.py
+-rw-rw-rw-   0        0        0    12585 2023-06-30 12:28:06.000000 guidata-3.0.1/guidata/widgets/console/interpreter.py
+-rw-rw-rw-   0        0        0    30662 2023-06-30 12:40:32.000000 guidata-3.0.1/guidata/widgets/console/mixins.py
+-rw-rw-rw-   0        0        0    33285 2023-07-06 14:15:58.000000 guidata-3.0.1/guidata/widgets/console/shell.py
+-rw-rw-rw-   0        0        0     4099 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/console/terminal.py
+-rw-rw-rw-   0        0        0    32563 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/dataframeeditor.py
+-rw-rw-rw-   0        0        0     3614 2023-07-19 16:00:45.000000 guidata-3.0.1/guidata/widgets/dockable.py
+-rw-rw-rw-   0        0        0    24121 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/importwizard.py
+-rw-rw-rw-   0        0        0    23460 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/nsview.py
+-rw-rw-rw-   0        0        0     3533 2023-07-19 16:04:51.000000 guidata-3.0.1/guidata/widgets/objecteditor.py
+-rw-rw-rw-   0        0        0     2122 2023-07-06 12:41:23.000000 guidata-3.0.1/guidata/widgets/rotatedlabel.py
+-rw-rw-rw-   0        0        0    62527 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/syntaxhighlighters.py
+-rw-rw-rw-   0        0        0     4022 2023-04-28 09:36:06.000000 guidata-3.0.1/guidata/widgets/texteditor.py
+drwxrwxrwx   0        0        0        0 2023-07-21 16:08:50.285075 guidata-3.0.1/guidata.egg-info/
+-rw-rw-rw-   0        0        0     5248 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4841 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 16:08:50.000000 guidata-3.0.1/guidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1957 2023-07-21 16:08:07.000000 guidata-3.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 16:08:50.688087 guidata-3.0.1/setup.cfg
```

### Comparing `guidata-3.0.0/LICENSE` & `guidata-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/PKG-INFO` & `guidata-3.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,18 @@
-Metadata-Version: 2.1
-Name: guidata
-Version: 3.0.0
-Summary: Signal and image processing software
-Home-page: https://github.com/CODRA-Ingenierie-Informatique/guidata/
-Author: Codra
-Author-email: p.raybaut@codra.fr
-License: BSD 3-Clause License
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <4,>=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: doc
-License-File: LICENSE
-
 # guidata: Automatic GUI generation for easy dataset editing and display with Python
 
 [![license](https://img.shields.io/pypi/l/guidata.svg)](./LICENSE)
 [![pypi version](https://img.shields.io/pypi/v/guidata.svg)](https://pypi.org/project/guidata/)
 [![PyPI status](https://img.shields.io/pypi/status/guidata.svg)](https://github.com/CODRA-Ingenierie-Informatique/guidata/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/guidata.svg)](https://pypi.python.org/pypi/guidata/)
 [![download count](https://img.shields.io/conda/dn/conda-forge/guidata.svg)](https://www.anaconda.com/download/)
 
 Simple example of ``guidata`` datasets embedded in an application window:
 
-<img src="https://raw.githubusercontent.com/PierreRaybaut/guidata/master/doc/images/screenshots/editgroupbox.png">
+<img src="https://raw.githubusercontent.com/CODRA-Ingenierie-Informatique/guidata/master/doc/images/screenshots/editgroupbox.png">
 
 See [documentation](https://guidata.readthedocs.io/en/latest/) for more details on
 the library and [changelog](CHANGELOG.md) for recent history of changes.
 
 Copyrights and licensing:
 
 * Copyright © 2023 [CEA](https://www.cea.fr), [Codra](https://codra.net/), [Pierre Raybaut](https://github.com/PierreRaybaut).
```

### Comparing `guidata-3.0.0/guidata/__init__.py` & `guidata-3.0.1/guidata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 =======
 
 Based on the Qt library :mod:`guidata` is a Python library generating graphical
 user interfaces for easy dataset editing and display. It also provides helpers
 and application development tools for Qt.
 """
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 
 
 # Dear (Debian, RPM, ...) package makers, please feel free to customize the
 # following path to module's data (images) and translations:
 DATAPATH = LOCALEPATH = ""
```

### Comparing `guidata-3.0.0/guidata/config.py` & `guidata-3.0.1/guidata/config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/configtools.py` & `guidata-3.0.1/guidata/configtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def get_module_data_path(modname: str, relpath: str | None = None) -> str:
     """Return module *modname* data path
     Handles py2exe/cx_Freeze distributions
 
     Args:
         modname (str): module name
-        relpath (str, optional): relative path to module data directory
+        relpath (str): relative path to module data directory
 
     Returns:
         str: module data path
     """
     datapath = getattr(sys.modules[modname], "DATAPATH", "")
     if not datapath:
         datapath = get_module_path(modname)
@@ -80,15 +80,15 @@
 
 
 def get_translation(modname: str, dirname: str | None = None) -> Callable[[str], str]:
     """Return translation callback for module *modname*
 
     Args:
         modname (str): module name
-        dirname (str, optional): module directory
+        dirname (str): module directory
 
     Returns:
         Callable[[str], str]: translation callback
     """
     if dirname is None:
         dirname = modname
     # fixup environment var LANG in case it's unknown
@@ -142,15 +142,15 @@
 
 
 def add_image_path(path: str, subfolders: bool = True) -> None:
     """Append image path (opt. with its subfolders) to global list IMG_PATH
 
     Args:
         path (str): image path
-        subfolders (bool, optional): include subfolders
+        subfolders (bool): include subfolders
     """
     if not isinstance(path, str):
         path = decode_fs_string(path)
     global IMG_PATH
     IMG_PATH.append(path)
     if subfolders:
         for fileobj in os.listdir(path):
@@ -167,27 +167,27 @@
 
     modname must be the name of an already imported module as found in
     sys.modules
 
     Args:
         modname (str): module name
         relpath (str): relative path to module data directory
-        subfolders (bool, optional): include subfolders
+        subfolders (bool): include subfolders
     """
     add_image_path(get_module_data_path(modname, relpath=relpath), subfolders)
 
 
 def get_image_file_path(name: str, default: str = "not_found.png") -> str:
     """
     Return the absolute path to image with specified name
     name, default: filenames with extensions
 
     Args:
         name (str): name of the image
-        default (str, optional): default image name. Defaults to "not_found.png".
+        default (str): default image name. Defaults to "not_found.png".
 
     Raises:
         RuntimeError: if image file not found
 
     Returns:
         str: absolute path to image
     """
@@ -210,15 +210,15 @@
 def get_icon(name: str, default: str = "not_found.png") -> QG.QIcon:
     """
     Construct a QIcon from the file with specified name
     name, default: filenames with extensions
 
     Args:
         name (str): name of the icon
-        default (str, optional): default icon name. Defaults to "not_found.png".
+        default (str): default icon name. Defaults to "not_found.png".
 
     Returns:
         QG.QIcon: icon
     """
     try:
         return ICON_CACHE[name]
     except KeyError:
@@ -233,15 +233,15 @@
 def get_image_label(name, default="not_found.png") -> QW.QLabel:
     """
     Construct a QLabel from the file with specified name
     name, default: filenames with extensions
 
     Args:
         name (str): name of the icon
-        default (str, optional): default icon name. Defaults to "not_found.png".
+        default (str): default icon name. Defaults to "not_found.png".
 
     Returns:
         QW.QLabel: label
     """
     # Importing Qt here because this module should be independent from it
     from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
     from qtpy import QtWidgets as QW  # pylint: disable=import-outside-toplevel
@@ -257,17 +257,17 @@
 ) -> tuple[QW.QHBoxLayout, QW.QLabel]:
     """
     Construct a QHBoxLayout including image from the file with specified name,
     left-aligned text [with specified tooltip]
 
     Args:
         imagename (str): name of the icon
-        text (str, optional): text to display. Defaults to "".
-        tooltip (str, optional): tooltip to display. Defaults to "".
-        alignment (QC.Qt.Alignment, optional): alignment of the text. Defaults to None.
+        text (str): text to display. Defaults to "".
+        tooltip (str): tooltip to display. Defaults to "".
+        alignment (QC.Qt.Alignment): alignment of the text. Defaults to None.
 
     Returns:
         tuple[QW.QHBoxLayout, QW.QLabel]: layout, label
     """
     # Importing Qt here because this module should be independent from it
     from qtpy import QtCore as QC  # pylint: disable=import-outside-toplevel
     from qtpy import QtWidgets as QW  # pylint: disable=import-outside-toplevel
@@ -343,15 +343,15 @@
     Construct a QFont from the specified configuration file entry
     conf: UserConfig instance
     section [, option]: configuration entry
 
     Args:
         conf (UserConfig): UserConfig instance
         section (str): configuration entry
-        option (str, optional): configuration entry. Defaults to "".
+        option (str): configuration entry. Defaults to "".
 
     Returns:
         QG.QFont: font
     """
     # Importing Qt here because this module should be independent from it
     from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
 
@@ -398,18 +398,18 @@
     [color]: default color
     [width]: default width
     [style]: default style
 
     Args:
         conf (UserConfig): UserConfig instance
         section (str): configuration entry
-        option (str, optional): configuration entry. Defaults to "".
-        color (str, optional): default color. Defaults to "black".
-        width (int, optional): default width. Defaults to 1.
-        style (str, optional): default style. Defaults to "SolidLine".
+        option (str): configuration entry. Defaults to "".
+        color (str): default color. Defaults to "black".
+        width (int): default width. Defaults to 1.
+        style (str): default style. Defaults to "SolidLine".
 
     Returns:
         QG.QPen: pen
     """
     # Importing Qt here because this module should be independent from it
     from qtpy import QtCore as QC  # pylint: disable=import-outside-toplevel
     from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
@@ -437,17 +437,17 @@
     section [, option]: configuration entry
     [color]: default color
     [alpha]: default alpha-channel
 
     Args:
         conf (UserConfig): UserConfig instance
         section (str): configuration entry
-        option (str, optional): configuration entry. Defaults to "".
-        color (str, optional): default color. Defaults to "black".
-        alpha (float, optional): default alpha-channel. Defaults to 1.0.
+        option (str): configuration entry. Defaults to "".
+        color (str): default color. Defaults to "black".
+        alpha (float): default alpha-channel. Defaults to 1.0.
 
     Returns:
         QG.QBrush: brush
     """
     # Importing Qt here because this module should be independent from it
     from qtpy import QtGui as QG  # pylint: disable=import-outside-toplevel
```

### Comparing `guidata-3.0.0/guidata/dataset/__init__.py` & `guidata-3.0.1/guidata/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/dataset/dataitems.py` & `guidata-3.0.1/guidata/dataset/dataitems.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 # Licensed under the terms of the BSD 3-Clause
 # (see guidata/LICENSE for details)
 
 """
 Data items
 ----------
 
+Base class
+^^^^^^^^^^
+
+.. autoclass:: DataItem
+
 Numeric items
 ^^^^^^^^^^^^^
 
 .. autoclass:: FloatItem
     :members:
 
 .. autoclass:: IntItem
@@ -82,57 +87,59 @@
 .. autoclass:: DictItem
     :members:
 
 .. autoclass:: FontFamilyItem
     :members:
 """
 
-import collections.abc
+from __future__ import annotations
+
 import datetime
 import os
 import re
-from typing import TYPE_CHECKING, Any, Callable, List, Optional, Tuple, Type, Union
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any
+
+from numpy import ndarray
 
 from guidata.config import _
 from guidata.dataset.datatypes import DataItem, DataSet, ItemProperty
-from guidata.dataset.iniio import UserConfigReader, UserConfigWriter
-from guidata.qthelpers import exec_dialog
-from numpy import ndarray
+from guidata.dataset.io import INIReader, INIWriter
 
 if TYPE_CHECKING:  # pragma: no cover
-    from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
-    from guidata.dataset.jsonio import JSONReader, JSONWriter
+    from guidata.dataset.io import HDF5Reader, HDF5Writer, JSONReader, JSONWriter
 
 
 class NumericTypeItem(DataItem):
-    """
-    Numeric data item
-    * label [string]: name
-    * default [int]: default value (optional)
-    * min [int]: minimum value (optional)
-    * max [int]: maximum value (optional)
-    * nonzero [bool]: if True, zero is not a valid value (optional)
-    * unit [string]: physical unit (optional)
-    * even [bool]: if True, even values are valid, if False,
-        odd values are valid if None (default), ignored (optional)
-    * slider [bool]: if True, shows a slider widget right after the line
-        edit widget (default is False)
-    * help [string]: text shown in tooltip (optional)
-    * check [bool]: if False, value is not checked (optional, default=True)
+    """Numeric data item
+
+    Args:
+        label (str): item name
+        default (int or float): default value (optional)
+        min (int or float): minimum value (optional)
+        max (int or float): maximum value (optional)
+        nonzero (bool): if True, zero is not a valid value (optional)
+        unit (str): physical unit (optional)
+        even (bool): if True, even values are valid, if False,
+          odd values are valid if None (default), ignored (optional)
+        slider (bool): if True, shows a slider widget right after the line
+          edit widget (default is False)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     type: Callable = None
 
     def __init__(
         self,
         label: str,
-        default: Optional[Union[float, int]] = None,
-        min: Optional[Union[float, int]] = None,
-        max: Optional[Union[float, int]] = None,
-        nonzero: Optional[bool] = None,
+        default: float | int | None = None,
+        min: float | int | None = None,
+        max: float | int | None = None,
+        nonzero: bool | None = None,
         unit: str = "",
         help: str = "",
         check: bool = True,
     ) -> None:
         DataItem.__init__(self, label, default=default, help=help)
         self.set_prop("data", min=min, max=max, nonzero=nonzero, check_value=check)
         self.set_prop("display", unit=unit)
@@ -153,26 +160,26 @@
         if nonzero:
             auto_help += ", " + _("non zero")
         if unit:
             auto_help += ", %s %s" % (_("unit:"), unit)
         return auto_help
 
     def format_string(
-        self, instance: "DataSet", value: Union[float, int], fmt: str, func: Callable
+        self, instance: DataSet, value: float | int, fmt: str, func: Callable
     ) -> str:
         """Override DataItem method"""
         text = fmt % (func(value),)
         # We add directly the unit to 'text' (instead of adding it
         # to 'fmt') to avoid string formatting error if '%' is in unit
         unit = self.get_prop_value("display", instance, "unit", "")
         if unit:
             text += " " + unit
         return text
 
-    def check_value(self, value: Union[float, int]) -> bool:
+    def check_value(self, value: float | int) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         if self.get_prop("data", "nonzero") and value == 0:
             return False
@@ -182,50 +189,54 @@
                 return False
         _max = self.get_prop("data", "max")
         if _max is not None:
             if value > _max:
                 return False
         return True
 
-    def from_string(self, value: str) -> Optional[Any]:
+    def from_string(self, value: str) -> Any | None:
         """Override DataItem method"""
         # String may contains numerical operands:
         if re.match(r"^([\d\(\)\+/\-\*.]|e)+$", value):
+            # pylint: disable=eval-used
+            # pylint: disable=broad-except
             try:
                 return self.type(eval(value))
-            except:
+            except:  # noqa
                 pass
         return None
 
 
 class FloatItem(NumericTypeItem):
-    """
-    Construct a float data item
-        * label [string]: name
-        * default [float]: default value (optional)
-        * min [float]: minimum value (optional)
-        * max [float]: maximum value (optional)
-        * slider [bool]: if True, shows a slider widget right after the line
-          edit widget (default is False)
-        * step [float]: step between tick values with a slider widget (optional)
-        * nonzero [bool]: if True, zero is not a valid value (optional)
-        * unit [string]: physical unit (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a float data item
+
+    Args:
+        label (str): item name
+        default (float): default value (optional)
+        min (float): minimum value (optional)
+        max (float): maximum value (optional)
+        nonzero (bool): if True, zero is not a valid value (optional)
+        unit (str): physical unit (optional)
+        even (bool): if True, even values are valid, if False,
+         odd values are valid if None (default), ignored (optional)
+        slider (bool): if True, shows a slider widget right after the line
+         edit widget (default is False)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     type = float
 
     def __init__(
         self,
         label: str,
-        default: Optional[float] = None,
-        min: Optional[float] = None,
-        max: Optional[float] = None,
-        nonzero: Optional[bool] = None,
+        default: float | None = None,
+        min: float | None = None,
+        max: float | None = None,
+        nonzero: bool | None = None,
         unit: str = "",
         step: float = 0.1,
         slider: bool = False,
         help: str = "",
         check: bool = True,
     ) -> None:
         super().__init__(
@@ -238,49 +249,50 @@
             help=help,
             check=check,
         )
         self.set_prop("display", slider=slider)
         self.set_prop("data", step=step)
 
     def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+        self, reader: HDF5Reader | JSONReader | INIReader
     ) -> float:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_float()
 
 
 class IntItem(NumericTypeItem):
-    """
-    Construct an integer data item
-        * label [string]: name
-        * default [int]: default value (optional)
-        * min [int]: minimum value (optional)
-        * max [int]: maximum value (optional)
-        * nonzero [bool]: if True, zero is not a valid value (optional)
-        * unit [string]: physical unit (optional)
-        * even [bool]: if True, even values are valid, if False,
-          odd values are valid if None (default), ignored (optional)
-        * slider [bool]: if True, shows a slider widget right after the line
-          edit widget (default is False)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct an integer data item
+
+    Args:
+        label (str): item name
+        default (int): default value (optional)
+        min (int): minimum value (optional)
+        max (int): maximum value (optional)
+        nonzero (bool): if True, zero is not a valid value (optional)
+        unit (str): physical unit (optional)
+        even (bool): if True, even values are valid, if False,
+         odd values are valid if None (default), ignored (optional)
+        slider (bool): if True, shows a slider widget right after the line
+         edit widget (default is False)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     type = int
 
     def __init__(
         self,
         label: str,
-        default: Optional[int] = None,
-        min: Optional[int] = None,
-        max: Optional[int] = None,
-        nonzero: Optional[bool] = None,
+        default: int | None = None,
+        min: int | None = None,
+        max: int | None = None,
+        nonzero: bool | None = None,
         unit: str = "",
-        even: Optional[bool] = None,
+        even: bool | None = None,
         slider: bool = False,
         help: str = "",
         check: bool = True,
     ) -> None:
         super().__init__(
             label,
             default=default,
@@ -290,15 +302,15 @@
             unit=unit,
             help=help,
             check=check,
         )
         self.set_prop("data", even=even)
         self.set_prop("display", slider=slider)
 
-    def get_auto_help(self, instance: "DataSet") -> str:
+    def get_auto_help(self, instance: DataSet) -> str:
         """Override DataItem method"""
         auto_help = super().get_auto_help(instance)
         even = self.get_prop_value("data", instance, "even")
         if even is not None:
             if even:
                 auto_help += ", " + _("even")
             else:
@@ -315,39 +327,38 @@
         even = self.get_prop("data", "even")
         if even is not None:
             is_even = value // 2 == value / 2.0
             if (even and not is_even) or (not even and is_even):
                 return False
         return True
 
-    def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> Any:
+    def get_value_from_reader(self, reader: HDF5Reader | JSONReader | INIReader) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_int()
 
 
 class StringItem(DataItem):
-    """
-    Construct a string data item
-        * label [string]: name
-        * default [string]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * notempty [bool]: if True, empty string is not a valid value (opt.)
-        * wordwrap [bool]: toggle word wrapping (optional)
+    """Construct a string data item
+
+    Args:
+        label (str): item name
+        default (str): default value (optional)
+        notempty (bool): if True, empty string is not a valid value (optional)
+        wordwrap (bool): toggle word wrapping (optional)
+        help (str): text shown in tooltip (optional)
     """
 
     type: Any = str
 
     def __init__(
         self,
         label: str,
-        default: Optional[str] = None,
-        notempty: Optional[bool] = None,
+        default: str | None = None,
+        notempty: bool | None = None,
         wordwrap: bool = False,
         help: str = "",
     ) -> None:
         DataItem.__init__(self, label, default=default, help=help)
         self.set_prop("data", notempty=notempty)
         self.set_prop("display", wordwrap=wordwrap)
 
@@ -358,166 +369,180 @@
             return False
         return True
 
     def from_string(self, value: str) -> str:
         """Override DataItem method"""
         return value
 
-    def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> Any:
+    def get_value_from_reader(self, reader: HDF5Reader | JSONReader | INIReader) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_unicode()
 
 
 class TextItem(StringItem):
-    """
-    Construct a text data item (multiline string)
-        * label [string]: name
-        * default [string]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * notempty [bool]: if True, empty string is not a valid value (opt.)
-        * wordwrap [bool]: toggle word wrapping (optional)
+    """Construct a text data item (multiline string)
+
+    Args:
+        label (str): item name
+        default (str): default value (optional)
+        notempty (bool): if True, empty string is not a valid value (optional)
+        wordwrap (bool): toggle word wrapping (optional)
+        help (str): text shown in tooltip (optional)
     """
 
     def __init__(
         self,
         label: str,
-        default: Optional[str] = None,
-        notempty: Optional[bool] = None,
+        default: str | None = None,
+        notempty: bool | None = None,
         wordwrap: bool = True,
         help: str = "",
     ) -> None:
         StringItem.__init__(
             self,
             label,
             default=default,
             notempty=notempty,
             wordwrap=wordwrap,
             help=help,
         )
 
 
 class BoolItem(DataItem):
-    """
-    Construct a boolean data item
-        * text [string]: form's field name (optional)
-        * label [string]: name
-        * default [string]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a boolean data item
+
+    Args:
+        text (str): form's field name (optional)
+        label (str): item name
+        default (bool): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     type = bool
 
     def __init__(
         self,
         text: str = "",
         label: str = "",
-        default: Optional[bool] = None,
+        default: bool | None = None,
         help: str = "",
         check: bool = True,
     ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("display", text=text)
 
     def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
+        self, reader: HDF5Reader | JSONReader | INIReader
     ) -> bool:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_bool()
 
 
 class DateItem(DataItem):
-    """
-    Construct a date data item.
-        * text [string]: form's field name (optional)
-        * label [string]: name
-        * default [datetime.date]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
+    """DataSet data item
+
+    Args:
+        label (str): item label
+        default (datetime.date): default value (optional)
+        format (str): date format (as in :py:func:`datetime.date.strftime`)
+        help (str): text displayed on data item's tooltip
+        check (bool): check value (default: True)
     """
 
     type = datetime.date
 
+    def __init__(
+        self,
+        label: str,
+        default: datetime.date | None = None,
+        format: str | None = None,
+        help: str | None = "",
+        check: bool | None = True,
+    ) -> None:
+        DataItem.__init__(self, label, default=default, help=help, check=check)
+        self.set_prop("display", format=format)
+
 
 class DateTimeItem(DateItem):
-    """
-    Construct a date time data item.
-        * text [string]: form's field name (optional)
-        * label [string]: name
-        * default [datetime.date]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
+    """DataSet data item
+
+    Args:
+        label (str): item label
+        default (datetime.datetime): default value (optional)
+        format (str): date format (as in :py:func:`datetime.date.strftime`)
+        help (str): text displayed on data item's tooltip
+        check (bool): check value (default: True)
     """
 
     pass
 
 
 class ColorItem(StringItem):
-    """
-    Construct a color data item
-        * label [string]: name
-        * default [string]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a color data item
 
-    Color values are encoded as hexadecimal strings or Qt color names
+    Args:
+        label (str): item name
+        default (str): default value (optional). Color can be specified as
+         a string (e.g. "#FF0000" or "red") or as a Qt name (e.g. "red")
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         from guidata.qthelpers import text_to_qcolor
 
         return text_to_qcolor(value).isValid()
 
-    def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> str:
+    def get_value_from_reader(self, reader: HDF5Reader | JSONReader | INIReader) -> str:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         # Using read_str converts `numpy.string_` to `str` -- otherwise,
         # when passing the string to a QColor Qt object, any numpy.string_ will
         # be interpreted as no color (black)
         return reader.read_str()
 
 
 class FileSaveItem(StringItem):
-    """
-    Construct a path data item for a file to be saved
-        * label [string]: name
-        * formats [string (or string list)]: wildcard filter
-        * default [string]: default value (optional)
-        * basedir [string]: default base directory (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a path data item for a file to be saved
+
+    Args:
+        label (str): item name
+        formats (str or list of str): wildcard filter
+        default (str): default value (optional)
+        basedir (str): default base directory (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def __init__(
         self,
         label: str,
-        formats: Union[Tuple[str, ...], str] = "*",
-        default: Optional[Union[List[str], str]] = None,
-        basedir: Optional[str] = None,
+        formats: tuple[str, ...] | str = "*",
+        default: list[str] | str | None = None,
+        basedir: str | None = None,
         all_files_first: bool = False,
         help: str = "",
         check: bool = True,
     ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         if isinstance(formats, str):
             formats = [formats]  # type:ignore
         self.set_prop("data", formats=formats)
         self.set_prop("data", basedir=basedir)
         self.set_prop("data", all_files_first=all_files_first)
 
-    def get_auto_help(self, instance: "DataSet") -> str:
+    def get_auto_help(self, instance: DataSet) -> str:
         """Override DataItem method"""
         formats = self.get_prop("data", "formats")
         return (
             _("all file types")
             if formats == ["*"]
             else _("supported file types:") + " *.%s" % ", *.".join(formats)
         )
@@ -542,52 +567,54 @@
         if len(formats) == 1 and formats[0] != "*":
             if not value.endswith("." + formats[0]) and len(value) > 0:
                 return value + "." + formats[0]
         return value
 
 
 class FileOpenItem(FileSaveItem):
-    """
-    Construct a path data item for a file to be opened
-        * label [string]: name
-        * formats [string (or string list)]: wildcard filter
-        * default [string]: default value (optional)
-        * basedir [string]: default base directory (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a path data item for a file to be opened
+
+    Args:
+        label (str): item name
+        formats (str or list of str): wildcard filter
+        default (str): default value (optional)
+        basedir (str): default base directory (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
             return False
         return os.path.exists(value) and os.path.isfile(value)
 
 
 class FilesOpenItem(FileSaveItem):
-    """
-    Construct a path data item for multiple files to be opened.
-        * label [string]: name
-        * formats [string (or string list)]: wildcard filter
-        * default [string]: default value (optional)
-        * basedir [string]: default base directory (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a path data item for multiple files to be opened.
+
+    Args:
+        label (str): item name
+        formats (str or list of str): wildcard filter
+        default (str): default value (optional)
+        basedir (str): default base directory (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     type = list
 
     def __init__(
         self,
         label: str,
         formats: str = "*",
-        default: Optional[Union[List[str], str]] = None,
-        basedir: Optional[str] = None,
+        default: list[str] | str | None = None,
+        basedir: str | None = None,
         all_files_first: bool = False,
         help: str = "",
         check: bool = True,
     ) -> None:
         if isinstance(default, str):
             default = [default]
         FileSaveItem.__init__(
@@ -608,46 +635,47 @@
         if value is None:
             return False
         allexist = True
         for path in value:
             allexist = allexist and os.path.exists(path) and os.path.isfile(path)
         return allexist
 
-    def from_string(self, value: Any) -> List[str]:  # type:ignore
+    def from_string(self, value: Any) -> list[str]:  # type:ignore
         """Override DataItem method"""
         if value.endswith("']") or value.endswith('"]'):
             value = eval(value)
         else:
             value = [value]
         return [self.add_extension(path) for path in value]
 
     def serialize(
         self,
-        instance: "DataSet",
-        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+        instance: DataSet,
+        writer: HDF5Writer | JSONWriter | INIWriter,
     ) -> None:
         """Serialize this item"""
         value = self.get_value(instance)
         writer.write_sequence([fname.encode("utf-8") for fname in value])
 
     def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> List[str]:
+        self, reader: HDF5Reader | JSONReader | INIReader
+    ) -> list[str]:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return [fname for fname in reader.read_sequence()]
 
 
 class DirectoryItem(StringItem):
-    """
-    Construct a path data item for a directory.
-        * label [string]: name
-        * default [string]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a path data item for a directory.
+
+    Args:
+        label (str): item name
+        default (str): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def check_value(self, value: str) -> bool:
         """Override DataItem method"""
         if not self.get_prop("data", "check_value", True):
             return True
         if not isinstance(value, self.type):
@@ -661,91 +689,91 @@
     is the first item.
     """
 
     pass
 
 
 class ChoiceItem(DataItem):
-    """
-    Construct a data item for a list of choices.
-        * label [string]: name
-        * choices [list, tuple or function]: string list or (key, label) list
-          function of two arguments (item, value) returning a list of tuples
-          (key, label, image) where image is an icon path, a QIcon instance
-          or a function of one argument (key) returning a QIcon instance
-        * default [-]: default label or default key (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
-        * radio [bool]: if True, shows radio buttons instead of a combo box
-          (default is False)
+    """Construct a data item for a list of choices.
+
+    Args:
+        label (str): item name
+        choices (list, tuple or Callable): string list or (key, label) list
+         function of two arguments (item, value) returning a list of tuples
+         (key, label, image) where image is an icon path, a QIcon instance
+         or a function of one argument (key) returning a QIcon instance
+        default (str): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
+        radio (bool): if True, shows radio buttons instead of a combo box
+         (default is False)
     """
 
     def __init__(
         self,
         label: str,
         choices: Any,
-        default: Optional[Union[Tuple[()], Type[FirstChoice], int]] = FirstChoice,
+        default: tuple[()] | type[FirstChoice] | int | None = FirstChoice,
         help: str = "",
         check: bool = True,
         radio: bool = False,
     ) -> None:
         _choices_data: Any
-        if isinstance(choices, collections.abc.Callable):  # type:ignore
+        if isinstance(choices, Callable):
             _choices_data = ItemProperty(choices)
         else:
             _choices_data = []
             for idx, choice in enumerate(choices):
                 _choices_data.append(self._normalize_choice(idx, choice))
-        if default is FirstChoice and not isinstance(
-            choices, collections.abc.Callable  # type:ignore
-        ):
+        if default is FirstChoice and not isinstance(choices, Callable):
             default = _choices_data[0][0]
         elif default is FirstChoice:
             default = None
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("data", choices=_choices_data)
         self.set_prop("display", radio=radio)
 
     def _normalize_choice(
-        self, idx: int, choice_tuple: Tuple[Any, ...]
-    ) -> Union[Tuple[int, str, None], Tuple[str, str, None]]:
+        self, idx: int, choice_tuple: tuple[Any, ...]
+    ) -> tuple[int, str, None] | tuple[str, str, None]:
         if isinstance(choice_tuple, tuple):
             key, value = choice_tuple
         else:
             key = idx
             value = choice_tuple
         return (key, value, None)
 
-    def get_string_value(self, instance: "DataSet") -> str:
+    def get_string_value(self, instance: DataSet) -> str:
         """Override DataItem method"""
         value = self.get_value(instance)
         choices = self.get_prop_value("data", instance, "choices")
         # print "ShowChoiceWidget:", choices, value
         for choice in choices:
             if choice[0] == value:
                 return str(choice[1])
         else:
             return DataItem.get_string_value(self, instance)
 
 
 class MultipleChoiceItem(ChoiceItem):
-    """
-    Construct a data item for a list of choices -- multiple choices can be selected
-        * label [string]: name
-        * choices [list or tuple]: string list or (key, label) list
-        * default [-]: default label or default key (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a data item for a list of choices -- multiple choices can be selected
+
+    Args:
+        label (str): item name
+        choices (list or tuple): string list or (key, label) list
+        default (str): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def __init__(
         self,
         label: str,
-        choices: List[str],
-        default: Tuple[()] = (),
+        choices: list[str],
+        default: tuple[()] = (),
         help: str = "",
         check: bool = True,
     ) -> None:
         ChoiceItem.__init__(self, label, choices, default, help, check=check)
         self.set_prop("display", shape=(1, -1))
 
     def horizontal(self, row_nb: int = 1) -> "MultipleChoiceItem":
@@ -766,29 +794,29 @@
         nb = MultipleChoiceItem("Number", ['1', '2', '3'] ).vertical(2)
         """
         self.set_prop("display", shape=(-1, col_nb))
         return self
 
     def serialize(
         self,
-        instance: "DataSet",
-        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+        instance: DataSet,
+        writer: HDF5Writer | JSONWriter | INIWriter,
     ) -> None:
         """Serialize this item"""
         value = self.get_value(instance)
         seq = []
         _choices = self.get_prop_value("data", instance, "choices")
         for key, _label, _img in _choices:
             seq.append(key in value)
         writer.write_sequence(seq)
 
     def deserialize(
         self,
-        instance: "DataSet",
-        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+        instance: DataSet,
+        reader: HDF5Reader | JSONReader | INIReader,
     ) -> None:
         """Deserialize this item"""
         try:
             flags = reader.read_sequence()
         except KeyError:
             self.set_default(instance)
         else:
@@ -799,67 +827,68 @@
             for idx, flag in enumerate(flags):
                 if flag:
                     value.append(_choices[idx][0])
             self.__set__(instance, value)
 
 
 class ImageChoiceItem(ChoiceItem):
-    """
-    Construct a data item for a list of choices with images
-        * label [string]: name
-        * choices [list, tuple or function]: (label, image) list or
-          (key, label, image) list function of two arguments (item, value)
-          returning a list of tuples (key, label, image) where image is an
-          icon path, a QIcon instance or a function of one argument (key)
-          returning a QIcon instance
-        * default [-]: default label or default key (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a data item for a list of choices with images
+
+    Args:
+        label (str): item name
+        choices (list or tuple): (label, image) list, or (key, label, image) list,
+         or function of two arguments (item, value) returning a list of tuples
+         (key, label, image) where image is an icon path, a QIcon instance or
+         a function of one argument (key) returning a QIcon instance
+        default (str): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def _normalize_choice(
-        self, idx: int, choice_tuple: Tuple[Any, ...]
-    ) -> Tuple[Any, Any, Any]:
+        self, idx: int, choice_tuple: tuple[Any, ...]
+    ) -> tuple[Any, Any, Any]:
         assert isinstance(choice_tuple, tuple)
         if len(choice_tuple) == 3:
             key, value, img = choice_tuple
         else:
             key = idx
             value, img = choice_tuple
         return (key, value, img)
 
 
 class FloatArrayItem(DataItem):
-    """
-    Construct a float array data item
-        * label [string]: name
-        * default [numpy.ndarray]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * format [string]: formatting string (example: '%.3f') (optional)
-        * transpose [bool]: transpose matrix (display only)
-        * large [bool]: view all float of the array
-        * minmax [string]: "all" (default), "columns", "rows"
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a float array data item
+
+    Args:
+        label (str): item name
+        default (numpy.ndarray): default value (optional)
+        help (str): text shown in tooltip (optional)
+        format (str): formatting string (example: '%.3f') (optional)
+        transpose (bool): transpose matrix (display only)
+        large (bool): view all float of the array
+        minmax (str): "all" (default), "columns", "rows"
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def __init__(
         self,
         label: str,
-        default: Optional[ndarray] = None,
+        default: ndarray | None = None,
         help: str = "",
         format: str = "%.3f",
         transpose: bool = False,
         minmax: str = "all",
         check: bool = True,
     ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("display", format=format, transpose=transpose, minmax=minmax)
 
     def format_string(
-        self, instance: "DataSet", value: Any, fmt: str, func: Callable
+        self, instance: DataSet, value: Any, fmt: str, func: Callable
     ) -> str:
         """Override DataItem method"""
         larg = self.get_prop_value("display", instance, "large", False)
         fmt = self.get_prop_value("display", instance, "format", "%s")
         unit = self.get_prop_value("display", instance, "unit", "")
         v = func(value)
         if larg:
@@ -873,123 +902,137 @@
             text += " .. " + fmt % v.max()
             text += "]"
         text += " %s" % unit
         return str(text)
 
     def serialize(
         self,
-        instance: "DataSet",
-        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+        instance: DataSet,
+        writer: HDF5Writer | JSONWriter | INIWriter,
     ) -> None:
         """Serialize this item"""
         value = self.get_value(instance)
         writer.write_array(value)
 
-    def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> Any:
+    def get_value_from_reader(self, reader: HDF5Reader | JSONReader | INIReader) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method"""
         return reader.read_array()
 
 
 class ButtonItem(DataItem):
-    """
-    Construct a simple button that calls a method when hit
-        * label [string]: text shown on the button
-        * callback [function]: function with four parameters (dataset, item, value, parent)
-            - dataset [DataSet]: instance of the parent dataset
-            - item [DataItem]: instance of ButtonItem (i.e. self)
-            - value [unspecified]: value of ButtonItem (default ButtonItem
-              value or last value returned by the callback)
-            - parent [QObject]: button's parent widget
-        * icon [QIcon or string]: icon show on the button (optional)
-          (string: icon filename as in guidata/guiqwt image search paths)
-        * default [unspecified]: default value passed to the callback (optional)
-        * help [string]: text shown in button's tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a simple button that calls a method when hit
+
+    Args:
+        label (str): item name
+        callback (Callable): function with four parameters (dataset, item, value,
+         parent) where dataset (DataSet) is an instance of the parent dataset,
+         item (DataItem) is an instance of ButtonItem (i.e. self), value (unspecified)
+         is the value of ButtonItem (default ButtonItem value or last value returned
+         by the callback) and parent (QObject) is button's parent widget
+        icon (QIcon or str): icon show on the button (optional)
+         (str: icon filename as in guidata/guiqwt image search paths)
+        default (Any): default value passed to the callback (optional)
+        help (str): text shown in button's tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
 
     The value of this item is unspecified but is passed to the callback along
     with the whole dataset. The value is assigned the callback`s return value.
     """
 
     def __init__(
         self,
         label: str,
         callback: Callable,
-        icon: Optional[str] = None,
-        default: Optional[Any] = None,
+        icon: str | None = None,
+        default: Any | None = None,
         help: str = "",
         check: bool = True,
     ) -> None:
         DataItem.__init__(self, label, default=default, help=help, check=check)
         self.set_prop("display", callback=callback)
         self.set_prop("display", icon=icon)
 
     def serialize(
         self,
-        instance: "DataSet",
-        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+        instance: DataSet,
+        writer: HDF5Writer | JSONWriter | INIWriter,
     ) -> Any:
         pass
 
     def deserialize(
         self,
-        instance: "DataSet",
-        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+        instance: DataSet,
+        reader: HDF5Reader | JSONReader | INIReader,
     ) -> Any:
         pass
 
 
+def dictedit(
+    instance: DataSet, item: DataItem, value: Any, parent: object
+) -> Any:  # pylint: disable=unused-argument
+    """Edit a dictionary value using a dialog box
+
+    Args:
+        instance (DataSet): dataset instance
+        item (DataItem): item instance
+        value (Any): item value
+        parent (object): parent widget
+    """
+    # Importing those modules here avoids Qt dependency when
+    # guidata is used without Qt
+    # pylint: disable=import-outside-toplevel
+    from guidata.qthelpers import exec_dialog
+    from guidata.widgets.collectionseditor import CollectionsEditor
+
+    editor = CollectionsEditor(parent)
+    value_was_none = value is None
+    if value_was_none:
+        value = {}
+    editor.setup(value)
+    if exec_dialog(editor):
+        return editor.get_value()
+    else:
+        if value_was_none:
+            return
+        return value
+
+
 class DictItem(ButtonItem):
-    """
-    Construct a dictionary data item
-        * label [string]: name
-        * default [dict]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
-        * check [bool]: if False, value is not checked (optional, default=True)
+    """Construct a dictionary data item
+
+    Args:
+        label (str): item name
+        default (dict): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     def __init__(
         self,
         label: str,
-        default: Optional[dict] = None,
+        default: dict | None = None,
         help: str = "",
         check: bool = True,
     ) -> None:
-        def dictedit(
-            instance: "DataSet", item: "DataItem", value: Any, parent: object
-        ) -> Any:
-            from guidata.widgets.collectionseditor import CollectionsEditor
-
-            editor = CollectionsEditor(parent)
-            value_was_none = value is None
-            if value_was_none:
-                value = {}
-            editor.setup(value)
-            if exec_dialog(editor):
-                return editor.get_value()
-            else:
-                if value_was_none:
-                    return
-                return value
-
         ButtonItem.__init__(
             self,
             label,
             dictedit,
             icon="dictedit.png",
             default=default,
             help=help,
             check=check,
         )
 
 
 class FontFamilyItem(StringItem):
-    """
-    Construct a font family name item
-        * label [string]: name
-        * default [string]: default value (optional)
-        * help [string]: text shown in tooltip (optional)
+    """Construct a font family name item
+
+    Args:
+        label (str): item name
+        default (str): default value (optional)
+        help (str): text shown in tooltip (optional)
+        check (bool): if False, value is not checked (optional, default=True)
     """
 
     pass
```

### Comparing `guidata-3.0.0/guidata/dataset/datatypes.py` & `guidata-3.0.1/guidata/dataset/datatypes.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
 .. autoclass:: EndTabGroup
     :members:
 
 Handling item properties
 ^^^^^^^^^^^^^^^^^^^^^^^^
 
+.. autoclass:: ItemProperty
+
 .. autoclass:: FormatProp
     :members:
 
 .. autoclass:: GetAttrProp
     :members:
 
 .. autoclass:: ValueProp
@@ -52,82 +54,89 @@
 .. autoclass:: FuncProp
     :members:
 """
 
 # pylint: disable-msg=W0622
 # pylint: disable-msg=W0212
 
-import collections.abc
+from __future__ import annotations
+
 import re
 import sys
 from abc import abstractmethod
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-)
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any
 
-from guidata.dataset.iniio import UserConfigReader, UserConfigWriter
-from guidata.qthelpers import exec_dialog
+from guidata.dataset.io import INIReader, INIWriter
 from guidata.userconfig import UserConfig
 from guidata.utils import update_dataset
-from qtpy.QtWidgets import QWidget
 
 DEBUG_DESERIALIZE = False
 
 if TYPE_CHECKING:  # pragma: no cover
-    from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
-    from guidata.dataset.jsonio import JSONReader, JSONWriter
+    from qtpy.QtWidgets import QWidget
+
+    from guidata.dataset.io import HDF5Reader, HDF5Writer, JSONReader, JSONWriter
     from guidata.dataset.qtwidgets import DataSetEditDialog
 
 
 class NoDefault:
     pass
 
 
 class ItemProperty:
+    """Base class for item properties
+
+    Args:
+        callable (Callable): callable to use to evaluate the value of the property
+    """
+
     def __init__(self, callable: Callable) -> None:
         self.callable = callable
 
-    def __call__(self, instance: "DataSet", item: Any, value: Any) -> Any:
+    def __call__(self, instance: DataSet, item: Any, value: Any) -> Any:
         """Evaluate the value of the property given, the instance,
         the item and the value maintained in the instance by the item"""
         return self.callable(instance, item, value)
 
-    def set(self, instance: "DataSet", item: Any, value: Any) -> Any:
+    def set(self, instance: DataSet, item: Any, value: Any) -> Any:
         """Sets the value of the property given an instance, item and value
         Depending on implementation the value will be stored either on the
         instance, item or self
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            item (Any): item to set the value of
+            value (Any): value to set
         """
         raise NotImplementedError
 
 
 FMT_GROUPS = re.compile(r"(?<!%)%\((\w+)\)")
 
 
 class FormatProp(ItemProperty):
     """A Property that returns a string to help
-    custom read-only representation of items"""
+    custom read-only representation of items
 
-    def __init__(self, fmt: str, ignore_error: Optional[bool] = True) -> None:
+    Args:
+        fmt (str): format string
+        ignore_error (bool): ignore errors when formatting. Defaults to True.
+    """
+
+    def __init__(self, fmt: str, ignore_error: bool | None = True) -> None:
         """fmt is a format string
         it can contain a single anonymous substition or
         several named substitions.
         """
         self.fmt = fmt
         self.ignore_error = ignore_error
         self.attrs = FMT_GROUPS.findall(fmt)
 
-    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
+    def __call__(self, instance: DataSet, item: DataItem, value: Any) -> Any:
         if not self.attrs:
             return self.fmt.format(value)
         dic = {}
         for attr in self.attrs:
             dic[attr] = getattr(instance, attr)
         try:
             return self.fmt % dic
@@ -135,310 +144,450 @@
             if not self.ignore_error:
                 print("Wrong Format for %s : %r %% %r" % (item._name, self.fmt, dic))
                 raise
 
 
 class GetAttrProp(ItemProperty):
     """A property that matches the value of
-    an instance's attribute"""
+    an instance's attribute
+
+    Args:
+        attr (str): attribute to match
+    """
 
     def __init__(self, attr: str) -> None:
         self.attr = attr
 
-    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
+    def __call__(self, instance: DataSet, item: DataItem, value: Any) -> Any:
         val = getattr(instance, self.attr)
         return val
 
-    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
+    def set(self, instance: DataSet, item: DataItem, value: Any) -> None:
         setattr(instance, self.attr, value)
 
 
 class ValueProp(ItemProperty):
-    """A property that retrieves a value stored elsewhere"""
+    """A property that retrieves a value stored elsewhere
+
+    Args:
+        value (Any): value to store
+    """
 
     def __init__(self, value: Any) -> None:
         self.value = value
 
-    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
+    def __call__(self, instance: DataSet, item: DataItem, value: Any) -> Any:
         return self.value
 
-    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
+    def set(self, instance: DataSet, item: DataItem, value: Any) -> None:
+        """Sets the value of the property given an instance, item and value
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            item (Any): item to set the value of
+            value (Any): value to set
+        """
         self.value = value
 
 
 class NotProp(ItemProperty):
-    """Not property"""
+    """Not property
+
+    Args:
+        prop (ItemProperty): property to negate
+    """
 
     def __init__(self, prop: ItemProperty):
         self.property = prop
 
-    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
+    def __call__(self, instance: DataSet, item: DataItem, value: Any) -> Any:
         return not self.property(instance, item, value)
 
-    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
+    def set(self, instance: DataSet, item: DataItem, value: Any) -> None:
+        """Sets the value of the property given an instance, item and value
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            item (Any): item to set the value of
+            value (Any): value to set
+        """
         self.property.set(instance, item, not value)
 
 
 class FuncProp(ItemProperty):
     """An 'operator property'
-    prop: ItemProperty instance
-    func: function
-    invfunc: inverse function (optional)
+
+    Args:
+        prop (ItemProperty): property to apply function to
+        func (function): function to apply
+        invfunc (function): inverse function (default: func)
     """
 
     def __init__(
         self,
         prop: ItemProperty,
         func: Callable,
-        invfunc: Optional[Callable] = None,
+        invfunc: Callable | None = None,
     ) -> None:
         self.property = prop
         self.function = func
         if invfunc is None:
             invfunc = func
         self.inverse_function = invfunc
 
-    def __call__(self, instance: "DataSet", item: "DataItem", value: Any) -> Any:
+    def __call__(self, instance: DataSet, item: DataItem, value: Any) -> Any:
         return self.function(self.property(instance, item, value))
 
-    def set(self, instance: "DataSet", item: "DataItem", value: Any) -> None:
+    def set(self, instance: DataSet, item: DataItem, value: Any) -> None:
+        """Sets the value of the property given an instance, item and value
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            item (Any): item to set the value of
+            value (Any): value to set
+        """
         self.property.set(instance, item, self.inverse_function(value))
 
 
 class DataItem:
-    """
-    DataSet data item
+    """DataSet data item
 
-    `label` : string
-    `default` : any type, optional
-    `help` : string Text displayed on data item's tooltip
+    Args:
+        label (str): item label
+        default (Any): default value
+        help (str): text displayed on data item's tooltip
+        check (bool): check value (default: True)
     """
 
     count = 0
 
     def __init__(
         self,
         label: str,
-        default: Optional[Any] = None,
-        help: Optional[str] = "",
-        check: Optional[bool] = True,
+        default: Any | None = None,
+        help: str | None = "",
+        check: bool | None = True,
     ) -> None:
         self._order = DataItem.count
         DataItem.count += 1
-        self._name: Optional[str] = None
+        self._name: str | None = None
         self._default = default
         self._help = help
-        self._props: Dict[
+        self._props: dict[
             Any, Any
         ] = {}  # a dict realm->dict containing realm-specific properties
         self.set_prop("display", col=0, colspan=None, row=None, label=label)
         self.set_prop("data", check_value=check)
 
     def get_prop(self, realm: str, name: str, default: Any = NoDefault) -> Any:
-        """Get one property of this item"""
+        """Get one property of this item
+
+        Args:
+            realm (str): realm name
+            name (str): property name
+            default (Any): default value (default: NoDefault)
+
+        Returns:
+            Any: property value
+        """
         prop = self._props.get(realm)
         if not prop:
             prop = {}
         if default is NoDefault:
             return prop[name]
         return prop.get(name, default)
 
     def get_prop_value(
-        self, realm: str, instance: "DataSet", name: str, default: Any = NoDefault
+        self, realm: str, instance: DataSet, name: str, default: Any = NoDefault
     ) -> Any:
+        """Get one property of this item
+
+        Args:
+            realm (str): realm name
+            instance (DataSet): instance of the DataSet
+            name (str): property name
+            default (Any): default value (default: NoDefault)
+
+        Returns:
+            Any: property value
+        """
         value = self.get_prop(realm, name, default)
         if isinstance(value, ItemProperty):
             return value(instance, self, self.get_value(instance))
         else:
             return value
 
-    def set_prop(self, realm: str, **kwargs) -> "DataItem":
-        """Set one or several properties using
-        the syntax set_prop(name1=value1, ..., nameX=valueX)
+    def set_prop(self, realm: str, **kwargs) -> DataItem:
+        """Set one or several properties using the syntax::
 
-        it returns self so that we can assign to the result like this:
+            set_prop(name1=value1, ..., nameX=valueX)
 
-        item = Item().set_prop(x=y)
-        """
+        It returns self so that we can assign to the result like this::
+
+            item = Item().set_prop(x=y)
+
+        Args:
+            realm (str): realm name
+            \*\*kwargs: properties to set
+
+        Returns:
+            DataItem: self
+        """  # noqa
         prop = self._props.get(realm)
         if not prop:
             prop = {}
             self._props[realm] = prop
         prop.update(kwargs)
         return self
 
     def set_pos(
-        self, col: int = 0, colspan: Optional[int] = None, row: Optional[int] = None
-    ) -> "DataItem":
-        """
-        Set data item's position on a GUI layout
+        self, col: int = 0, colspan: int | None = None, row: int | None = None
+    ) -> DataItem:
+        """Set data item's position on a GUI layout
+
+        Args:
+            col (int): column number (default: 0)
+            colspan (int): number of columns (default: None)
+            row (int): row number (default: None)
         """
         self.set_prop("display", col=col, colspan=colspan, row=row)
         return self
 
     def __str__(self) -> str:
         return "%s : %s" % (self._name, self.__class__.__name__)
 
-    def get_help(self, instance: "DataSet") -> str:
-        """
-        Return data item's tooltip
+    def get_help(self, instance: DataSet) -> str:
+        """Return data item's tooltip
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            str: tooltip
         """
         auto_help = self.get_auto_help(instance)
         help = self._help
         if auto_help:
             if help:
                 help = help + "\n(" + auto_help + ")"
             else:
                 help = auto_help.capitalize()
         return help
 
-    def get_auto_help(self, instance: "DataSet") -> str:
-        """
-        Return the automatically generated part of data item's tooltip
+    def get_auto_help(self, instance: DataSet) -> str:
+        """Return the automatically generated part of data item's tooltip
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            str: automatically generated part of tooltip
         """
         return ""
 
     def format_string(self, instance: Any, value: Any, fmt: str, func: Callable) -> str:
-        """Apply format to string representation of the item's value"""
-        return fmt % (func(value),)
+        """Apply format to string representation of the item's value
+
+        Args:
+            instance (Any): instance of the DataSet
+            value (Any): item's value
+            fmt (str): format string
+            func (Callable): function to apply to the value before formatting
 
-    def get_string_value(self, instance: "DataSet") -> str:
+        Returns:
+            str: formatted string
         """
-        Return a formatted unicode representation of the item's value
+        return fmt % (func(value),)
+
+    def get_string_value(self, instance: DataSet) -> str:
+        """Return a formatted unicode representation of the item's value
         obeying 'display' or 'repr' properties
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            str: formatted string
         """
         value = self.get_value(instance)
         repval = self.get_prop_value("display", instance, "repr", None)
         if repval is not None:
             return repval
         else:
             fmt = self.get_prop_value("display", instance, "format", "%s")
+            fmt = "%s" if fmt is None else fmt
             func = self.get_prop_value("display", instance, "func", lambda x: x)
             if (
-                isinstance(fmt, collections.abc.Callable)  # type:ignore
+                isinstance(fmt, Callable)  # type:ignore
                 and value is not None
             ):
                 return fmt(func(value))
             if value is not None:
                 text = self.format_string(instance, value, fmt, func)
             else:
                 text = ""
             return text
 
     def set_name(self, new_name: str) -> None:
-        """
-        Set data item's name
+        """Set data item's name
+
+        Args:
+            new_name (str): new name
         """
         self._name = new_name
 
     def set_help(self, new_help: str) -> None:
-        """
-        Set data item's help text
+        """Set data item's help text
+
+        Args:
+            new_help (str): new help text
         """
         self._help = new_help
 
-    def set_from_string(self, instance: "DataSet", string_value: str) -> None:
-        """
-        Set data item's value from specified string
+    def set_from_string(self, instance: DataSet, string_value: str) -> None:
+        """Set data item's value from specified string
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            string_value (str): string value
         """
         value = self.from_string(string_value)
         self.__set__(instance, value)
 
-    def set_default(self, instance: "DataSet") -> None:
-        """
-        Set data item's value to default
+    def set_default(self, instance: DataSet) -> None:
+        """Set data item's value to default
+
+        Args:
+            instance (DataSet): instance of the DataSet
         """
         self.__set__(instance, self._default)
 
     def accept(self, visitor: object) -> None:
-        """
-        This is the visitor pattern's accept function.
+        """This is the visitor pattern's accept function.
         It calls the corresponding visit_MYCLASS method
         of the visitor object.
 
         Python's allow a generic base class implementation of
         this method so there's no need to write an accept function
         for each derived class unless you need to override the
         default behavior
+
+        Args:
+            visitor (object)
         """
         funcname = "visit_" + self.__class__.__name__
         func = getattr(visitor, funcname)
         func(self)
 
     def __set__(self, instance: Any, value: Any):
         setattr(instance, "_%s" % (self._name), value)
 
-    def __get__(self, instance: Any, klass: type) -> Optional[Any]:
+    def __get__(self, instance: Any, klass: type) -> Any | None:
         if instance is not None:
             return getattr(instance, "_%s" % (self._name), self._default)
         else:
             return self
 
     def get_value(self, instance: Any) -> Any:
-        """
-        Return data item's value
+        """Return data item's value
+
+        Args:
+            instance (Any): instance of the DataSet
+
+        Returns:
+            Any: data item's value
         """
         return self.__get__(instance, instance.__class__)
 
     def check_item(self, instance: Any) -> Any:
-        """
-        Check data item's current value (calling method check_value)
+        """Check data item's current value (calling method check_value)
+
+        Args:
+            instance (Any): instance of the DataSet
+
+        Returns:
+            Any: data item's value
         """
         value = getattr(instance, "_%s" % (self._name))
         return self.check_value(value)
 
     def check_value(self, value: Any) -> Any:
-        """
-        Check if `value` is valid for this data item
+        """Check if `value` is valid for this data item
+
+        Args:
+            value (Any): value to check
+
+        Returns:
+            Any: value
         """
         raise NotImplementedError()
 
     def from_string(self, string_value: str) -> Any:
-        """
-        Transform string into valid data item's value
+        """Transform string into valid data item's value
+
+        Args:
+            string_value (str): string value
+
+        Returns:
+            Any: data item's value
         """
         raise NotImplementedError()
 
-    def bind(self, instance: "DataSet") -> "DataItemVariable":
-        """
-        Return a DataItemVariable instance bound to the data item
+    def bind(self, instance: DataSet) -> DataItemVariable:
+        """Return a DataItemVariable instance bound to the data item
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            DataItemVariable: DataItemVariable instance
         """
         return DataItemVariable(self, instance)
 
     def serialize(
         self,
-        instance: "DataSet",
-        writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"],
+        instance: DataSet,
+        writer: HDF5Writer | JSONWriter | INIWriter,
     ) -> None:
         """Serialize this item using the writer object
 
-        this is a default implementation that should work for
+        This is a default implementation that should work for
         everything but new datatypes
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            writer (HDF5Writer | JSONWriter | INIWriter): writer object
         """
         value = self.get_value(instance)
         writer.write(value)
 
-    def get_value_from_reader(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> Any:
+    def get_value_from_reader(self, reader: HDF5Reader | JSONReader | INIReader) -> Any:
         """Reads value from the reader object, inside the try...except
         statement defined in the base item `deserialize` method
 
-        This method is reimplemented in some child classes"""
+        This method is reimplemented in some child classes
+
+        Args:
+            reader (HDF5Reader | JSONReader | INIReader): reader object
+        """
         return reader.read_any()
 
     def deserialize(
         self,
         instance: Any,
-        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+        reader: HDF5Reader | JSONReader | INIReader,
     ) -> None:
         """Deserialize this item using the reader object
 
         Default base implementation supposes the reader can
         detect expected datatype from the stream
+
+        Args:
+            instance (Any): instance of the DataSet
+            reader (HDF5Reader | JSONReader | INIReader): reader object
         """
         try:
             value = self.get_value_from_reader(reader)
         except KeyError:
             self.set_default(instance)
             return
         except RuntimeError as e:
@@ -461,202 +610,372 @@
         self.__dict__.update(kwargs)
 
 
 class ObjectItem(DataItem):
     """Simple helper class implementing default
     for composite objects"""
 
-    klass: Optional[Type] = None
+    klass: type | None = None
 
-    def set_default(self, instance: "DataSet") -> None:
-        """Make a copy of the default value"""
+    def set_default(self, instance: DataSet) -> None:
+        """Make a copy of the default value
+
+        Args:
+            instance (DataSet): instance of the DataSet
+        """
         if self.klass is not None:
             value = self.klass()
             if self._default is not None:
                 update_dataset(value, self._default)
             self.__set__(instance, value)
 
     def deserialize(
         self,
-        instance: "DataSet",
-        reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"],
+        instance: DataSet,
+        reader: HDF5Reader | JSONReader | INIReader,
     ) -> None:
         """Deserialize this item using the reader object
 
         We build a new default object and deserialize it
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            reader (HDF5Reader | JSONReader | INIReader): reader object
         """
         if self.klass is not None:
             value = self.klass()
             value.deserialize(reader)
             self.__set__(instance, value)
 
 
 class DataItemProxy:
     """
     Proxy for DataItem objects
 
     This class is needed to construct GroupItem class
     (see module guidata.qtwidgets)
+
+    Args:
+        item (DataItem): data item to proxy
     """
 
-    def __init__(self, item: "DataItem"):
+    def __init__(self, item: DataItem):
         self.item = item
 
     def __str__(self):
         return self.item._name + "_proxy: " + self.__class__.__name__
 
-    def get_help(self, instance: "DataSet") -> str:
-        """DataItem method proxy"""
+    def get_help(self, instance: DataSet) -> str:
+        """DataItem method proxy
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            str: help string
+        """
         return self.item.get_help(instance)
 
-    def get_auto_help(self, instance: "DataSet") -> str:
-        """DataItem method proxy"""
+    def get_auto_help(self, instance: DataSet) -> str:
+        """DataItem method proxy
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            str: help string
+        """
         return self.item.get_auto_help(instance)
 
-    def get_string_value(self, instance: "DataSet") -> str:
-        """DataItem method proxy"""
+    def get_string_value(self, instance: DataSet) -> str:
+        """DataItem method proxy
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            str: string value
+        """
         return self.item.get_string_value(instance)
 
-    def set_from_string(self, instance: "DataSet", string_value: str) -> None:
-        """DataItem method proxy"""
+    def set_from_string(self, instance: DataSet, string_value: str) -> None:
+        """DataItem method proxy
+
+        Args:
+            instance (DataSet): instance of the DataSet
+            string_value (str): string value
+        """
         self.item.set_from_string(instance, string_value)
 
-    def set_default(self, instance: "DataSet") -> None:
-        """DataItem method proxy"""
+    def set_default(self, instance: DataSet) -> None:
+        """DataItem method proxy
+
+        Args:
+            instance (DataSet): instance of the DataSet
+        """
         self.item.set_default(instance)
 
     def __set__(self, instance: Any, value: Any):
         pass
 
-    def accept(self, visitor: "object") -> None:
-        """DataItem method proxy"""
+    def accept(self, visitor: object) -> None:
+        """DataItem method proxy
+
+        Args:
+            visitor (object): visitor object
+        """
         self.item.accept(visitor)
 
-    def get_value(self, instance: "DataItem") -> Any:
-        """DataItem method proxy"""
+    def get_value(self, instance: DataItem) -> Any:
+        """DataItem method proxy
+
+        Args:
+            instance (DataItem): instance of the DataItem
+
+        Returns:
+            Any: value
+        """
         return self.item.get_value(instance)
 
-    def check_item(self, instance: "DataItem") -> Any:
-        """DataItem method proxy"""
+    def check_item(self, instance: DataItem) -> Any:
+        """DataItem method proxy
+
+        Args:
+            instance (DataItem): instance of the DataItem
+
+        Returns:
+            Any: value
+        """
         return self.item.check_item(instance)
 
     def check_value(self, value: Any) -> Any:
-        """DataItem method proxy"""
+        """DataItem method proxy
+
+        Args:
+            value (Any): value
+
+        Returns:
+            Any: value
+        """
         return self.item.check_value(value)
 
     def from_string(self, string_value: str) -> Any:
-        """DataItem method proxy"""
+        """DataItem method proxy
+
+        Args:
+            string_value (str): string value
+
+        Returns:
+            Any: value
+        """
         return self.item.from_string(string_value)
 
     def get_prop(self, realm: str, name: str, default=NoDefault) -> Any:
-        """DataItem method proxy"""
+        """DataItem method proxy
+
+        Args:
+            realm (str): realm
+            name (str): name
+            default (Any): default value
+
+        Returns:
+            Any: value
+        """
         return self.item.get_prop(realm, name, default)
 
     def get_prop_value(
-        self, realm, instance: "DataSet", name: str, default: Any = NoDefault
+        self, realm, instance: DataSet, name: str, default: Any = NoDefault
     ) -> Any:
-        """DataItem method proxy"""
+        """DataItem method proxy
+
+        Args:
+            realm (str): realm
+            instance (DataSet): instance of the DataSet
+            name (str): name
+            default (Any): default value
+
+        Returns:
+            Any: value
+        """
         return self.item.get_prop_value(realm, instance, name, default)
 
-    def set_prop(self, realm: str, **kwargs) -> "DataItem":
-        """DataItem method proxy"""
+    def set_prop(self, realm: str, **kwargs) -> DataItem:
+        """DataItem method proxy
+
+        Args:
+            realm (str): realm
+            \*\*kwargs: keyword arguments
+
+        Returns:
+            DataItem: data item
+        """  # noqa
         return self.item.set_prop(realm, **kwargs)
 
-    def bind(self, instance: "DataSet") -> "DataItemVariable":
-        """DataItem method proxy"""
+    def bind(self, instance: DataSet) -> DataItemVariable:
+        """DataItem method proxy
+
+        Args:
+            instance (DataSet): instance of the DataSet
+
+        Returns:
+            DataItemVariable: data item variable
+        """
         return DataItemVariable(self, instance)
 
 
 class DataItemVariable:
     """An instance of a DataItemVariable represent a binding between
     an item and a dataset.
 
     could be called a bound property.
 
     since DataItem instances are class attributes they need to have a
     DataSet instance to store their value. This class binds the two
     together.
+
+    Args:
+        item (DataItem): data item
+        instance (DataSet): instance of the DataSet
     """
 
     def __init__(
         self,
-        item: "DataItem",
-        instance: "DataSet",
+        item: DataItem,
+        instance: DataSet,
     ):
         self.item = item
         self.instance = instance
 
     def get_prop_value(self, realm: str, name: str, default: object = NoDefault) -> Any:
-        """DataItem method proxy"""
+        """DataItem method proxy
+
+        Args:
+            realm (str): realm
+            name (str): name
+            default (object): default value
+
+        Returns:
+            Any: value
+        """
         return self.item.get_prop_value(realm, self.instance, name, default)
 
-    def get_prop(
-        self, realm: str, name: str, default: Optional[type] = NoDefault
-    ) -> Any:
-        """DataItem method proxy"""
+    def get_prop(self, realm: str, name: str, default: type | None = NoDefault) -> Any:
+        """DataItem method proxy
+
+        Args:
+            realm (str): realm
+            name (str): name
+            default (type | None): default value
+
+        Returns:
+            Any: value
+        """
         return self.item.get_prop(realm, name, default)
 
     def get_help(self) -> str:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Returns:
+            str: help string
+        """
         return self.item.get_help(self.instance)
 
     def get_auto_help(self) -> str:
-        """Re-implement DataItem method"""
-        # XXX incohérent ?
+        """Re-implement DataItem method
+
+        Returns:
+            str: help string
+        """
         return self.item.get_auto_help(self.instance)
 
     def get_string_value(self) -> str:
-        """
-        Return a unicode representation of the item's value
+        """Return a unicode representation of the item's value
         obeying 'display' or 'repr' properties
+
+        Returns:
+            str: string value
         """
         return self.item.get_string_value(self.instance)
 
     def set_default(self) -> None:
         """Re-implement DataItem method"""
         return self.item.set_default(self.instance)
 
     def get(self) -> Any:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Returns:
+            Any: value
+        """
         return self.item.get_value(self.instance)
 
     def set(self, value: Any) -> None:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Args:
+            value (Any): value
+        """
         return self.item.__set__(self.instance, value)
 
     def set_from_string(self, string_value) -> None:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Args:
+            string_value (str): string value
+        """
         return self.item.set_from_string(self.instance, string_value)
 
     def check_item(self) -> Any:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Returns:
+            Any: value
+        """
         return self.item.check_item(self.instance)
 
     def check_value(self, value) -> Any:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Args:
+            value (Any): value
+
+        Returns:
+            Any: value
+        """
         return self.item.check_value(value)
 
     def from_string(self, string_value: str) -> Any:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Args:
+            string_value (str): string value
+
+        Returns:
+            Any: value
+        """
         return self.item.from_string(string_value)
 
     def label(self) -> str:
-        """Re-implement DataItem method"""
+        """Re-implement DataItem method
+
+        Returns:
+            str: label
+        """
         return self.item.get_prop("display", "label")
 
 
 class DataSetMeta(type):
     """
     DataSet metaclass
 
     Create class attribute `_items`: list of the DataSet class attributes,
     created in the same order as these attributes were written
     """
 
-    def __new__(cls: Type, name: str, bases: Any, dct: Dict[str, Any]) -> Type:
+    def __new__(cls: type, name: str, bases: Any, dct: dict[str, Any]) -> type:
         items = {}
         for base in bases:
             if getattr(base, "__metaclass__", None) is DataSetMeta:
                 for item in base._items:
                     items[item._name] = item
 
         for attrname, value in list(dct.items()):
@@ -671,29 +990,29 @@
         return type.__new__(cls, name, bases, dct)
 
 
 Meta_Py3Compat = DataSetMeta("Meta_Py3Compat", (object,), {})
 
 
 class DataSet(metaclass=DataSetMeta):
-    """
-    Construct a DataSet object is a set of DataItem objects
-        * title [string]
-        * comment [string]: text shown on the top of the first data item
-        * icon [QIcon or string]: icon show on the button (optional)
-          (string: icon filename as in guidata/guiqwt image search paths)
+    """Construct a DataSet object is a set of DataItem objects
+
+    Args:
+        title (str): title
+        comment (str): comment. Text shown on the top of the first data item
+        icon (str): icon filename as in image search paths
     """
 
-    _items: List["DataItem"]
+    _items: list[DataItem]
     __metaclass__ = DataSetMeta  # keep it even with Python 3 (see DataSetMeta)
 
     def __init__(
         self,
-        title: Optional[str] = None,
-        comment: Optional[str] = None,
+        title: str | None = None,
+        comment: str | None = None,
         icon: str = "",
     ):
         self.__comment = comment
         self.__icon = icon
         comp_title, comp_comment = self._compute_title_and_comment()
         if title:
             self.__title = title
@@ -702,23 +1021,23 @@
         if comment is None:
             self.__comment = comp_comment
         self.__changed = False
         # Set default values
         self.set_defaults()
 
     @classmethod
-    def create(cls, **kwargs) -> "DataSet":
+    def create(cls, **kwargs) -> DataSet:
         """Create a new instance of the DataSet class
 
         Args:
             \*\*kwargs: keyword arguments to set the DataItem values
 
         Returns:
             DataSet instance
-        """
+        """  # noqa
         instance = cls()
         for item in instance._items:
             name = item._name
             if name in kwargs:
                 setattr(instance, name, kwargs[name])
         return instance
 
@@ -731,15 +1050,15 @@
         """
         module = sys.modules[self.__class__.__module__]
         if hasattr(module, "_"):
             return module._
         else:
             return lambda x: x
 
-    def _compute_title_and_comment(self) -> Tuple[str, Optional[str]]:
+    def _compute_title_and_comment(self) -> tuple[str, str | None]:
         """
         Private method to compute title and comment of the data set
         """
         comp_title = self.__class__.__name__
         comp_comment = None
         if self.__doc__:
             doc_lines = self.__doc__.splitlines()
@@ -749,97 +1068,127 @@
             if doc_lines:
                 comp_title = doc_lines.pop(0).strip()
             if doc_lines:
                 comp_comment = "\n".join([x.strip() for x in doc_lines])
         return comp_title, comp_comment
 
     def get_title(self) -> str:
-        """
-        Return data set title
+        """Return data set title
+
+        Returns:
+            str: title
         """
         return self.__title
 
-    def get_comment(self) -> Optional[str]:
-        """
-        Return data set comment
+    def get_comment(self) -> str | None:
+        """Return data set comment
+
+        Returns:
+            str | None: comment
         """
         return self.__comment
 
-    def get_icon(self) -> Optional[str]:
-        """
-        Return data set icon
+    def get_icon(self) -> str | None:
+        """Return data set icon
+
+        Returns:
+            str | None: icon
         """
         return self.__icon
 
     def set_defaults(self) -> None:
         """Set default values"""
         for item in self._items:
             item.set_default(self)
 
     def __str__(self):
         return self.to_string(debug=False)
 
-    def check(self) -> List[str]:
-        """
-        Check the dataset item values
+    def check(self) -> list[str]:
+        """Check the dataset item values
+
+        Returns:
+            list[str]: list of errors
         """
         errors = []
         for item in self._items:
             if not item.check_item(self) and item._name is not None:
                 errors.append(item._name)
         return errors
 
     def text_edit(self) -> None:
-        """
-        Edit data set with text input only
-        """
+        """Edit data set with text input only"""
         from guidata.dataset import textedit
 
         self.accept(textedit.TextEditVisitor(self))
 
     def edit(
         self,
-        parent: Optional[QWidget] = None,
-        apply: Optional[Callable] = None,
-        size: Optional[Any] = None,
-    ) -> "DataSetEditDialog":
-        """
-        Open a dialog box to edit data set
-            * parent: parent widget (default is None, meaning no parent)
-            * apply: apply callback (default is None)
-            * size: dialog size (QSize object or integer tuple (width, height))
-        """
+        parent: QWidget | None = None,
+        apply: Callable | None = None,
+        size: Any | None = None,
+    ) -> DataSetEditDialog:
+        """Open a dialog box to edit data set
+
+        Args:
+            parent (QWidget): parent widget (default is None,
+             meaning no parent)
+            apply (Callable): apply callback (default is None)
+            size (QSize | tuple[int, int]): dialog size (QSize object
+             or integer tuple (width, height))
+        """
+        # Importing those modules here avoids Qt dependency when
+        # guidata is used without Qt
+        # pylint: disable=import-outside-toplevel
         from guidata.dataset.qtwidgets import DataSetEditDialog
+        from guidata.qthelpers import exec_dialog
 
         dial = DataSetEditDialog(
             self, icon=self.__icon, parent=parent, apply=apply, size=size
         )
         return exec_dialog(dial)
 
-    def view(self, parent: Optional[QWidget] = None, size: Optional[Any] = None):
-        """
-        Open a dialog box to view data set
-            * parent: parent widget (default is None, meaning no parent)
-            * size: dialog size (QSize object or integer tuple (width, height))
-        """
+    def view(self, parent: QWidget | None = None, size: Any | None = None) -> None:
+        """Open a dialog box to view data set
+
+        Args:
+            parent (QWidget): parent widget (default is None,
+             meaning no parent)
+            size (QSize | tuple[int, int]): dialog size (QSize object
+             or integer tuple (width, height))
+        """
+        # Importing those modules here avoids Qt dependency when
+        # guidata is used without Qt
+        # pylint: disable=import-outside-toplevel
         from guidata.dataset.qtwidgets import DataSetShowDialog
+        from guidata.qthelpers import exec_dialog
 
         dial = DataSetShowDialog(self, icon=self.__icon, parent=parent, size=size)
         return exec_dialog(dial)
 
     def to_string(
         self,
-        debug: Optional[bool] = False,
-        indent: Optional[str] = None,
-        align: Optional[bool] = False,
-        show_hidden: Optional[bool] = True,
-    ):
-        """
-        Return readable string representation of the data set
+        debug: bool | None = False,
+        indent: str | None = None,
+        align: bool | None = False,
+        show_hidden: bool | None = True,
+    ) -> str:
+        """Return readable string representation of the data set
         If debug is True, add more details on data items
+
+        Args:
+            debug (bool): if True, add more details on data items
+            indent (str): indentation string (default is None,
+                meaning no indentation)
+            align (bool): if True, align data items (default is False)
+            show_hidden (bool): if True, show hidden data items
+                (default is True)
+
+        Returns:
+            str: string representation of the data set
         """
         if indent is None:
             indent = "\n    "
         txt = "%s:" % (self.__title)
 
         def _get_label(item):
             if debug:
@@ -886,31 +1235,39 @@
                 label = label.ljust(length)
             txt += "%s%s: %s" % (indent, label, value_str)
             if debug:
                 txt += " (" + item.__class__.__name__ + ")"
         return txt
 
     def accept(self, vis: object) -> None:
-        """
-        helper function that passes the visitor to the accept methods of all
+        """Helper function that passes the visitor to the accept methods of all
         the items in this dataset
+
+        Args:
+            vis (object): visitor object
         """
         for item in self._items:
             item.accept(vis)
 
-    def serialize(
-        self, writer: Union["HDF5Writer", "JSONWriter", "UserConfigWriter"]
-    ) -> None:
+    def serialize(self, writer: HDF5Writer | JSONWriter | INIWriter) -> None:
+        """Serialize the dataset
+
+        Args:
+            writer (HDF5Writer | JSONWriter | INIWriter): writer object
+        """
         for item in self._items:
             with writer.group(item._name):
                 item.serialize(self, writer)
 
-    def deserialize(
-        self, reader: Union["HDF5Reader", "JSONReader", "UserConfigReader"]
-    ) -> None:
+    def deserialize(self, reader: HDF5Reader | JSONReader | INIReader) -> None:
+        """Deserialize the dataset
+
+        Args:
+            reader (HDF5Reader | JSONReader | INIReader): reader object
+        """
         for item in self._items:
             with reader.group(item._name):
                 try:
                     item.deserialize(self, reader)
                 except RuntimeError as error:
                     if DEBUG_DESERIALIZE:
                         import traceback
@@ -918,53 +1275,77 @@
                         print(
                             "DEBUG_DESERIALIZE enabled in datatypes.py", file=sys.stderr
                         )
                         traceback.print_stack()
                         print(error, file=sys.stderr)
                     item.set_default(self)
 
-    def read_config(self, conf: "UserConfig", section: str, option: str) -> None:
-        from guidata.dataset.iniio import UserConfigReader
+    def read_config(self, conf: UserConfig, section: str, option: str) -> None:
+        """Read configuration from a UserConfig instance
 
-        reader = UserConfigReader(conf, section, option)
+        Args:
+            conf (UserConfig): UserConfig instance
+            section (str): section name
+            option (str): option name
+        """
+        from guidata.dataset.io import INIReader
+
+        reader = INIReader(conf, section, option)
         self.deserialize(reader)
 
-    def write_config(self, conf: "UserConfig", section: str, option: str) -> None:
-        from guidata.dataset.iniio import UserConfigWriter
+    def write_config(self, conf: UserConfig, section: str, option: str) -> None:
+        """Write configuration to a UserConfig instance
+
+        Args:
+            conf (UserConfig): UserConfig instance
+            section (str): section name
+            option (str): option name
+        """
+        from guidata.dataset.io import INIWriter
 
-        writer = UserConfigWriter(conf, section, option)
+        writer = INIWriter(conf, section, option)
         self.serialize(writer)
 
     @classmethod
     def set_global_prop(klass, realm: str, **kwargs) -> None:
+        """Set global properties for all data items in the dataset
+
+        Args:
+            realm (str): realm name
+            \*\*kwargs (dict): properties to set
+        """  # noqa
         for item in klass._items:
             item.set_prop(realm, **kwargs)
 
 
 class ActivableDataSet(DataSet):
-    """
-    An ActivableDataSet instance must have an "enable" class attribute which
+    """An ActivableDataSet instance must have an "enable" class attribute which
     will set the active state of the dataset instance
     (see example in: tests/activable_dataset.py)
+
+    Args:
+        title (str): dataset title (optional)
+        comment (str): dataset comment (optional)
+        icon (str): dataset icon. Default is "" (no icon)
     """
 
     _ro = True  # default *instance* attribute value
     _active = True
     _ro_prop = GetAttrProp("_ro")
     _active_prop = GetAttrProp("_active")
 
     @property
     @abstractmethod
-    def enable(self) -> "DataItem":
+    def enable(self) -> DataItem:
         ...
 
     def __init__(
         self,
-        title: Optional[str] = None,
-        comment: Optional[str] = None,
+        title: str | None = None,
+        comment: str | None = None,
         icon: str = "",
     ):
         DataSet.__init__(self, title, comment, icon)
 
     #        self.set_readonly()
 
     @classmethod
@@ -975,148 +1356,188 @@
         """
         cls.set_global_prop("display", active=cls._active_prop)
         cls.enable.set_prop(  # type:ignore
             "display", active=True, hide=cls._ro_prop, store=cls._active_prop
         )
 
     def set_readonly(self) -> None:
-        """
-        The dataset is now in read-only mode, i.e. all data items are disabled
-        """
+        """The dataset is now in read-only mode, i.e. all data items are disabled"""
         self._ro = True
         self._active = self.enable
 
     def set_writeable(self) -> None:
-        """
-        The dataset is now in read/write mode, i.e. all data items are enabled
-        """
+        """The dataset is now in read/write mode, i.e. all data items are enabled"""
         self._ro = False
         self._active = self.enable
 
 
 class DataSetGroup:
-    """
-    Construct a DataSetGroup object, used to group several datasets together
-        * datasets [list of DataSet objects]
-        * title [string]
-        * icon [QIcon or string]: icon show on the button (optional)
-          (string: icon filename as in guidata/guiqwt image search paths)
+    """Construct a DataSetGroup object, used to group several datasets together
+
+    Args:
+        datasets (list[DataSet]): list of datasets
+        title (str): group title (optional)
+        icon (str): group icon. Default is "" (no icon)
 
     This class tries to mimics the DataSet interface.
 
     The GUI should represent it as a notebook with one page for each
     contained dataset.
     """
 
     def __init__(
-        self, datasets: List["DataSet"], title: Optional[str] = None, icon: str = ""
+        self, datasets: list[DataSet], title: str | None = None, icon: str = ""
     ) -> None:
         self.__icon = icon
         self.datasets = datasets
         if title:
             self.__title = title
         else:
             self.__title = self.__class__.__name__
 
     def __str__(self) -> str:
         return "\n".join([dataset.__str__() for dataset in self.datasets])
 
     def get_title(self) -> str:
-        """
-        Return data set group title
+        """Return data set group title
+
+        Returns:
+            str: data set group title
         """
         return self.__title
 
     def get_comment(self) -> None:
-        """
-        Return data set group comment --> not implemented (will return None)
+        """Return data set group comment --> not implemented (will return None)
+
+        Returns:
+            None: data set group comment
         """
         return None
 
-    def get_icon(self) -> Union[str, None]:
-        """
-        Return data set icon
+    def get_icon(self) -> str | None:
+        """Return data set icon
+
+        Returns:
+            str | None: data set icon
         """
         return self.__icon
 
-    def check(self) -> List[List[str]]:
-        """
-        Check data set group items
+    def check(self) -> list[list[str]]:
+        """Check data set group items
+
+        Returns:
+            list[list[str]]: list of errors
         """
         return [dataset.check() for dataset in self.datasets]
 
     def text_edit(self) -> None:
-        """
-        Edit data set with text input only
-        """
+        """Edit data set with text input only"""
         raise NotImplementedError()
 
-    def edit(
-        self, parent: Optional[QWidget] = None, apply: Optional[Callable] = None
-    ) -> int:
-        """
-        Open a dialog box to edit data set
+    def edit(self, parent: QWidget | None = None, apply: Callable | None = None) -> int:
+        """Open a dialog box to edit data set
+
+        Args:
+            parent (QWidget): parent widget. Defaults to None.
+            apply (Callable): apply callback. Defaults to None.
+
+        Returns:
+            int: dialog box return code
         """
+        # Importing those modules here avoids Qt dependency when
+        # guidata is used without Qt
+        # pylint: disable=import-outside-toplevel
         from guidata.dataset.qtwidgets import DataSetGroupEditDialog
+        from guidata.qthelpers import exec_dialog
 
         dial = DataSetGroupEditDialog(
             self, icon=self.__icon, parent=parent, apply=apply
         )
         return exec_dialog(dial)
 
     def accept(self, vis: object) -> None:
-        """
-        helper function that passes the visitor to the accept methods of all
+        """Helper function that passes the visitor to the accept methods of all
         the items in this dataset
+
+        Args:
+            vis (object): visitor
         """
         for dataset in self.datasets:
             dataset.accept(vis)
 
 
 class GroupItem(DataItemProxy):
-    """GroupItem proxy"""
+    """GroupItem proxy
+
+    Args:
+        item (DataItem): data item
+    """
 
-    def __init__(self, item: "DataItem") -> None:
+    def __init__(self, item: DataItem) -> None:
         DataItemProxy.__init__(self, item)
-        self.group: List[Any] = []
+        self.group: list[Any] = []
 
 
 class BeginGroup(DataItem):
-    """
-    Data item which does not represent anything
+    """Data item which does not represent anything
     but a begin flag to define a data set group
+
+    Args:
+        label (str): group label
     """
 
+    def __init__(self, label: str) -> None:
+        super().__init__(label)
+
     def serialize(self, instance, writer) -> None:
         pass
 
     def deserialize(self, instance, reader) -> None:
         pass
 
     def get_group(self) -> "GroupItem":
         return GroupItem(self)
 
 
 class EndGroup(DataItem):
-    """
-    Data item which does not represent anything
+    """Data item which does not represent anything
     but an end flag to define a data set group
+
+    Args:
+        label (str): group label
     """
 
+    def __init__(self, label: str) -> None:
+        super().__init__(label)
+
     def serialize(self, instance, writer) -> None:
         pass
 
     def deserialize(self, instance, reader) -> None:
         pass
 
 
 class TabGroupItem(GroupItem):
     pass
 
 
 class BeginTabGroup(BeginGroup):
+    """Data item which does not represent anything
+    but a begin flag to define a data set tab group
+
+    Args:
+        label (str): group label
+    """
+
     def get_group(self) -> "TabGroupItem":
         return TabGroupItem(self)
 
 
 class EndTabGroup(EndGroup):
+    """Data item which does not represent anything
+    but an end flag to define a data set tab group
+
+    Args:
+        label (str): group label
+    """
+
     pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `guidata-3.0.0/guidata/dataset/hdf5io.py` & `guidata-3.0.1/guidata/dataset/io/h5fmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 #
 # Licensed under the terms of the BSD 3-Clause
 # (see guidata/LICENSE for details)
 
 """
-Reader and Writer for the serialization of DataSets into HDF5 files
+HDF5 files (.h5)
 """
 
 from __future__ import annotations
 
 import sys
 from collections.abc import Callable, Sequence
 from typing import Any
 from uuid import uuid1
 
 import h5py
 import numpy as np
 
-from guidata.dataset.iniio import BaseIOHandler, WriterMixin
+from guidata.dataset.io.base import BaseIOHandler, WriterMixin
 
 
 class TypeConverter:
     """Handles conversion between types for HDF5 serialization.
 
     Args:
         to_type (Any): The target type for the HDF5 representation.
@@ -192,20 +192,20 @@
 class Dset(Attr):
     """
     Class for generic load/save for an hdf5 dataset.
     Handles the conversion of the scalar value, if any.
 
     Args:
         hdf_name (str): The name of the HDF5 attribute.
-        struct_name (str, optional): The name of the structure. Defaults to None.
-        type (type, optional): The expected data type of the attribute.
+        struct_name (str): The name of the structure. Defaults to None.
+        type (type): The expected data type of the attribute.
             Defaults to None.
-        scalar (callable, optional): Function to convert the scalar value, if any.
+        scalar (Callable): Function to convert the scalar value, if any.
             Defaults to None.
-        optional (bool, optional): Whether the attribute is optional. Defaults to False.
+        optional (bool): Whether the attribute is optional. Defaults to False.
     """
 
     def __init__(
         self,
         hdf_name: str,
         struct_name: str | None = None,
         type: type | None = None,
@@ -217,15 +217,15 @@
 
     def save(self, group: h5py.Group, struct: Any) -> None:
         """
         Save the attribute to the given HDF5 group.
 
         Args:
             group (h5py.Group): The group in the HDF5 file to save the attribute to.
-            struct (any): The structure containing the attribute.
+            struct (Any): The structure containing the attribute.
 
         Returns:
             None
         """
         value = self.get_value(struct)
         if isinstance(value, float):
             value = np.float64(value)
@@ -246,15 +246,15 @@
 
     def load(self, group: h5py.Group, struct: Any) -> None:
         """
         Load the attribute from the given HDF5 group.
 
         Args:
             group (h5py.Group): The group in the HDF5 file to load the attribute from.
-            struct (any): The structure to load the attribute into.
+            struct (Any): The structure to load the attribute into.
 
         Raises:
             KeyError: If the attribute cannot be found in the HDF5 group.
 
         Returns:
             None
         """
@@ -276,42 +276,42 @@
     Class for handling lists in HDF5 datasets. Inherits from the Dset class.
 
     Overrides the get_value and set_value methods from the Dset class to
     handle lists specifically.
 
     Args:
         hdf_name (str): The name of the HDF5 attribute.
-        struct_name (str, optional): The name of the structure. Defaults to None.
-        type (type, optional): The expected data type of the attribute.
+        struct_name (str): The name of the structure. Defaults to None.
+        type (type): The expected data type of the attribute.
             Defaults to None.
-        scalar (callable, optional): Function to convert the scalar value, if any.
+        scalar (Callable): Function to convert the scalar value, if any.
             Defaults to None.
-        optional (bool, optional): Whether the attribute is optional. Defaults to False.
+        optional (bool): Whether the attribute is optional. Defaults to False.
     """
 
     def get_value(self, struct: Any) -> np.ndarray:
         """
         Returns the value of the attribute in the given structure as a numpy array.
 
         Args:
-            struct (any): The structure containing the attribute.
+            struct (Any): The structure containing the attribute.
 
         Returns:
             np.ndarray: The value of the attribute in the given structure as a
                 numpy array.
         """
         return np.array(getattr(struct, self.struct_name))
 
     def set_value(self, struct: Any, value: np.ndarray) -> None:
         """
         Sets the value of the attribute in the given structure to a list containing
         the values of the given numpy array.
 
         Args:
-            struct (any): The structure in which to set the attribute.
+            struct (Any): The structure in which to set the attribute.
             value (np.ndarray): A numpy array containing the values to set the
                 attribute to.
 
         Returns:
             None
         """
         setattr(struct, self.struct_name, list(value))
@@ -334,15 +334,15 @@
         self.h5 = None
 
     def open(self, mode: str = "a") -> h5py._hl.files.File:
         """
         Opens an HDF5 file in the given mode.
 
         Args:
-            mode (str, optional): The mode in which to open the file. Defaults to "a".
+            mode (str): The mode in which to open the file. Defaults to "a".
 
         Returns:
             h5py._hl.files.File: The opened HDF5 file.
 
         Raises:
             Exception: If there is an error while trying to open the file.
         """
@@ -391,16 +391,16 @@
         self.close()
 
     def generic_save(self, parent: Any, source: Any, structure: list[Attr]) -> None:
         """
         Saves the data from source into the file using 'structure' as a descriptor.
 
         Args:
-            parent (any): The parent HDF5 group.
-            source (any): The source of the data to save.
+            parent (Any): The parent HDF5 group.
+            source (Any): The source of the data to save.
             structure (List[Attr]): A list of attribute descriptors (Attr, Dset,
                 Dlist, etc.) that describe the conversion of data and the names
                 of the attributes in the source and in the file.
 
         Returns:
             None
         """
@@ -408,16 +408,16 @@
             instr.save(parent, source)
 
     def generic_load(self, parent: Any, dest: Any, structure: list[Attr]) -> None:
         """
         Loads the data from the file into 'dest' using 'structure' as a descriptor.
 
         Args:
-            parent (any): The parent HDF5 group.
-            dest (any): The destination to load the data into.
+            parent (Any): The parent HDF5 group.
+            dest (Any): The destination to load the data into.
             structure (List[Attr]): A list of attribute descriptors (Attr, Dset,
                 Dlist, etc.) that describe the conversion of data and the names
                 of the attributes in the file and in the destination.
 
         Returns:
             None
 
@@ -475,15 +475,15 @@
         self.open("w")
 
     def write_any(self, val: Any) -> None:
         """
         Write the value to the HDF5 file as an attribute.
 
         Args:
-            val (any): The value to write.
+            val (Any): The value to write.
 
         Returns:
             None
         """
         group = self.get_parent_group()
         group.attrs[self.option[-1]] = val
 
@@ -545,15 +545,15 @@
 
     def write_object_list(self, seq: Sequence[Any] | None, group_name: str) -> None:
         """
         Write an object sequence to the HDF5 file in a group.
         Objects must implement the DataSet-like `serialize` method.
 
         Args:
-            seq (Sequence[Any], optional): The object sequence to write.
+            seq (Sequence[Any]): The object sequence to write.
                 Defaults to None.
             group_name (str): The name of the group in which to write the objects.
 
         Returns:
             None
         """
         with self.group(group_name):
@@ -590,19 +590,19 @@
         func: Callable[[], Any] | None = None,
         instance: Any | None = None,
     ) -> Any:
         """
         Read a value from the current group or specified group_name.
 
         Args:
-            group_name (str, optional): The name of the group to read from.
+            group_name (str): The name of the group to read from.
                 Defaults to None.
-            func (Callable[[], Any], optional): The function to use for reading
+            func (Callable[[], Any]): The function to use for reading
                 the value. Defaults to None.
-            instance (Any, optional): An object that implements the DataSet-like
+            instance (Any): An object that implements the DataSet-like
                 `deserialize` method. Defaults to None.
 
         Returns:
             Any: The read value.
         """
         if group_name:
             self.begin(group_name)
```

### Comparing `guidata-3.0.0/guidata/dataset/jsonio.py` & `guidata-3.0.1/guidata/dataset/io/jsonfmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 # This file is part of CodraFT Project
 # https://codra-ingenierie-informatique.github.io/CodraFT/
 #
 # Licensed under the terms of the BSD 3-Clause or the CeCILL-B License
 # (see codraft/LICENSE for details)
 
 """
-Reader and Writer for the serialization of DataSets into JSON files
+JSON files (.json)
 """
 
 # pylint: disable=invalid-name  # Allows short reference names like x, y, ...
 
 import json
 import os
 from uuid import uuid1
 
 import numpy as np
 
-from guidata.dataset.iniio import BaseIOHandler, WriterMixin
+from guidata.dataset.io.base import BaseIOHandler, WriterMixin
 
 
 class CustomJSONEncoder(json.JSONEncoder):
     """Custom JSON Encoder"""
 
     def default(self, o):
         """Override JSONEncoder method"""
@@ -72,15 +72,19 @@
         """Object hook"""
         for key, value in list(obj.items()):
             obj[key] = self.__iterate_dict(value)
         return obj
 
 
 class JSONHandler(BaseIOHandler):
-    """Class handling JSON r/w"""
+    """Class handling JSON r/w
+
+    Args:
+        filename: JSON filename (if None, use `jsontext` attribute)
+    """
 
     def __init__(self, filename=None):
         super().__init__()
         self.jsondata = {}
         self.jsontext = None
         self.filename = filename
 
@@ -157,19 +161,22 @@
                             self.write_none()
                         else:
                             obj.serialize(self)
                 self.write(ids, "IDs")
 
 
 class JSONReader(JSONHandler):
-    """Class handling JSON deserialization"""
+    """Class handling JSON deserialization
+
+    Args:
+        fname_or_jsontext: JSON filename or JSON text
+    """
 
     def __init__(self, fname_or_jsontext):
-        """JSONReader constructor:
-        * fname_or_jsontext: JSON filename or JSON text"""
+        """JSONReader constructor"""
         JSONHandler.__init__(self, fname_or_jsontext)
         if fname_or_jsontext is not None and not os.path.isfile(fname_or_jsontext):
             self.filename = None
             self.jsontext = fname_or_jsontext
         self.load()
 
     def read(self, group_name=None, func=None, instance=None):
```

### Comparing `guidata-3.0.0/guidata/dataset/qtitemwidgets.py` & `guidata-3.0.1/guidata/dataset/qtitemwidgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Widget factories used to edit data items
 (factory registration is done in guidata.dataset.qtwidgets)
 (data item types are defined in guidata.dataset.datatypes)
 
 There is one widget type for each data item type.
 Example: ChoiceWidget <--> ChoiceItem, ImageChoiceItem
 """
+
 import collections.abc
 import datetime
 import os
 import os.path as osp
 import sys
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, Callable, List, Optional, Protocol
@@ -49,14 +50,15 @@
 )
 
 from guidata.config import _
 from guidata.configtools import get_icon, get_image_file_path, get_image_layout
 from guidata.dataset.datatypes import DataItemVariable
 from guidata.qthelpers import get_std_icon, text_to_qcolor
 from guidata.utils import restore_dataset, update_dataset
+from guidata.utils.misc import convert_date_format
 from guidata.widgets.arrayeditor import ArrayEditor
 
 # ========================== <!> IMPORTANT <!> =================================
 #
 # In this module, `item` is an instance of DataItemVariable (not DataItem)
 # (see guidata.datatypes for details)
 #
@@ -461,14 +463,18 @@
     def __init__(
         self, item: "DataItemVariable", parent_layout: "DataSetEditLayout"
     ) -> None:
         super().__init__(item, parent_layout)
         self.dateedit = self.group = QDateEdit()
         self.dateedit.setToolTip(item.get_help())
         self.dateedit.dateTimeChanged.connect(self.date_changed)
+        fmt = self.item.get_prop("display", "format", None)
+        if fmt:
+            qt_fmt = convert_date_format(fmt)
+            self.dateedit.setDisplayFormat(qt_fmt)
 
     def date_changed(self, value):
         """Date changed"""
         _display_callback(self, value)
         self.notify_value_change()
 
     def get(self) -> None:
@@ -511,14 +517,18 @@
         super().__init__(item, parent_layout)
         self.dateedit = self.group = QDateTimeEdit()
         self.dateedit.setCalendarPopup(True)
         self.dateedit.setToolTip(item.get_help())
         self.dateedit.dateTimeChanged.connect(  # type:ignore
             lambda value: self.notify_value_change()
         )
+        fmt = self.item.get_prop("display", "format", None)
+        if fmt:
+            qt_fmt = convert_date_format(fmt)
+            self.dateedit.setDisplayFormat(qt_fmt)
 
     def date_changed(self, value):
         """Date changed"""
         _display_callback(self, value)
         self.notify_value_change()
 
     def get(self):
```

### Comparing `guidata-3.0.0/guidata/dataset/qtwidgets.py` & `guidata-3.0.1/guidata/dataset/qtwidgets.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/dataset/textedit.py` & `guidata-3.0.1/guidata/dataset/textedit.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/env.py` & `guidata-3.0.1/guidata/env.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/external/darkdetect/__init__.py` & `guidata-3.0.1/guidata/external/darkdetect/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/external/darkdetect/_linux_detect.py` & `guidata-3.0.1/guidata/external/darkdetect/_linux_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/external/darkdetect/_mac_detect.py` & `guidata-3.0.1/guidata/external/darkdetect/_mac_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/external/darkdetect/_windows_detect.py` & `guidata-3.0.1/guidata/external/darkdetect/_windows_detect.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/guitest.py` & `guidata-3.0.1/guidata/guitest.py`

 * *Files 6% similar despite different names*

```diff
@@ -163,16 +163,16 @@
             return "<br>".join(lines)
         return self.error_msg
 
     def run(self, args: str = "", timeout: int = None) -> None:
         """Run test script
 
         Args:
-            args (str, optional): arguments to pass to the script
-            timeout (int, optional): timeout in seconds
+            args (str): arguments to pass to the script
+            timeout (int): timeout in seconds
         """
         # Keep the same sys.path environment in child process:
         # (useful when the program is executed from Spyder, for example)
         os.environ["PYTHONPATH"] = os.pathsep.join(sys.path)
 
         command = [sys.executable, '"' + self.path + '"']
         if args:
@@ -182,15 +182,15 @@
             proc.wait(timeout)
 
 
 class TestPropertiesWidget(QW.QWidget):
     """Test module properties panel
 
     Args:
-        parent (QWidget, optional): parent widget
+        parent (QWidget): parent widget
     """
 
     def __init__(self, parent: QW.QWidget = None) -> None:
         super().__init__(parent)
         self.lbl_icon = QW.QLabel()
         self.lbl_icon.setFixedWidth(32)
         self.desc_label = QW.QLabel()
@@ -230,15 +230,15 @@
 
 
 class TestMainView(QW.QSplitter):
     """Test launcher main view
 
     Args:
         package (module): test package
-        parent (QWidget, optional): parent widget
+        parent (QWidget): parent widget
     """
 
     def __init__(self, package, parent=None):
         super().__init__(parent)
         self.tests = get_tests(package, category="visible")
 
         listgroup = QW.QFrame()
@@ -313,15 +313,15 @@
 
 
 class TestLauncherWindow(QW.QMainWindow):
     """Test launcher main window
 
     Args:
         package (module): test package
-        parent (QWidget, optional): parent widget
+        parent (QWidget): parent widget
     """
 
     def __init__(self, package, parent: QW.QWidget = None) -> None:
         super().__init__(parent)
         win32_fix_title_bar_background(self)
         self.setWindowTitle(_("Tests - %s module") % package.__name__)
         self.setWindowIcon(get_icon("%s.svg" % package.__name__, "guidata.svg"))
```

### Comparing `guidata-3.0.0/guidata/images/apply.png` & `guidata-3.0.1/guidata/images/apply.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/arredit.png` & `guidata-3.0.1/guidata/images/arredit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/busy.png` & `guidata-3.0.1/guidata/images/busy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/cell_edit.png` & `guidata-3.0.1/guidata/images/cell_edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/copy.png` & `guidata-3.0.1/guidata/images/copy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/delete.png` & `guidata-3.0.1/guidata/images/delete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/dictedit.png` & `guidata-3.0.1/guidata/images/dictedit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/dtype.png` & `guidata-3.0.1/guidata/images/dtype.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/edit.png` & `guidata-3.0.1/guidata/images/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/copywop.png` & `guidata-3.0.1/guidata/images/editors/copywop.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/edit.png` & `guidata-3.0.1/guidata/images/editors/edit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/edit_add.png` & `guidata-3.0.1/guidata/images/editors/edit_add.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/editclear.png` & `guidata-3.0.1/guidata/images/editors/editclear.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/editcopy.png` & `guidata-3.0.1/guidata/images/editors/editcopy.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/editcut.png` & `guidata-3.0.1/guidata/images/editors/editcut.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/editdelete.png` & `guidata-3.0.1/guidata/images/editors/editdelete.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/editpaste.png` & `guidata-3.0.1/guidata/images/editors/editpaste.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/fileimport.png` & `guidata-3.0.1/guidata/images/editors/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/filesave.png` & `guidata-3.0.1/guidata/images/editors/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/imshow.png` & `guidata-3.0.1/guidata/images/editors/imshow.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/insert.png` & `guidata-3.0.1/guidata/images/editors/insert.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/plot.png` & `guidata-3.0.1/guidata/images/editors/plot.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/rename.png` & `guidata-3.0.1/guidata/images/editors/rename.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/editors/selectall.png` & `guidata-3.0.1/guidata/images/editors/selectall.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/exit.png` & `guidata-3.0.1/guidata/images/exit.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/file.png` & `guidata-3.0.1/guidata/images/file.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/fileclose.png` & `guidata-3.0.1/guidata/images/fileclose.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/fileimport.png` & `guidata-3.0.1/guidata/images/fileimport.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/fileopen.png` & `guidata-3.0.1/guidata/images/fileopen.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filesave.png` & `guidata-3.0.1/guidata/images/filesave.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filesaveas.png` & `guidata-3.0.1/guidata/images/filesaveas.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/doc.png` & `guidata-3.0.1/guidata/images/filetypes/doc.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/gif.png` & `guidata-3.0.1/guidata/images/filetypes/gif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/html.png` & `guidata-3.0.1/guidata/images/filetypes/html.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/jpg.png` & `guidata-3.0.1/guidata/images/filetypes/jpg.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/pdf.png` & `guidata-3.0.1/guidata/images/filetypes/pdf.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/png.png` & `guidata-3.0.1/guidata/images/filetypes/png.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/pps.png` & `guidata-3.0.1/guidata/images/filetypes/pps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/ps.png` & `guidata-3.0.1/guidata/images/filetypes/ps.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/tar.png` & `guidata-3.0.1/guidata/images/filetypes/tar.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/tgz.png` & `guidata-3.0.1/guidata/images/filetypes/tgz.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/tif.png` & `guidata-3.0.1/guidata/images/filetypes/tif.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/txt.png` & `guidata-3.0.1/guidata/images/filetypes/txt.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/xls.png` & `guidata-3.0.1/guidata/images/filetypes/xls.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/filetypes/zip.png` & `guidata-3.0.1/guidata/images/filetypes/zip.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/guidata-banner.svg` & `guidata-3.0.1/guidata/images/guidata-banner.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/guidata-vertical.svg` & `guidata-3.0.1/guidata/images/guidata-vertical.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/guidata.svg` & `guidata-3.0.1/guidata/images/guidata.svg`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/not_found.png` & `guidata-3.0.1/guidata/images/not_found.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/python.png` & `guidata-3.0.1/guidata/images/python.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/quickview.png` & `guidata-3.0.1/guidata/images/quickview.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/save_all.png` & `guidata-3.0.1/guidata/images/save_all.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/selection.png` & `guidata-3.0.1/guidata/images/selection.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/images/settings.png` & `guidata-3.0.1/guidata/images/settings.png`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/locale/fr/LC_MESSAGES/guidata.mo` & `guidata-3.0.1/guidata/locale/fr/LC_MESSAGES/guidata.mo`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/qthelpers.py` & `guidata-3.0.1/guidata/qthelpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,16 +169,16 @@
     enabled: bool | None = None,
 ) -> QW.QAction:
     """Create a new QAction
 
     Args:
         parent (QWidget or None): Parent widget
         title (str): Action title
-        triggered (callable or None): Triggered callback
-        toggled (callable or None): Toggled callback
+        triggered (Callable or None): Triggered callback
+        toggled (Callable or None): Toggled callback
         shortcut (QKeySequence or None): Shortcut
         icon (QIcon or None): Icon
         tip (str or None): Tooltip
         checkable (bool or None): Checkable
         context (Qt.ShortcutContext): Shortcut context
         enabled (bool or None): Enabled
 
@@ -226,17 +226,17 @@
 ) -> QW.QToolButton:
     """Create a QToolButton
 
     Args:
         parent (QWidget): Parent widget
         icon (QIcon or str or None): Icon
         text (str or None): Text
-        triggered (callable or None): Triggered callback
+        triggered (Callable or None): Triggered callback
         tip (str or None): Tooltip
-        toggled (callable or None): Toggled callback
+        toggled (Callable or None): Toggled callback
         shortcut (QKeySequence or None): Shortcut
         autoraise (bool): Auto raise
         enabled (bool or None): Enabled
 
     Returns:
         QToolButton: New toolbutton
     """
@@ -276,15 +276,15 @@
     layout: QW.QLayout | None = None,
 ) -> QW.QGroupBox:
     """Create a QGroupBox
 
     Args:
         parent (QWidget): Parent widget
         title (str or None): Title
-        toggled (callable or None): Toggled callback
+        toggled (Callable or None): Toggled callback
         checked (bool or None): Checked
         flat (bool): Flat
         layout (QLayout or None): Layout
 
     Returns:
         QGroupBox: New groupbox
     """
```

### Comparing `guidata-3.0.0/guidata/tests/_all_tests.py` & `guidata-3.0.1/guidata/tests/_all_tests.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_activable_dataset.py` & `guidata-3.0.1/guidata/tests/test_activable_dataset.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_activable_items.py` & `guidata-3.0.1/guidata/tests/test_activable_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_all_features.py` & `guidata-3.0.1/guidata/tests/test_all_features.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_all_items.py` & `guidata-3.0.1/guidata/tests/test_all_items.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_arrayeditor.py` & `guidata-3.0.1/guidata/tests/test_arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_bool_selector.py` & `guidata-3.0.1/guidata/tests/test_bool_selector.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_callbacks.py` & `guidata-3.0.1/guidata/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_codeeditor.py` & `guidata-3.0.1/guidata/tests/test_codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_collectionseditor.py` & `guidata-3.0.1/guidata/tests/test_collectionseditor.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 Tests for collectionseditor.py
 """
 
 # guitest: show
 
 import datetime
 
+import numpy as np
+
 from guidata.env import execenv
 from guidata.qthelpers import qt_app_context
 from guidata.widgets.collectionseditor import CollectionsEditor
 
+try:
+    from PIL import Image as PILImage
+except ImportError:
+    # PIL is not installed
+    PILImage = None
+
 
 def get_test_data():
     """Create test data."""
-    import numpy as np
-    from PIL import Image
-
-    image = Image.fromarray(np.random.randint(256, size=(100, 100)), mode="P")
     testdict = {"d": 1, "a": np.random.rand(10, 10), "b": [1, 2]}
     testdate = datetime.date(1945, 5, 8)
     test_timedelta = datetime.timedelta(days=-1, minutes=42, seconds=13)
 
     try:
         import pandas as pd
     except (ModuleNotFoundError, ImportError):
@@ -54,15 +58,15 @@
 
         def __init__(self):
             self.text = "toto"
             self.testdict = testdict
             self.testdate = testdate
 
     foobar = Foobar()
-    return {
+    test_data = {
         "object": foobar,
         "module": np,
         "str": "kjkj kj k j j kj k jkj",
         "unicode": "éù",
         "list": [1, 3, [sorted, 5, 6], "kjkj", None],
         "tuple": ([1, testdate, testdict, test_timedelta], "kjkj", None),
         "dict": testdict,
@@ -72,15 +76,14 @@
         "array": np.random.rand(10, 10).astype(np.int64),
         "masked_array": np.ma.array(
             [[1, 0], [1, 0]], mask=[[True, False], [False, False]]
         ),
         "1D-array": np.linspace(-10, 10).astype(np.float16),
         "3D-array": np.random.randint(2, size=(5, 5, 5)).astype(np.bool_),
         "empty_array": np.array([]),
-        "image": image,
         "date": testdate,
         "datetime": datetime.datetime(1945, 5, 8, 23, 1, 0, int(1.5e5)),
         "timedelta": test_timedelta,
         "complex": 2 + 1j,
         "complex64": np.complex64(2 + 1j),
         "complex128": np.complex128(9j),
         "int8_scalar": np.int8(8),
@@ -101,14 +104,18 @@
         "unsupported1": np.arccos,
         "unsupported2": np.cast,
         # Test for Issue #3518
         "big_struct_array": np.zeros(
             1000, dtype=[("ID", "f8"), ("param1", "f8", 5000)]
         ),
     }
+    if PILImage is not None:
+        image = PILImage.fromarray(np.random.randint(256, size=(100, 100)), mode="P")
+        test_data["image"] = image
+    return test_data
 
 
 def test_collectionseditor():
     """Test Collections editor."""
     with qt_app_context(exec_loop=True):
         dialog = CollectionsEditor()
         dialog.setup(get_test_data())
```

### Comparing `guidata-3.0.0/guidata/tests/test_config.py` & `guidata-3.0.1/guidata/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_console.py` & `guidata-3.0.1/guidata/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_data.py` & `guidata-3.0.1/guidata/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_dataframeeditor.py` & `guidata-3.0.1/guidata/tests/test_dataframeeditor.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,23 +7,30 @@
 """
 Tests for dataframeeditor.py
 """
 
 # guitest: show
 
 import numpy as np
-from numpy import nan
-from pandas import DataFrame, Series
-from pandas.testing import assert_frame_equal, assert_series_equal
+import pytest
+
+try:
+    import pandas as pd
+    import pandas.testing as pdt
+
+    from guidata.widgets.dataframeeditor import DataFrameEditor
+except ImportError:
+    # pandas is not installed
+    pd = pdt = DataFrameEditor = None
 
 from guidata.env import execenv
 from guidata.qthelpers import exec_dialog, qt_app_context
-from guidata.widgets.dataframeeditor import DataFrameEditor
 
 
+@pytest.mark.skipif(pd is None, reason="pandas is not installed")
 def test_dataframeeditor():
     """DataFrame editor test"""
 
     def test_edit(data, title="", parent=None):
         """Test subroutine"""
         dlg = DataFrameEditor(parent=parent)
 
@@ -32,41 +39,41 @@
             return dlg.get_value()
         else:
             import sys
 
             sys.exit(1)
 
     with qt_app_context():
-        df1 = DataFrame(
+        df1 = pd.DataFrame(
             [
                 [True, "bool"],
                 [1 + 1j, "complex"],
                 ["test", "string"],
                 [1.11, "float"],
                 [1, "int"],
                 [np.random.rand(3, 3), "Unkown type"],
                 ["Large value", 100],
                 ["áéí", "unicode"],
             ],
-            index=["a", "b", nan, nan, nan, "c", "Test global max", "d"],
-            columns=[nan, "Type"],
+            index=["a", "b", np.nan, np.nan, np.nan, "c", "Test global max", "d"],
+            columns=[np.nan, "Type"],
         )
         out = test_edit(df1)
-        assert_frame_equal(df1, out)
+        pdt.assert_frame_equal(df1, out)
 
-        result = Series([True, "bool"], index=[nan, "Type"], name="a")
+        result = pd.Series([True, "bool"], index=[np.nan, "Type"], name="a")
         out = test_edit(df1.iloc[0])
-        assert_series_equal(result, out)
+        pdt.assert_series_equal(result, out)
 
-        df1 = DataFrame(np.random.rand(100100, 10))
+        df1 = pd.DataFrame(np.random.rand(100100, 10))
         out = test_edit(df1)
-        assert_frame_equal(out, df1)
+        pdt.assert_frame_equal(out, df1)
 
-        series = Series(np.arange(10), name=0)
+        series = pd.Series(np.arange(10), name=0)
         out = test_edit(series)
-        assert_series_equal(series, out)
+        pdt.assert_series_equal(series, out)
 
         execenv.print("OK")
 
 
 if __name__ == "__main__":
     test_dataframeeditor()
```

### Comparing `guidata-3.0.0/guidata/tests/test_datasetgroup.py` & `guidata-3.0.1/guidata/tests/test_datasetgroup.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_disthelpers.py` & `guidata-3.0.1/guidata/tests/test_disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_editgroupbox.py` & `guidata-3.0.1/guidata/tests/test_editgroupbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     _a_group = gdt.EndGroup("A group")
     b_group = gdt.BeginGroup("B group")
     param3 = gdi.FloatItem("Foobar 3", default=123)
     param4 = gdi.BoolItem("Boolean")
     _b_group = gdt.EndGroup("B group")
     c_group = gdt.BeginGroup("C group")
     param5 = gdi.FloatItem("Foobar 4", default=250)
-    param6 = gdi.DateItem("Date")
+    param6 = gdi.DateItem("Date").set_prop("display", format="dd.MM.yyyy")
     param7 = gdi.ColorItem("Color")
     _c_group = gdt.EndGroup("C group")
     _t_group = gdt.EndTabGroup("T group")
 
 
 class OtherDataSet(gdt.DataSet):
     """Another example dataset"""
```

### Comparing `guidata-3.0.0/guidata/tests/test_importwizard.py` & `guidata-3.0.1/guidata/tests/test_importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_inheritance.py` & `guidata-3.0.1/guidata/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_item_order.py` & `guidata-3.0.1/guidata/tests/test_item_order.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_loadsave_hdf5.py` & `guidata-3.0.1/guidata/tests/test_loadsave_hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 file.
 """
 
 # guitest: show
 
 import os
 
-from guidata.dataset.hdf5io import HDF5Reader, HDF5Writer
+from guidata.dataset.io import HDF5Reader, HDF5Writer
 from guidata.env import execenv
 from guidata.qthelpers import qt_app_context
 from guidata.tests.test_all_items import Parameters
 
 
 def test_loadsave_hdf5():
     """Test HDF5 I/O"""
```

### Comparing `guidata-3.0.0/guidata/tests/test_loadsave_json.py` & `guidata-3.0.1/guidata/tests/test_loadsave_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 This script shows how to save in and then reload data from a JSON file.
 """
 
 # guitest: show
 
 import os
 
-from guidata.dataset.jsonio import JSONReader, JSONWriter
+from guidata.dataset.io import JSONReader, JSONWriter
 from guidata.env import execenv
 from guidata.qthelpers import qt_app_context
 from guidata.tests.test_all_items import Parameters
 
 
 def test_loadsave_json():
     """Test JSON I/O"""
```

### Comparing `guidata-3.0.0/guidata/tests/test_objecteditor.py` & `guidata-3.0.1/guidata/tests/test_objecteditor.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,37 +7,43 @@
 """
 
 # guitest: show
 
 import datetime
 
 import numpy as np
-import PIL.Image
+
+try:
+    from PIL import Image
+except ImportError:
+    # PIL is not installed
+    Image = None
 
 from guidata.env import execenv
 from guidata.qthelpers import qt_app_context
 from guidata.widgets.objecteditor import oedit
 
 
 def test_objecteditor():
     """Run object editor test"""
     with qt_app_context():
-        data = np.random.randint(255, size=(100, 100)).astype("uint8")
-        image = PIL.Image.fromarray(data)
         example = {
             "str": "kjkj kj k j j kj k jkj",
             "list": [1, 3, 4, "kjkj", None],
             "dict": {"d": 1, "a": np.random.rand(10, 10), "b": [1, 2]},
             "float": 1.2233,
             "array": np.random.rand(10, 10),
-            "image": image,
             "date": datetime.date(1945, 5, 8),
             "datetime": datetime.datetime(1945, 5, 8),
         }
-        image = oedit(image)
+        if Image is not None:
+            data = np.random.randint(255, size=(100, 100)).astype("uint8")
+            image = Image.fromarray(data)
+            example["image"] = image
+            image = oedit(image)
 
         class Foobar:
             """ """
 
             def __init__(self):
                 self.text = "toto"
```

### Comparing `guidata-3.0.0/guidata/tests/test_rotatedlabel.py` & `guidata-3.0.1/guidata/tests/test_rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_text.py` & `guidata-3.0.1/guidata/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/tests/test_userconfig_app.py` & `guidata-3.0.1/guidata/tests/test_userconfig_app.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/userconfig.py` & `guidata-3.0.1/guidata/userconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,34 @@
 #    HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 #    WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 #    FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 #    OTHER DEALINGS IN THE SOFTWARE.
 
 
 """
-userconfig
-----------
+User configuration management
+-----------------------------
 
 The ``guidata.userconfig`` module provides user configuration file (.ini file)
 management features based on ``ConfigParser`` (standard Python library).
 
 It is the exact copy of the open-source package `userconfig` (MIT license).
+
+This module provides the following functions and classes:
+
+* :py:func:`get_home_dir`: return user home directory
+* :py:func:`get_config_basedir`: return user configuration base directory
+* :py:class:`UserConfig`: user configuration file management class
+
+.. autofunction:: get_home_dir
+
+.. autofunction:: get_config_basedir
+
+.. autoclass:: UserConfig
+    :members:
 """
 
 import configparser as cp
 import os
 import os.path as osp
 import re
 import sys
```

### Comparing `guidata-3.0.0/guidata/utils/__init__.py` & `guidata-3.0.1/guidata/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ) -> None:
     """Update `dest` dataset items from `source` dataset.
 
     Args:
         dest (DataSet): The destination dataset object to update.
         source (Union[Any, Dict[str, Any]]): The source object or dictionary containing
            matching attribute names.
-        visible_only (bool, optional): If True, update only visible items. Defaults
+        visible_only (bool): If True, update only visible items. Defaults
            to False.
 
     For each DataSet item, the function will try to get the attribute
     of the same name from the source.
 
     If the attribute exists in the source object or the key exists in the dictionary,
     it will be set as the corresponding attribute in the destination dataset.
```

### Comparing `guidata-3.0.0/guidata/utils/disthelpers.py` & `guidata-3.0.1/guidata/utils/disthelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/utils/encoding.py` & `guidata-3.0.1/guidata/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/utils/gettext_helpers.py` & `guidata-3.0.1/guidata/utils/gettext_helpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/utils/misc.py` & `guidata-3.0.1/guidata/utils/misc.py`

 * *Files 11% similar despite different names*

```diff
@@ -158,18 +158,18 @@
 def run_program(
     name, args: str = "", cwd: str = None, shell: bool = True, wait: bool = False
 ) -> None:
     """Run program in a separate process.
 
     Args:
         name (str): The program name.
-        args (str, optional): The program arguments. Defaults to "".""
-        cwd (str, optional): The current working directory. Defaults to None.
-        shell (bool, optional): If True, run program in a shell. Defaults to True.
-        wait (bool, optional): If True, wait for program to finish. Defaults to False.
+        args (str): The program arguments. Defaults to "".""
+        cwd (str): The current working directory. Defaults to None.
+        shell (bool): If True, run program in a shell. Defaults to True.
+        wait (bool): If True, wait for program to finish. Defaults to False.
 
     Raises:
         RuntimeError: If program is not installed.
     """
     path = is_program_installed(name)
     if not path:
         raise RuntimeError("Program %s was not found" % name)
@@ -279,7 +279,65 @@
         # Removing trailing single backslash
         if path.endswith("\\") and not path.endswith("\\\\"):
             path = path[:-1]
         # Replacing backslashes by slashes
         path = path.replace("\\", "/")
         path = path.replace("/'", "\\'")
     return path
+
+
+def convert_date_format(format_string: str) -> str:
+    """
+    Converts a date format string in Python strftime format to QDateTime style format.
+
+    Args:
+        format_string: The date format string in Python strftime format.
+
+    Returns:
+        The converted date format string in QDateTime style.
+
+    Examples:
+        >>> format_string = '%d.%m.%Y'
+        >>> qt_format = convert_date_format(format_string)
+        >>> print(qt_format)
+        dd.MM.yyyy
+    """
+    format_mapping = {
+        "%d": "dd",
+        "%-d": "d",
+        "%dd": "dd",
+        "%-dd": "d",
+        "%ddd": "ddd",
+        "%dddd": "dddd",
+        "%b": "MMM",
+        "%B": "MMMM",
+        "%m": "MM",
+        "%-m": "M",
+        "%mm": "MM",
+        "%-mm": "M",
+        "%y": "yy",
+        "%Y": "yyyy",
+        "%I": "h",
+        "%H": "HH",
+        "%-H": "H",
+        "%M": "mm",
+        "%-M": "m",
+        "%S": "ss",
+        "%-S": "s",
+        "%z": "z",
+        "%Z": "zzz",
+    }
+
+    qt_format = ""
+    i = 0
+    while i < len(format_string):
+        if format_string[i : i + 2] in format_mapping:
+            qt_format += format_mapping[format_string[i : i + 2]]
+            i += 2
+        elif format_string[i] in format_mapping:
+            qt_format += format_mapping[format_string[i]]
+            i += 1
+        else:
+            qt_format += format_string[i]
+            i += 1
+
+    return qt_format
```

### Comparing `guidata-3.0.0/guidata/widgets/__init__.py` & `guidata-3.0.1/guidata/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/arrayeditor.py` & `guidata-3.0.1/guidata/widgets/arrayeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/codeeditor.py` & `guidata-3.0.1/guidata/widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/collectionseditor.py` & `guidata-3.0.1/guidata/widgets/collectionseditor.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # (see spyder/__init__.py for details)
 # ----------------------------------------------------------------------------
 
 """
 guidata.widgets.collectionseditor
 =================================
 
-This package provides a Collections (i.e. dictionary, list and tuple) editor widget and dialog.
+This package provides a Collections (i.e. dictionary, list and tuple) editor widget
+and dialog.
 
 .. autoclass:: CollectionsEditor
 
 """
 
 # TODO: Multiple selection: open as many editors (array/dict/...) as necessary,
 #      at the same time
@@ -27,38 +28,73 @@
 
 import datetime
 import io
 import re
 import sys
 import warnings
 
-import PIL.Image
+try:
+    from PIL import Image as PILImage
+except ImportError:
+    PILImage = None
+from qtpy.compat import getsavefilename
+from qtpy.QtCore import QAbstractTableModel, QDateTime, QModelIndex, Qt, Signal, Slot
+from qtpy.QtGui import QColor, QKeySequence
+from qtpy.QtWidgets import (
+    QAbstractItemDelegate,
+    QApplication,
+    QDateEdit,
+    QDateTimeEdit,
+    QDialog,
+    QHBoxLayout,
+    QInputDialog,
+    QItemDelegate,
+    QLineEdit,
+    QMenu,
+    QMessageBox,
+    QPushButton,
+    QTableView,
+    QVBoxLayout,
+    QWidget,
+)
+
 from guidata.config import CONF, _
 from guidata.configtools import get_font, get_icon
-from guidata.qthelpers import (add_actions, create_action, mimedata2url,
-                               win32_fix_title_bar_background)
+from guidata.qthelpers import (
+    add_actions,
+    create_action,
+    mimedata2url,
+    win32_fix_title_bar_background,
+)
 from guidata.utils.misc import getcwd_or_home
 from guidata.widgets.importwizard import ImportWizard
-from guidata.widgets.nsview import (DataFrame, DatetimeIndex, FakeObject,
-                                    Image, MaskedArray, Series, array,
-                                    display_to_value, get_color_name,
-                                    get_human_readable_type, get_object_attrs,
-                                    get_size, get_type_string,
-                                    is_editable_type, is_known_type, ndarray,
-                                    np_savetxt, sort_against, try_to_eval,
-                                    unsorted_unique, value_to_display)
+from guidata.widgets.nsview import (
+    DataFrame,
+    DatetimeIndex,
+    FakeObject,
+    Image,
+    MaskedArray,
+    Series,
+    array,
+    display_to_value,
+    get_color_name,
+    get_human_readable_type,
+    get_object_attrs,
+    get_size,
+    get_type_string,
+    is_editable_type,
+    is_known_type,
+    ndarray,
+    np_savetxt,
+    sort_against,
+    try_to_eval,
+    unsorted_unique,
+    value_to_display,
+)
 from guidata.widgets.texteditor import TextEditor
-from qtpy.compat import getsavefilename
-from qtpy.QtCore import (QAbstractTableModel, QDateTime, QModelIndex, Qt,
-                         Signal, Slot)
-from qtpy.QtGui import QColor, QKeySequence
-from qtpy.QtWidgets import (QAbstractItemDelegate, QApplication, QDateEdit,
-                            QDateTimeEdit, QDialog, QHBoxLayout, QInputDialog,
-                            QItemDelegate, QLineEdit, QMenu, QMessageBox,
-                            QPushButton, QTableView, QVBoxLayout, QWidget)
 
 if ndarray is not FakeObject:
     from guidata.widgets.arrayeditor import ArrayEditor
 
 if DataFrame is not FakeObject:
     from guidata.widgets.dataframeeditor import DataFrameEditor
 
@@ -74,15 +110,19 @@
         if not re.match(r"[a-zA-Z]", name[0]):
             name = name[1:]
             continue
     name = str(name)
     if not name:
         name = "data"
     if blacklist is not None and name in blacklist:
-        get_new_name = lambda index: name + ("%03d" % index)
+
+        def get_new_name(index):
+            """Generate new name"""
+            return name + ("%03d" % index)
+
         index = 0
         while get_new_name(index) in blacklist:
             index += 1
         name = get_new_name(index)
     return name
 
 
@@ -243,29 +283,29 @@
         """Overriding sort method"""
         reverse = order == Qt.DescendingOrder
         if column == 0:
             self.sizes = sort_against(self.sizes, self.keys, reverse)
             self.types = sort_against(self.types, self.keys, reverse)
             try:
                 self.keys.sort(reverse=reverse)
-            except:
+            except Exception:  # pylint: disable=broad-except
                 pass
         elif column == 1:
             self.keys[: self.rows_loaded] = sort_against(self.keys, self.types, reverse)
             self.sizes = sort_against(self.sizes, self.types, reverse)
             try:
                 self.types.sort(reverse=reverse)
-            except:
+            except Exception:  # pylint: disable=broad-except
                 pass
         elif column == 2:
             self.keys[: self.rows_loaded] = sort_against(self.keys, self.sizes, reverse)
             self.types = sort_against(self.types, self.sizes, reverse)
             try:
                 self.sizes.sort(reverse=reverse)
-            except:
+            except Exception:  # pylint: disable=broad-except
                 pass
         elif column == 3:
             values = [self._data[key] for key in self.keys]
             self.keys = sort_against(self.keys, values, reverse)
             self.sizes = sort_against(self.sizes, values, reverse)
             self.types = sort_against(self.types, values, reverse)
         self.beginResetModel()
@@ -431,15 +471,14 @@
         self.dataChanged.emit(index, index)
         return True
 
 
 class CollectionsDelegate(QItemDelegate):
     """CollectionsEditor Item Delegate"""
 
-
     def __init__(self, parent=None):
         QItemDelegate.__init__(self, parent)
         self._editors = {}  # keep references on opened editors
 
     def get_value(self, index):
         """
 
@@ -469,15 +508,15 @@
 
         The problem is when a variable is too big, it can take a
         lot of time just to get its value
         """
         try:
             val_size = index.model().sizes[index.row()]
             val_type = index.model().types[index.row()]
-        except:
+        except Exception:  # pylint: disable=broad-except
             return False
         if val_type in ["list", "tuple", "dict"] and int(val_size) > 1e5:
             return True
         else:
             return False
 
     def createEditor(self, parent, option, index):
@@ -544,15 +583,19 @@
             and ndarray is not FakeObject
             and Image is not FakeObject
         ):
             arr = array(value)
             editor = ArrayEditor(parent=parent)
             if not editor.setup_and_check(arr, title=key, readonly=readonly):
                 return
-            conv_func = lambda arr: PIL.Image.fromarray(arr, mode=value.mode)
+
+            def conv_func(arr):
+                """Conversion function"""
+                return PILImage.fromarray(arr, mode=value.mode)
+
             self.create_dialog(
                 editor,
                 dict(
                     model=index.model(),
                     editor=editor,
                     key=key,
                     readonly=readonly,
@@ -686,15 +729,15 @@
         Model --> Editor
         """
         value = self.get_value(index)
         if isinstance(editor, QLineEdit):
             if isinstance(value, bytes):
                 try:
                     value = str(value, "utf8")
-                except:
+                except Exception:  # pylint: disable=broad-except
                     pass
             if not isinstance(value, str):
                 value = repr(value)
             editor.setText(value)
         elif isinstance(editor, QDateEdit):
             editor.setDate(value)
         elif isinstance(editor, QDateTimeEdit):
@@ -1169,22 +1212,22 @@
             self.new_value(key, try_to_eval(str(value)))
 
     def __prepare_plot(self):
         try:
             import guiqwt.pyplot  # analysis:ignore
 
             return True
-        except:
+        except Exception:  # pylint: disable=broad-except
             try:
                 if "matplotlib" not in sys.modules:
                     import matplotlib
 
                     matplotlib.use("Qt5Agg")
                 return True
-            except:
+            except Exception:  # pylint: disable=broad-except
                 QMessageBox.warning(
                     self,
                     _("Import error"),
                     _("Please install <b>matplotlib</b>" " or <b>guiqwt</b>."),
                 )
 
     def plot_item(self, funcname):
@@ -1258,28 +1301,28 @@
             obj = self.delegate.get_value(idx)
             # Check if we are trying to copy a numpy array, and if so make sure
             # to copy the whole thing in a tab separated format
             if isinstance(obj, (ndarray, MaskedArray)) and ndarray is not FakeObject:
                 output = io.BytesIO()
                 try:
                     np_savetxt(output, obj, delimiter="\t")
-                except:
+                except Exception:  # pylint: disable=broad-except
                     QMessageBox.warning(
                         self,
                         _("Warning"),
                         _("It was not possible to copy " "this array"),
                     )
                     return
                 obj = output.getvalue().decode("utf-8")
                 output.close()
             elif isinstance(obj, (DataFrame, Series)) and DataFrame is not FakeObject:
                 output = io.StringIO()
                 try:
                     obj.to_csv(output, sep="\t", index=True, header=True)
-                except Exception:
+                except Exception:  # pylint: disable=broad-except
                     QMessageBox.warning(
                         self,
                         _("Warning"),
                         _("It was not possible to copy " "this dataframe"),
                     )
                     return
                 obj = output.getvalue()
```

### Comparing `guidata-3.0.0/guidata/widgets/console/__init__.py` & `guidata-3.0.1/guidata/widgets/console/__init__.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/base.py` & `guidata-3.0.1/guidata/widgets/console/base.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/calltip.py` & `guidata-3.0.1/guidata/widgets/console/calltip.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/dochelpers.py` & `guidata-3.0.1/guidata/widgets/console/dochelpers.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/internalshell.py` & `guidata-3.0.1/guidata/widgets/console/internalshell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/interpreter.py` & `guidata-3.0.1/guidata/widgets/console/interpreter.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/mixins.py` & `guidata-3.0.1/guidata/widgets/console/mixins.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/shell.py` & `guidata-3.0.1/guidata/widgets/console/shell.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/console/terminal.py` & `guidata-3.0.1/guidata/widgets/console/terminal.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/dataframeeditor.py` & `guidata-3.0.1/guidata/widgets/dataframeeditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/dockable.py` & `guidata-3.0.1/guidata/widgets/dockable.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         location: Qt.DockWidgetArea | None = None,
         features: QDockWidget.DockWidgetFeatures | None = None,
         allowed_areas: Qt.DockWidgetAreas | None = None,
     ) -> None:
         """Setup dockwidget parameters
 
         Args:
-            location (Qt.DockWidgetArea, optional): Dockwidget location
-            features (QDockWidget.DockWidgetFeatures, optional): Dockwidget features
-            allowed_areas (Qt.DockWidgetAreas, optional): Dockwidget allowed areas
+            location (Qt.DockWidgetArea): Dockwidget location
+            features (QDockWidget.DockWidgetFeatures): Dockwidget features
+            allowed_areas (Qt.DockWidgetAreas): Dockwidget allowed areas
         """
         assert (
             self.dockwidget is None
         ), "Dockwidget must be setup before calling 'create_dockwidget'"
         if location is not None:
             self._location = location
         if features is not None:
```

### Comparing `guidata-3.0.0/guidata/widgets/importwizard.py` & `guidata-3.0.1/guidata/widgets/importwizard.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/nsview.py` & `guidata-3.0.1/guidata/widgets/nsview.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/objecteditor.py` & `guidata-3.0.1/guidata/widgets/objecteditor.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,25 @@
 
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import PIL.Image
+try:
+    from PIL import Image as PILImage
+except ImportError:
+    PILImage = None
+from numpy.core.multiarray import ndarray
+
 from guidata.qthelpers import exec_dialog
 from guidata.widgets.arrayeditor import ArrayEditor
 from guidata.widgets.collectionseditor import CollectionsEditor
 from guidata.widgets.nsview import DataFrame, FakeObject, Series, is_known_type
 from guidata.widgets.texteditor import TextEditor
-from numpy.core.multiarray import ndarray
 
 try:
     from guidata.widgets.dataframeeditor import DataFrameEditor
 except ImportError:
     DataFrameEditor = FakeObject()
 
 
@@ -43,28 +47,35 @@
     quitting the dialog box
 
     The role of this intermediate function is to allow easy monkey-patching.
     (uschmitt suggested this indirection here so that he can monkey patch
     oedit to show eMZed related data)
     """
 
-    conv_func = lambda data: data
+    def conv_func(data):
+        """Conversion function"""
+        return data
+
     readonly = not is_known_type(obj)
     if isinstance(obj, ndarray):
         dialog = ArrayEditor(parent)
         if not dialog.setup_and_check(obj, title=title, readonly=readonly):
             return
-    elif isinstance(obj, PIL.Image.Image):
+    elif PILImage is not None and isinstance(obj, PILImage.Image):
         dialog = ArrayEditor(parent)
         import numpy as np
 
         data = np.array(obj)
         if not dialog.setup_and_check(data, title=title, readonly=readonly):
             return
-        conv_func = lambda data: PIL.Image.fromarray(data, mode=obj.mode)
+
+        def conv_func(data):
+            """Conversion function"""
+            return PILImage.fromarray(data, mode=obj.mode)
+
     elif isinstance(obj, (DataFrame, Series)) and DataFrame is not FakeObject:
         dialog = DataFrameEditor(parent)
         if not dialog.setup_and_check(obj):
             return
     elif isinstance(obj, str):
         dialog = TextEditor(obj, title=title, readonly=readonly, parent=parent)
     else:
@@ -88,16 +99,16 @@
     parent: QW.QWidget = None,
 ) -> dict | list | tuple | str | np.ndarray:
     """Edit the object 'obj' in a GUI-based editor and return the edited copy
     (if Cancel is pressed, return None)
 
     Args:
         obj (dict | list | tuple | str | np.ndarray): object to edit
-        title (str, optional): dialog title
-        parent (QW.QWidget, optional): parent widget
+        title (str): dialog title
+        parent (QW.QWidget): parent widget
 
     Returns:
         dict | list | tuple | str | np.ndarray: edited object
     """
     title = "" if title is None else title
     result = create_dialog(obj, title, parent)
     if result is None:
```

### Comparing `guidata-3.0.0/guidata/widgets/rotatedlabel.py` & `guidata-3.0.1/guidata/widgets/rotatedlabel.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/syntaxhighlighters.py` & `guidata-3.0.1/guidata/widgets/syntaxhighlighters.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata/widgets/texteditor.py` & `guidata-3.0.1/guidata/widgets/texteditor.py`

 * *Files identical despite different names*

### Comparing `guidata-3.0.0/guidata.egg-info/SOURCES.txt` & `guidata-3.0.1/guidata.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,10 @@
-CHANGELOG.md
 LICENSE
-MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-doc/basic_example.py
-doc/conf.py
-doc/examples.rst
-doc/index.rst
-doc/installation.rst
-doc/overview.rst
-doc/_static/favicon.ico
-doc/dev/contribute.rst
-doc/dev/howto.rst
-doc/dev/index.rst
-doc/dev/v2_to_v3.rst
-doc/images/basic_example.png
-doc/images/guidata-banner.png
-doc/images/guidata-vertical.png
-doc/images/layout_example.png
-doc/images/screenshots/__init__.png
-doc/images/screenshots/activable_dataset.png
-doc/images/screenshots/all_features.png
-doc/images/screenshots/all_items.png
-doc/images/screenshots/bool_selector.png
-doc/images/screenshots/datasetgroup.png
-doc/images/screenshots/editgroupbox.png
-doc/reference/guitest.rst
-doc/reference/index.rst
-doc/reference/utils.rst
-doc/reference/widgets.rst
-doc/reference/dataset/dataitems.rst
-doc/reference/dataset/datatypes.rst
-doc/reference/dataset/index.rst
-doc/reference/dataset/qtwidgets.rst
 guidata/__init__.py
 guidata/config.py
 guidata/configtools.py
 guidata/env.py
 guidata/guidata.chm
 guidata/guitest.py
 guidata/qthelpers.py
@@ -46,20 +13,22 @@
 guidata.egg-info/SOURCES.txt
 guidata.egg-info/dependency_links.txt
 guidata.egg-info/requires.txt
 guidata.egg-info/top_level.txt
 guidata/dataset/__init__.py
 guidata/dataset/dataitems.py
 guidata/dataset/datatypes.py
-guidata/dataset/hdf5io.py
-guidata/dataset/iniio.py
-guidata/dataset/jsonio.py
 guidata/dataset/qtitemwidgets.py
 guidata/dataset/qtwidgets.py
 guidata/dataset/textedit.py
+guidata/dataset/io/__init__.py
+guidata/dataset/io/base.py
+guidata/dataset/io/h5fmt.py
+guidata/dataset/io/inifmt.py
+guidata/dataset/io/jsonfmt.py
 guidata/external/__init__.py
 guidata/external/darkdetect/__init__.py
 guidata/external/darkdetect/_dummy.py
 guidata/external/darkdetect/_linux_detect.py
 guidata/external/darkdetect/_mac_detect.py
 guidata/external/darkdetect/_windows_detect.py
 guidata/images/apply.png
@@ -121,17 +90,15 @@
 guidata/images/filetypes/ps.png
 guidata/images/filetypes/tar.png
 guidata/images/filetypes/tgz.png
 guidata/images/filetypes/tif.png
 guidata/images/filetypes/txt.png
 guidata/images/filetypes/xls.png
 guidata/images/filetypes/zip.png
-guidata/locale/guidata.pot
 guidata/locale/fr/LC_MESSAGES/guidata.mo
-guidata/locale/fr/LC_MESSAGES/guidata.po
 guidata/tests/__init__.py
 guidata/tests/_all_tests.py
 guidata/tests/conftest.py
 guidata/tests/test_activable_dataset.py
 guidata/tests/test_activable_items.py
 guidata/tests/test_all_features.py
 guidata/tests/test_all_items.py
@@ -143,24 +110,28 @@
 guidata/tests/test_config.py
 guidata/tests/test_console.py
 guidata/tests/test_data.py
 guidata/tests/test_dataframeeditor.py
 guidata/tests/test_datasetgroup.py
 guidata/tests/test_disthelpers.py
 guidata/tests/test_editgroupbox.py
+guidata/tests/test_genreqs.py
 guidata/tests/test_importwizard.py
 guidata/tests/test_inheritance.py
 guidata/tests/test_item_order.py
 guidata/tests/test_loadsave_hdf5.py
 guidata/tests/test_loadsave_json.py
+guidata/tests/test_no_qt.py
 guidata/tests/test_objecteditor.py
 guidata/tests/test_rotatedlabel.py
 guidata/tests/test_text.py
 guidata/tests/test_translations.py
 guidata/tests/test_userconfig_app.py
+guidata/tests/data/genreqs/pyproject.toml
+guidata/tests/data/genreqs/setup.cfg
 guidata/utils/__init__.py
 guidata/utils/disthelpers.py
 guidata/utils/encoding.py
 guidata/utils/genreqs.py
 guidata/utils/gettext_helpers.py
 guidata/utils/misc.py
 guidata/widgets/__init__.py
```

