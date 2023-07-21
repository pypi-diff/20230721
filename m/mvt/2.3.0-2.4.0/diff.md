# Comparing `tmp/mvt-2.3.0.tar.gz` & `tmp/mvt-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvt-2.3.0.tar", last modified: Thu Jun 29 15:10:48 2023, max compression
+gzip compressed data, was "mvt-2.4.0.tar", last modified: Fri Jul 21 10:21:45 2023, max compression
```

## Comparing `mvt-2.3.0.tar` & `mvt-2.4.0.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.301082 mvt-2.3.0/
--rw-r--r--   0 donncha    (501) staff       (20)    17791 2022-06-22 15:39:11.000000 mvt-2.3.0/LICENSE
--rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-06-29 15:10:48.301158 mvt-2.3.0/PKG-INFO
--rw-r--r--   0 donncha    (501) staff       (20)     3711 2023-06-29 14:48:56.000000 mvt-2.3.0/README.md
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.272590 mvt-2.3.0/mvt/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.274896 mvt-2.3.0/mvt/android/
--rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/android/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)    11065 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cli.py
--rw-r--r--   0 donncha    (501) staff       (20)     1007 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_adb.py
--rw-r--r--   0 donncha    (501) staff       (20)     1094 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_androidqf.py
--rw-r--r--   0 donncha    (501) staff       (20)     3727 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_backup.py
--rw-r--r--   0 donncha    (501) staff       (20)     2598 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_check_bugreport.py
--rw-r--r--   0 donncha    (501) staff       (20)     6138 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/cmd_download_apks.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.275045 mvt-2.3.0/mvt/android/modules/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/android/modules/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.278345 mvt-2.3.0/mvt/android/modules/adb/
--rw-r--r--   0 donncha    (501) staff       (20)     1290 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)    12370 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     3274 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/chrome_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     1798 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_accessibility.py
--rw-r--r--   0 donncha    (501) staff       (20)     1779 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_activities.py
--rw-r--r--   0 donncha    (501) staff       (20)     2779 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_appops.py
--rw-r--r--   0 donncha    (501) staff       (20)     1992 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_daily.py
--rw-r--r--   0 donncha    (501) staff       (20)     1635 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     1757 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_dbinfo.py
--rw-r--r--   0 donncha    (501) staff       (20)     1353 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_full.py
--rw-r--r--   0 donncha    (501) staff       (20)     3269 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/dumpsys_receivers.py
--rw-r--r--   0 donncha    (501) staff       (20)     5185 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/files.py
--rw-r--r--   0 donncha    (501) staff       (20)     2190 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)     1820 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/logcat.py
--rw-r--r--   0 donncha    (501) staff       (20)    12214 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/packages.py
--rw-r--r--   0 donncha    (501) staff       (20)     2687 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/processes.py
--rw-r--r--   0 donncha    (501) staff       (20)     1777 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/root_binaries.py
--rw-r--r--   0 donncha    (501) staff       (20)     1389 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/selinux_status.py
--rw-r--r--   0 donncha    (501) staff       (20)     3664 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/settings.py
--rw-r--r--   0 donncha    (501) staff       (20)     5613 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/sms.py
--rw-r--r--   0 donncha    (501) staff       (20)     3422 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/adb/whatsapp.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.280354 mvt-2.3.0/mvt/android/modules/androidqf/
--rw-r--r--   0 donncha    (501) staff       (20)      736 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1315 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     2394 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_accessibility.py
--rw-r--r--   0 donncha    (501) staff       (20)     2347 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_activities.py
--rw-r--r--   0 donncha    (501) staff       (20)     3225 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_appops.py
--rw-r--r--   0 donncha    (501) staff       (20)     3894 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_packages.py
--rw-r--r--   0 donncha    (501) staff       (20)     3808 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_receivers.py
--rw-r--r--   0 donncha    (501) staff       (20)     2759 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)     3016 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/processes.py
--rw-r--r--   0 donncha    (501) staff       (20)     2221 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/settings.py
--rw-r--r--   0 donncha    (501) staff       (20)     2914 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/androidqf/sms.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.281067 mvt-2.3.0/mvt/android/modules/backup/
--rw-r--r--   0 donncha    (501) staff       (20)      238 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/android/modules/backup/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2069 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/backup/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     2176 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/backup/sms.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.282866 mvt-2.3.0/mvt/android/modules/bugreport/
--rw-r--r--   0 donncha    (501) staff       (20)      664 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2471 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/accessibility.py
--rw-r--r--   0 donncha    (501) staff       (20)     2435 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/activities.py
--rw-r--r--   0 donncha    (501) staff       (20)     3408 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/appops.py
--rw-r--r--   0 donncha    (501) staff       (20)     2949 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/base.py
--rw-r--r--   0 donncha    (501) staff       (20)     2701 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/battery_daily.py
--rw-r--r--   0 donncha    (501) staff       (20)     2189 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/battery_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     2401 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/dbinfo.py
--rw-r--r--   0 donncha    (501) staff       (20)     2440 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)     4158 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/packages.py
--rw-r--r--   0 donncha    (501) staff       (20)     4010 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/modules/bugreport/receivers.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.283493 mvt-2.3.0/mvt/android/parsers/
--rw-r--r--   0 donncha    (501) staff       (20)      492 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     7297 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/backup.py
--rw-r--r--   0 donncha    (501) staff       (20)    16021 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/dumpsys.py
--rw-r--r--   0 donncha    (501) staff       (20)      689 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/android/parsers/getprop.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.286051 mvt-2.3.0/mvt/common/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/common/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2598 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/cmd_check_iocs.py
--rw-r--r--   0 donncha    (501) staff       (20)     6294 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/command.py
--rw-r--r--   0 donncha    (501) staff       (20)      799 2023-05-10 16:45:13.000000 mvt-2.3.0/mvt/common/help.py
--rw-r--r--   0 donncha    (501) staff       (20)    22958 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/indicators.py
--rw-r--r--   0 donncha    (501) staff       (20)     2208 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/logo.py
--rw-r--r--   0 donncha    (501) staff       (20)     8455 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/module.py
--rw-r--r--   0 donncha    (501) staff       (20)     1258 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/options.py
--rw-r--r--   0 donncha    (501) staff       (20)     7545 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/updates.py
--rw-r--r--   0 donncha    (501) staff       (20)     5744 2023-06-29 12:27:56.000000 mvt-2.3.0/mvt/common/url.py
--rw-r--r--   0 donncha    (501) staff       (20)     6932 2023-06-29 12:58:31.000000 mvt-2.3.0/mvt/common/utils.py
--rw-r--r--   0 donncha    (501) staff       (20)      215 2023-06-29 15:01:05.000000 mvt-2.3.0/mvt/common/version.py
--rw-r--r--   0 donncha    (501) staff       (20)     1358 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/common/virustotal.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.286903 mvt-2.3.0/mvt/ios/
--rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/ios/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)    10651 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/cli.py
--rw-r--r--   0 donncha    (501) staff       (20)     1200 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/cmd_check_backup.py
--rw-r--r--   0 donncha    (501) staff       (20)     1181 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/cmd_check_fs.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.287351 mvt-2.3.0/mvt/ios/data/
--rw-r--r--   0 donncha    (501) staff       (20)     3550 2023-05-21 15:40:36.000000 mvt-2.3.0/mvt/ios/data/ios_models.json
--rw-r--r--   0 donncha    (501) staff       (20)    15419 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/data/ios_versions.json
--rw-r--r--   0 donncha    (501) staff       (20)     9049 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/decrypt.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.287792 mvt-2.3.0/mvt/ios/modules/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/ios/modules/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.288588 mvt-2.3.0/mvt/ios/modules/backup/
--rw-r--r--   0 donncha    (501) staff       (20)      439 2023-02-28 15:49:54.000000 mvt-2.3.0/mvt/ios/modules/backup/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2601 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/backup_info.py
--rw-r--r--   0 donncha    (501) staff       (20)     7211 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/configuration_profiles.py
--rw-r--r--   0 donncha    (501) staff       (20)     6914 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/manifest.py
--rw-r--r--   0 donncha    (501) staff       (20)     3838 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/backup/profile_events.py
--rw-r--r--   0 donncha    (501) staff       (20)     7146 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/base.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.290762 mvt-2.3.0/mvt/ios/modules/fs/
--rw-r--r--   0 donncha    (501) staff       (20)      913 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     4835 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/analytics.py
--rw-r--r--   0 donncha    (501) staff       (20)     2792 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/analytics_ios_versions.py
--rw-r--r--   0 donncha    (501) staff       (20)     3072 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/cache_files.py
--rw-r--r--   0 donncha    (501) staff       (20)     2980 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/filesystem.py
--rw-r--r--   0 donncha    (501) staff       (20)     1725 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/net_netusage.py
--rw-r--r--   0 donncha    (501) staff       (20)     3862 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/safari_favicon.py
--rw-r--r--   0 donncha    (501) staff       (20)     3934 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/shutdownlog.py
--rw-r--r--   0 donncha    (501) staff       (20)     2197 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/version_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     1423 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_base.py
--rw-r--r--   0 donncha    (501) staff       (20)     1708 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_indexeddb.py
--rw-r--r--   0 donncha    (501) staff       (20)     1731 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_localstorage.py
--rw-r--r--   0 donncha    (501) staff       (20)     1462 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/fs/webkit_safariviewservice.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.294201 mvt-2.3.0/mvt/ios/modules/mixed/
--rw-r--r--   0 donncha    (501) staff       (20)     1512 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     5579 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/applications.py
--rw-r--r--   0 donncha    (501) staff       (20)     5143 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/calendar.py
--rw-r--r--   0 donncha    (501) staff       (20)     2488 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/calls.py
--rw-r--r--   0 donncha    (501) staff       (20)     3406 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/chrome_favicon.py
--rw-r--r--   0 donncha    (501) staff       (20)     3213 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/chrome_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     2381 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/contacts.py
--rw-r--r--   0 donncha    (501) staff       (20)     3266 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/firefox_favicon.py
--rw-r--r--   0 donncha    (501) staff       (20)     2957 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/firefox_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     4352 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/idstatuscache.py
--rw-r--r--   0 donncha    (501) staff       (20)    14749 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/interactionc.py
--rw-r--r--   0 donncha    (501) staff       (20)     5343 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/locationd.py
--rw-r--r--   0 donncha    (501) staff       (20)     1456 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/net_datausage.py
--rw-r--r--   0 donncha    (501) staff       (20)     2943 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/osanalytics_addaily.py
--rw-r--r--   0 donncha    (501) staff       (20)     6570 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/safari_browserstate.py
--rw-r--r--   0 donncha    (501) staff       (20)     5971 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/safari_history.py
--rw-r--r--   0 donncha    (501) staff       (20)     5510 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/shortcuts.py
--rw-r--r--   0 donncha    (501) staff       (20)     5171 2023-06-29 15:09:26.000000 mvt-2.3.0/mvt/ios/modules/mixed/sms.py
--rw-r--r--   0 donncha    (501) staff       (20)     4334 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/sms_attachments.py
--rw-r--r--   0 donncha    (501) staff       (20)     7508 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/tcc.py
--rw-r--r--   0 donncha    (501) staff       (20)     4830 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
--rw-r--r--   0 donncha    (501) staff       (20)     6699 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/mixed/webkit_session_resource_log.py
--rw-r--r--   0 donncha    (501) staff       (20)     4663 2023-06-29 08:51:11.000000 mvt-2.3.0/mvt/ios/modules/mixed/whatsapp.py
--rw-r--r--   0 donncha    (501) staff       (20)    10973 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/modules/net_base.py
--rw-r--r--   0 donncha    (501) staff       (20)     1848 2023-06-28 19:46:39.000000 mvt-2.3.0/mvt/ios/versions.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.273496 mvt-2.3.0/mvt.egg-info/
--rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/PKG-INFO
--rw-r--r--   0 donncha    (501) staff       (20)     6342 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/SOURCES.txt
--rw-r--r--   0 donncha    (501) staff       (20)        1 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/dependency_links.txt
--rw-r--r--   0 donncha    (501) staff       (20)       70 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/entry_points.txt
--rw-r--r--   0 donncha    (501) staff       (20)      210 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/requires.txt
--rw-r--r--   0 donncha    (501) staff       (20)       10 2023-06-29 15:10:48.000000 mvt-2.3.0/mvt.egg-info/top_level.txt
--rw-r--r--   0 donncha    (501) staff       (20)     1740 2023-06-29 15:10:48.301587 mvt-2.3.0/setup.cfg
--rwxr-xr-x   0 donncha    (501) staff       (20)      231 2023-02-28 15:49:54.000000 mvt-2.3.0/setup.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.295811 mvt-2.3.0/tests/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/__init__.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.296479 mvt-2.3.0/tests/android/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/android/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     2719 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android/test_backup_module.py
--rw-r--r--   0 donncha    (501) staff       (20)     2168 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android/test_backup_parser.py
--rw-r--r--   0 donncha    (501) staff       (20)     2304 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android/test_dumpsys_parser.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.298158 mvt-2.3.0/tests/android_androidqf/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/android_androidqf/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)      623 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsysaccessbility.py
--rw-r--r--   0 donncha    (501) staff       (20)      633 2023-03-03 21:19:21.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsysappops.py
--rw-r--r--   0 donncha    (501) staff       (20)     1389 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsyspackages.py
--rw-r--r--   0 donncha    (501) staff       (20)      607 2023-03-03 21:19:21.000000 mvt-2.3.0/tests/android_androidqf/test_dumpsysreceivers.py
--rw-r--r--   0 donncha    (501) staff       (20)     1385 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_getprop.py
--rw-r--r--   0 donncha    (501) staff       (20)      692 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_processes.py
--rw-r--r--   0 donncha    (501) staff       (20)      618 2023-03-03 21:19:21.000000 mvt-2.3.0/tests/android_androidqf/test_settings.py
--rw-r--r--   0 donncha    (501) staff       (20)      661 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_androidqf/test_sms.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.298444 mvt-2.3.0/tests/android_bugreport/
--rw-r--r--   0 donncha    (501) staff       (20)        0 2023-05-10 16:45:13.000000 mvt-2.3.0/tests/android_bugreport/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1838 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/android_bugreport/test_bugreport.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.298931 mvt-2.3.0/tests/common/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/common/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1743 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/common/test_indicators.py
--rw-r--r--   0 donncha    (501) staff       (20)     2291 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/common/test_utils.py
--rw-r--r--   0 donncha    (501) staff       (20)      725 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/conftest.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.300552 mvt-2.3.0/tests/ios_backup/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/ios_backup/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)      570 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_backup_info.py
--rw-r--r--   0 donncha    (501) staff       (20)     1132 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_calendar.py
--rw-r--r--   0 donncha    (501) staff       (20)     1124 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_datausage.py
--rw-r--r--   0 donncha    (501) staff       (20)     1007 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_manifest.py
--rw-r--r--   0 donncha    (501) staff       (20)     1257 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_safari_browserstate.py
--rw-r--r--   0 donncha    (501) staff       (20)     1009 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_sms.py
--rw-r--r--   0 donncha    (501) staff       (20)     1265 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_tcc.py
--rw-r--r--   0 donncha    (501) staff       (20)      690 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_backup/test_webkit_resource_load_statistics.py
-drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-06-29 15:10:48.300854 mvt-2.3.0/tests/ios_fs/
--rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/ios_fs/__init__.py
--rw-r--r--   0 donncha    (501) staff       (20)     1160 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/ios_fs/test_filesystem.py
--rw-r--r--   0 donncha    (501) staff       (20)      572 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_check_android_androidqf.py
--rw-r--r--   0 donncha    (501) staff       (20)      586 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_check_android_bugreport.py
--rw-r--r--   0 donncha    (501) staff       (20)      525 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_check_ios_backup.py
--rw-r--r--   0 donncha    (501) staff       (20)      483 2023-06-28 19:46:39.000000 mvt-2.3.0/tests/test_ios_versions.py
--rw-r--r--   0 donncha    (501) staff       (20)      928 2023-02-28 15:49:54.000000 mvt-2.3.0/tests/utils.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.607245 mvt-2.4.0/
+-rw-r--r--   0 donncha    (501) staff       (20)    17791 2022-06-22 15:39:11.000000 mvt-2.4.0/LICENSE
+-rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-07-21 10:21:45.607338 mvt-2.4.0/PKG-INFO
+-rw-r--r--   0 donncha    (501) staff       (20)     3711 2023-07-16 15:19:41.000000 mvt-2.4.0/README.md
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.567529 mvt-2.4.0/mvt/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.570012 mvt-2.4.0/mvt/android/
+-rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/android/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)    11122 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cli.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1031 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_adb.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1118 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_androidqf.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3751 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2622 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/cmd_check_bugreport.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6138 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/cmd_download_apks.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.570301 mvt-2.4.0/mvt/android/modules/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/android/modules/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.574777 mvt-2.4.0/mvt/android/modules/adb/
+-rw-r--r--   0 donncha    (501) staff       (20)     1290 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/modules/adb/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)    12394 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3298 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/chrome_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1822 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_accessibility.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1803 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_activities.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2803 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_appops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2016 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_daily.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1659 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1781 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_dbinfo.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1377 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_full.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3293 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/dumpsys_receivers.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5278 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/files.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2214 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/adb/getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1844 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/logcat.py
+-rw-r--r--   0 donncha    (501) staff       (20)    12266 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/packages.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2711 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/adb/processes.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1928 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/android/modules/adb/root_binaries.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1413 2023-07-20 16:29:29.000000 mvt-2.4.0/mvt/android/modules/adb/selinux_status.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3688 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/adb/settings.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5637 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/sms.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3446 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/adb/whatsapp.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.581494 mvt-2.4.0/mvt/android/modules/androidqf/
+-rw-r--r--   0 donncha    (501) staff       (20)      736 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/modules/androidqf/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1339 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2418 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_accessibility.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2371 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_activities.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3249 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_appops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3918 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_packages.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3832 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_receivers.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2783 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/androidqf/getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3040 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/androidqf/processes.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2245 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/androidqf/settings.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2938 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/androidqf/sms.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.582212 mvt-2.4.0/mvt/android/modules/backup/
+-rw-r--r--   0 donncha    (501) staff       (20)      238 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/android/modules/backup/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2093 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/backup/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2200 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/backup/sms.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.584556 mvt-2.4.0/mvt/android/modules/bugreport/
+-rw-r--r--   0 donncha    (501) staff       (20)      664 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/modules/bugreport/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2495 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/accessibility.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2459 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/activities.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3432 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/appops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2973 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2725 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/battery_daily.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2213 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/battery_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2425 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/dbinfo.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2464 2023-07-21 10:09:58.000000 mvt-2.4.0/mvt/android/modules/bugreport/getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4182 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/packages.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4034 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/android/modules/bugreport/receivers.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.585711 mvt-2.4.0/mvt/android/parsers/
+-rw-r--r--   0 donncha    (501) staff       (20)      492 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/parsers/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7297 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/parsers/backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)    16326 2023-07-16 15:19:45.000000 mvt-2.4.0/mvt/android/parsers/dumpsys.py
+-rw-r--r--   0 donncha    (501) staff       (20)      689 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/android/parsers/getprop.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.588730 mvt-2.4.0/mvt/common/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/common/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2622 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/common/cmd_check_iocs.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6593 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/common/command.py
+-rw-r--r--   0 donncha    (501) staff       (20)      799 2023-07-17 16:31:28.000000 mvt-2.4.0/mvt/common/help.py
+-rw-r--r--   0 donncha    (501) staff       (20)    22958 2023-07-20 17:03:04.000000 mvt-2.4.0/mvt/common/indicators.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2208 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/logo.py
+-rw-r--r--   0 donncha    (501) staff       (20)     8515 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/common/module.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1258 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/options.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7545 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/updates.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5744 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/url.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6932 2023-07-16 15:19:45.000000 mvt-2.4.0/mvt/common/utils.py
+-rw-r--r--   0 donncha    (501) staff       (20)      215 2023-07-21 10:17:32.000000 mvt-2.4.0/mvt/common/version.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1358 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/common/virustotal.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.589888 mvt-2.4.0/mvt/ios/
+-rw-r--r--   0 donncha    (501) staff       (20)      214 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/ios/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)    10764 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/cli.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1224 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/cmd_check_backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1205 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/cmd_check_fs.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.590388 mvt-2.4.0/mvt/ios/data/
+-rw-r--r--   0 donncha    (501) staff       (20)     3550 2023-05-21 15:40:36.000000 mvt-2.4.0/mvt/ios/data/ios_models.json
+-rw-r--r--   0 donncha    (501) staff       (20)    15419 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/data/ios_versions.json
+-rw-r--r--   0 donncha    (501) staff       (20)     9049 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/decrypt.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.591049 mvt-2.4.0/mvt/ios/modules/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/ios/modules/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.592479 mvt-2.4.0/mvt/ios/modules/backup/
+-rw-r--r--   0 donncha    (501) staff       (20)      439 2023-02-28 15:49:54.000000 mvt-2.4.0/mvt/ios/modules/backup/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2625 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/backup/backup_info.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7235 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/backup/configuration_profiles.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6409 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/ios/modules/backup/manifest.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3862 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/backup/profile_events.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7170 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/base.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.594942 mvt-2.4.0/mvt/ios/modules/fs/
+-rw-r--r--   0 donncha    (501) staff       (20)      913 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/modules/fs/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4859 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/analytics.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2816 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/analytics_ios_versions.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3096 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/cache_files.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3032 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/filesystem.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1749 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/net_netusage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3886 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/safari_favicon.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3958 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/shutdownlog.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2221 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/version_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1423 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1732 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_indexeddb.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1755 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_localstorage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1486 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/fs/webkit_safariviewservice.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.600420 mvt-2.4.0/mvt/ios/modules/mixed/
+-rw-r--r--   0 donncha    (501) staff       (20)     1512 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/modules/mixed/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5603 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/applications.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5167 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/calendar.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2522 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/calls.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3430 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/chrome_favicon.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3237 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/chrome_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2405 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/contacts.py
+-rw-r--r--   0 donncha    (501) staff       (20)     3290 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/firefox_favicon.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2981 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/firefox_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4376 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/idstatuscache.py
+-rw-r--r--   0 donncha    (501) staff       (20)    14773 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/interactionc.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5367 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/locationd.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1480 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/net_datausage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2967 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/osanalytics_addaily.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6594 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/safari_browserstate.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5995 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/safari_history.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5534 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/shortcuts.py
+-rw-r--r--   0 donncha    (501) staff       (20)     5546 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/ios/modules/mixed/sms.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4437 2023-07-21 10:13:15.000000 mvt-2.4.0/mvt/ios/modules/mixed/sms_attachments.py
+-rw-r--r--   0 donncha    (501) staff       (20)     7532 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/tcc.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4854 2023-07-18 15:50:33.000000 mvt-2.4.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py
+-rw-r--r--   0 donncha    (501) staff       (20)     6723 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/webkit_session_resource_log.py
+-rw-r--r--   0 donncha    (501) staff       (20)     4687 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/mixed/whatsapp.py
+-rw-r--r--   0 donncha    (501) staff       (20)    11032 2023-07-17 17:35:22.000000 mvt-2.4.0/mvt/ios/modules/net_base.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1848 2023-07-16 15:19:41.000000 mvt-2.4.0/mvt/ios/versions.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.568567 mvt-2.4.0/mvt.egg-info/
+-rw-r--r--   0 donncha    (501) staff       (20)     4242 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/PKG-INFO
+-rw-r--r--   0 donncha    (501) staff       (20)     6342 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/SOURCES.txt
+-rw-r--r--   0 donncha    (501) staff       (20)        1 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/dependency_links.txt
+-rw-r--r--   0 donncha    (501) staff       (20)       70 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/entry_points.txt
+-rw-r--r--   0 donncha    (501) staff       (20)      210 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/requires.txt
+-rw-r--r--   0 donncha    (501) staff       (20)       10 2023-07-21 10:21:45.000000 mvt-2.4.0/mvt.egg-info/top_level.txt
+-rw-r--r--   0 donncha    (501) staff       (20)     1740 2023-07-21 10:21:45.607706 mvt-2.4.0/setup.cfg
+-rwxr-xr-x   0 donncha    (501) staff       (20)      231 2023-02-28 15:49:54.000000 mvt-2.4.0/setup.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.601951 mvt-2.4.0/tests/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/__init__.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.602814 mvt-2.4.0/tests/android/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/android/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2719 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android/test_backup_module.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2168 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android/test_backup_parser.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2304 2023-07-16 15:19:45.000000 mvt-2.4.0/tests/android/test_dumpsys_parser.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.604552 mvt-2.4.0/tests/android_androidqf/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/android_androidqf/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)      623 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsysaccessbility.py
+-rw-r--r--   0 donncha    (501) staff       (20)      633 2023-03-03 21:19:21.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsysappops.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1389 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsyspackages.py
+-rw-r--r--   0 donncha    (501) staff       (20)      607 2023-03-03 21:19:21.000000 mvt-2.4.0/tests/android_androidqf/test_dumpsysreceivers.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1385 2023-07-21 09:07:25.000000 mvt-2.4.0/tests/android_androidqf/test_getprop.py
+-rw-r--r--   0 donncha    (501) staff       (20)      692 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_processes.py
+-rw-r--r--   0 donncha    (501) staff       (20)      618 2023-03-03 21:19:21.000000 mvt-2.4.0/tests/android_androidqf/test_settings.py
+-rw-r--r--   0 donncha    (501) staff       (20)      661 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_androidqf/test_sms.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.604813 mvt-2.4.0/tests/android_bugreport/
+-rw-r--r--   0 donncha    (501) staff       (20)        0 2023-05-10 16:45:13.000000 mvt-2.4.0/tests/android_bugreport/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1838 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/android_bugreport/test_bugreport.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.605294 mvt-2.4.0/tests/common/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/common/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1743 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/common/test_indicators.py
+-rw-r--r--   0 donncha    (501) staff       (20)     2291 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/common/test_utils.py
+-rw-r--r--   0 donncha    (501) staff       (20)      725 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/conftest.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.606659 mvt-2.4.0/tests/ios_backup/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/ios_backup/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)      570 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_backup_info.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1132 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_calendar.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1124 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_datausage.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1007 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_manifest.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1257 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_safari_browserstate.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1042 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_sms.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1265 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_tcc.py
+-rw-r--r--   0 donncha    (501) staff       (20)      690 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_backup/test_webkit_resource_load_statistics.py
+drwxr-xr-x   0 donncha    (501) staff       (20)        0 2023-07-21 10:21:45.606988 mvt-2.4.0/tests/ios_fs/
+-rw-r--r--   0 donncha    (501) staff       (20)      192 2023-02-28 15:49:54.000000 mvt-2.4.0/tests/ios_fs/__init__.py
+-rw-r--r--   0 donncha    (501) staff       (20)     1160 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/ios_fs/test_filesystem.py
+-rw-r--r--   0 donncha    (501) staff       (20)      572 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_check_android_androidqf.py
+-rw-r--r--   0 donncha    (501) staff       (20)      586 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_check_android_bugreport.py
+-rw-r--r--   0 donncha    (501) staff       (20)      525 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_check_ios_backup.py
+-rw-r--r--   0 donncha    (501) staff       (20)      483 2023-07-16 15:19:41.000000 mvt-2.4.0/tests/test_ios_versions.py
+-rw-r--r--   0 donncha    (501) staff       (20)      928 2023-06-29 17:03:21.000000 mvt-2.4.0/tests/utils.py
```

### Comparing `mvt-2.3.0/LICENSE` & `mvt-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/PKG-INFO` & `mvt-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.3.0
+Version: 2.4.0
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.3.0/README.md` & `mvt-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/android/cli.py` & `mvt-2.4.0/mvt/android/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,20 +141,22 @@
 @click.option("--fast", "-f", is_flag=True, help=HELP_MSG_FAST)
 @click.option("--list-modules", "-l", is_flag=True, help=HELP_MSG_LIST_MODULES)
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.pass_context
 def check_adb(ctx, serial, iocs, output, fast, list_modules, module, verbose):
     set_verbose_logging(verbose)
