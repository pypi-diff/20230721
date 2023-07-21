# Comparing `tmp/fishy-0.5.8.tar.gz` & `tmp/fishy-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fishy-0.5.8.tar", last modified: Sat Feb 26 17:41:01 2022, max compression
+gzip compressed data, was "dist\fishy-0.5.9.tar", last modified: Fri Mar 18 05:08:26 2022, max compression
```

## Comparing `fishy-0.5.8.tar` & `fishy-0.5.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/
--rw-rw-rw-   0        0        0     1104 2019-02-03 06:58:31.000000 fishy-0.5.8/LICENSE
--rw-rw-rw-   0        0        0      289 2021-03-28 05:40:42.000000 fishy-0.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2157 2022-02-26 17:41:01.000000 fishy-0.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2022-01-31 08:04:06.000000 fishy-0.5.8/README.md
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/
--rw-rw-rw-   0        0        0      206 2022-01-31 07:56:40.000000 fishy-0.5.8/fishy/__init__.py
--rw-rw-rw-   0        0        0     2411 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/__main__.py
--rw-rw-rw-   0        0        0    20840 2020-11-30 22:45:35.000000 fishy-0.5.8/fishy/beep.wav
--rw-rw-rw-   0        0        0      461 2022-02-26 17:40:49.000000 fishy-0.5.8/fishy/constants.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/engine/
--rw-rw-rw-   0        0        0       61 2020-06-01 09:00:06.000000 fishy-0.5.8/fishy/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/engine/common/
--rw-rw-rw-   0        0        0     2340 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/common/IEngine.py
--rw-rw-rw-   0        0        0        0 2020-11-30 22:45:35.000000 fishy-0.5.8/fishy/engine/common/__init__.py
--rw-rw-rw-   0        0        0     2290 2022-02-26 17:40:49.000000 fishy-0.5.8/fishy/engine/common/event_handler.py
--rw-rw-rw-   0        0        0     1607 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/common/qr_detection.py
--rw-rw-rw-   0        0        0     3420 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/common/window.py
--rw-rw-rw-   0        0        0     3506 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/common/window_server.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/engine/fullautofisher/
--rw-rw-rw-   0        0        0        0 2020-06-25 01:29:58.000000 fishy-0.5.8/fishy/engine/fullautofisher/__init__.py
--rw-rw-rw-   0        0        0     1336 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/fullautofisher/controls.py
--rw-rw-rw-   0        0        0     7150 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/fullautofisher/engine.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/engine/fullautofisher/mode/
--rw-rw-rw-   0        0        0        0 2021-05-15 13:01:59.000000 fishy-0.5.8/fishy/engine/fullautofisher/mode/__init__.py
--rw-rw-rw-   0        0        0     3396 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/fullautofisher/mode/calibrator.py
--rw-rw-rw-   0        0        0      204 2021-05-15 13:01:59.000000 fishy-0.5.8/fishy/engine/fullautofisher/mode/imode.py
--rw-rw-rw-   0        0        0     3712 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/fullautofisher/mode/player.py
--rw-rw-rw-   0        0        0     5374 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/fullautofisher/mode/recorder.py
--rw-rw-rw-   0        0        0      988 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/engine/fullautofisher/test.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/engine/semifisher/
--rw-rw-rw-   0        0        0        0 2020-05-23 04:46:15.000000 fishy-0.5.8/fishy/engine/semifisher/__init__.py
--rw-rw-rw-   0        0        0     3700 2022-02-26 17:40:49.000000 fishy-0.5.8/fishy/engine/semifisher/engine.py
--rw-rw-rw-   0        0        0     4930 2022-02-26 17:40:49.000000 fishy-0.5.8/fishy/engine/semifisher/fishing_event.py
--rw-rw-rw-   0        0        0     1127 2022-02-26 17:40:49.000000 fishy-0.5.8/fishy/engine/semifisher/fishing_mode.py
--rw-rw-rw-   0        0        0   463113 2020-04-11 20:41:10.000000 fishy-0.5.8/fishy/fishybot_logo.png
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/gui/
--rw-rw-rw-   0        0        0       57 2020-05-16 04:43:04.000000 fishy-0.5.8/fishy/gui/__init__.py
--rw-rw-rw-   0        0        0     6524 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/gui/config_top.py
--rw-rw-rw-   0        0        0     2633 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/gui/discord_login.py
--rw-rw-rw-   0        0        0     1407 2021-05-22 00:43:11.000000 fishy-0.5.8/fishy/gui/funcs.py
--rw-rw-rw-   0        0        0     3233 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/gui/gui.py
--rw-rw-rw-   0        0        0     1230 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/gui/log_config.py
--rw-rw-rw-   0        0        0     5988 2022-02-26 17:40:49.000000 fishy-0.5.8/fishy/gui/main_gui.py
--rw-rw-rw-   0        0        0     1673 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/gui/splash.py
--rw-rw-rw-   0        0        0     3105 2022-02-02 19:59:32.000000 fishy-0.5.8/fishy/gui/terms_gui.py
--rw-rw-rw-   0        0        0     2302 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/gui/update_dialog.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/helper/
--rw-rw-rw-   0        0        0      463 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/__init__.py
--rw-rw-rw-   0        0        0      690 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/active_poll.py
--rw-rw-rw-   0        0        0     2710 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/auto_update.py
--rw-rw-rw-   0        0        0     4389 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/config.py
--rw-rw-rw-   0        0        0     7569 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/helper.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/helper/hotkey/
--rw-rw-rw-   0        0        0        0 2021-05-21 23:22:09.000000 fishy-0.5.8/fishy/helper/hotkey/__init__.py
--rw-rw-rw-   0        0        0     1993 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/hotkey/hotkey_process.py
--rw-rw-rw-   0        0        0      901 2021-05-21 23:22:09.000000 fishy-0.5.8/fishy/helper/hotkey/process.py
--rw-rw-rw-   0        0        0     2716 2021-05-15 13:01:07.000000 fishy-0.5.8/fishy/helper/luaparser.py
--rw-rw-rw-   0        0        0      822 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/migration.py
--rw-rw-rw-   0        0        0      997 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/helper/popup.py
--rw-rw-rw-   0        0        0   105721 2020-04-19 13:42:00.000000 fishy-0.5.8/fishy/icon.ico
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/libs/
--rw-rw-rw-   0        0        0       26 2020-05-20 10:45:41.000000 fishy-0.5.8/fishy/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/libs/tkhtmlview/
--rw-rw-rw-   0        0        0     4566 2020-05-20 10:59:01.000000 fishy-0.5.8/fishy/libs/tkhtmlview/__init__.py
--rw-rw-rw-   0        0        0    26456 2020-05-20 10:45:41.000000 fishy-0.5.8/fishy/libs/tkhtmlview/html_parser.py
--rw-rw-rw-   0        0        0     9856 2016-06-28 17:23:09.000000 fishy-0.5.8/fishy/sound.mp3
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy/web/
--rw-rw-rw-   0        0        0      183 2021-05-15 13:01:07.000000 fishy-0.5.8/fishy/web/__init__.py
--rw-rw-rw-   0        0        0      729 2022-02-01 14:33:36.000000 fishy-0.5.8/fishy/web/decorators.py
--rw-rw-rw-   0        0        0      663 2021-05-21 23:22:09.000000 fishy-0.5.8/fishy/web/urls.py
--rw-rw-rw-   0        0        0     4598 2022-02-03 01:36:32.000000 fishy-0.5.8/fishy/web/web.py
-drwxrwxrwx   0        0        0        0 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/
--rw-rw-rw-   0        0        0     2157 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1813 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      194 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-02-26 17:41:01.000000 fishy-0.5.8/fishy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      210 2022-01-31 07:56:40.000000 fishy-0.5.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-02-26 17:41:01.000000 fishy-0.5.8/setup.cfg
--rw-rw-rw-   0        0        0     9190 2021-05-15 13:01:07.000000 fishy-0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/
+-rw-rw-rw-   0        0        0     1104 2019-02-03 06:58:31.000000 fishy-0.5.9/LICENSE
+-rw-rw-rw-   0        0        0      289 2021-03-28 05:40:42.000000 fishy-0.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2157 2022-03-18 05:08:26.000000 fishy-0.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1176 2022-01-31 08:04:06.000000 fishy-0.5.9/README.md
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/
+-rw-rw-rw-   0        0        0      206 2022-01-31 07:56:40.000000 fishy-0.5.9/fishy/__init__.py
+-rw-rw-rw-   0        0        0     2411 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/__main__.py
+-rw-rw-rw-   0        0        0    20840 2020-11-30 22:45:35.000000 fishy-0.5.9/fishy/beep.wav
+-rw-rw-rw-   0        0        0      461 2022-03-18 05:08:14.000000 fishy-0.5.9/fishy/constants.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/engine/
+-rw-rw-rw-   0        0        0       61 2020-06-01 09:00:06.000000 fishy-0.5.9/fishy/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/engine/common/
+-rw-rw-rw-   0        0        0     2340 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/common/IEngine.py
+-rw-rw-rw-   0        0        0        0 2020-11-30 22:45:35.000000 fishy-0.5.9/fishy/engine/common/__init__.py
+-rw-rw-rw-   0        0        0     2290 2022-02-26 17:40:49.000000 fishy-0.5.9/fishy/engine/common/event_handler.py
+-rw-rw-rw-   0        0        0     1607 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/common/qr_detection.py
+-rw-rw-rw-   0        0        0     3420 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/common/window.py
+-rw-rw-rw-   0        0        0     3506 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/common/window_server.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/engine/fullautofisher/
+-rw-rw-rw-   0        0        0        0 2020-06-25 01:29:58.000000 fishy-0.5.9/fishy/engine/fullautofisher/__init__.py
+-rw-rw-rw-   0        0        0     1336 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/fullautofisher/controls.py
+-rw-rw-rw-   0        0        0     7150 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/fullautofisher/engine.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/engine/fullautofisher/mode/
+-rw-rw-rw-   0        0        0        0 2021-05-15 13:01:59.000000 fishy-0.5.9/fishy/engine/fullautofisher/mode/__init__.py
+-rw-rw-rw-   0        0        0     3396 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/fullautofisher/mode/calibrator.py
+-rw-rw-rw-   0        0        0      204 2021-05-15 13:01:59.000000 fishy-0.5.9/fishy/engine/fullautofisher/mode/imode.py
+-rw-rw-rw-   0        0        0     3712 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/fullautofisher/mode/player.py
+-rw-rw-rw-   0        0        0     5374 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/fullautofisher/mode/recorder.py
+-rw-rw-rw-   0        0        0      988 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/engine/fullautofisher/test.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/engine/semifisher/
+-rw-rw-rw-   0        0        0        0 2020-05-23 04:46:15.000000 fishy-0.5.9/fishy/engine/semifisher/__init__.py
+-rw-rw-rw-   0        0        0     3700 2022-02-26 17:40:49.000000 fishy-0.5.9/fishy/engine/semifisher/engine.py
+-rw-rw-rw-   0        0        0     4930 2022-02-26 17:40:49.000000 fishy-0.5.9/fishy/engine/semifisher/fishing_event.py
+-rw-rw-rw-   0        0        0     1127 2022-02-26 17:40:49.000000 fishy-0.5.9/fishy/engine/semifisher/fishing_mode.py
+-rw-rw-rw-   0        0        0   463113 2020-04-11 20:41:10.000000 fishy-0.5.9/fishy/fishybot_logo.png
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/gui/
+-rw-rw-rw-   0        0        0       57 2020-05-16 04:43:04.000000 fishy-0.5.9/fishy/gui/__init__.py
+-rw-rw-rw-   0        0        0     6524 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/gui/config_top.py
+-rw-rw-rw-   0        0        0     2633 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/gui/discord_login.py
+-rw-rw-rw-   0        0        0     1407 2021-05-22 00:43:11.000000 fishy-0.5.9/fishy/gui/funcs.py
+-rw-rw-rw-   0        0        0     3233 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/gui/gui.py
+-rw-rw-rw-   0        0        0     1230 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/gui/log_config.py
+-rw-rw-rw-   0        0        0     5988 2022-02-26 17:40:49.000000 fishy-0.5.9/fishy/gui/main_gui.py
+-rw-rw-rw-   0        0        0     1673 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/gui/splash.py
+-rw-rw-rw-   0        0        0     3105 2022-02-02 19:59:32.000000 fishy-0.5.9/fishy/gui/terms_gui.py
+-rw-rw-rw-   0        0        0     2302 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/gui/update_dialog.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/helper/
+-rw-rw-rw-   0        0        0      463 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/__init__.py
+-rw-rw-rw-   0        0        0      710 2022-03-18 05:07:49.000000 fishy-0.5.9/fishy/helper/active_poll.py
+-rw-rw-rw-   0        0        0     2710 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/auto_update.py
+-rw-rw-rw-   0        0        0     4389 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/config.py
+-rw-rw-rw-   0        0        0     7569 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/helper.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/helper/hotkey/
+-rw-rw-rw-   0        0        0        0 2021-05-21 23:22:09.000000 fishy-0.5.9/fishy/helper/hotkey/__init__.py
+-rw-rw-rw-   0        0        0     1993 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/hotkey/hotkey_process.py
+-rw-rw-rw-   0        0        0      901 2021-05-21 23:22:09.000000 fishy-0.5.9/fishy/helper/hotkey/process.py
+-rw-rw-rw-   0        0        0     2716 2021-05-15 13:01:07.000000 fishy-0.5.9/fishy/helper/luaparser.py
+-rw-rw-rw-   0        0        0      822 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/migration.py
+-rw-rw-rw-   0        0        0      997 2022-02-03 01:36:32.000000 fishy-0.5.9/fishy/helper/popup.py
+-rw-rw-rw-   0        0        0   105721 2020-04-19 13:42:00.000000 fishy-0.5.9/fishy/icon.ico
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/libs/
+-rw-rw-rw-   0        0        0       26 2020-05-20 10:45:41.000000 fishy-0.5.9/fishy/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/libs/tkhtmlview/
+-rw-rw-rw-   0        0        0     4566 2020-05-20 10:59:01.000000 fishy-0.5.9/fishy/libs/tkhtmlview/__init__.py
+-rw-rw-rw-   0        0        0    26456 2020-05-20 10:45:41.000000 fishy-0.5.9/fishy/libs/tkhtmlview/html_parser.py
+-rw-rw-rw-   0        0        0     9856 2016-06-28 17:23:09.000000 fishy-0.5.9/fishy/sound.mp3
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy/web/
+-rw-rw-rw-   0        0        0      183 2021-05-15 13:01:07.000000 fishy-0.5.9/fishy/web/__init__.py
+-rw-rw-rw-   0        0        0      729 2022-02-01 14:33:36.000000 fishy-0.5.9/fishy/web/decorators.py
+-rw-rw-rw-   0        0        0      663 2021-05-21 23:22:09.000000 fishy-0.5.9/fishy/web/urls.py
+-rw-rw-rw-   0        0        0     4725 2022-03-18 05:07:49.000000 fishy-0.5.9/fishy/web/web.py
+drwxrwxrwx   0        0        0        0 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy.egg-info/
+-rw-rw-rw-   0        0        0     2157 2022-03-18 05:08:25.000000 fishy-0.5.9/fishy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1813 2022-03-18 05:08:26.000000 fishy-0.5.9/fishy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-03-18 05:08:25.000000 fishy-0.5.9/fishy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2022-03-18 05:08:25.000000 fishy-0.5.9/fishy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      194 2022-03-18 05:08:25.000000 fishy-0.5.9/fishy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2022-03-18 05:08:25.000000 fishy-0.5.9/fishy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      210 2022-01-31 07:56:40.000000 fishy-0.5.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-03-18 05:08:26.000000 fishy-0.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     9190 2021-05-15 13:01:07.000000 fishy-0.5.9/setup.py
```

### Comparing `fishy-0.5.8/LICENSE` & `fishy-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/PKG-INFO` & `fishy-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fishy
-Version: 0.5.8
+Version: 0.5.9
 Summary: Fishing bot for Elder Scrolls Online
 Home-page: https://github.com/adsau59/fishyboteso
 Author: Adam Saudagar
 Author-email: adam_saudagar@live.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/adsau59/fishyboteso/issues/
 Project-URL: Funding, https://www.paypal.me/AdamSaudagar
