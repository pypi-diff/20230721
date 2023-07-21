# Comparing `tmp/kameleo.local_api_client-2.9.0.tar.gz` & `tmp/kameleo.local_api_client-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kameleo.local_api_client-2.9.0.tar", last modified: Fri Aug 19 09:54:29 2022, max compression
+gzip compressed data, was "kameleo.local_api_client-3.0.0.tar", last modified: Fri Jul 21 06:22:25 2023, max compression
```

## Comparing `kameleo.local_api_client-2.9.0.tar` & `kameleo.local_api_client-3.0.0.tar`

### file list

```diff
@@ -1,87 +1,42 @@
-drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.583867 kameleo.local_api_client-2.9.0/
--rw-rw-rw-   0        0        0     1100 2021-07-21 14:14:28.000000 kameleo.local_api_client-2.9.0/LICENSE.txt
--rw-rw-rw-   0        0        0     9589 2022-08-19 09:54:29.582892 kameleo.local_api_client-2.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     9023 2022-08-19 09:48:42.000000 kameleo.local_api_client-2.9.0/README.md
-drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.428869 kameleo.local_api_client-2.9.0/kameleo/
--rw-rw-rw-   0        0        0       57 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.443895 kameleo.local_api_client-2.9.0/kameleo/local_api_client/
--rw-rw-rw-   0        0        0      479 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/__init__.py
--rw-rw-rw-   0        0        0    12918 2022-08-19 09:33:39.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/builder_for_create_profile.py
--rw-rw-rw-   0        0        0    48266 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/kameleo_local_api_client.py
-drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.580873 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/
--rw-rw-rw-   0        0        0     6325 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/__init__.py
--rw-rw-rw-   0        0        0     3065 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile.py
--rw-rw-rw-   0        0        0     2048 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_preview.py
--rw-rw-rw-   0        0        0     2004 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_preview_py3.py
--rw-rw-rw-   0        0        0     2988 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_py3.py
--rw-rw-rw-   0        0        0     2125 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_search_parameters.py
--rw-rw-rw-   0        0        0     2112 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/base_profile_search_parameters_py3.py
--rw-rw-rw-   0        0        0     1383 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser.py
--rw-rw-rw-   0        0        0     5149 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_cookie.py
--rw-rw-rw-   0        0        0     5118 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_cookie_py3.py
--rw-rw-rw-   0        0        0     1374 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/browser_py3.py
--rw-rw-rw-   0        0        0     4298 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/cookie_request.py
--rw-rw-rw-   0        0        0     4287 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/cookie_request_py3.py
--rw-rw-rw-   0        0        0     5865 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/create_profile_request.py
--rw-rw-rw-   0        0        0     5757 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/create_profile_request_py3.py
--rw-rw-rw-   0        0        0     1092 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/device.py
--rw-rw-rw-   0        0        0     1090 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/device_py3.py
--rw-rw-rw-   0        0        0     1168 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice.py
--rw-rw-rw-   0        0        0     1158 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/font_spoofing_type_font_ilist_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1231 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_options.py
--rw-rw-rw-   0        0        0     1237 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_options_py3.py
--rw-rw-rw-   0        0        0     1333 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice.py
--rw-rw-rw-   0        0        0     1323 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0      932 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request.py
--rw-rw-rw-   0        0        0      934 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request_py3.py
--rw-rw-rw-   0        0        0     1513 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/os.py
--rw-rw-rw-   0        0        0     1506 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/os_py3.py
--rw-rw-rw-   0        0        0     1180 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice.py
--rw-rw-rw-   0        0        0     1170 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/plugin_spoofing_type_plugin_ilist_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1192 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/preference.py
--rw-rw-rw-   0        0        0     1180 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/preference_py3.py
--rw-rw-rw-   0        0        0     1303 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/problem_response.py
--rw-rw-rw-   0        0        0     1302 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/problem_response_py3.py
--rw-rw-rw-   0        0        0     2958 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_preview.py
--rw-rw-rw-   0        0        0     2904 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_preview_py3.py
--rw-rw-rw-   0        0        0     7042 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_response.py
--rw-rw-rw-   0        0        0     6882 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/profile_response_py3.py
--rw-rw-rw-   0        0        0     1215 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice.py
--rw-rw-rw-   0        0        0     1205 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/proxy_connection_type_server_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0      921 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/save_profile_request.py
--rw-rw-rw-   0        0        0      923 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/save_profile_request_py3.py
--rw-rw-rw-   0        0        0     1252 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice.py
--rw-rw-rw-   0        0        0     1247 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1852 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/server.py
--rw-rw-rw-   0        0        0     1837 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/server_py3.py
--rw-rw-rw-   0        0        0     1844 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/status_response.py
--rw-rw-rw-   0        0        0     1871 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/status_response_py3.py
--rw-rw-rw-   0        0        0     1188 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_request.py
--rw-rw-rw-   0        0        0     1173 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_request_py3.py
--rw-rw-rw-   0        0        0     1670 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_response.py
--rw-rw-rw-   0        0        0     1677 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/test_proxy_response_py3.py
--rw-rw-rw-   0        0        0     1302 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice.py
--rw-rw-rw-   0        0        0     1297 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/timezone_spoofing_type_timezone_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     5691 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/update_profile_request.py
--rw-rw-rw-   0        0        0     5576 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/update_profile_request_py3.py
--rw-rw-rw-   0        0        0     2067 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/user_info_response.py
--rw-rw-rw-   0        0        0     2057 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/user_info_response_py3.py
--rw-rw-rw-   0        0        0     1831 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_driver_settings.py
--rw-rw-rw-   0        0        0     1841 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_driver_settings_py3.py
--rw-rw-rw-   0        0        0     1327 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_options.py
--rw-rw-rw-   0        0        0     1331 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_options_py3.py
--rw-rw-rw-   0        0        0     1293 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice.py
--rw-rw-rw-   0        0        0     1283 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0     1013 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_options.py
--rw-rw-rw-   0        0        0     1022 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_options_py3.py
--rw-rw-rw-   0        0        0     1265 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice.py
--rw-rw-rw-   0        0        0     1255 2022-02-10 08:12:52.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/webgl_spoofing_type_webgl_spoofing_options_multi_level_choice_py3.py
--rw-rw-rw-   0        0        0      343 2022-08-19 09:53:43.000000 kameleo.local_api_client-2.9.0/kameleo/local_api_client/version.py
-drwxrwxrwx   0        0        0        0 2022-08-19 09:54:29.436894 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/
--rw-rw-rw-   0        0        0     9589 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4746 2022-08-19 09:54:29.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-19 09:54:28.000000 kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-19 09:54:29.584880 kameleo.local_api_client-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1016 2022-02-18 09:57:17.000000 kameleo.local_api_client-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.950855 kameleo.local_api_client-3.0.0/
+-rw-rw-rw-   0        0        0     1100 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    11384 2023-07-21 06:22:25.949874 kameleo.local_api_client-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10813 2023-07-20 10:31:06.000000 kameleo.local_api_client-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.808854 kameleo.local_api_client-3.0.0/kameleo/
+-rw-rw-rw-   0        0        0       82 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.908855 kameleo.local_api_client-3.0.0/kameleo/local_api_client/
+-rw-rw-rw-   0        0        0      807 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/__init__.py
+-rw-rw-rw-   0        0        0     3080 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_client.py
+-rw-rw-rw-   0        0        0     1974 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.916853 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_operations/
+-rw-rw-rw-   0        0        0      727 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_operations/__init__.py
+-rw-rw-rw-   0        0        0    85639 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_operations/_patch.py
+-rw-rw-rw-   0        0        0      694 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_patch.py
+-rw-rw-rw-   0        0        0    80832 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_serialization.py
+-rw-rw-rw-   0        0        0     1435 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_vendor.py
+-rw-rw-rw-   0        0        0      390 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.930853 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/
+-rw-rw-rw-   0        0        0      751 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/__init__.py
+-rw-rw-rw-   0        0        0     3185 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_client.py
+-rw-rw-rw-   0        0        0     1985 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_configuration.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.936852 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_operations/
+-rw-rw-rw-   0        0        0      727 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_operations/__init__.py
+-rw-rw-rw-   0        0        0    72648 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_operations/_operations.py
+-rw-rw-rw-   0        0        0      694 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_operations/_patch.py
+-rw-rw-rw-   0        0        0      694 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_patch.py
+-rw-rw-rw-   0        0        0      929 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_vendor.py
+-rw-rw-rw-   0        0        0    12002 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/builder_for_create_profile.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.947858 kameleo.local_api_client-3.0.0/kameleo/local_api_client/models/
+-rw-rw-rw-   0        0        0     3942 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/models/__init__.py
+-rw-rw-rw-   0        0        0     6341 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/models/_enums.py
+-rw-rw-rw-   0        0        0   106457 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/models/_models.py
+-rw-rw-rw-   0        0        0      694 2023-07-20 09:02:55.000000 kameleo.local_api_client-3.0.0/kameleo/local_api_client/models/_patch.py
+drwxrwxrwx   0        0        0        0 2023-07-21 06:22:25.869852 kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/
+-rw-rw-rw-   0        0        0    11384 2023-07-21 06:22:25.000000 kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2023-07-21 06:22:25.000000 kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 06:22:25.000000 kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 06:22:25.000000 kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 06:22:25.000000 kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 06:22:25.950855 kameleo.local_api_client-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      895 2023-07-20 09:03:28.000000 kameleo.local_api_client-3.0.0/setup.py
```

### Comparing `kameleo.local_api_client-2.9.0/LICENSE.txt` & `kameleo.local_api_client-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kameleo.local_api_client-2.9.0/PKG-INFO` & `kameleo.local_api_client-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,15 @@
-Metadata-Version: 2.1
-Name: kameleo.local_api_client
-Version: 2.9.0
-Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
-Home-page: https://github.com/kameleo-io/local-api-client-python
-Author: Kameleo Team
-Author-email: support@kameleo.io
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <img src="https://raw.githubusercontent.com/kameleo-io/local-api-client-python/HEAD/docs/kameleo-logo.png" width="150" align="right" />
 
 # Kameleo Local API Client
 With [Kameleo](https://kameleo.io), you can easily create multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
 
 
 # Features
-- Stay completely undetected, so websites wonâ€™t be able to detect that you are using automation tools
+- Stay completely undetected, so websites won’t be able to detect that you are using automation tools
 - Start unlimited number of profiles with different natural browser fingerprints
 - Use authenticated HTTP/SOCKS/SSH proxies in browsers
 - Create isolated browsing environments simultaneously
 - Use real browser profiles of Chrome, Firefox, Safari and Edge
 - Edit, Import or Export browser cookies
 - Modify WebRTC parameters
 - Modify Geolocation settings
@@ -45,57 +30,53 @@
 ```
 
 ## 2. Start the Kameleo.CLI on your computer
 ```
 ./Kameleo.CLI.exe email="your@email.com" password="Pa$$w0rd"
 ```
 
-## 3. Start a browser with out-of-the-box fingerprinting protection 
+## 3. Start a browser with out-of-the-box fingerprinting protection
 ```python
-from kameleo.local_api_client.kameleo_local_api_client import KameleoLocalApiClient
+from kameleo.local_api_client import KameleoLocalApiClient
 from kameleo.local_api_client.builder_for_create_profile import BuilderForCreateProfile
-from kameleo.local_api_client.models.problem_response_py3 import ProblemResponseException
-import json
 
-try:
-    client = KameleoLocalApiClient()
-    base_profiles = client.search_base_profiles(
-        device_type='desktop',
-        browser_product='chrome'
-    )
-    
-    # Create a new profile with recommended settings
-    # for browser fingerprinting protection
-    create_profile_request = BuilderForCreateProfile \
-        .for_base_profile(base_profiles[0].id) \
-        .set_recommended_defaults() \
-        .build()
-    profile = client.create_profile(body=create_profile_request)
-    
-    # Start the browser
-    client.start_profile(profile.id)
-    
-    # At this point you can automate the browser with your favorite framework
-except ProblemResponseException as e:
-    raise Exception([str(e), json.dumps(e.error.error)])
+client = KameleoLocalApiClient()
+base_profiles = client.search_base_profiles(
+    device_type='desktop',
+    browser_product='chrome'
+)
+
+# Create a new profile with recommended settings
+# for browser fingerprinting protection
+create_profile_request = BuilderForCreateProfile \
+    .for_base_profile(base_profiles[0].id) \
+    .set_recommended_defaults() \
+    .build()
+profile = client.create_profile(body=create_profile_request)
+
+# Start the browser
+client.start_profile(profile.id)
+
+# At this point you can automate the browser with your favorite framework
 ```
 
 # Automate Kameleo profiles with Selenium
 Kameleo gives you the ability to control any supported browser using Selenium. It uses the WebDriver protocol, a W3C specification, and industry-standard to interact with a browser.
 
 You need to install the official [Selenium package](https://pypi.org/project/selenium/).
 
 ```python
 from selenium import webdriver
 ```
 
 ```python
 # Connect to the running browser instance using WebDriver
+kameleo_port = 5050
 options = webdriver.ChromeOptions()
-options.add_experimental_option("kameleo:profileId", profile.id)
+options.add_experimental_option('kameleo:profileId', profile.id)
 driver = webdriver.Remote(
     command_executor=f'http://localhost:{kameleo_port}/webdriver',
     options=options
 )
 
 # Use any WebDriver command to drive the browser
 # and enjoy full protection from bot detection products
@@ -106,43 +87,47 @@
 
 # Automate Kameleo profiles with Puppeteer (Chromium-based)
 Kameleo lets you control Chromium-based browsers (sorry Firefox fans) using the [Pyppeteer library](https://pypi.org/project/pyppeteer/). In this simple example you can see how to connect to the browser that Kameleo starts.
 
 You need to import the [Pyppeteer library](https://pypi.org/project/pyppeteer/).
 
 ```python
-import pyppeteer   
+import pyppeteer
 ```
 
 ```python
 # Connect to the browser with Puppeteer through CDP
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/puppeteer/{profile.id}'
 browser = await pyppeteer.launcher.connect(browserWSEndpoint=browser_ws_endpoint, defaultViewport=False)
 page = await browser.newPage()
 
 # Use any Playwright command to drive the browser
 # and enjoy full protection from bot detection products
 await page.goto('https://google.com')
 ```
 
-The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_puppeteer_to_chrome/app.py).
+The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_puppeteer/app.py).
 
 # Automate Kameleo profiles with Playwright
 Kameleo allows you to control the browser with the official [Playwright package](https://pypi.org/project/playwright/). It works little bit different with Chromium-based browsers and Firefox, so we provide an example for both. Here we showcase how you can connect to the browser that is already started by Kameleo.
 
 You need to import the official [Playwright package](https://pypi.org/project/playwright/).
 ```python
 import playwright
 from playwright.sync_api import sync_playwright
 ```
 
+You can find more details here: [Using Kameleo with Playwright framework – Kameleo Support Center](https://help.kameleo.io/hc/en-us/articles/4419471627793-Using-Kameleo-with-Playwright-framework).
+
 ## Chromium-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright through CDP
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
     browser = playwright.chromium.connect_over_cdp(endpoint_url=browser_ws_endpoint)
     context = browser.contexts[0]
     page = context.new_page()
 
     # Use any Playwright command to drive the browser
@@ -152,61 +137,106 @@
 
 The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_playwright_to_chrome/app.py).
 
 ## Firefox-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
+    # The exact path to the bridge executable is subject to change. Here, we use %LOCALAPPDATA%\Programs\Kameleo\pw-bridge.exe
+    executable_path_example = path.expandvars(r'%LOCALAPPDATA%\Programs\Kameleo\pw-bridge.exe')
     browser = playwright.firefox.launch_persistent_context(
         '',
         # The Playwright framework is not designed to connect to already running
         # browsers. To overcome this limitation, a tool bundled with Kameleo, named
         # pw-bridge.exe will bridge the communication gap between the running Firefox
         # instance and this playwright script.
-        executable_path='<PATH_TO_KAMELEO_FOLDER>\\pw-bridge.exe',
+        executable_path=executable_path_example,
         args=[f'-target {browser_ws_endpoint}'],
         viewport=None)
-    
+
     # Kameleo will open the a new page in the default browser context.
-    # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere 
+    # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere
     #       with Kameleo's browser fingerprint modification features.
     page = browser.new_page()
 
     # Use any Playwright command to drive the browser
     # and enjoy full protection from bot detection products
     page.goto('https://google.com')
 
     # Here we need to close the browser object as well, it is not enough just to stop the profile
     client.stop_profile(profile.id)
     browser.close()
 ```
 
 The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_playwright_to_firefox/app.py).
 
+# Automate mobile profiles
+Kameleo can emulate mobile devices in the custom built Chromium.
+
+```python
+# Search for a mobile Base Profiles
+base_profile_list = client.search_base_profiles(
+    device_type='mobile',
+    os_family='ios',
+    browser_product='safari',
+    language='en-us'
+)
+
+# Create a new profile with recommended settings
+# Choose one of the Base Profiles
+# Set the launcher to 'chromium' so the mobile profile will be started in Chromium by Kameleo
+create_profile_request = BuilderForCreateProfile \
+    .for_base_profile(base_profile_list[0].id) \
+    .set_recommended_defaults() \
+    .set_launcher('chromium') \
+    .build()
+profile = client.create_profile(body=create_profile_request)
+
+# Start the profile
+client.start_profile_with_options(profile.id, body={
+    # This allows you to click on elements using the cursor when emulating a touch screen in the browser.
+    # If you leave this out, your script may time out after clicks and fail.
+    'additionalOptions': [
+        {
+            'key': 'disableTouchEmulation',
+            'value': True,
+        },
+    ],
+})
+
+# At this point you can automate the browser with your favorite framework
+```
+The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/automate_mobile_profiles_on_desktop/app.py).
+
+
 # Example codes
 [Several examples](https://github.com/kameleo-io/local-api-examples) have been prepared in a different repository to showcase the most interesting features. Feel free to create a pull request to add new example codes.
 
 - Finding base profiles
 - Creating profiles with custom options
 - Updating profiles with new settings
 - How to start a profile
 - Using Selenium with Local API
 - Using Playwright with Kameleo
 - Using Puppeteer with Kameleo
+- How to emulate mobile devices
 - Adding an HTTP, SOCKS or SSH proxy to profile
 - Saving/Loading a browsing session to/from a .kameleo file
 - Modify and Delete browser cookies
 - Start profile with extra WebDriver capabilities
+- How to duplicate virtual browser profiles
+- Refresh the browser of the emulated profiles
 
 > Note: _If you are interested in more information about Kameleo, or have encountered an issue with using it, please check out our [Help Center](https://help.kameleo.io/)._
 
 
 # Endpoints
 Available API endpoints with exhaustive descriptions and example values are documented on this [SwaggerHub](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) page. This package has built-in [IntelliSense](https://code.visualstudio.com/docs/editor/intellisense) support in Visual Studio Code, no extra package installation needed.
 
+# Package
+This package can be found on PyPI here: [kameleo.local-api-client](https://pypi.org/project/kameleo.local-api-client/).
 
 # License
 This project is released under MIT License. Please refer the LICENSE.txt for more details.
-
-
```

### Comparing `kameleo.local_api_client-2.9.0/README.md` & `kameleo.local_api_client-3.0.0/kameleo.local_api_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,30 @@
+Metadata-Version: 2.1
+Name: kameleo.local-api-client
+Version: 3.0.0
+Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
+Home-page: https://github.com/kameleo-io/local-api-client-python
+Author: Kameleo Team
+Author-email: support@kameleo.io
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <img src="https://raw.githubusercontent.com/kameleo-io/local-api-client-python/HEAD/docs/kameleo-logo.png" width="150" align="right" />
 
 # Kameleo Local API Client
 With [Kameleo](https://kameleo.io), you can easily create multiple virtual browser profiles to work with multiple accounts. It helps you hide your actual timezone, geolocation, language, IP address and creates natural browser fingerprints to prevent detection by anti-bot systems. Kameleo is compatible with [Selenium](https://www.selenium.dev/), [Playwright](https://playwright.dev/), and [Puppeteer](https://pptr.dev/) frameworks for automating web scraping tasks. This Python package provides convenient access to the [Local API](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) REST interface of the Kameleo Client. See the [article](https://help.kameleo.io/hc/en-us/articles/4418166326417) in our knowledge base for Getting Started with Kameleo Automation.
 
 
 # Features
-- Stay completely undetected, so websites won’t be able to detect that you are using automation tools
+- Stay completely undetected, so websites wonâ€™t be able to detect that you are using automation tools
 - Start unlimited number of profiles with different natural browser fingerprints
 - Use authenticated HTTP/SOCKS/SSH proxies in browsers
 - Create isolated browsing environments simultaneously
 - Use real browser profiles of Chrome, Firefox, Safari and Edge
 - Edit, Import or Export browser cookies
 - Modify WebRTC parameters
 - Modify Geolocation settings
@@ -30,57 +45,53 @@
 ```
 
 ## 2. Start the Kameleo.CLI on your computer
 ```
 ./Kameleo.CLI.exe email="your@email.com" password="Pa$$w0rd"
 ```
 
-## 3. Start a browser with out-of-the-box fingerprinting protection 
+## 3. Start a browser with out-of-the-box fingerprinting protection
 ```python
-from kameleo.local_api_client.kameleo_local_api_client import KameleoLocalApiClient
+from kameleo.local_api_client import KameleoLocalApiClient
 from kameleo.local_api_client.builder_for_create_profile import BuilderForCreateProfile
-from kameleo.local_api_client.models.problem_response_py3 import ProblemResponseException
-import json
 
-try:
-    client = KameleoLocalApiClient()
-    base_profiles = client.search_base_profiles(
-        device_type='desktop',
-        browser_product='chrome'
-    )
-    
-    # Create a new profile with recommended settings
-    # for browser fingerprinting protection
-    create_profile_request = BuilderForCreateProfile \
-        .for_base_profile(base_profiles[0].id) \
-        .set_recommended_defaults() \
-        .build()
-    profile = client.create_profile(body=create_profile_request)
-    
-    # Start the browser
-    client.start_profile(profile.id)
-    
-    # At this point you can automate the browser with your favorite framework
-except ProblemResponseException as e:
-    raise Exception([str(e), json.dumps(e.error.error)])
+client = KameleoLocalApiClient()
+base_profiles = client.search_base_profiles(
+    device_type='desktop',
+    browser_product='chrome'
+)
+
+# Create a new profile with recommended settings
+# for browser fingerprinting protection
+create_profile_request = BuilderForCreateProfile \
+    .for_base_profile(base_profiles[0].id) \
+    .set_recommended_defaults() \
+    .build()
+profile = client.create_profile(body=create_profile_request)
+
+# Start the browser
+client.start_profile(profile.id)
+
+# At this point you can automate the browser with your favorite framework
 ```
 
 # Automate Kameleo profiles with Selenium
 Kameleo gives you the ability to control any supported browser using Selenium. It uses the WebDriver protocol, a W3C specification, and industry-standard to interact with a browser.
 
 You need to install the official [Selenium package](https://pypi.org/project/selenium/).
 
 ```python
 from selenium import webdriver
 ```
 
 ```python
 # Connect to the running browser instance using WebDriver
+kameleo_port = 5050
 options = webdriver.ChromeOptions()
-options.add_experimental_option("kameleo:profileId", profile.id)
+options.add_experimental_option('kameleo:profileId', profile.id)
 driver = webdriver.Remote(
     command_executor=f'http://localhost:{kameleo_port}/webdriver',
     options=options
 )
 
 # Use any WebDriver command to drive the browser
 # and enjoy full protection from bot detection products
@@ -91,43 +102,47 @@
 
 # Automate Kameleo profiles with Puppeteer (Chromium-based)
 Kameleo lets you control Chromium-based browsers (sorry Firefox fans) using the [Pyppeteer library](https://pypi.org/project/pyppeteer/). In this simple example you can see how to connect to the browser that Kameleo starts.
 
 You need to import the [Pyppeteer library](https://pypi.org/project/pyppeteer/).
 
 ```python
-import pyppeteer   
+import pyppeteer
 ```
 
 ```python
 # Connect to the browser with Puppeteer through CDP
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/puppeteer/{profile.id}'
 browser = await pyppeteer.launcher.connect(browserWSEndpoint=browser_ws_endpoint, defaultViewport=False)
 page = await browser.newPage()
 
 # Use any Playwright command to drive the browser
 # and enjoy full protection from bot detection products
 await page.goto('https://google.com')
 ```
 
-The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_puppeteer_to_chrome/app.py).
+The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_puppeteer/app.py).
 
 # Automate Kameleo profiles with Playwright
 Kameleo allows you to control the browser with the official [Playwright package](https://pypi.org/project/playwright/). It works little bit different with Chromium-based browsers and Firefox, so we provide an example for both. Here we showcase how you can connect to the browser that is already started by Kameleo.
 
 You need to import the official [Playwright package](https://pypi.org/project/playwright/).
 ```python
 import playwright
 from playwright.sync_api import sync_playwright
 ```
 
+You can find more details here: [Using Kameleo with Playwright framework â€“ Kameleo Support Center](https://help.kameleo.io/hc/en-us/articles/4419471627793-Using-Kameleo-with-Playwright-framework).
+
 ## Chromium-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright through CDP
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
     browser = playwright.chromium.connect_over_cdp(endpoint_url=browser_ws_endpoint)
     context = browser.contexts[0]
     page = context.new_page()
 
     # Use any Playwright command to drive the browser
@@ -137,59 +152,108 @@
 
 The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_playwright_to_chrome/app.py).
 
 ## Firefox-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
+    # The exact path to the bridge executable is subject to change. Here, we use %LOCALAPPDATA%\Programs\Kameleo\pw-bridge.exe
+    executable_path_example = path.expandvars(r'%LOCALAPPDATA%\Programs\Kameleo\pw-bridge.exe')
     browser = playwright.firefox.launch_persistent_context(
         '',
         # The Playwright framework is not designed to connect to already running
         # browsers. To overcome this limitation, a tool bundled with Kameleo, named
         # pw-bridge.exe will bridge the communication gap between the running Firefox
         # instance and this playwright script.
-        executable_path='<PATH_TO_KAMELEO_FOLDER>\\pw-bridge.exe',
+        executable_path=executable_path_example,
         args=[f'-target {browser_ws_endpoint}'],
         viewport=None)
-    
+
     # Kameleo will open the a new page in the default browser context.
-    # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere 
+    # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere
     #       with Kameleo's browser fingerprint modification features.
     page = browser.new_page()
 
     # Use any Playwright command to drive the browser
     # and enjoy full protection from bot detection products
     page.goto('https://google.com')
 
     # Here we need to close the browser object as well, it is not enough just to stop the profile
     client.stop_profile(profile.id)
     browser.close()
 ```
 
 The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_playwright_to_firefox/app.py).
 
+# Automate mobile profiles
+Kameleo can emulate mobile devices in the custom built Chromium.
+
+```python
+# Search for a mobile Base Profiles
+base_profile_list = client.search_base_profiles(
+    device_type='mobile',
+    os_family='ios',
+    browser_product='safari',
+    language='en-us'
+)
+
+# Create a new profile with recommended settings
+# Choose one of the Base Profiles
+# Set the launcher to 'chromium' so the mobile profile will be started in Chromium by Kameleo
+create_profile_request = BuilderForCreateProfile \
+    .for_base_profile(base_profile_list[0].id) \
+    .set_recommended_defaults() \
+    .set_launcher('chromium') \
+    .build()
+profile = client.create_profile(body=create_profile_request)
+
+# Start the profile
+client.start_profile_with_options(profile.id, body={
+    # This allows you to click on elements using the cursor when emulating a touch screen in the browser.
+    # If you leave this out, your script may time out after clicks and fail.
+    'additionalOptions': [
+        {
+            'key': 'disableTouchEmulation',
+            'value': True,
+        },
+    ],
+})
+
+# At this point you can automate the browser with your favorite framework
+```
+The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/automate_mobile_profiles_on_desktop/app.py).
+
+
 # Example codes
 [Several examples](https://github.com/kameleo-io/local-api-examples) have been prepared in a different repository to showcase the most interesting features. Feel free to create a pull request to add new example codes.
 
 - Finding base profiles
 - Creating profiles with custom options
 - Updating profiles with new settings
 - How to start a profile
 - Using Selenium with Local API
 - Using Playwright with Kameleo
 - Using Puppeteer with Kameleo
+- How to emulate mobile devices
 - Adding an HTTP, SOCKS or SSH proxy to profile
 - Saving/Loading a browsing session to/from a .kameleo file
 - Modify and Delete browser cookies
 - Start profile with extra WebDriver capabilities
+- How to duplicate virtual browser profiles
+- Refresh the browser of the emulated profiles
 
 > Note: _If you are interested in more information about Kameleo, or have encountered an issue with using it, please check out our [Help Center](https://help.kameleo.io/)._
 
 
 # Endpoints
 Available API endpoints with exhaustive descriptions and example values are documented on this [SwaggerHub](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) page. This package has built-in [IntelliSense](https://code.visualstudio.com/docs/editor/intellisense) support in Visual Studio Code, no extra package installation needed.
 
+# Package
+This package can be found on PyPI here: [kameleo.local-api-client](https://pypi.org/project/kameleo.local-api-client/).
 
 # License
 This project is released under MIT License. Please refer the LICENSE.txt for more details.
+
+
```

### Comparing `kameleo.local_api_client-2.9.0/kameleo/local_api_client/builder_for_create_profile.py` & `kameleo.local_api_client-3.0.0/kameleo/local_api_client/builder_for_create_profile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,222 +1,246 @@
-from .models.create_profile_request_py3 import CreateProfileRequest
-from .models.webgl_spoofing_type_webgl_spoofing_options_multi_level_choice_py3 import WebglSpoofingTypeWebglSpoofingOptionsMultiLevelChoice
-from .models.timezone_spoofing_type_timezone_multi_level_choice_py3 import TimezoneSpoofingTypeTimezoneMultiLevelChoice
-from .models.geolocation_spoofing_type_geolocation_spoofing_options_multi_level_choice_py3 import GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice
-from .models.proxy_connection_type_server_multi_level_choice_py3 import ProxyConnectionTypeServerMultiLevelChoice
-from .models.web_rtc_spoofing_type_web_rtc_spoofing_options_multi_level_choice_py3 import WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice
-from .models.font_spoofing_type_font_ilist_multi_level_choice_py3 import FontSpoofingTypeFontIListMultiLevelChoice
-from .models.plugin_spoofing_type_plugin_ilist_multi_level_choice_py3 import PluginSpoofingTypePluginIListMultiLevelChoice
-from .models.screen_spoofing_type_screen_size_multi_level_choice_py3 import ScreenSpoofingTypeScreenSizeMultiLevelChoice
+from typing import Optional, Union, IO
+
+from kameleo.local_api_client._serialization import JSON
 
 
 class BuilderForCreateProfile:
     def __init__(self, base_profile_id):
         self.profile_request = self.reset(base_profile_id)
 
     @staticmethod
     def for_base_profile(base_profile_id):
         if not base_profile_id:
             raise ValueError("base_profile_id must be set")
         return BuilderForCreateProfile(base_profile_id)
 
     def build(self):
         result = self.profile_request
-        self.profile_request = self.reset(result.base_profile_id)
+        self.profile_request = self.reset(result['baseProfileId'])
         return result
 
     def set_canvas(self, value):
         """Tells the mode how the canvas will be spoofed. Possible values:
             'noise': Add some noise to the Canvas generation.
             'block': Completely block the 2D API.
             'off': Turn off the spoofing, use the original settings.
         :param string value: Canvas spoofing type. Possible values: 'noise', 'block', 'off'
         """
-        self.profile_request.canvas = value
+        self.profile_request['canvas'] = value
         return self
-    
-    def set_webgl(self, value, options):
+
+    def set_webgl(self, value):
         """Set the Webgl spoofing. Possible values:
             'noise': Add some noise to the WebGL generation
             'block': Completely block the 3D API
             'off': Turn off the spoofing, use the original settings
         :param string value: WebGL spoofing type. Possible values: 'noise', 'block', 'off'
-        :param options: Provide unmasked_vendor and unmasked_renderer
-        :type options: ~kameleo.local_api_client.models.WebglSpoofingOptions
         """
-        self.profile_request.webgl.value = value
-        self.profile_request.webgl.extra = options
+        self.profile_request['webgl'] = value
+        return self
+
+    def set_webgl_meta(self, value, options):
+        """Tells the mode how the WebGL vendor and renderer will be spoofed. Possible values:
+            'automatic': The vendor and renderer values comes from the base profile.
+            'manual': Manually set the vendor and renderer values.
+            'off': Turn off the spoofing, use the original settings.
+            :param string value: WebGLMeta spoofing type. Possible values: 'automatic', 'manual', 'off'
+            :param options: When the WebglMeta spoofing is set to manual the webgl gpu vendor and renderer is required. For example: Google Inc. (NVIDIA)/ANGLE (NVIDIA, NVIDIA GeForce GTX 1050 Ti Direct3D11 vs_5_0 ps_5_0, D3D11)
+            :type options: ~kameleo.local_api_client.models.WebglMetaSpoofingOptions
+        """
+        self.profile_request['webglMeta']['value'] = value
+        self.profile_request['webglMeta']['extra'] = options
         return self
 
     def set_audio(self, value):
         """Tells the mode how the audio will be spoofed. Possible values:
             'noise': Add some noise to the Audio generation.
             'block': Completely block the Audio API.
             'off': Turn off the audio spoofing, use the original settings.
         :param string value: Audio spoofing type. Possible values: 'noise', 'block', 'off'
         """
-        self.profile_request.audio = value
+        self.profile_request['audio'] = value
         return self
 
     def set_timezone(self, value, options):
         """Tells the mode how the Timezone will be spoofed. Possble values:
             'automatic': Timezone is automatically set by the IP
             'manual': Timezone is manually overridden in the profile
             'off': Turn off the spoofing, use the original settings
         :param string value: Timezone spoofing type. Possible values: 'automatic', 'manual', 'off'
         :param str options: When the Timezone spoofing is set to manual the timezone in Iana format is required. For example: America/Grenada
         """
-        self.profile_request.timezone.value = value
-        self.profile_request.timezone.extra = options
+        self.profile_request['timezone']['value'] = value
+        self.profile_request['timezone']['extra'] = options
         return self
 
     def set_geolocation(self, value, options):
         """Tells the mode how the Geolocation will be spoofed. Possible values:
             'automatic': Automatically set the values based on the IP address
             'manual': Manually set the longitude and latitude in the profile
             'block': Completely block the GeolocationAPI
             'off': Turn off the spoofing, use the original settings
         :param string value: Geolocation spoofing type. Possible values: 'automatic', 'manual', 'block', 'off'
         :param options: When the Geolocation spoofing is set to manual the Geolocation coordinates must be provided
         :type options: ~kameleo.local_api_client.models.GeolocationSpoofingOptions
         """
-        self.profile_request.geolocation.value = value
-        self.profile_request.geolocation.extra = options
+        self.profile_request['geolocation']['value'] = value
+        self.profile_request['geolocation']['extra'] = options
         return self
 
     def set_proxy(self, value, options):
         """Proxy connection settings of the profiles. Possible values:
             'none': Direct connection without any proxy.</para>
             'http': Use a HTTP(S) proxy for upstream communication.</para>
             'socks5': Use a SOCKS5 proxy for upstream communication.</para>
             'ssh': Use an SSH connection for upstream communication. Basically a SOCKS5 proxy created at the given SSH host.</para>
         :param string value: Proxy connection type. Possible values: 'none', 'http', 'socks5', 'ssh'
         :param options: When the Proxy connection is set, a Proxy Server must be provided
         :type options: ~kameleo.local_api_client.models.Server
         """
-        self.profile_request.proxy.value = value
-        self.profile_request.proxy.extra = options
+        self.profile_request['proxy']['value'] = value
+        self.profile_request['proxy']['extra'] = options
         return self
 
     def set_web_rtc(self, value, options):
         """Tells the mode how the WebRTC will be spoofed. Possible values:
             'automatic': Automatically set the webRTC public IP by the IP, and generates a random private IP like '2d2f78e7-1b1e-4345-a21b-07c904c98394.local'
             'manual': Manually override the webRTC public IP and private IP in the profile
             'block': Block the WebRTC functionality
             'off': Turn off the spoofing, use the original settings
         :param string value: WebRTC spoofing type. Possible values: 'automatic', 'manual', 'block', 'off'
         :param options: When the WebRTC spoofing is set to manual, the private_ip and public_ip must be provided
         :type options: ~kameleo.local_api_client.models.WebRtcSpoofingOptions
         """
-        self.profile_request.web_rtc.value = value
-        self.profile_request.web_rtc.extra = options
+        self.profile_request['webRtc']['value'] = value
+        self.profile_request['webRtc']['extra'] = options
         return self
 
     def set_fonts(self, value, options):
         """Tells the mode how the Fonts will be spoofed. Possible values:
             'enabled': Enable fonts spoofing. A list can be provided to override the fonts coming from the base profile.
             'disable': Disable fonts spoofing.
         :param string value: Fonts spoofing type. Possible values: 'enabled', 'disabled'
         :param options: When the Font spoofing is set to enabled, a list can be provided to overrider the fonts coming from the base profile.
         :type options: list[str]
         """
-        self.profile_request.fonts.value = value
-        self.profile_request.fonts.extra = options
-        return self
-
-    def set_plugins(self, value, options):
-        """Tells the mode how the Plugins will be spoofed. Possible values:
-            'enabled': Enable plugins spoofing. A list can be provided to EXCLUDE plugins from the plugins of the base profile.
-            'disable': Disable plugins spoofing.
-        :param string value: Plugins spoofing type. Possible values: 'enabled', 'disabled'
-        :param options: When the Plugins spoofing is set to enabled, a list can be provided to EXCLUDE plugins from the plugins of the base profile.
-        :type options: list[str]
-        """
-        self.profile_request.plugins.value = value
-        self.profile_request.plugins.extra = options
+        self.profile_request['fonts']['value'] = value
+        self.profile_request['fonts']['extra'] = options
         return self
 
     def set_start_page(self, value):
         """This website will be opened in the browser when the profile launches.
         :param string value: The url of the start page
         """
-        self.profile_request.start_page = value
+        self.profile_request['startPage'] = value
         return self
 
     def set_password_manager(self, value):
         """Enable or disable the password manager function in the browser. Possible values:
             'enabled': Enable password manager so browser will ask to save and load passwords on logins.
             'disable': Disable password manager.
         :param string value: Password Manager possible values: 'enabled', 'disabled'
         """
-        self.profile_request.password_manager = value
+        self.profile_request['passwordManager'] = value
         return self
 
     def set_screen(self, value, options):
         """Tells the mode how the screen will be spoofed. Possible values:
             'automatic': Automatically override the screen resolution based on the Base Profile.
             'manual': Manually override the screen resolution.
             'off': Turn off the spoofing, use the original settings.
         :param string value: Screen spoofing type. Possible values: 'automatic', 'manual', 'off'
         :param string options: When the Screen spoofing is set to manual, the required screen size must be provided. For example: 1080x1920
         """
-        self.profile_request.screen.value = value
-        self.profile_request.screen.extra = options
+        self.profile_request['screen']['value'] = value
+        self.profile_request['screen']['extra'] = options
         return self
 
     def set_extensions(self, absolute_paths):
         """A list of absolute paths from where the profile should load extensions or addons when starting the browser. For chrome and edge use CRX3 format extensions. For firefox use signed xpi format addons.
         :param absolute_paths: A list of abolute paths from where the profile should load extensions or addons when starting the browser.
         :type absolute_paths: list[str]
         """
-        self.profile_request.extensions = absolute_paths
+        self.profile_request['extensions'] = absolute_paths
         return self
-    
+
     def set_notes(self, notes):
         """A free text including any notes written by the user.
         """
-        self.profile_request.notes = notes
+        self.profile_request['notes'] = notes
+        return self
+
+    def set_name(self, name):
+        """Sets the name of the profile.
+        """
+        self.profile_request['name'] = name
+        return self
+
+    def set_tags(self, tags):
+        """Sets the tags of the profile.
+        """
+        self.profile_request['tags'] = tags
         return self
 
     def set_launcher(self, browser_launcher):
-        """The mode how the profile should be launched. It determines which browser to launch. This cannot be modified after creation. Possible values are:
-            'automatic': Automatically choose launcher based on DeviceType and BrowserProduct property.
-            'chrome': Forcefully start the profile in Chrome.
-            'chromium': Forcefully start the profile in Chromium.
-            'firefox': Forcefully start the profile in Firefox.
-            'edge': Forcefully start the profile in Edge.
-            'external': Only start the external spoofing engine and connect any browser manually. This is also used for Mobile Device spoofing.
-        :param string browser_launcher: Browser Launcher. Possible values: 'automatic', 'chrome', 'chromium', 'firefox', 'edge', 'external'
+        """The mode how the profile should be launched. It determines which browser to launch. This cannot be modified after creation.
+            Possible values for Desktop profiles 'automatic'.
+            Possible values for Mobile profiles: 'chromium', 'external'.
+        :param string browser_launcher: Browser Launcher. Possible values: 'automatic', 'external'
         """
-        self.profile_request.launcher = browser_launcher
+        self.profile_request['launcher'] = browser_launcher
         return self
 
     def set_recommended_defaults(self):
         """This sets all the profile options to the defaults recommended by Kameleo Team. Please consider providing Proxy settings to your profile.
         """
-        self.profile_request.canvas = "intelligent"
-        self.profile_request.webgl.value = "off"
-        self.profile_request.audio = "off"
-        self.profile_request.timezone.value = "automatic"
-        self.profile_request.geolocation.value = "automatic"
-        self.profile_request.web_rtc.value = "automatic"
-        self.profile_request.fonts.value = "enabled"
-        self.profile_request.plugins.value = "enabled"
-        self.profile_request.screen.value = "automatic"
-        self.profile_request.launcher = "automatic"
-
-        return self;
-    
-    def reset(self, base_profile_id):
-        return CreateProfileRequest(
-            base_profile_id=base_profile_id,
-            canvas="off",
-            webgl=WebglSpoofingTypeWebglSpoofingOptionsMultiLevelChoice(value="off", extra=None),
-            audio="off",
-            timezone=TimezoneSpoofingTypeTimezoneMultiLevelChoice(value="off", extra=None),
-            geolocation=GeolocationSpoofingTypeGeolocationSpoofingOptionsMultiLevelChoice(value="off", extra=None),
-            proxy=ProxyConnectionTypeServerMultiLevelChoice(value="none", extra=None),
-            web_rtc=WebRtcSpoofingTypeWebRtcSpoofingOptionsMultiLevelChoice(value="off", extra=None),
-            fonts=FontSpoofingTypeFontIListMultiLevelChoice(value="disabled", extra=None),
-            plugins=PluginSpoofingTypePluginIListMultiLevelChoice(value="disabled", extra=None),
-            screen=ScreenSpoofingTypeScreenSizeMultiLevelChoice(value="off", extra=None),
-            password_manager="disabled")
+        self.profile_request['name'] = ""
+        self.profile_request['canvas'] = "intelligent"
+        self.profile_request['webgl'] = "off"
+        self.profile_request['webglMeta']['value'] = "automatic"
+        self.profile_request['audio'] = "off"
+        self.profile_request['timezone']['value'] = "automatic"
+        self.profile_request['geolocation']['value'] = "automatic"
+        self.profile_request['webRtc']['value'] = "automatic"
+        self.profile_request['fonts']['value'] = "enabled"
+        self.profile_request['screen']['value'] = "automatic"
+        self.profile_request['launcher'] = "automatic"
+
+        return self
+
+    def reset(self, base_profile_id) -> Optional[Union[JSON, IO]]:
+        data = {
+            "baseProfileId": base_profile_id,
+            "canvas": "off",
+            "webgl": "off",
+            "webglMeta": {
+                "value": "off",
+                "extra": None
+            },
+            "audio": "off",
+            "timezone": {
+                "value": "off",
+                "extra": None
+            },
+            "geolocation": {
+                "value": "off",
+                "extra": None
+            },
+            "proxy": {
+                "value": "none",
+                "extra": None
+            },
+            "webRtc": {
+                "value": "off",
+                "extra": None
+            },
+            "fonts": {
+                "value": "disabled",
+                "extra": None
+            },
+            "screen": {
+                "value": "off",
+                "extra": None
+            },
+            "passwordManager": "disabled"
+        }
+        return data
```

### Comparing `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/load_profile_request.py` & `kameleo.local_api_client-3.0.0/kameleo/local_api_client/_vendor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,36 @@
-# coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator.
-# Changes may cause incorrect behavior and will be lost if the code is
-# regenerated.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.5.1)
+# Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from msrest.serialization import Model
+from abc import ABC
+from typing import List, TYPE_CHECKING, cast
 
+from ._configuration import KameleoLocalApiClientConfiguration
 
-class LoadProfileRequest(Model):
-    """Tells where the profile should be loaded from.
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from azure.core import PipelineClient
 
-    All required parameters must be populated in order to send to Azure.
+    from ._serialization import Deserializer, Serializer
 
-    :param path: Required. The path where the profile should be loaded from
-    :type path: str
-    """
 
-    _validation = {
-        'path': {'required': True},
-    }
+def _format_url_section(template, **kwargs):
+    components = template.split("/")
+    while components:
+        try:
+            return template.format(**kwargs)
+        except KeyError as key:
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
+            components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
+            template = "/".join(components)
 
-    _attribute_map = {
-        'path': {'key': 'path', 'type': 'str'},
-    }
 
-    def __init__(self, **kwargs):
-        super(LoadProfileRequest, self).__init__(**kwargs)
-        self.path = kwargs.get('path', None)
+class KameleoLocalApiClientMixinABC(ABC):
+    """DO NOT use this class. It is for internal typing use only."""
+
+    _client: "PipelineClient"
+    _config: KameleoLocalApiClientConfiguration
+    _serialize: "Serializer"
+    _deserialize: "Deserializer"
```

### Comparing `kameleo.local_api_client-2.9.0/kameleo/local_api_client/models/screen_spoofing_type_screen_size_multi_level_choice.py` & `kameleo.local_api_client-3.0.0/kameleo/local_api_client/aio/_vendor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,24 @@
-# coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator.
-# Changes may cause incorrect behavior and will be lost if the code is
-# regenerated.
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.6, generator: @autorest/python@6.5.1)
+# Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from msrest.serialization import Model
+from abc import ABC
+from typing import TYPE_CHECKING
 
+from ._configuration import KameleoLocalApiClientConfiguration
 
-class ScreenSpoofingTypeScreenSizeMultiLevelChoice(Model):
-    """ScreenSpoofingTypeScreenSizeMultiLevelChoice.
+if TYPE_CHECKING:
+    # pylint: disable=unused-import,ungrouped-imports
+    from azure.core import AsyncPipelineClient
 
-    All required parameters must be populated in order to send to Azure.
+    from .._serialization import Deserializer, Serializer
 
-    :param value: Required. Possible values include: 'automatic', 'manual',
-     'off'
-    :type value: str or ~kameleo.local_api_client.models.enum
-    :param extra: The screen size of the device in pixels. For example:
-     1920x1080
-    :type extra: str
-    """
-
-    _validation = {
-        'value': {'required': True},
-    }
-
-    _attribute_map = {
-        'value': {'key': 'value', 'type': 'str'},
-        'extra': {'key': 'extra', 'type': 'str'},
-    }
-
-    def __init__(self, **kwargs):
-        super(ScreenSpoofingTypeScreenSizeMultiLevelChoice, self).__init__(**kwargs)
-        self.value = kwargs.get('value', None)
-        self.extra = kwargs.get('extra', None)
+
+class KameleoLocalApiClientMixinABC(ABC):
+    """DO NOT use this class. It is for internal typing use only."""
+
+    _client: "AsyncPipelineClient"
+    _config: KameleoLocalApiClientConfiguration
+    _serialize: "Serializer"
+    _deserialize: "Deserializer"
```

### Comparing `kameleo.local_api_client-2.9.0/kameleo.local_api_client.egg-info/PKG-INFO` & `kameleo.local_api_client-3.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kameleo.local-api-client
-Version: 2.9.0
+Name: kameleo.local_api_client
+Version: 3.0.0
 Summary: This Python package provides convenient access to the Local API REST interface of the Kameleo Client.
 Home-page: https://github.com/kameleo-io/local-api-client-python
 Author: Kameleo Team
 Author-email: support@kameleo.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -45,57 +45,53 @@
 ```
 
 ## 2. Start the Kameleo.CLI on your computer
 ```
 ./Kameleo.CLI.exe email="your@email.com" password="Pa$$w0rd"
 ```
 
-## 3. Start a browser with out-of-the-box fingerprinting protection 
+## 3. Start a browser with out-of-the-box fingerprinting protection
 ```python
-from kameleo.local_api_client.kameleo_local_api_client import KameleoLocalApiClient
+from kameleo.local_api_client import KameleoLocalApiClient
 from kameleo.local_api_client.builder_for_create_profile import BuilderForCreateProfile
-from kameleo.local_api_client.models.problem_response_py3 import ProblemResponseException
-import json
 
-try:
-    client = KameleoLocalApiClient()
-    base_profiles = client.search_base_profiles(
-        device_type='desktop',
-        browser_product='chrome'
-    )
-    
-    # Create a new profile with recommended settings
-    # for browser fingerprinting protection
-    create_profile_request = BuilderForCreateProfile \
-        .for_base_profile(base_profiles[0].id) \
-        .set_recommended_defaults() \
-        .build()
-    profile = client.create_profile(body=create_profile_request)
-    
-    # Start the browser
-    client.start_profile(profile.id)
-    
-    # At this point you can automate the browser with your favorite framework
-except ProblemResponseException as e:
-    raise Exception([str(e), json.dumps(e.error.error)])
+client = KameleoLocalApiClient()
+base_profiles = client.search_base_profiles(
+    device_type='desktop',
+    browser_product='chrome'
+)
+
+# Create a new profile with recommended settings
+# for browser fingerprinting protection
+create_profile_request = BuilderForCreateProfile \
+    .for_base_profile(base_profiles[0].id) \
+    .set_recommended_defaults() \
+    .build()
+profile = client.create_profile(body=create_profile_request)
+
+# Start the browser
+client.start_profile(profile.id)
+
+# At this point you can automate the browser with your favorite framework
 ```
 
 # Automate Kameleo profiles with Selenium
 Kameleo gives you the ability to control any supported browser using Selenium. It uses the WebDriver protocol, a W3C specification, and industry-standard to interact with a browser.
 
 You need to install the official [Selenium package](https://pypi.org/project/selenium/).
 
 ```python
 from selenium import webdriver
 ```
 
 ```python
 # Connect to the running browser instance using WebDriver
+kameleo_port = 5050
 options = webdriver.ChromeOptions()
-options.add_experimental_option("kameleo:profileId", profile.id)
+options.add_experimental_option('kameleo:profileId', profile.id)
 driver = webdriver.Remote(
     command_executor=f'http://localhost:{kameleo_port}/webdriver',
     options=options
 )
 
 # Use any WebDriver command to drive the browser
 # and enjoy full protection from bot detection products
@@ -106,43 +102,47 @@
 
 # Automate Kameleo profiles with Puppeteer (Chromium-based)
 Kameleo lets you control Chromium-based browsers (sorry Firefox fans) using the [Pyppeteer library](https://pypi.org/project/pyppeteer/). In this simple example you can see how to connect to the browser that Kameleo starts.
 
 You need to import the [Pyppeteer library](https://pypi.org/project/pyppeteer/).
 
 ```python
-import pyppeteer   
+import pyppeteer
 ```
 
 ```python
 # Connect to the browser with Puppeteer through CDP
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/puppeteer/{profile.id}'
 browser = await pyppeteer.launcher.connect(browserWSEndpoint=browser_ws_endpoint, defaultViewport=False)
 page = await browser.newPage()
 
 # Use any Playwright command to drive the browser
 # and enjoy full protection from bot detection products
 await page.goto('https://google.com')
 ```
 
-The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_puppeteer_to_chrome/app.py).
+The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_puppeteer/app.py).
 
 # Automate Kameleo profiles with Playwright
 Kameleo allows you to control the browser with the official [Playwright package](https://pypi.org/project/playwright/). It works little bit different with Chromium-based browsers and Firefox, so we provide an example for both. Here we showcase how you can connect to the browser that is already started by Kameleo.
 
 You need to import the official [Playwright package](https://pypi.org/project/playwright/).
 ```python
 import playwright
 from playwright.sync_api import sync_playwright
 ```
 
+You can find more details here: [Using Kameleo with Playwright framework â€“ Kameleo Support Center](https://help.kameleo.io/hc/en-us/articles/4419471627793-Using-Kameleo-with-Playwright-framework).
+
 ## Chromium-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright through CDP
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
     browser = playwright.chromium.connect_over_cdp(endpoint_url=browser_ws_endpoint)
     context = browser.contexts[0]
     page = context.new_page()
 
     # Use any Playwright command to drive the browser
@@ -152,61 +152,108 @@
 
 The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_playwright_to_chrome/app.py).
 
 ## Firefox-based profiles with Playwright
 
 ```python
 # Connect to the browser with Playwright
+kameleo_port = 5050
 browser_ws_endpoint = f'ws://localhost:{kameleo_port}/playwright/{profile.id}'
 with sync_playwright() as playwright:
+    # The exact path to the bridge executable is subject to change. Here, we use %LOCALAPPDATA%\Programs\Kameleo\pw-bridge.exe
+    executable_path_example = path.expandvars(r'%LOCALAPPDATA%\Programs\Kameleo\pw-bridge.exe')
     browser = playwright.firefox.launch_persistent_context(
         '',
         # The Playwright framework is not designed to connect to already running
         # browsers. To overcome this limitation, a tool bundled with Kameleo, named
         # pw-bridge.exe will bridge the communication gap between the running Firefox
         # instance and this playwright script.
-        executable_path='<PATH_TO_KAMELEO_FOLDER>\\pw-bridge.exe',
+        executable_path=executable_path_example,
         args=[f'-target {browser_ws_endpoint}'],
         viewport=None)
-    
+
     # Kameleo will open the a new page in the default browser context.
-    # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere 
+    # NOTE: We DO NOT recommend using multiple browser contexts, as this might interfere
     #       with Kameleo's browser fingerprint modification features.
     page = browser.new_page()
 
     # Use any Playwright command to drive the browser
     # and enjoy full protection from bot detection products
     page.goto('https://google.com')
 
     # Here we need to close the browser object as well, it is not enough just to stop the profile
     client.stop_profile(profile.id)
     browser.close()
 ```
 
 The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/connect_with_playwright_to_firefox/app.py).
 
+# Automate mobile profiles
+Kameleo can emulate mobile devices in the custom built Chromium.
+
+```python
+# Search for a mobile Base Profiles
+base_profile_list = client.search_base_profiles(
+    device_type='mobile',
+    os_family='ios',
+    browser_product='safari',
+    language='en-us'
+)
+
+# Create a new profile with recommended settings
+# Choose one of the Base Profiles
+# Set the launcher to 'chromium' so the mobile profile will be started in Chromium by Kameleo
+create_profile_request = BuilderForCreateProfile \
+    .for_base_profile(base_profile_list[0].id) \
+    .set_recommended_defaults() \
+    .set_launcher('chromium') \
+    .build()
+profile = client.create_profile(body=create_profile_request)
+
+# Start the profile
+client.start_profile_with_options(profile.id, body={
+    # This allows you to click on elements using the cursor when emulating a touch screen in the browser.
+    # If you leave this out, your script may time out after clicks and fail.
+    'additionalOptions': [
+        {
+            'key': 'disableTouchEmulation',
+            'value': True,
+        },
+    ],
+})
+
+# At this point you can automate the browser with your favorite framework
+```
+The full example can be found [here](https://github.com/kameleo-io/local-api-examples/blob/master/python/automate_mobile_profiles_on_desktop/app.py).
+
+
 # Example codes
 [Several examples](https://github.com/kameleo-io/local-api-examples) have been prepared in a different repository to showcase the most interesting features. Feel free to create a pull request to add new example codes.
 
 - Finding base profiles
 - Creating profiles with custom options
 - Updating profiles with new settings
 - How to start a profile
 - Using Selenium with Local API
 - Using Playwright with Kameleo
 - Using Puppeteer with Kameleo
+- How to emulate mobile devices
 - Adding an HTTP, SOCKS or SSH proxy to profile
 - Saving/Loading a browsing session to/from a .kameleo file
 - Modify and Delete browser cookies
 - Start profile with extra WebDriver capabilities
+- How to duplicate virtual browser profiles
+- Refresh the browser of the emulated profiles
 
 > Note: _If you are interested in more information about Kameleo, or have encountered an issue with using it, please check out our [Help Center](https://help.kameleo.io/)._
 
 
 # Endpoints
 Available API endpoints with exhaustive descriptions and example values are documented on this [SwaggerHub](https://app.swaggerhub.com/apis/kameleo-team/kameleo-local-api/) page. This package has built-in [IntelliSense](https://code.visualstudio.com/docs/editor/intellisense) support in Visual Studio Code, no extra package installation needed.
 
+# Package
+This package can be found on PyPI here: [kameleo.local-api-client](https://pypi.org/project/kameleo.local-api-client/).
 
 # License
 This project is released under MIT License. Please refer the LICENSE.txt for more details.
```

### Comparing `kameleo.local_api_client-2.9.0/setup.py` & `kameleo.local_api_client-3.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import setuptools
 from distutils.util import convert_path
 
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-# Version parsing
-main_ns = {}
-ver_path = convert_path('kameleo/local_api_client/version.py')
-with open(ver_path) as ver_file:
-    exec(ver_file.read(), main_ns)
-
+VERSION = '1.0.0'
+exec(open(convert_path('kameleo/local_api_client/_version.py')).read())
 
 setuptools.setup(
     name='kameleo.local_api_client',
-    version=main_ns['VERSION'],
+    version=VERSION,
     author='Kameleo Team',
     author_email='support@kameleo.io',
     description='This Python package provides convenient access to the Local API REST interface of the Kameleo Client.',
-    long_description=long_description,
+    long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/kameleo-io/local-api-client-python',
     packages=setuptools.find_packages(),
+    setup_requires=['wheel'],
     install_requires=['msrest'],
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