+    module_options = {"fast_mode": fast}
+
     cmd = CmdAndroidCheckADB(
         results_path=output,
         ioc_files=iocs,
         module_name=module,
         serial=serial,
-        fast_mode=fast,
+        module_options=module_options,
     )
 
     if list_modules:
         cmd.list_modules()
         return
 
     log.info("Checking Android device over debug bridge")
```

### Comparing `mvt-2.3.0/mvt/android/cmd_check_adb.py` & `mvt-2.4.0/mvt/android/cmd_check_adb.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,21 +17,21 @@
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
         )
 
         self.name = "check-adb"
         self.modules = ADB_MODULES
```

### Comparing `mvt-2.3.0/mvt/android/cmd_check_androidqf.py` & `mvt-2.4.0/mvt/android/cmd_check_androidqf.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         hashes: bool = False,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             hashes=hashes,
             log=log,
         )
 
         self.name = "check-androidqf"
         self.modules = ANDROIDQF_MODULES
```

### Comparing `mvt-2.3.0/mvt/android/cmd_check_backup.py` & `mvt-2.4.0/mvt/android/cmd_check_backup.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,24 +31,24 @@
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         hashes: bool = False,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             hashes=hashes,
             log=log,
         )
 
         self.name = "check-backup"
         self.modules = BACKUP_MODULES