```

### Comparing `fishy-0.5.8/README.md` & `fishy-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/__main__.py` & `fishy-0.5.9/fishy/__main__.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/beep.wav` & `fishy-0.5.9/fishy/beep.wav`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/common/IEngine.py` & `fishy-0.5.9/fishy/engine/common/IEngine.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/common/event_handler.py` & `fishy-0.5.9/fishy/engine/common/event_handler.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/common/qr_detection.py` & `fishy-0.5.9/fishy/engine/common/qr_detection.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/common/window.py` & `fishy-0.5.9/fishy/engine/common/window.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/common/window_server.py` & `fishy-0.5.9/fishy/engine/common/window_server.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/fullautofisher/controls.py` & `fishy-0.5.9/fishy/engine/fullautofisher/controls.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/fullautofisher/engine.py` & `fishy-0.5.9/fishy/engine/fullautofisher/engine.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/fullautofisher/mode/calibrator.py` & `fishy-0.5.9/fishy/engine/fullautofisher/mode/calibrator.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/fullautofisher/mode/player.py` & `fishy-0.5.9/fishy/engine/fullautofisher/mode/player.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/fullautofisher/mode/recorder.py` & `fishy-0.5.9/fishy/engine/fullautofisher/mode/recorder.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/fullautofisher/test.py` & `fishy-0.5.9/fishy/engine/fullautofisher/test.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/semifisher/engine.py` & `fishy-0.5.9/fishy/engine/semifisher/engine.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/semifisher/fishing_event.py` & `fishy-0.5.9/fishy/engine/semifisher/fishing_event.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/engine/semifisher/fishing_mode.py` & `fishy-0.5.9/fishy/engine/semifisher/fishing_mode.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/fishybot_logo.png` & `fishy-0.5.9/fishy/fishybot_logo.png`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/config_top.py` & `fishy-0.5.9/fishy/gui/config_top.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/discord_login.py` & `fishy-0.5.9/fishy/gui/discord_login.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/funcs.py` & `fishy-0.5.9/fishy/gui/funcs.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/gui.py` & `fishy-0.5.9/fishy/gui/gui.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/log_config.py` & `fishy-0.5.9/fishy/gui/log_config.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/main_gui.py` & `fishy-0.5.9/fishy/gui/main_gui.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/splash.py` & `fishy-0.5.9/fishy/gui/splash.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/terms_gui.py` & `fishy-0.5.9/fishy/gui/terms_gui.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/gui/update_dialog.py` & `fishy-0.5.9/fishy/gui/update_dialog.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/active_poll.py` & `fishy-0.5.9/fishy/helper/active_poll.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
         active._scheduler = EventScheduler()
         active._scheduler.start()
         logging.debug("active scheduler initialized")
 
     @staticmethod
     def start():
