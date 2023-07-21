# Comparing `tmp/ChatGPT-Cloud-0.6.5.tar.gz` & `tmp/ChatGPT-Cloud-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-92v8p43l/ChatGPT-Cloud-0.6.5.tar", last modified: Thu Jul 20 15:46:32 2023, max compression
+gzip compressed data, was "/home/runner/work/pandora-cloud/pandora-cloud/dist/.tmp-_klmg273/ChatGPT-Cloud-0.6.6.tar", last modified: Fri Jul 21 05:43:42 2023, max compression
```

## Comparing `ChatGPT-Cloud-0.6.5.tar` & `ChatGPT-Cloud-0.6.6.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/
--rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
--rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    74170 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js
--rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js
--rw-r--r--   0 runner    (1001) docker     (123)   417223 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js
--rw-r--r--   0 runner    (1001) docker     (123)   248252 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js
--rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js
--rw-r--r--   0 runner    (1001) docker     (123)  1085662 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js
--rw-r--r--   0 runner    (1001) docker     (123)    26962 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js
--rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
--rw-r--r--   0 runner    (1001) docker     (123)   121704 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-164e4ecc13479ecd.js
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-c7a1640505b9cfd2.js
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js
--rw-r--r--   0 runner    (1001) docker     (123)   987027 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-979cf95f72688cf4.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-fdab57c4b88e5b1c.js
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
--rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-9047ec54adb32ef3.js
--rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   138266 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/ssgManifest.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/
--rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/
--rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/sweetalert2/
--rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    68840 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/ulp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/ulp/react-components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
--rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:32.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/chat.html
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/share.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19534 2023-07-20 15:46:21.000000 ChatGPT-Cloud-0.6.5/src/pandora_cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    69737 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js
+-rw-r--r--   0 runner    (1001) docker     (123)   262802 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74170 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29389 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js
+-rw-r--r--   0 runner    (1001) docker     (123)   417223 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   248252 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1085662 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26962 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141071 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)   121704 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/cancel-164e4ecc13479ecd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/manage-c7a1640505b9cfd2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-21 05:43:29.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js
+-rw-r--r--   0 runner    (1001) docker     (123)   987027 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/bypass-979cf95f72688cf4.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/error-fdab57c4b88e5b1c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/status-9047ec54adb32ef3.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   138266 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/ssgManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28532 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35268 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28060 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37480 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    11316 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    25324 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16780 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    26272 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/
+-rw-r--r--   0 runner    (1001) docker     (123)    56682 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56021 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    56456 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    53009 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/
+-rw-r--r--   0 runner    (1001) docker     (123)    34084 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    33350 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40456 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38746 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    35690 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28148 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    27437 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28285 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/sweetalert2/
+-rw-r--r--   0 runner    (1001) docker     (123)    19844 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    68840 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/ulp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/ulp/react-components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   233073 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:42.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)    17935 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/share.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-21 05:43:30.000000 ChatGPT-Cloud-0.6.6/src/pandora_cloud/server.py
```

### Comparing `ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/PKG-INFO` & `ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPT-Cloud
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/lannychan/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/lannychan/pandora-cloud
 Project-URL: Tracker, https://github.com/lannychan/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `ChatGPT-Cloud-0.6.5/ChatGPT_Cloud.egg-info/SOURCES.txt` & `ChatGPT-Cloud-0.6.6/ChatGPT_Cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/LICENSE` & `ChatGPT-Cloud-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/PKG-INFO` & `ChatGPT-Cloud-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatGPT-Cloud
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package for Pandora-ChatGPT
 Home-page: https://github.com/lannychan/pandora-cloud
 Author: Neo Peng
 Author-email: pengzhile@gmail.com
 Project-URL: Source, https://github.com/lannychan/pandora-cloud
 Project-URL: Tracker, https://github.com/lannychan/pandora-cloud/issues
 Keywords: OpenAI ChatGPT ChatGPT-Plus
```

### Comparing `ChatGPT-Cloud-0.6.5/README.md` & `ChatGPT-Cloud-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/setup.py` & `ChatGPT-Cloud-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/012ff928-bcfa62e3ac82441c.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/1f110208-cda4026aba1898fb.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/238-882950710bdd3e1e.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/271.f8fe486a0f5b221c.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/2802bd5f-15923fb46be55b45.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/297-e180277ece10e844.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/412-c00b85b4ef66af2f.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/435-2b015d294e66ccbc.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/564-f0043ba04d4fcd3d.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/68a27ff6-b1db347c50639918.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/800-a82eb647282afb06.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/937-36e251f389e9e752.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/984-1278472924e49180.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/bd26816a-7ae54dd3357d90b4.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/framework-e23f030857e925d4.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/main-0438431c68fbeb27.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/account/upgrade-1457e593ce508c31.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/admin-810915a9e0227b64.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/aip/pluginId/oauth/callback-b7d4a081f7ad5b5b.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/app-573ad0910def0e5d.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/error-9faed2db943661ab.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback-7b50f284300a7ff6.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/ext_callback_refresh-47f3cd5abd2d99b6.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/login-267fffdf86e9e08a.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/logout-5817b04f45f270e2.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/auth/mocked_login-060c0092bc682b49.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/c/chatId-5d264bebf7157821.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/index-b00721778b6b9fff.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/payments/success-c423ec16521d5906.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/pages/share/shareParams-1c5c5056584e8afb.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/chunks/webpack-305aad91bdd6a592.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/css/59d85ffe80f6c774.css`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/_next/static/m__df_2bcLUqGXlko-rBN/buildManifest.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/apple-touch-icon.png` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/favicon-16x16.png` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/favicon-32x32.png` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/colfax/ColfaxAIRegularItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/katex/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-bold.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-light-italic.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/signifier/signifier-light.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-buch.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-kraftig.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch-kursiv.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-buch.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/fonts/soehne/soehne-mono-halbfett.woff2`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/service-worker.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/service-worker.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/sweetalert2/bulma.min.css`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/sweetalert2/sweetalert2.all.min-bc15590d.js`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/static/ulp/react-components/1.66.5/css/main.cdn.min.css`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/404.html` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/404.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/chat.html` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/chat.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/detail.html` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/detail.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/login.html` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/login.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/flask/templates/share.html` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/flask/templates/share.html`

 * *Files identical despite different names*

### Comparing `ChatGPT-Cloud-0.6.5/src/pandora_cloud/server.py` & `ChatGPT-Cloud-0.6.6/src/pandora_cloud/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,14 +501,15 @@
                         'layout_may_2023',
                         'plugins_available',
                         'beta_features',
                         'infinite_scroll_history',
                         'browsing_inner_monologue',
                         'new_plugin_oauth_endpoint',
                         'code_interpreter_available',
+                        'chat_preferences_available',
                         'plugin_review_tools',
                         'message_debug_info',
                         'shareable_links',
                         'tools3_dev',
                         'tools2',
                         'debug',
                     ],
```