```

### Comparing `mvt-2.3.0/mvt/android/cmd_check_bugreport.py` & `mvt-2.4.0/mvt/android/cmd_check_bugreport.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,24 @@
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         hashes: bool = False,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             hashes=hashes,
             log=log,
         )
 
         self.name = "check-bugreport"
         self.modules = BUGREPORT_MODULES
```

### Comparing `mvt-2.3.0/mvt/android/cmd_download_apks.py` & `mvt-2.4.0/mvt/android/cmd_download_apks.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/android/modules/adb/__init__.py` & `mvt-2.4.0/mvt/android/modules/adb/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/android/modules/adb/base.py` & `mvt-2.4.0/mvt/android/modules/adb/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,23 @@
     """This class provides a base for all Android extraction modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.device = None
         self.serial = None
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/chrome_history.py` & `mvt-2.4.0/mvt/android/modules/adb/chrome_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     """This module extracts records from Android's Chrome browsing history."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.results = []
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_accessibility.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_accessibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module extracts stats on accessibility."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_activities.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_activities.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_appops.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_appops.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     slug = "dumpsys_appops"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for perm in record["permissions"]:
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_daily.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_daily.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module extracts records from battery daily updates."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["from"],
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_battery_history.py` & `mvt-2.4.0/mvt/android/modules/adb/getprop.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,67 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
+from datetime import datetime, timedelta
 from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_battery_history
+from mvt.android.parsers import parse_getprop
 
 from .base import AndroidExtraction
 
 
-class DumpsysBatteryHistory(AndroidExtraction):
-    """This module extracts records from battery history events."""
+class Getprop(AndroidExtraction):
+    """This module extracts device properties from getprop command."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
+        self.results = {} if not results else results
+
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            ioc = self.indicators.check_app_id(result["package_name"])
+            ioc = self.indicators.check_android_property_name(result.get("name", ""))
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
-                continue
 
     def run(self) -> None:
         self._adb_connect()
-        output = self._adb_command("dumpsys batterystats --history")
+        output = self._adb_command("getprop")
         self._adb_disconnect()
 
-        self.results = parse_dumpsys_battery_history(output)
+        self.results = parse_getprop(output)
+
+        # Alert if phone is outdated.
+        for entry in self.results:
+            if entry.get("name", "") != "ro.build.version.security_patch":
+                continue
+            patch_date = datetime.strptime(entry["value"], "%Y-%m-%d")
+            if (datetime.now() - patch_date) > timedelta(days=6 * 30):
+                self.log.warning(
+                    "This phone has not received security updates "
+                    "for more than six months (last update: %s)",
+                    entry["value"],
+                )
 
-        self.log.info("Extracted %d records from battery history", len(self.results))
+        self.log.info("Extracted %d Android system properties", len(self.results))
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_dbinfo.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_battery_history.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,59 +2,52 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_dbinfo
+from mvt.android.parsers import parse_dumpsys_battery_history
 
 from .base import AndroidExtraction
 
 
-class DumpsysDBInfo(AndroidExtraction):
-    """This module extracts records from battery daily updates."""
-
-    slug = "dumpsys_dbinfo"
+class DumpsysBatteryHistory(AndroidExtraction):
+    """This module extracts records from battery history events."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            path = result.get("path", "")
-            for part in path.split("/"):
-                ioc = self.indicators.check_app_id(part)
-                if ioc:
-                    result["matched_indicator"] = ioc
-                    self.detected.append(result)
-                    continue
+            ioc = self.indicators.check_app_id(result["package_name"])
+            if ioc:
+                result["matched_indicator"] = ioc
+                self.detected.append(result)
+                continue
 
     def run(self) -> None:
         self._adb_connect()
-        output = self._adb_command("dumpsys dbinfo")
+        output = self._adb_command("dumpsys batterystats --history")
         self._adb_disconnect()
 