+        web.ping()
         active._scheduler.enter_recurring(60, 1, web.ping)
         logging.debug("active scheduler started")
 
     @staticmethod
     def stop():
         active._scheduler.stop(hard_stop=True)
         logging.debug("active scheduler stopped")
```

### Comparing `fishy-0.5.8/fishy/helper/auto_update.py` & `fishy-0.5.9/fishy/helper/auto_update.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/config.py` & `fishy-0.5.9/fishy/helper/config.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/helper.py` & `fishy-0.5.9/fishy/helper/helper.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/hotkey/hotkey_process.py` & `fishy-0.5.9/fishy/helper/hotkey/hotkey_process.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/hotkey/process.py` & `fishy-0.5.9/fishy/helper/hotkey/process.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/luaparser.py` & `fishy-0.5.9/fishy/helper/luaparser.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/migration.py` & `fishy-0.5.9/fishy/helper/migration.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/helper/popup.py` & `fishy-0.5.9/fishy/helper/popup.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/icon.ico` & `fishy-0.5.9/fishy/icon.ico`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/libs/tkhtmlview/__init__.py` & `fishy-0.5.9/fishy/libs/tkhtmlview/__init__.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/libs/tkhtmlview/html_parser.py` & `fishy-0.5.9/fishy/libs/tkhtmlview/html_parser.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/sound.mp3` & `fishy-0.5.9/fishy/sound.mp3`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/web/decorators.py` & `fishy-0.5.9/fishy/web/decorators.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/web/urls.py` & `fishy-0.5.9/fishy/web/urls.py`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/fishy/web/web.py` & `fishy-0.5.9/fishy/web/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,41 +122,43 @@
 
     # then create session
     if uid:
         _session_id, online = _create_new_session(uid)
     # if not, create new id then try creating session again
     else:
         uid = register_user()
-        logging.debug("New User, generated new uid")
+        config.set("uid", uid, True)
+        logging.debug(f"New User, generated new uid: {uid}")
         if uid:
             _session_id, online = _create_new_session(uid)
         else:
             online = False
 
     # when the user is already registered but session is not created as uid is not found
     if online and not _session_id:
         logging.error("user not found, generating new uid.. contact dev if you don't want to loose data")
         new_uid = register_user()
         _session_id, online = _create_new_session(new_uid)
-        config.set("uid", new_uid)
-        config.set("old_uid", uid)
+        config.set("uid", new_uid, True)
+        config.set("old_uid", uid, True)
 
     return _session_id
 
 
 @fallback((None, False))
 def _create_new_session(uid):
     body = {"uid": uid, "apiversion": apiversion}
     response = requests.post(urls.session, params=body)
 
     if response.status_code == 405:
         return None, True
 
     return response.json()["session_id"], True
 
+
 @fallback(False)
 def has_beta():
     body = {"uid": config.get("uid"), "apiversion": apiversion}
     response = requests.get(urls.beta, params=body)
     result = response.json()
 
     if not result["success"]:
@@ -164,8 +166,9 @@
 
     return response.json()["beta"]
 
 
 @fallback(None)
 def ping():
     body = {"uid": config.get("uid"), "apiversion": apiversion}
-    requests.post(urls.ping, params=body)
+    response = requests.post(urls.ping, params=body)
+    logging.debug(f"ping response: {response.json()}")
```

### Comparing `fishy-0.5.8/fishy.egg-info/PKG-INFO` & `fishy-0.5.9/fishy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fishy
-Version: 0.5.8
+Version: 0.5.9
 Summary: Fishing bot for Elder Scrolls Online
 Home-page: https://github.com/adsau59/fishyboteso
 Author: Adam Saudagar
 Author-email: adam_saudagar@live.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/adsau59/fishyboteso/issues/
 Project-URL: Funding, https://www.paypal.me/AdamSaudagar
```

### Comparing `fishy-0.5.8/fishy.egg-info/SOURCES.txt` & `fishy-0.5.9/fishy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fishy-0.5.8/setup.py` & `fishy-0.5.9/setup.py`

 * *Files identical despite different names*