-        self.results = parse_dumpsys_dbinfo(output)
+        self.results = parse_dumpsys_battery_history(output)
 
-        self.log.info(
-            "Extracted a total of %d records from database information",
-            len(self.results),
-        )
+        self.log.info("Extracted %d records from battery history", len(self.results))
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_full.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_full.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     """This module extracts stats on battery consumption by processes."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def run(self) -> None:
         self._adb_connect()
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/dumpsys_receivers.py` & `mvt-2.4.0/mvt/android/modules/adb/dumpsys_receivers.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/files.py` & `mvt-2.4.0/mvt/android/modules/adb/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     """This module extracts the list of files on the device."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.full_find = False
 
     def serialize(self, record: dict) -> Union[dict, list, None]:
         if "modified_time" in record:
@@ -138,16 +138,18 @@
         for media_folder in ANDROID_MEDIA_FOLDERS:
             self.find_files(media_folder)
 
         self.log.info(
             "Found %s files in primary Android tmp and media folders", len(self.results)
         )
 
-        if self.fast_mode:
-            self.log.info("Flag --fast was enabled: skipping full file listing")
+        if self.module_options.get("fast_mode", None):
+            self.log.info(
+                "The `fast_mode` option was enabled: skipping full file listing"
+            )
         else:
             self.log.info("Processing full file listing. This may take a while...")
             self.find_files("/")
 
             self.log.info("Found %s total files", len(self.results))
 
         self._adb_disconnect()
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/getprop.py` & `mvt-2.4.0/mvt/android/modules/bugreport/getprop.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,63 +5,73 @@
 
 import logging
 from datetime import datetime, timedelta
 from typing import Optional
 
 from mvt.android.parsers import parse_getprop
 
-from .base import AndroidExtraction
+from .base import BugReportModule
 
 
-class Getprop(AndroidExtraction):
+class Getprop(BugReportModule):
     """This module extracts device properties from getprop command."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = {} if not results else results
 
-    def check_indicators(self) -> None:
-        if not self.indicators:
+    def run(self) -> None:
+        content = self._get_dumpstate_file()
+        if not content:
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
-        for result in self.results:
-            ioc = self.indicators.check_android_property_name(result.get("name", ""))
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+        lines = []
+        in_getprop = False
 
-    def run(self) -> None:
-        self._adb_connect()
-        output = self._adb_command("getprop")
-        self._adb_disconnect()
+        for line in content.decode(errors="ignore").splitlines():
+            if line.strip().startswith("------ SYSTEM PROPERTIES"):
+                in_getprop = True
+                continue
+
+            if not in_getprop:
+                continue
+
+            if line.strip() == "------":
+                break
 
-        self.results = parse_getprop(output)
+            lines.append(line)
+
+        self.results = parse_getprop("\n".join(lines))
 
         # Alert if phone is outdated.
         for entry in self.results:
-            if entry.get("name", "") != "ro.build.version.security_patch":
-                continue
-            patch_date = datetime.strptime(entry["value"], "%Y-%m-%d")
-            if (datetime.now() - patch_date) > timedelta(days=6 * 30):
-                self.log.warning(
-                    "This phone has not received security updates "
-                    "for more than six months (last update: %s)",
-                    entry["value"],
-                )
+            if entry["name"] == "ro.build.version.security_patch":
+                security_patch = entry["value"]
+                patch_date = datetime.strptime(security_patch, "%Y-%m-%d")
+                if (datetime.now() - patch_date) > timedelta(days=6 * 30):
+                    self.log.warning(
+                        "This phone has not received security updates "
+                        "for more than six months (last update: %s)",
+                        security_patch,
+                    )
 
         self.log.info("Extracted %d Android system properties", len(self.results))
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/logcat.py` & `mvt-2.4.0/mvt/android/modules/adb/logcat.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     """This module extracts details on installed packages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def run(self) -> None:
         self._adb_connect()
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/packages.py` & `mvt-2.4.0/mvt/android/modules/adb/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,23 +89,23 @@
     """This module extracts the list of installed packages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
 
@@ -347,15 +347,15 @@
             self.log.info(
                 'Found non-system package with name "%s" installed by "%s" on %s',
                 result["package_name"],
                 result["installer"],
                 result["timestamp"],
             )
 
-        if not self.fast_mode:
+        if not self.module_options.get("fast_mode", None):
             self.check_virustotal(packages_to_lookup)
 
         self.log.info(
             "Extracted at total of %d installed package names", len(self.results)
         )
 
         self._adb_disconnect()
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/processes.py` & `mvt-2.4.0/mvt/android/modules/adb/processes.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     """This module extracts details on running processes."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/root_binaries.py` & `mvt-2.4.0/mvt/android/modules/adb/root_binaries.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,32 @@
     """This module extracts the list of installed packages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
+    def check_indicators(self) -> None:
+        for root_binary in self.results:
+            self.detected.append(root_binary)
+            self.log.warning('Found root binary "%s"', root_binary)
+
     def run(self) -> None:
         root_binaries = [
             "su",
             "busybox",
             "supersu",
             "Superuser.apk",
             "KingoUser.apk",
@@ -56,11 +61,10 @@
 
             if not output:
                 continue
 
             if "which: not found" in output:
                 continue
 
-            self.detected.append(root_binary)
-            self.log.warning('Found root binary "%s"', root_binary)
+            self.results.append(root_binary)
 
         self._adb_disconnect()
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/selinux_status.py` & `mvt-2.4.0/mvt/android/modules/adb/selinux_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     slug = "selinux_status"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = {} if not results else results
 
     def run(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/settings.py` & `mvt-2.4.0/mvt/android/modules/adb/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,23 +61,23 @@
     """This module extracts Android system settings."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = {} if not results else results
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/sms.py` & `mvt-2.4.0/mvt/android/modules/adb/sms.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,23 @@
     """This module extracts all SMS messages."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.sms_db_type = 0
 
     def serialize(self, record: dict) -> Union[dict, list]:
```

### Comparing `mvt-2.3.0/mvt/android/modules/adb/whatsapp.py` & `mvt-2.4.0/mvt/android/modules/adb/whatsapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     """This module extracts all WhatsApp messages containing links."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         text = record["data"].replace("\n", "\\n")
         return {
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/__init__.py` & `mvt-2.4.0/mvt/android/modules/androidqf/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/base.py` & `mvt-2.4.0/mvt/android/modules/androidqf/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This class provides a base for all Android Data analysis modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self._path = target_path
         self._files = []
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_accessibility.py` & `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_accessibility.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module analyse dumpsys accessbility"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_activities.py` & `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_activities.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_appops.py` & `mvt-2.4.0/mvt/android/modules/bugreport/appops.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,32 +4,34 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional, Union
 
 from mvt.android.parsers import parse_dumpsys_appops
 
-from .base import AndroidQFModule
+from .base import BugReportModule
 
 
-class DumpsysAppops(AndroidQFModule):
+class Appops(BugReportModule):
+    """This module extracts information on package from App-Ops Manager."""
+
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for perm in record["permissions"]:
@@ -40,15 +42,15 @@
                 if "timestamp" in entry:
                     records.append(
                         {
                             "timestamp": entry["timestamp"],
                             "module": self.__class__.__name__,
                             "event": entry["access"],
                             "data": f"{record['package_name']} access to "
-                            f"{perm['name']} : {entry['access']}",
+                            f"{perm['name']}: {entry['access']}",
                         }
                     )
 
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
@@ -66,29 +68,37 @@
                 ):
                     self.log.info(
                         "Package %s with REQUEST_INSTALL_PACKAGES permission",
                         result["package_name"],
                     )
 
     def run(self) -> None:
-        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
-        if not dumpsys_file:
+        content = self._get_dumpstate_file()
+        if not content:
+            self.log.error(
+                "Unable to find dumpstate file. "
+                "Did you provide a valid bug report archive?"
+            )
             return
 
         lines = []
-        in_package = False
-        with open(dumpsys_file[0]) as handle:
-            for line in handle:
-                if line.startswith("DUMP OF SERVICE appops:"):
-                    in_package = True
-                    continue
+        in_appops = False
+        for line in content.decode(errors="ignore").splitlines():
+            if line.strip() == "DUMP OF SERVICE appops:":
+                in_appops = True
+                continue
 
-                if in_package:
-                    if line.startswith(
-                        "-------------------------------------------------------------------------------"
-                    ):  # pylint: disable=line-too-long
-                        break
+            if not in_appops:
+                continue
 
-                    lines.append(line.rstrip())
+            if line.strip().startswith(
+                "------------------------------------------------------------------------------"
+            ):  # pylint: disable=line-too-long
+                break
+
+            lines.append(line)
 
         self.results = parse_dumpsys_appops("\n".join(lines))
-        self.log.info("Identified %d applications in AppOps Manager", len(self.results))
+
+        self.log.info(
+            "Identified a total of %d packages in App-Ops Manager", len(self.results)
+        )
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_packages.py` & `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     """This module analyse dumpsys packages"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[List[Dict[str, Any]]] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         entries = []
         for entry in ["timestamp", "first_install_time", "last_update_time"]:
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/dumpsys_receivers.py` & `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_receivers.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     """This module analyse dumpsys receivers"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Union[List[Any], Dict[str, Any], None] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/getprop.py` & `mvt-2.4.0/mvt/android/modules/androidqf/getprop.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,23 +30,23 @@
     """This module extracts data from get properties."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.results = []
 
     def check_indicators(self) -> None:
         if not self.indicators:
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/processes.py` & `mvt-2.4.0/mvt/android/modules/androidqf/processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     """This module analyse running processes"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/settings.py` & `mvt-2.4.0/mvt/android/modules/androidqf/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module analyse setting files"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.results = {}
 
     def run(self) -> None:
         for setting_file in self._get_files_by_pattern("*/settings_*.txt"):
```

### Comparing `mvt-2.3.0/mvt/android/modules/androidqf/sms.py` & `mvt-2.4.0/mvt/android/modules/androidqf/sms.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     """This module analyse SMS file in backup"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.3.0/mvt/android/modules/backup/base.py` & `mvt-2.4.0/mvt/android/modules/backup/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     """This class provides a base for all backup extractios modules"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.ab = None
         self.backup_path = None
         self.tar = None
         self.files = []
```

### Comparing `mvt-2.3.0/mvt/android/modules/backup/sms.py` & `mvt-2.4.0/mvt/android/modules/backup/sms.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 class SMS(BackupExtraction):
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.results = []
 
     def check_indicators(self) -> None:
         if not self.indicators:
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/__init__.py` & `mvt-2.4.0/mvt/android/modules/bugreport/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/accessibility.py` & `mvt-2.4.0/mvt/android/modules/bugreport/accessibility.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module extracts stats on accessibility."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/activities.py` & `mvt-2.4.0/mvt/android/modules/bugreport/activities.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/appops.py` & `mvt-2.4.0/mvt/android/modules/bugreport/dbinfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,104 +1,81 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional, Union
+from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_appops
+from mvt.android.parsers import parse_dumpsys_dbinfo
 
 from .base import BugReportModule
 
 
-class Appops(BugReportModule):
-    """This module extracts information on package from App-Ops Manager."""
+class DBInfo(BugReportModule):
+    """This module extracts records from battery daily updates."""
+
+    slug = "dbinfo"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
-    def serialize(self, record: dict) -> Union[dict, list]:
-        records = []
-        for perm in record["permissions"]:
-            if "entries" not in perm:
-                continue
-
-            for entry in perm["entries"]:
-                if "timestamp" in entry:
-                    records.append(
-                        {
-                            "timestamp": entry["timestamp"],
-                            "module": self.__class__.__name__,
-                            "event": entry["access"],
-                            "data": f"{record['package_name']} access to "
-                            f"{perm['name']}: {entry['access']}",
-                        }
-                    )
-
-        return records
-
     def check_indicators(self) -> None:
+        if not self.indicators:
+            return
+
         for result in self.results:
-            if self.indicators:
-                ioc = self.indicators.check_app_id(result.get("package_name"))
+            path = result.get("path", "")
+            for part in path.split("/"):
+                ioc = self.indicators.check_app_id(part)
                 if ioc:
                     result["matched_indicator"] = ioc
                     self.detected.append(result)
                     continue
 
-            for perm in result["permissions"]:
-                if (
-                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
-                    and perm["access"] == "allow"
-                ):
-                    self.log.info(
-                        "Package %s with REQUEST_INSTALL_PACKAGES permission",
-                        result["package_name"],
-                    )
-
     def run(self) -> None:
         content = self._get_dumpstate_file()
         if not content:
             self.log.error(
                 "Unable to find dumpstate file. "
                 "Did you provide a valid bug report archive?"
             )
             return
 
+        in_dbinfo = False
         lines = []
-        in_appops = False
         for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE appops:":
-                in_appops = True
+            if line.strip() == "DUMP OF SERVICE dbinfo:":
+                in_dbinfo = True
                 continue
 
-            if not in_appops:
+            if not in_dbinfo:
                 continue
 
             if line.strip().startswith(
                 "------------------------------------------------------------------------------"
             ):  # pylint: disable=line-too-long
                 break
 
             lines.append(line)
 
-        self.results = parse_dumpsys_appops("\n".join(lines))
+        self.results = parse_dumpsys_dbinfo("\n".join(lines))
 
         self.log.info(
-            "Identified a total of %d packages in App-Ops Manager", len(self.results)
+            "Extracted a total of %d database connection pool records",
+            len(self.results),
         )
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/base.py` & `mvt-2.4.0/mvt/android/modules/bugreport/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     """This class provides a base for all Android Bug Report modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.zip_archive: Optional[ZipFile] = None
         self.extract_path: Optional[str] = None
         self.extract_files: List[str] = []
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/battery_daily.py` & `mvt-2.4.0/mvt/android/modules/bugreport/battery_history.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,41 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional, Union
+from typing import Optional
 
-from mvt.android.parsers import parse_dumpsys_battery_daily
+from mvt.android.parsers import parse_dumpsys_battery_history
 
 from .base import BugReportModule
 
 
-class BatteryDaily(BugReportModule):
+class BatteryHistory(BugReportModule):
     """This module extracts records from battery daily updates."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
-    def serialize(self, record: dict) -> Union[dict, list]:
-        return {
-            "timestamp": record["from"],
-            "module": self.__class__.__name__,
-            "event": "battery_daily",
-            "data": f"Recorded update of package {record['package_name']} "
-            f"with vers {record['vers']}",
-        }
-
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
             ioc = self.indicators.check_app_id(result["package_name"])
             if ioc:
@@ -58,33 +49,27 @@
             self.log.error(
                 "Unable to find dumpstate file. "
                 "Did you provide a valid bug report archive?"
             )
             return
 
         lines = []
-        in_batterystats = False
-        in_daily = False
+        in_history = False
         for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE batterystats:":
-                in_batterystats = True
-                continue
-
-            if not in_batterystats:
-                continue
-
-            if line.strip() == "Daily stats:":
+            if line.strip().startswith("Battery History "):
                 lines.append(line)
-                in_daily = True
+                in_history = True
                 continue
 
-            if not in_daily:
+            if not in_history:
                 continue
 
             if line.strip() == "":
                 break
 
             lines.append(line)
 
-        self.results = parse_dumpsys_battery_daily("\n".join(lines))
+        self.results = parse_dumpsys_battery_history("\n".join(lines))
 
-        self.log.info("Extracted a total of %d battery daily stats", len(self.results))
+        self.log.info(
+            "Extracted a total of %d battery history records", len(self.results)
+        )
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/dbinfo.py` & `mvt-2.4.0/mvt/ios/modules/fs/filesystem.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,92 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-from typing import Optional
+import os
+from typing import Optional, Union
 
-from mvt.android.parsers import parse_dumpsys_dbinfo
+from mvt.common.utils import convert_unix_to_iso
 
-from .base import BugReportModule
+from ..base import IOSExtraction
 
 
-class DBInfo(BugReportModule):
-    """This module extracts records from battery daily updates."""
-
-    slug = "dbinfo"
+class Filesystem(IOSExtraction):
+    """This module extracts creation and modification date of files from a
+    full file-system dump.
+    """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
+    def serialize(self, record: dict) -> Union[dict, list]:
+        return {
+            "timestamp": record["modified"],
+            "module": self.__class__.__name__,
+            "event": "entry_modified",
+            "data": record["path"],
+        }
+
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            path = result.get("path", "")
-            for part in path.split("/"):
-                ioc = self.indicators.check_app_id(part)
-                if ioc:
-                    result["matched_indicator"] = ioc
-                    self.detected.append(result)
-                    continue
+            if "path" not in result:
+                continue
 
-    def run(self) -> None:
-        content = self._get_dumpstate_file()
-        if not content:
-            self.log.error(
-                "Unable to find dumpstate file. "
-                "Did you provide a valid bug report archive?"
-            )
-            return
+            ioc = self.indicators.check_file_path(result["path"])
+            if ioc:
+                result["matched_indicator"] = ioc
+                self.detected.append(result)
 
-        in_dbinfo = False
-        lines = []
-        for line in content.decode(errors="ignore").splitlines():
-            if line.strip() == "DUMP OF SERVICE dbinfo:":
-                in_dbinfo = True
+            # If we are instructed to run fast, we skip the rest.
+            if self.module_options.get("fast_mode", None):
                 continue
 
-            if not in_dbinfo:
-                continue
+            ioc = self.indicators.check_file_path_process(result["path"])
+            if ioc:
+                result["matched_indicator"] = ioc
+                self.detected.append(result)
 
-            if line.strip().startswith(
-                "------------------------------------------------------------------------------"
-            ):  # pylint: disable=line-too-long
-                break
-
-            lines.append(line)
-
-        self.results = parse_dumpsys_dbinfo("\n".join(lines))
-
-        self.log.info(
-            "Extracted a total of %d database connection pool records",
-            len(self.results),
-        )
+    def run(self) -> None:
+        for root, dirs, files in os.walk(self.target_path):
+            for dir_name in dirs:
+                try:
+                    dir_path = os.path.join(root, dir_name)
+                    result = {
+                        "path": os.path.relpath(dir_path, self.target_path),
+                        "modified": convert_unix_to_iso(os.stat(dir_path).st_mtime),
+                    }
+                except Exception:
+                    continue
+                else:
+                    self.results.append(result)
+
+            for file_name in files:
+                try:
+                    file_path = os.path.join(root, file_name)
+                    result = {
+                        "path": os.path.relpath(file_path, self.target_path),
+                        "modified": convert_unix_to_iso(os.stat(file_path).st_mtime),
+                    }
+                except Exception:
+                    continue
+                else:
+                    self.results.append(result)
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/packages.py` & `mvt-2.4.0/mvt/android/modules/bugreport/packages.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,23 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
```

### Comparing `mvt-2.3.0/mvt/android/modules/bugreport/receivers.py` & `mvt-2.4.0/mvt/android/modules/bugreport/receivers.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """This module extracts details on receivers for risky activities."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = results if results else {}
 
     def check_indicators(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/android/parsers/backup.py` & `mvt-2.4.0/mvt/android/parsers/backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/android/parsers/dumpsys.py` & `mvt-2.4.0/mvt/android/parsers/dumpsys.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,14 +335,25 @@
             in_packages = True
 
         if not in_packages:
             continue
 
         if line.startswith("  Uid "):
             uid = line[6:-1]
+            if entry:
+                perm["entries"].append(entry)
+                entry = {}
+
+            if package:
+                if perm:
+                    package["permissions"].append(perm)
+
+                perm = {}
+                results.append(package)
+            package = {}
             continue
 
         if line.startswith("    Package "):
             if entry:
                 perm["entries"].append(entry)
                 entry = {}
 
@@ -356,15 +367,15 @@
             package = {
                 "package_name": line[12:-1],
                 "permissions": [],
                 "uid": uid,
             }
             continue
 
-        if line.startswith("      ") and line[6] != " ":
+        if package and line.startswith("      ") and line[6] != " ":
             if entry:
                 perm["entries"].append(entry)
                 entry = {}
             if perm:
                 package["permissions"].append(perm)
                 perm = {}
```

### Comparing `mvt-2.3.0/mvt/android/parsers/getprop.py` & `mvt-2.4.0/mvt/android/parsers/getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/common/cmd_check_iocs.py` & `mvt-2.4.0/mvt/common/cmd_check_iocs.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,23 @@
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
         )
 
         self.name = "check-iocs"
 
     def run(self) -> None:
         assert self.target_path is not None
```

### Comparing `mvt-2.3.0/mvt/common/command.py` & `mvt-2.4.0/mvt/common/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,33 @@
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         hashes: bool = False,
         log: logging.Logger = logging.getLogger(__name__),
     ) -> None:
         self.name = ""
         self.modules = []
 
         self.target_path = target_path
         self.results_path = results_path
         self.ioc_files = ioc_files if ioc_files else []
         self.module_name = module_name
         self.serial = serial
-        self.fast_mode = fast_mode
         self.log = log
 
+        # This dictionary can contain options that will be passed down from
+        # the Command to all modules. This can for example be used to pass
+        # down a password to decrypt a backup or flags which are need by some modules.
+        self.module_options = module_options if module_options else {}
+
         # This list will contain all executed modules.
         # We can use this to reference e.g. self.executed[0].results.
         self.executed = []
         self.detected_count = 0
         self.hashes = hashes
         self.hash_values = []
         self.timeline = []
@@ -168,15 +172,15 @@
 
             # FIXME: do we need the logger here
             module_logger = logging.getLogger(module.__module__)
 
             m = module(
                 target_path=self.target_path,
                 results_path=self.results_path,
-                fast_mode=self.fast_mode,
+                module_options=self.module_options,
                 log=module_logger,
             )
 
             if self.iocs.total_ioc_count:
                 m.indicators = self.iocs
                 m.indicators.log = m.log
```

### Comparing `mvt-2.3.0/mvt/common/help.py` & `mvt-2.4.0/mvt/common/help.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/common/indicators.py` & `mvt-2.4.0/mvt/common/indicators.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import json
 import logging
 import os
-from typing import Any, Dict, Iterator, List, Optional, Union
 from functools import lru_cache
+from typing import Any, Dict, Iterator, List, Optional, Union
 
 import ahocorasick
 from appdirs import user_data_dir
 
 from .url import URL
 
 MVT_DATA_FOLDER = user_data_dir("mvt")
```

### Comparing `mvt-2.3.0/mvt/common/logo.py` & `mvt-2.4.0/mvt/common/logo.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/common/module.py` & `mvt-2.4.0/mvt/common/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     slug: Optional[str] = None
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[Dict[str, Any]] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Union[List[Dict[str, Any]], Dict[str, Any], None] = None,
     ) -> None:
         """Initialize module.
 
         :param file_path: Path to the module's database file, if there is any
         :type file_path: str
@@ -55,15 +55,15 @@
         :param log: Handle to logger
         :param results: Provided list of results entries
         :type results: list
         """
         self.file_path = file_path
         self.target_path = target_path
         self.results_path = results_path
-        self.fast_mode = fast_mode
+        self.module_options = module_options if module_options else {}
         self.log = log
         self.indicators = None
         self.results = results if results else []
         self.detected: List[Dict[str, Any]] = []
         self.timeline: List[Dict[str, str]] = []
         self.timeline_detected: List[Dict[str, str]] = []
```

### Comparing `mvt-2.3.0/mvt/common/options.py` & `mvt-2.4.0/mvt/common/options.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/common/updates.py` & `mvt-2.4.0/mvt/common/updates.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/common/url.py` & `mvt-2.4.0/mvt/common/url.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/common/utils.py` & `mvt-2.4.0/mvt/common/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
+import cProfile
 import datetime
 import hashlib
 import logging
 import os
 import re
-import cProfile
 from typing import Any, Iterator, Union
 
 from rich.logging import RichHandler
 
 
 def convert_chrometime_to_datetime(timestamp: int) -> datetime.datetime:
     """Converts Chrome timestamp to a datetime.
```

### Comparing `mvt-2.3.0/mvt/common/virustotal.py` & `mvt-2.4.0/mvt/common/virustotal.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/cli.py` & `mvt-2.4.0/mvt/ios/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -215,21 +215,22 @@
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("BACKUP_PATH", type=click.Path(exists=True))
 @click.pass_context
 def check_backup(
     ctx, iocs, output, fast, list_modules, module, hashes, verbose, backup_path
 ):
     set_verbose_logging(verbose)
+    module_options = {"fast_mode": fast}
 
     cmd = CmdIOSCheckBackup(
         target_path=backup_path,
         results_path=output,
         ioc_files=iocs,
         module_name=module,
-        fast_mode=fast,
+        module_options=module_options,
         hashes=hashes,
     )
 
     if list_modules:
         cmd.list_modules()
         return
 
@@ -265,20 +266,22 @@
 @click.option("--module", "-m", help=HELP_MSG_MODULE)
 @click.option("--hashes", "-H", is_flag=True, help=HELP_MSG_HASHES)
 @click.option("--verbose", "-v", is_flag=True, help=HELP_MSG_VERBOSE)
 @click.argument("DUMP_PATH", type=click.Path(exists=True))
 @click.pass_context
 def check_fs(ctx, iocs, output, fast, list_modules, module, hashes, verbose, dump_path):
     set_verbose_logging(verbose)
+    module_options = {"fast_mode": fast}
+
     cmd = CmdIOSCheckFS(
         target_path=dump_path,
         results_path=output,
         ioc_files=iocs,
         module_name=module,
-        fast_mode=fast,
+        module_options=module_options,
         hashes=hashes,
     )
 
     if list_modules:
         cmd.list_modules()
         return
```

### Comparing `mvt-2.3.0/mvt/ios/cmd_check_backup.py` & `mvt-2.4.0/mvt/ios/cmd_check_fs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
 from mvt.common.command import Command
 
-from .modules.backup import BACKUP_MODULES
+from .modules.fs import FS_MODULES
 from .modules.mixed import MIXED_MODULES
 
 log = logging.getLogger(__name__)
 
 
-class CmdIOSCheckBackup(Command):
+class CmdIOSCheckFS(Command):
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         hashes: bool = False,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             hashes=hashes,
             log=log,
         )
 
-        self.name = "check-backup"
-        self.modules = BACKUP_MODULES + MIXED_MODULES
+        self.name = "check-fs"
+        self.modules = FS_MODULES + MIXED_MODULES
 
     def module_init(self, module):
-        module.is_backup = True
+        module.is_fs_dump = True
```

### Comparing `mvt-2.3.0/mvt/ios/cmd_check_fs.py` & `mvt-2.4.0/mvt/ios/cmd_check_backup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 #   https://license.mvt.re/1.1/
 
 import logging
 from typing import Optional
 
 from mvt.common.command import Command
 
-from .modules.fs import FS_MODULES
+from .modules.backup import BACKUP_MODULES
 from .modules.mixed import MIXED_MODULES
 
 log = logging.getLogger(__name__)
 
 
-class CmdIOSCheckFS(Command):
+class CmdIOSCheckBackup(Command):
     def __init__(
         self,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
         ioc_files: Optional[list] = None,
         module_name: Optional[str] = None,
         serial: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         hashes: bool = False,
     ) -> None:
         super().__init__(
             target_path=target_path,
             results_path=results_path,
             ioc_files=ioc_files,
             module_name=module_name,
             serial=serial,
-            fast_mode=fast_mode,
+            module_options=module_options,
             hashes=hashes,
             log=log,
         )
 
-        self.name = "check-fs"
-        self.modules = FS_MODULES + MIXED_MODULES
+        self.name = "check-backup"
+        self.modules = BACKUP_MODULES + MIXED_MODULES
 
     def module_init(self, module):
-        module.is_fs_dump = True
+        module.is_backup = True
```

### Comparing `mvt-2.3.0/mvt/ios/data/ios_models.json` & `mvt-2.4.0/mvt/ios/data/ios_models.json`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/data/ios_versions.json` & `mvt-2.4.0/mvt/ios/data/ios_versions.json`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/decrypt.py` & `mvt-2.4.0/mvt/ios/decrypt.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/modules/backup/backup_info.py` & `mvt-2.4.0/mvt/ios/modules/backup/backup_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,23 @@
     """This module extracts information about the device and the backup."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = {}
 
     def run(self) -> None:
```

### Comparing `mvt-2.3.0/mvt/ios/modules/backup/configuration_profiles.py` & `mvt-2.4.0/mvt/ios/modules/backup/configuration_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     """This module extracts the full plist data from configuration profiles."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         if not record["install_date"]:
             return {}
```

### Comparing `mvt-2.3.0/mvt/ios/modules/backup/manifest.py` & `mvt-2.4.0/mvt/ios/modules/backup/manifest.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     """This module extracts information from a backup Manifest.db file."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def _get_key(self, dictionary, key):
         """Unserialized plist objects can have keys which are str or byte types
         This is a helper to try fetch a key as both a byte or string type.
@@ -87,27 +87,14 @@
         return records
 
     def check_indicators(self) -> None:
         for result in self.results:
             if not result.get("relative_path"):
                 continue
 
-            if result["domain"]:
-                if (
-                    os.path.basename(result["relative_path"])
-                    == "com.apple.CrashReporter.plist"
-                    and result["domain"] == "RootDomain"
-                ):
-                    self.log.warning(
-                        "Found a potentially suspicious "
-                        '"com.apple.CrashReporter.plist" file created in RootDomain'
-                    )
-                    self.detected.append(result)
-                    continue
-
             if not self.indicators:
                 continue
 
             if self.indicators.check_file_path("/" + result["relative_path"]):
                 self.detected.append(result)
                 continue
```

### Comparing `mvt-2.3.0/mvt/ios/modules/backup/profile_events.py` & `mvt-2.4.0/mvt/ios/modules/backup/profile_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record.get("timestamp"),
```

### Comparing `mvt-2.3.0/mvt/ios/modules/base.py` & `mvt-2.4.0/mvt/ios/modules/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.is_backup = False
         self.is_fs_dump = False
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/__init__.py` & `mvt-2.4.0/mvt/ios/modules/fs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/analytics.py` & `mvt-2.4.0/mvt/ios/modules/fs/analytics.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     private/var/Keychains/Analytics/*.db files."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/analytics_ios_versions.py` & `mvt-2.4.0/mvt/ios/modules/fs/analytics_ios_versions.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     files."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/cache_files.py` & `mvt-2.4.0/mvt/ios/modules/fs/cache_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 class CacheFiles(IOSExtraction):
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         records = []
         for item in self.results[record]:
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/filesystem.py` & `mvt-2.4.0/mvt/ios/modules/mixed/osanalytics_addaily.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-import os
+import plistlib
 from typing import Optional, Union
 
-from mvt.common.utils import convert_unix_to_iso
+from mvt.common.utils import convert_datetime_to_iso
 
 from ..base import IOSExtraction
 
+OSANALYTICS_ADDAILY_BACKUP_IDS = [
+    "f65b5fafc69bbd3c60be019c6e938e146825fa83",
+]
+OSANALYTICS_ADDAILY_ROOT_PATHS = [
+    "private/var/mobile/Library/Preferences/com.apple.osanalytics.addaily.plist",
+]
 
-class Filesystem(IOSExtraction):
-    """This module extracts creation and modification date of files from a
-    full file-system dump.
-    """
+
+class OSAnalyticsADDaily(IOSExtraction):
+    """Extract network usage information by process,
+    from com.apple.osanalytics.addaily.plist"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
-            "timestamp": record["modified"],
+            "timestamp": record["ts"],
             "module": self.__class__.__name__,
-            "event": "entry_modified",
-            "data": record["path"],
+            "event": "osanalytics_addaily",
+            "data": f"{record['package']} WIFI IN: {record['wifi_in']}, "
+            f"WIFI OUT: {record['wifi_out']} - "
+            f"WWAN IN: {record['wwan_in']}, "
+            f"WWAN OUT: {record['wwan_out']}",
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
         for result in self.results:
-            if "path" not in result:
-                continue
-
-            ioc = self.indicators.check_file_path(result["path"])
+            ioc = self.indicators.check_process(result["package"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
-            # If we are instructed to run fast, we skip the rest.
-            if self.fast_mode:
-                continue
+    def run(self) -> None:
+        self._find_ios_database(
+            backup_ids=OSANALYTICS_ADDAILY_BACKUP_IDS,
+            root_paths=OSANALYTICS_ADDAILY_ROOT_PATHS,
+        )
+        self.log.info(
+            "Found com.apple.osanalytics.addaily plist at path: %s", self.file_path
+        )
 
-            ioc = self.indicators.check_file_path_process(result["path"])
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+        with open(self.file_path, "rb") as handle:
+            file_plist = plistlib.load(handle)
 
-    def run(self) -> None:
-        for root, dirs, files in os.walk(self.target_path):
-            for dir_name in dirs:
-                try:
-                    dir_path = os.path.join(root, dir_name)
-                    result = {
-                        "path": os.path.relpath(dir_path, self.target_path),
-                        "modified": convert_unix_to_iso(os.stat(dir_path).st_mtime),
-                    }
-                except Exception:
-                    continue
-                else:
-                    self.results.append(result)
-
-            for file_name in files:
-                try:
-                    file_path = os.path.join(root, file_name)
-                    result = {
-                        "path": os.path.relpath(file_path, self.target_path),
-                        "modified": convert_unix_to_iso(os.stat(file_path).st_mtime),
-                    }
-                except Exception:
-                    continue
-                else:
-                    self.results.append(result)
+        for app, values in file_plist.get("netUsageBaseline", {}).items():
+            self.results.append(
+                {
+                    "package": app,
+                    "ts": convert_datetime_to_iso(values[0]),
+                    "wifi_in": values[1],
+                    "wifi_out": values[2],
+                    "wwan_in": values[3],
+                    "wwan_out": values[4],
+                }
+            )
+
+        self.log.info(
+            "Extracted a total of %d com.apple.osanalytics.addaily entries",
+            len(self.results),
+        )
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/net_netusage.py` & `mvt-2.4.0/mvt/ios/modules/fs/net_netusage.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def run(self) -> None:
         for netusage_path in self._get_fs_files_from_patterns(NETUSAGE_ROOT_PATHS):
             self.file_path = netusage_path
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/safari_favicon.py` & `mvt-2.4.0/mvt/ios/modules/fs/safari_favicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """This module extracts all Safari favicon records."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/shutdownlog.py` & `mvt-2.4.0/mvt/ios/modules/fs/shutdownlog.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     """This module extracts processes information from the shutdown log file."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/version_history.py` & `mvt-2.4.0/mvt/ios/modules/fs/version_history.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """This module extracts iOS update history from Analytics Journal log files."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/webkit_base.py` & `mvt-2.4.0/mvt/ios/modules/fs/webkit_base.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/webkit_indexeddb.py` & `mvt-2.4.0/mvt/ios/modules/fs/webkit_indexeddb.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     slug = "webkit_indexeddb"
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/webkit_localstorage.py` & `mvt-2.4.0/mvt/ios/modules/fs/webkit_localstorage.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/fs/webkit_safariviewservice.py` & `mvt-2.4.0/mvt/ios/modules/fs/webkit_safariviewservice.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def run(self) -> None:
         self._process_webkit_folder(WEBKIT_SAFARIVIEWSERVICE_ROOT_PATHS)
         self.log.info(
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/__init__.py` & `mvt-2.4.0/mvt/ios/modules/mixed/__init__.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/applications.py` & `mvt-2.4.0/mvt/ios/modules/mixed/applications.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     """Extract information from accounts installed on the phone."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         if "isodate" in record:
             return {
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/calendar.py` & `mvt-2.4.0/mvt/ios/modules/mixed/calendar.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """This module extracts all calendar entries."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
         self.timestamps = [
             "start_date",
             "end_date",
             "last_modified",
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/calls.py` & `mvt-2.4.0/mvt/ios/modules/mixed/calls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
 import sqlite3
-from typing import Union
+from typing import Union, Optional
 
 from mvt.common.utils import convert_mactime_to_iso
 
 from ..base import IOSExtraction
 
 CALLS_BACKUP_IDS = [
     "5a4935c78a5255723f707230a451d79c540d2741",
@@ -21,23 +21,23 @@
     """This module extracts phone calls details"""
 
     def __init__(
         self,
         file_path: str = None,
         target_path: str = None,
         results_path: str = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: list = [],
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/chrome_favicon.py` & `mvt-2.4.0/mvt/ios/modules/mixed/chrome_favicon.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     """This module extracts all Chrome favicon records."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/chrome_history.py` & `mvt-2.4.0/mvt/ios/modules/mixed/chrome_history.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     """This module extracts all Chome visits."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/contacts.py` & `mvt-2.4.0/mvt/ios/modules/mixed/contacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,23 +21,23 @@
     """This module extracts all contact details from the phone's address book."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def run(self) -> None:
         self._find_ios_database(
             backup_ids=CONTACTS_BACKUP_IDS, root_paths=CONTACTS_ROOT_PATHS
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/firefox_favicon.py` & `mvt-2.4.0/mvt/ios/modules/mixed/firefox_favicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     """This module extracts all Firefox favicon"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/firefox_history.py` & `mvt-2.4.0/mvt/ios/modules/mixed/firefox_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/idstatuscache.py` & `mvt-2.4.0/mvt/ios/modules/mixed/idstatuscache.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     """Extracts Apple Authentication information from idstatuscache.plist"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/interactionc.py` & `mvt-2.4.0/mvt/ios/modules/mixed/interactionc.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,23 +217,23 @@
     """This module extracts data from InteractionC db."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.timestamps = [
             "start_date",
             "end_date",
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/locationd.py` & `mvt-2.4.0/mvt/ios/modules/mixed/locationd.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     """Extract information from apps who used geolocation."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.timestamps = [
             "ConsumptionPeriodBegin",
             "ReceivingLocationInformationTimeStopped",
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/net_datausage.py` & `mvt-2.4.0/mvt/ios/modules/mixed/net_datausage.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def run(self) -> None:
         self._find_ios_database(
             backup_ids=DATAUSAGE_BACKUP_IDS, root_paths=DATAUSAGE_ROOT_PATHS
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/osanalytics_addaily.py` & `mvt-2.4.0/mvt/android/modules/androidqf/dumpsys_appops.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,92 +1,94 @@
 # Mobile Verification Toolkit (MVT)
 # Copyright (c) 2021-2023 Claudio Guarnieri.
 # Use of this software is governed by the MVT License 1.1 that can be found at
 #   https://license.mvt.re/1.1/
 
 import logging
-import plistlib
 from typing import Optional, Union
 
-from mvt.common.utils import convert_datetime_to_iso
+from mvt.android.parsers import parse_dumpsys_appops
 
-from ..base import IOSExtraction
+from .base import AndroidQFModule
 
-OSANALYTICS_ADDAILY_BACKUP_IDS = [
-    "f65b5fafc69bbd3c60be019c6e938e146825fa83",
-]
-OSANALYTICS_ADDAILY_ROOT_PATHS = [
-    "private/var/mobile/Library/Preferences/com.apple.osanalytics.addaily.plist",
-]
-
-
-class OSAnalyticsADDaily(IOSExtraction):
-    """Extract network usage information by process,
-    from com.apple.osanalytics.addaily.plist"""
 
+class DumpsysAppops(AndroidQFModule):
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
-        return {
-            "timestamp": record["ts"],
-            "module": self.__class__.__name__,
-            "event": "osanalytics_addaily",
-            "data": f"{record['package']} WIFI IN: {record['wifi_in']}, "
-            f"WIFI OUT: {record['wifi_out']} - "
-            f"WWAN IN: {record['wwan_in']}, "
-            f"WWAN OUT: {record['wwan_out']}",
-        }
+        records = []
+        for perm in record["permissions"]:
+            if "entries" not in perm:
+                continue
+
+            for entry in perm["entries"]:
+                if "timestamp" in entry:
+                    records.append(
+                        {
+                            "timestamp": entry["timestamp"],
+                            "module": self.__class__.__name__,
+                            "event": entry["access"],
+                            "data": f"{record['package_name']} access to "
+                            f"{perm['name']} : {entry['access']}",
+                        }
+                    )
 
-    def check_indicators(self) -> None:
-        if not self.indicators:
-            return
+        return records
 
+    def check_indicators(self) -> None:
         for result in self.results:
-            ioc = self.indicators.check_process(result["package"])
-            if ioc:
-                result["matched_indicator"] = ioc
-                self.detected.append(result)
+            if self.indicators:
+                ioc = self.indicators.check_app_id(result.get("package_name"))
+                if ioc:
+                    result["matched_indicator"] = ioc
+                    self.detected.append(result)
+                    continue
+
+            for perm in result["permissions"]:
+                if (
+                    perm["name"] == "REQUEST_INSTALL_PACKAGES"
+                    and perm["access"] == "allow"
+                ):
+                    self.log.info(
+                        "Package %s with REQUEST_INSTALL_PACKAGES permission",
+                        result["package_name"],
+                    )
 
     def run(self) -> None:
-        self._find_ios_database(
-            backup_ids=OSANALYTICS_ADDAILY_BACKUP_IDS,
-            root_paths=OSANALYTICS_ADDAILY_ROOT_PATHS,
-        )
-        self.log.info(
-            "Found com.apple.osanalytics.addaily plist at path: %s", self.file_path
-        )
+        dumpsys_file = self._get_files_by_pattern("*/dumpsys.txt")
+        if not dumpsys_file:
+            return
 
-        with open(self.file_path, "rb") as handle:
-            file_plist = plistlib.load(handle)
+        lines = []
+        in_package = False
+        with open(dumpsys_file[0]) as handle:
+            for line in handle:
+                if line.startswith("DUMP OF SERVICE appops:"):
+                    in_package = True
+                    continue
+
+                if in_package:
+                    if line.startswith(
+                        "-------------------------------------------------------------------------------"
+                    ):  # pylint: disable=line-too-long
+                        break
 
-        for app, values in file_plist.get("netUsageBaseline", {}).items():
-            self.results.append(
-                {
-                    "package": app,
-                    "ts": convert_datetime_to_iso(values[0]),
-                    "wifi_in": values[1],
-                    "wifi_out": values[2],
-                    "wwan_in": values[3],
-                    "wwan_out": values[4],
-                }
-            )
-
-        self.log.info(
-            "Extracted a total of %d com.apple.osanalytics.addaily entries",
-            len(self.results),
-        )
+                    lines.append(line.rstrip())
+
+        self.results = parse_dumpsys_appops("\n".join(lines))
+        self.log.info("Identified %d applications in AppOps Manager", len(self.results))
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/safari_browserstate.py` & `mvt-2.4.0/mvt/ios/modules/mixed/safari_browserstate.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     """This module extracts all Safari browser state records."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self._session_history_count = 0
 
     def serialize(self, record: dict) -> Union[dict, list]:
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/safari_history.py` & `mvt-2.4.0/mvt/ios/modules/mixed/safari_history.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,23 +28,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/shortcuts.py` & `mvt-2.4.0/mvt/ios/modules/mixed/shortcuts.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     """This module extracts all info about SMS/iMessage attachments."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         found_urls = ""
         if record["action_urls"]:
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/sms.py` & `mvt-2.4.0/mvt/ios/modules/mixed/sms.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,38 +24,54 @@
     """This module extracts all SMS messages containing links."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         text = record["text"].replace("\n", "\\n")
-        return {
-            "timestamp": record["isodate"],
-            "module": self.__class__.__name__,
-            "event": "sms_received",
-            "data": f"{record['service']}: {record['guid']} \"{text}\" "
-            f"from {record['phone_number']} ({record['account']})",
-        }
+        sms_data = f"{record['service']}: {record['guid']} \"{text}\" from {record['phone_number']} ({record['account']})"
+        return [
+            {
+                "timestamp": record["isodate"],
+                "module": self.__class__.__name__,
+                "event": "sms_received",
+                "data": sms_data,
+            },
+            {
+                "timestamp": record["isodate_read"],
+                "module": self.__class__.__name__,
+                "event": "sms_read",
+                "data": sms_data,
+            },
+        ]
 
     def check_indicators(self) -> None:
+        for message in self.results:
+            alert = "ALERT: State-sponsored attackers may be targeting your iPhone"
+            if message.get("text", "").startswith(alert):
+                self.log.warning(
+                    "Apple warning about state-sponsored attack received on the %s",
+                    message["isodate"],
+                )
+
         if not self.indicators:
             return
 
         for result in self.results:
             message_links = result.get("links", [])
             # Making sure not link was ignored
             if message_links == []:
@@ -116,32 +132,25 @@
                     value = b64encode(value).decode()
 
                 # We store the value of each column under the proper key.
                 message[names[index]] = value
 
             # We convert Mac's ridiculous timestamp format.
             message["isodate"] = convert_mactime_to_iso(message["date"])
+            message["isodate_read"] = convert_mactime_to_iso(message["date_read"])
             message["direction"] = (
                 "sent" if message.get("is_from_me", 0) == 1 else "received"
             )
 
             # Sometimes "text" is None instead of empty string.
             if not message.get("text", None):
                 message["text"] = ""
 
-            alert = "ALERT: State-sponsored attackers may be targeting your iPhone"
-            if message.get("text", "").startswith(alert):
-                self.log.warning(
-                    "Apple warning about state-sponsored attack received on the %s",
-                    message["isodate"],
-                )
-            else:
-                # Extract links from the SMS message.
-                message_links = check_for_links(message.get("text", ""))
-                message["links"] = message_links
-
+            # Extract links from the SMS message.
+            message_links = check_for_links(message.get("text", ""))
+            message["links"] = message_links
             self.results.append(message)
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d SMS messages", len(self.results))
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/sms_attachments.py` & `mvt-2.4.0/mvt/ios/modules/mixed/sms_attachments.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     """This module extracts all info about SMS/iMessage attachments."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         return {
             "timestamp": record["isodate"],
@@ -50,14 +50,28 @@
             f"'{record['transfer_name']}' {record['direction']} "
             f"from {record['phone_number']} "
             f"with {record['total_bytes']} bytes "
             f"(is_sticker: {record['is_sticker']}, "
             f"has_user_info: {record['has_user_info']})",
         }
 
+    def check_indicators(self) -> None:
+        for attachment in self.results:
+            if (
+                attachment["filename"].startswith("/var/tmp/")
+                and attachment["filename"].endswith("-1")
+                and attachment["direction"] == "received"
+            ):
+                self.log.warning(
+                    "Suspicious iMessage attachment %s on %s",
+                    attachment["filename"],
+                    attachment["isodate"],
+                )
+                self.detected.append(attachment)
+
     def run(self) -> None:
         self._find_ios_database(backup_ids=SMS_BACKUP_IDS, root_paths=SMS_ROOT_PATHS)
         self.log.info("Found SMS database at path: %s", self.file_path)
 
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
         cur.execute(
@@ -97,26 +111,13 @@
             attachment["start_date"] = convert_mactime_to_iso(attachment["start_date"])
             attachment["direction"] = (
                 "sent" if attachment["is_outgoing"] == 1 else "received"
             )
             attachment["has_user_info"] = attachment["user_info"] is not None
             attachment["service"] = attachment["service"] or "Unknown"
             attachment["filename"] = attachment["filename"] or "NULL"
-
-            if (
-                attachment["filename"].startswith("/var/tmp/")
-                and attachment["filename"].endswith("-1")
-                and attachment["direction"] == "received"
-            ):
-                self.log.warning(
-                    "Suspicious iMessage attachment %s on %s",
-                    attachment["filename"],
-                    attachment["isodate"],
-                )
-                self.detected.append(attachment)
-
             self.results.append(attachment)
 
         cur.close()
         conn.close()
 
         self.log.info("Extracted a total of %d SMS attachments", len(self.results))
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/tcc.py` & `mvt-2.4.0/mvt/ios/modules/mixed/tcc.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,23 +45,23 @@
     """This module extracts records from the TCC.db SQLite database."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         if "last_modified" in record:
             if "allowed_value" in record:
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py` & `mvt-2.4.0/mvt/ios/modules/mixed/webkit_resource_load_statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     observations.db."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = [] if not results else results
 
     def serialize(self, record: dict) -> Union[dict, list]:
@@ -54,15 +54,15 @@
             "data": msg,
         }
 
     def check_indicators(self) -> None:
         if not self.indicators:
             return
 
-        self.detected = {}
+        self.detected = []
         for result in self.results:
             ioc = self.indicators.check_domain(result["registrable_domain"])
             if ioc:
                 result["matched_indicator"] = ioc
                 self.detected.append(result)
 
     def _process_observations_db(self, db_path: str, domain: str, path: str) -> None:
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/webkit_session_resource_log.py` & `mvt-2.4.0/mvt/ios/modules/mixed/webkit_session_resource_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     """
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
         self.results = {} if not results else results
 
     @staticmethod
```

### Comparing `mvt-2.3.0/mvt/ios/modules/mixed/whatsapp.py` & `mvt-2.4.0/mvt/ios/modules/mixed/whatsapp.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,23 @@
     """This module extracts all WhatsApp messages containing links."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def serialize(self, record: dict) -> Union[dict, list]:
         text = record.get("ZTEXT", "").replace("\n", "\\n")
         links_text = ""
```

### Comparing `mvt-2.3.0/mvt/ios/modules/net_base.py` & `mvt-2.4.0/mvt/ios/modules/net_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,23 @@
     modules."""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         target_path: Optional[str] = None,
         results_path: Optional[str] = None,
-        fast_mode: bool = False,
+        module_options: Optional[dict] = None,
         log: logging.Logger = logging.getLogger(__name__),
         results: Optional[list] = None,
     ) -> None:
         super().__init__(
             file_path=file_path,
             target_path=target_path,
             results_path=results_path,
-            fast_mode=fast_mode,
+            module_options=module_options,
             log=log,
             results=results,
         )
 
     def _extract_net_data(self):
         conn = sqlite3.connect(self.file_path)
         cur = conn.cursor()
@@ -153,17 +153,17 @@
         if not self.is_fs_dump:
             return
 
         if not self.results:
             return
 
         # If we are instructed to run fast, we skip this.
-        if self.fast_mode:
+        if self.module_options.get("fast_mode", None):
             self.log.info(
-                "Flag --fast was enabled: skipping extended "
+                "Option 'fast_mode' was enabled: skipping extended "
                 "search for suspicious processes"
             )
             return
 
         self.log.info("Extended search for suspicious processes ...")
 
         files = []
```

### Comparing `mvt-2.3.0/mvt/ios/versions.py` & `mvt-2.4.0/mvt/ios/versions.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/mvt.egg-info/PKG-INFO` & `mvt-2.4.0/mvt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvt
-Version: 2.3.0
+Version: 2.4.0
 Summary: Mobile Verification Toolkit
 Home-page: https://github.com/mvt-project/mvt
 Author: Claudio Guarnieri
 Author-email: nex@nex.sx
 License: MVT v1.1
 Keywords: security,mobile,forensics,malware
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mvt-2.3.0/mvt.egg-info/SOURCES.txt` & `mvt-2.4.0/mvt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/setup.cfg` & `mvt-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android/test_backup_module.py` & `mvt-2.4.0/tests/android/test_backup_module.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android/test_backup_parser.py` & `mvt-2.4.0/tests/android/test_backup_parser.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android/test_dumpsys_parser.py` & `mvt-2.4.0/tests/android/test_dumpsys_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def test_appops_parsing(self):
         file = get_artifact("android_data/dumpsys_appops.txt")
         with open(file) as f:
             data = f.read()
 
         res = parse_dumpsys_appops(data)
 
-        assert len(res) == 12
+        assert len(res) == 13
         assert res[0]["package_name"] == "com.android.phone"
         assert res[0]["uid"] == "0"
         assert len(res[0]["permissions"]) == 1
         assert res[0]["permissions"][0]["name"] == "MANAGE_IPSEC_TUNNELS"
         assert res[0]["permissions"][0]["access"] == "allow"
         assert res[6]["package_name"] == "com.sec.factory.camera"
         assert len(res[6]["permissions"][1]["entries"]) == 1
```

### Comparing `mvt-2.3.0/tests/android_androidqf/test_dumpsysaccessbility.py` & `mvt-2.4.0/tests/android_androidqf/test_dumpsysaccessbility.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_dumpsysappops.py` & `mvt-2.4.0/tests/android_androidqf/test_dumpsysappops.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_dumpsyspackages.py` & `mvt-2.4.0/tests/android_androidqf/test_dumpsyspackages.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_dumpsysreceivers.py` & `mvt-2.4.0/tests/android_androidqf/test_dumpsysreceivers.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_getprop.py` & `mvt-2.4.0/tests/android_androidqf/test_getprop.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_processes.py` & `mvt-2.4.0/tests/android_androidqf/test_processes.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_settings.py` & `mvt-2.4.0/tests/android_androidqf/test_settings.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_androidqf/test_sms.py` & `mvt-2.4.0/tests/android_androidqf/test_sms.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/android_bugreport/test_bugreport.py` & `mvt-2.4.0/tests/android_bugreport/test_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/common/test_indicators.py` & `mvt-2.4.0/tests/common/test_indicators.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/common/test_utils.py` & `mvt-2.4.0/tests/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/conftest.py` & `mvt-2.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_backup_info.py` & `mvt-2.4.0/tests/ios_backup/test_backup_info.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_calendar.py` & `mvt-2.4.0/tests/ios_backup/test_calendar.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_datausage.py` & `mvt-2.4.0/tests/ios_backup/test_datausage.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_manifest.py` & `mvt-2.4.0/tests/ios_backup/test_manifest.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_safari_browserstate.py` & `mvt-2.4.0/tests/ios_backup/test_safari_browserstate.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_sms.py` & `mvt-2.4.0/tests/ios_backup/test_sms.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class TestSMSModule:
     def test_sms(self):
         m = SMS(target_path=get_ios_backup_folder())
         run_module(m)
         assert len(m.results) == 1
-        assert len(m.timeline) == 1
+        assert len(m.timeline) == 2  # SMS received and read events.
         assert len(m.detected) == 0
 
     def test_detection(self, indicator_file):
         m = SMS(target_path=get_ios_backup_folder())
         ind = Indicators(log=logging.getLogger())
         ind.parse_stix2(indicator_file)
         # Adds a file that exists in the manifest.
```

### Comparing `mvt-2.3.0/tests/ios_backup/test_tcc.py` & `mvt-2.4.0/tests/ios_backup/test_tcc.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_backup/test_webkit_resource_load_statistics.py` & `mvt-2.4.0/tests/ios_backup/test_webkit_resource_load_statistics.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/ios_fs/test_filesystem.py` & `mvt-2.4.0/tests/ios_fs/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/test_check_android_androidqf.py` & `mvt-2.4.0/tests/test_check_android_androidqf.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/test_check_android_bugreport.py` & `mvt-2.4.0/tests/test_check_android_bugreport.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/test_check_ios_backup.py` & `mvt-2.4.0/tests/test_check_ios_backup.py`

 * *Files identical despite different names*

### Comparing `mvt-2.3.0/tests/utils.py` & `mvt-2.4.0/tests/utils.py`

 * *Files identical despite different names*

