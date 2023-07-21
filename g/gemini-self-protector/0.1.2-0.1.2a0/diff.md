# Comparing `tmp/gemini_self_protector-0.1.2.tar.gz` & `tmp/gemini_self_protector-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_self_protector-0.1.2.tar", max compression
+gzip compressed data, was "gemini_self_protector-0.1.2a0.tar", max compression
```

## Comparing `gemini_self_protector-0.1.2.tar` & `gemini_self_protector-0.1.2a0.tar`

### file list

```diff
@@ -1,133 +1,137 @@
--rwxr-xr-x   0        0        0     1069 2023-04-17 13:13:50.672809 gemini_self_protector-0.1.2/LICENSE
--rw-r--r--   0        0        0     6700 2023-06-26 14:16:25.914242 gemini_self_protector-0.1.2/README.md
--rw-r--r--   0        0        0      489 2023-07-12 15:08:56.794162 gemini_self_protector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      558 2023-06-19 16:47:36.851640 gemini_self_protector-0.1.2/src/gemini_self_protector/__init__.py
--rw-r--r--   0        0        0     1824 2023-06-19 16:47:28.845395 gemini_self_protector-0.1.2/src/gemini_self_protector/_audit.py
--rw-r--r--   0        0        0     4000 2023-06-19 16:47:22.196160 gemini_self_protector-0.1.2/src/gemini_self_protector/_cli.py
--rw-r--r--   0        0        0    13840 2023-07-04 17:18:00.743973 gemini_self_protector-0.1.2/src/gemini_self_protector/_config.py
--rw-r--r--   0        0        0    20786 2023-07-12 14:31:35.889747 gemini_self_protector-0.1.2/src/gemini_self_protector/_gemini.py
--rw-r--r--   0        0        0    35678 2023-07-12 14:30:47.625077 gemini_self_protector-0.1.2/src/gemini_self_protector/_gui.py
--rw-r--r--   0        0        0     2737 2023-06-14 15:41:22.128264 gemini_self_protector-0.1.2/src/gemini_self_protector/_logger.py
--rw-r--r--   0        0        0     3508 2023-07-12 14:32:01.923270 gemini_self_protector-0.1.2/src/gemini_self_protector/_model.py
--rw-r--r--   0        0        0    14724 2023-07-03 17:28:57.174109 gemini_self_protector-0.1.2/src/gemini_self_protector/_protect.py
--rw-r--r--   0        0        0     1667 2023-06-19 16:46:34.460479 gemini_self_protector-0.1.2/src/gemini_self_protector/_template.py
--rw-r--r--   0        0        0    16392 2023-07-12 14:57:22.958818 gemini_self_protector-0.1.2/src/gemini_self_protector/_utils.py
--rw-r--r--   0        0        0     6391 2023-07-03 17:31:00.908120 gemini_self_protector-0.1.2/src/gemini_self_protector/gemini_self_protector.py
--rw-r--r--   0        0        0     3356 2023-06-20 14:32:27.097647 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/dark.css
--rw-r--r--   0        0        0     5484 2023-06-19 17:02:55.146292 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/install.css
--rw-r--r--   0        0        0   311910 2023-07-04 17:15:39.423308 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/style.css
--rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.149256 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css
--rw-r--r--   0        0        0     2548 2023-06-19 17:02:55.149663 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot
--rw-r--r--   0        0        0     2530 2023-06-19 17:02:55.150002 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg
--rw-r--r--   0        0        0     2400 2023-06-19 17:02:55.150303 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf
--rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.150704 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff
--rw-r--r--   0        0        0    11805 2023-06-19 17:02:55.151201 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css
--rw-r--r--   0        0        0    55828 2023-06-19 17:02:55.152093 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot
--rw-r--r--   0        0        0   191595 2023-06-19 17:02:55.154892 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg
--rw-r--r--   0        0        0    55664 2023-06-19 17:02:55.156107 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf
--rw-r--r--   0        0        0    26432 2023-06-19 17:02:55.156890 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff
--rw-r--r--   0        0        0    41065 2023-06-19 17:02:55.160256 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css
--rw-r--r--   0        0        0   111620 2023-06-19 17:02:55.162260 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   599834 2023-06-19 17:02:55.169295 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   111384 2023-06-19 17:02:55.171076 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    71560 2023-06-19 17:02:55.174761 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    61336 2023-06-19 17:02:55.175547 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    31272 2023-06-19 17:02:55.176292 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   104706 2023-06-19 17:02:55.177586 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    31044 2023-06-19 17:02:55.178645 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    14724 2023-06-19 17:02:55.179411 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    12188 2023-06-19 17:02:55.179988 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   133140 2023-06-19 17:02:55.181538 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   488395 2023-06-19 17:02:55.190179 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   132920 2023-06-19 17:02:55.194157 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    63836 2023-06-19 17:02:55.195167 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    50372 2023-06-19 17:02:55.204039 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     3822 2023-06-19 17:02:55.204861 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/chrome.png
--rw-r--r--   0        0        0     4809 2023-06-19 17:02:55.205402 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/firefox.png
--rw-r--r--   0        0        0     4359 2023-06-19 17:02:55.205942 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/ie.png
--rw-r--r--   0        0        0     3379 2023-06-19 17:02:55.206498 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/opera.png
--rw-r--r--   0        0        0     4915 2023-06-19 17:02:55.207015 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/safari.png
--rw-r--r--   0        0        0    15406 2023-06-21 08:29:54.000000 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/favicon.ico
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/gemini-7.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-dark.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-thumb.png
--rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo.png
--rw-r--r--   0        0        0    31417 2023-06-19 17:02:55.211234 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg
--rw-r--r--   0        0        0    66369 2023-06-19 17:02:55.212675 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg
--rw-r--r--   0        0        0    22071 2023-06-19 17:02:55.213564 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg
--rw-r--r--   0        0        0    21820 2023-06-19 17:02:55.214458 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg
--rw-r--r--   0        0        0    33652 2023-06-19 17:02:55.215162 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg
--rw-r--r--   0        0        0   246009 2023-06-19 17:02:55.221542 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img1.jpg
--rw-r--r--   0        0        0   165567 2023-06-19 17:02:55.223424 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img2.jpg
--rw-r--r--   0        0        0   168914 2023-06-19 17:02:55.225478 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img3.jpg
--rw-r--r--   0        0        0     9287 2023-06-19 17:02:55.226420 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg
--rw-r--r--   0        0        0     9372 2023-06-19 17:02:55.227034 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg
--rw-r--r--   0        0        0     9408 2023-06-19 17:02:55.227611 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg
--rw-r--r--   0        0        0     8489 2023-06-19 17:02:55.228264 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg
--rw-r--r--   0        0        0     9350 2023-06-19 17:02:55.228810 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg
--rw-r--r--   0        0        0   411771 2023-06-19 17:02:55.233572 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg
--rw-r--r--   0        0        0    42085 2023-06-19 17:02:55.234686 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/profile.jpg
--rw-r--r--   0        0        0     1662 2023-06-19 17:02:55.235481 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-1.png
--rw-r--r--   0        0        0     1560 2023-06-19 17:02:55.236026 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-2.png
--rw-r--r--   0        0        0    32086 2023-06-22 15:43:25.323112 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/box.png
--rw-r--r--   0        0        0   104704 2023-06-19 17:02:55.237763 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png
--rw-r--r--   0        0        0   170223 2023-06-19 17:02:55.238852 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png
--rw-r--r--   0        0        0   115557 2023-06-19 17:02:55.240831 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png
--rw-r--r--   0        0        0    14068 2023-06-19 17:02:55.241456 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png
--rw-r--r--   0        0        0     6239 2023-06-19 17:02:55.242061 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png
--rw-r--r--   0        0        0     8193 2023-06-19 17:02:55.245012 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png
--rw-r--r--   0        0        0   111459 2023-06-19 17:02:55.245681 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/emoticon.png
--rw-r--r--   0        0        0     2070 2023-06-19 17:02:55.246414 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/dark-mode.js
--rw-r--r--   0        0        0    10781 2023-07-12 14:30:13.012279 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/install.js
--rw-r--r--   0        0        0     8283 2023-06-20 14:50:28.132874 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js
--rw-r--r--   0        0        0     4186 2023-06-19 17:02:55.248210 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/google-maps.js
--rw-r--r--   0        0        0    15246 2023-06-19 17:02:55.248828 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pcoded.min.js
--rw-r--r--   0        0        0   117119 2023-06-19 17:02:55.250050 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/vendor-all.min.js
--rw-r--r--   0        0        0   209436 2023-06-19 17:02:55.251932 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js
--rw-r--r--   0        0        0   168766 2023-06-19 17:02:55.253536 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js
--rw-r--r--   0        0        0    12853 2023-06-19 17:02:55.254172 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js
--rw-r--r--   0        0        0      664 2023-06-19 17:02:55.254824 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg
--rw-r--r--   0        0        0      533 2023-06-19 17:02:55.255352 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg
--rw-r--r--   0        0        0     2915 2023-06-19 17:02:55.256048 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js
--rw-r--r--   0        0        0    14700 2023-06-19 17:02:55.256659 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js
--rw-r--r--   0        0        0     6464 2023-06-19 17:02:55.260444 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js
--rw-r--r--   0        0        0    49474 2023-06-19 17:02:55.261308 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js
--rw-r--r--   0        0        0    30335 2023-06-19 17:02:55.262045 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js
--rw-r--r--   0        0        0   130785 2023-06-19 17:02:55.263354 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js
--rw-r--r--   0        0        0    57902 2023-06-19 17:02:55.264343 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css
--rw-r--r--   0        0        0   173477 2023-06-20 14:32:33.510617 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   183849 2023-06-20 14:32:39.581340 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   123727 2023-06-20 14:32:53.377164 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0    57656 2023-06-20 14:33:05.897034 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0    22774 2023-06-20 14:32:56.220296 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js
--rw-r--r--   0        0        0      433 2023-06-19 17:02:55.269431 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/css/morris.css
--rw-r--r--   0        0        0    35652 2023-06-19 17:02:55.270307 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js
--rw-r--r--   0        0        0    92631 2023-06-19 17:02:55.271715 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js
--rw-r--r--   0        0        0    45950 2023-06-19 17:02:55.272798 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js
--rw-r--r--   0        0        0    86927 2023-06-19 17:02:55.274313 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js
--rw-r--r--   0        0        0     2850 2023-06-19 17:02:55.275041 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
--rw-r--r--   0        0        0    11662 2023-06-19 17:02:55.275780 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
--rw-r--r--   0        0        0   461387 2023-06-19 17:02:55.278722 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js
--rw-r--r--   0        0        0     7416 2023-06-20 14:30:54.723653 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js
--rw-r--r--   0        0        0     1774 2023-06-20 14:34:31.583987 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css
--rw-r--r--   0        0        0     3582 2023-06-19 17:02:55.282733 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/scss/dark.scss
--rw-r--r--   0        0        0     2873 2023-06-20 13:40:16.409928 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/accounts/login.html
--rw-r--r--   0        0        0    11196 2023-07-04 17:16:01.979812 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/acl.html
--rw-r--r--   0        0        0    23017 2023-07-12 14:42:39.685655 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/config.html
--rw-r--r--   0        0        0     7827 2023-07-04 17:16:19.165269 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/dependency.html
--rw-r--r--   0        0        0     4563 2023-07-04 17:16:27.724233 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/endpoint.html
--rw-r--r--   0        0        0     5184 2023-07-05 11:53:27.086067 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/feedback.html
--rw-r--r--   0        0        0    32266 2023-07-04 17:17:24.326002 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/index.html
--rw-r--r--   0        0        0      845 2023-06-19 17:02:55.286540 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-403.html
--rw-r--r--   0        0        0      846 2023-06-19 17:02:55.287062 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-404.html
--rw-r--r--   0        0        0     1130 2023-06-19 17:02:55.287848 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-500.html
--rw-r--r--   0        0        0     3050 2023-06-19 17:02:55.288892 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-blank.html
--rw-r--r--   0        0        0     8348 2023-06-19 17:02:55.289793 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/profile.html
--rw-r--r--   0        0        0     7700 2023-06-19 17:02:55.291327 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/navigation.html
--rw-r--r--   0        0        0      547 2023-06-19 17:02:55.291941 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/scripts.html
--rw-r--r--   0        0        0     5310 2023-07-12 14:31:09.510236 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/sidebar.html
--rw-r--r--   0        0        0    15819 2023-07-12 14:30:33.367878 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/install.html
--rw-r--r--   0        0        0     1683 2023-07-12 14:31:24.110465 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/key.html
--rw-r--r--   0        0        0     2842 2023-06-19 17:02:55.293834 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html
--rw-r--r--   0        0        0     2945 2023-06-19 17:02:55.294311 gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base.html
--rw-r--r--   0        0        0     7452 1970-01-01 00:00:00.000000 gemini_self_protector-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-17 13:13:50.672809 gemini_self_protector-0.1.2a0/LICENSE
+-rw-r--r--   0        0        0     6700 2023-06-26 14:16:25.914242 gemini_self_protector-0.1.2a0/README.md
+-rw-r--r--   0        0        0      491 2023-07-21 12:12:49.647645 gemini_self_protector-0.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-06-19 16:48:28.286310 gemini_self_protector-0.1.2a0/src/gemini_self_protector/.DS_Store
+-rw-r--r--   0        0        0      558 2023-06-19 16:47:36.851640 gemini_self_protector-0.1.2a0/src/gemini_self_protector/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-19 16:47:28.845395 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_audit.py
+-rw-r--r--   0        0        0     4000 2023-06-19 16:47:22.196160 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_cli.py
+-rw-r--r--   0        0        0    13840 2023-07-04 17:18:00.743973 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_config.py
+-rw-r--r--   0        0        0    20786 2023-07-12 14:31:35.889747 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_gemini.py
+-rw-r--r--   0        0        0    36293 2023-07-21 12:02:49.953482 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_gui.py
+-rw-r--r--   0        0        0     2737 2023-06-14 15:41:22.128264 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_logger.py
+-rw-r--r--   0        0        0     3508 2023-07-12 14:32:01.923270 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_model.py
+-rw-r--r--   0        0        0    14724 2023-07-03 17:28:57.174109 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_protect.py
+-rw-r--r--   0        0        0     1667 2023-06-19 16:46:34.460479 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_template.py
+-rw-r--r--   0        0        0    16402 2023-07-21 12:08:02.593658 gemini_self_protector-0.1.2a0/src/gemini_self_protector/_utils.py
+-rw-r--r--   0        0        0     6391 2023-07-03 17:31:00.908120 gemini_self_protector-0.1.2a0/src/gemini_self_protector/gemini_self_protector.py
+-rw-r--r--   0        0        0     6148 2023-06-08 10:29:06.101686 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/.DS_Store
+-rw-r--r--   0        0        0     8196 2023-06-21 15:35:28.362352 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/.DS_Store
+-rw-r--r--   0        0        0     3356 2023-06-20 14:32:27.097647 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/css/dark.css
+-rw-r--r--   0        0        0     5484 2023-06-19 17:02:55.146292 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/css/install.css
+-rw-r--r--   0        0        0   311910 2023-07-04 17:15:39.423308 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/css/style.css
+-rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.149256 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css
+-rw-r--r--   0        0        0     2548 2023-06-19 17:02:55.149663 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot
+-rw-r--r--   0        0        0     2530 2023-06-19 17:02:55.150002 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg
+-rw-r--r--   0        0        0     2400 2023-06-19 17:02:55.150303 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf
+-rw-r--r--   0        0        0     1544 2023-06-19 17:02:55.150704 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff
+-rw-r--r--   0        0        0    11805 2023-06-19 17:02:55.151201 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css
+-rw-r--r--   0        0        0    55828 2023-06-19 17:02:55.152093 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot
+-rw-r--r--   0        0        0   191595 2023-06-19 17:02:55.154892 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg
+-rw-r--r--   0        0        0    55664 2023-06-19 17:02:55.156107 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf
+-rw-r--r--   0        0        0    26432 2023-06-19 17:02:55.156890 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff
+-rw-r--r--   0        0        0    41065 2023-06-19 17:02:55.160256 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css
+-rw-r--r--   0        0        0   111620 2023-06-19 17:02:55.162260 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   599834 2023-06-19 17:02:55.169295 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   111384 2023-06-19 17:02:55.171076 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    71560 2023-06-19 17:02:55.174761 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    61336 2023-06-19 17:02:55.175547 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    31272 2023-06-19 17:02:55.176292 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   104706 2023-06-19 17:02:55.177586 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    31044 2023-06-19 17:02:55.178645 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    14724 2023-06-19 17:02:55.179411 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    12188 2023-06-19 17:02:55.179988 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   133140 2023-06-19 17:02:55.181538 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   488395 2023-06-19 17:02:55.190179 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   132920 2023-06-19 17:02:55.194157 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    63836 2023-06-19 17:02:55.195167 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    50372 2023-06-19 17:02:55.204039 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     3822 2023-06-19 17:02:55.204861 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/chrome.png
+-rw-r--r--   0        0        0     4809 2023-06-19 17:02:55.205402 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/firefox.png
+-rw-r--r--   0        0        0     4359 2023-06-19 17:02:55.205942 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/ie.png
+-rw-r--r--   0        0        0     3379 2023-06-19 17:02:55.206498 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/opera.png
+-rw-r--r--   0        0        0     4915 2023-06-19 17:02:55.207015 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/safari.png
+-rw-r--r--   0        0        0    15406 2023-06-21 08:29:54.000000 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/favicon.ico
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/gemini-7.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/logo-dark.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/logo-thumb.png
+-rw-r--r--   0        0        0    33174 2023-06-21 14:45:03.762621 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/logo.png
+-rw-r--r--   0        0        0    31417 2023-06-19 17:02:55.211234 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg
+-rw-r--r--   0        0        0    66369 2023-06-19 17:02:55.212675 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg
+-rw-r--r--   0        0        0    22071 2023-06-19 17:02:55.213564 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg
+-rw-r--r--   0        0        0    21820 2023-06-19 17:02:55.214458 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg
+-rw-r--r--   0        0        0    33652 2023-06-19 17:02:55.215162 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg
+-rw-r--r--   0        0        0   246009 2023-06-19 17:02:55.221542 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img1.jpg
+-rw-r--r--   0        0        0   165567 2023-06-19 17:02:55.223424 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img2.jpg
+-rw-r--r--   0        0        0   168914 2023-06-19 17:02:55.225478 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img3.jpg
+-rw-r--r--   0        0        0     9287 2023-06-19 17:02:55.226420 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg
+-rw-r--r--   0        0        0     9372 2023-06-19 17:02:55.227034 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg
+-rw-r--r--   0        0        0     9408 2023-06-19 17:02:55.227611 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg
+-rw-r--r--   0        0        0     8489 2023-06-19 17:02:55.228264 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg
+-rw-r--r--   0        0        0     9350 2023-06-19 17:02:55.228810 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg
+-rw-r--r--   0        0        0   411771 2023-06-19 17:02:55.233572 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg
+-rw-r--r--   0        0        0    42085 2023-06-19 17:02:55.234686 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/profile.jpg
+-rw-r--r--   0        0        0     1662 2023-06-19 17:02:55.235481 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/user-1.png
+-rw-r--r--   0        0        0     1560 2023-06-19 17:02:55.236026 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/user-2.png
+-rw-r--r--   0        0        0    32086 2023-06-22 15:43:25.323112 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/box.png
+-rw-r--r--   0        0        0   104704 2023-06-19 17:02:55.237763 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png
+-rw-r--r--   0        0        0   170223 2023-06-19 17:02:55.238852 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png
+-rw-r--r--   0        0        0   115557 2023-06-19 17:02:55.240831 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png
+-rw-r--r--   0        0        0    14068 2023-06-19 17:02:55.241456 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png
+-rw-r--r--   0        0        0     6239 2023-06-19 17:02:55.242061 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png
+-rw-r--r--   0        0        0     8193 2023-06-19 17:02:55.245012 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png
+-rw-r--r--   0        0        0   111459 2023-06-19 17:02:55.245681 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/emoticon.png
+-rw-r--r--   0        0        0     2070 2023-06-19 17:02:55.246414 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/dark-mode.js
+-rw-r--r--   0        0        0    10781 2023-07-12 14:30:13.012279 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/install.js
+-rw-r--r--   0        0        0     8283 2023-06-20 14:50:28.132874 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js
+-rw-r--r--   0        0        0     4186 2023-06-19 17:02:55.248210 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/pages/google-maps.js
+-rw-r--r--   0        0        0    15246 2023-06-19 17:02:55.248828 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/pcoded.min.js
+-rw-r--r--   0        0        0   117119 2023-06-19 17:02:55.250050 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/vendor-all.min.js
+-rw-r--r--   0        0        0   209436 2023-06-19 17:02:55.251932 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js
+-rw-r--r--   0        0        0   168766 2023-06-19 17:02:55.253536 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js
+-rw-r--r--   0        0        0    12853 2023-06-19 17:02:55.254172 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js
+-rw-r--r--   0        0        0      664 2023-06-19 17:02:55.254824 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg
+-rw-r--r--   0        0        0      533 2023-06-19 17:02:55.255352 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg
+-rw-r--r--   0        0        0     2915 2023-06-19 17:02:55.256048 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js
+-rw-r--r--   0        0        0    14700 2023-06-19 17:02:55.256659 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js
+-rw-r--r--   0        0        0     6464 2023-06-19 17:02:55.260444 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js
+-rw-r--r--   0        0        0    49474 2023-06-19 17:02:55.261308 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js
+-rw-r--r--   0        0        0    30335 2023-06-19 17:02:55.262045 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js
+-rw-r--r--   0        0        0   130785 2023-06-19 17:02:55.263354 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js
+-rw-r--r--   0        0        0    57902 2023-06-19 17:02:55.264343 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css
+-rw-r--r--   0        0        0   173477 2023-06-20 14:32:33.510617 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   183849 2023-06-20 14:32:39.581340 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   123727 2023-06-20 14:32:53.377164 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0    57656 2023-06-20 14:33:05.897034 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0    22774 2023-06-20 14:32:56.220296 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js
+-rw-r--r--   0        0        0      433 2023-06-19 17:02:55.269431 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/chart-morris/css/morris.css
+-rw-r--r--   0        0        0    35652 2023-06-19 17:02:55.270307 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js
+-rw-r--r--   0        0        0    92631 2023-06-19 17:02:55.271715 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js
+-rw-r--r--   0        0        0    45950 2023-06-19 17:02:55.272798 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js
+-rw-r--r--   0        0        0    86927 2023-06-19 17:02:55.274313 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js
+-rw-r--r--   0        0        0     2850 2023-06-19 17:02:55.275041 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css
+-rw-r--r--   0        0        0    11662 2023-06-19 17:02:55.275780 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js
+-rw-r--r--   0        0        0   461387 2023-06-19 17:02:55.278722 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js
+-rw-r--r--   0        0        0     7416 2023-06-20 14:30:54.723653 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js
+-rw-r--r--   0        0        0     1774 2023-06-20 14:34:31.583987 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css
+-rw-r--r--   0        0        0     3582 2023-06-19 17:02:55.282733 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/scss/dark.scss
+-rw-r--r--   0        0        0     6148 2023-06-20 17:13:15.353918 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/.DS_Store
+-rw-r--r--   0        0        0     2873 2023-06-20 13:40:16.409928 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/accounts/login.html
+-rw-r--r--   0        0        0    11196 2023-07-04 17:16:01.979812 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/acl.html
+-rw-r--r--   0        0        0    23042 2023-07-21 12:07:10.268507 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/config.html
+-rw-r--r--   0        0        0     7827 2023-07-04 17:16:19.165269 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/dependency.html
+-rw-r--r--   0        0        0     4563 2023-07-04 17:16:27.724233 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/endpoint.html
+-rw-r--r--   0        0        0     5184 2023-07-05 11:53:27.086067 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/feedback.html
+-rw-r--r--   0        0        0    32271 2023-07-21 12:20:25.954872 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/index.html
+-rw-r--r--   0        0        0      845 2023-06-19 17:02:55.286540 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-403.html
+-rw-r--r--   0        0        0      846 2023-06-19 17:02:55.287062 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-404.html
+-rw-r--r--   0        0        0     1130 2023-06-19 17:02:55.287848 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-500.html
+-rw-r--r--   0        0        0     3050 2023-06-19 17:02:55.288892 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-blank.html
+-rw-r--r--   0        0        0     8348 2023-06-19 17:02:55.289793 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/profile.html
+-rw-r--r--   0        0        0     7700 2023-06-19 17:02:55.291327 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/includes/navigation.html
+-rw-r--r--   0        0        0      547 2023-06-19 17:02:55.291941 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/includes/scripts.html
+-rw-r--r--   0        0        0     5310 2023-07-12 14:31:09.510236 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/includes/sidebar.html
+-rw-r--r--   0        0        0    15819 2023-07-12 14:30:33.367878 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/install.html
+-rw-r--r--   0        0        0     1683 2023-07-12 14:31:24.110465 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/key.html
+-rw-r--r--   0        0        0     2842 2023-06-19 17:02:55.293834 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html
+-rw-r--r--   0        0        0     2945 2023-06-19 17:02:55.294311 gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/layouts/base.html
+-rw-r--r--   0        0        0     7454 1970-01-01 00:00:00.000000 gemini_self_protector-0.1.2a0/PKG-INFO
```

### Comparing `gemini_self_protector-0.1.2/LICENSE` & `gemini_self_protector-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/README.md` & `gemini_self_protector-0.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/__init__.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/__init__.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_audit.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_audit.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_cli.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_cli.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_config.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_config.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_gemini.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_gemini.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_gui.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import ipaddress
 import re
 import os
 import json
 import ast
 from math import floor
 
+
 class _Gemini_GUI(object):
 
     def __init__(self, flask_app: Flask) -> None:
         logger.info(
             "[+] Running gemini-self protector - GUI Mode")
 
         # @flask_app.before_request
@@ -22,31 +23,31 @@
 
         # Create a blueprint for the nested Flask service
         nested_service = Blueprint(
             'nested_service', __name__, template_folder="templates", static_folder='static')
 
         if flask_app.secret_key is None:
             flask_app.secret_key = _Gemini.get_gemini_config().secret_key
-        
+
         if flask_app.config.get('MAX_CONTENT_LENGTH') is None:
             flask_app.config.update(
-                MAX_CONTENT_LENGTH= _Gemini.get_gemini_config().max_content_length
+                MAX_CONTENT_LENGTH=_Gemini.get_gemini_config().max_content_length
             )
-        
+
         if flask_app.template_folder and flask_app.static_folder:
             if _Gemini.get_gemini_config().app_path is None:
                 _Gemini.init_gemini_app_path()
 
             _Gemini.init_gemini_dashboard(
                 flask_app.template_folder, flask_app.static_folder)
 
             gemini_app_path = _Gemini.get_gemini_config().app_path
             logger.info(
                 "[+] Access Your Gemini Dashboard as Path: http://host:port/{0}".format(gemini_app_path))
-            
+
             @nested_service.app_template_filter('gemini_datetime_format')
             def datetime_format(value, format='%d %B %H:%M'):
                 if isinstance(value, str):
                     value = datetime.strptime(value, '%Y-%m-%d %H:%M:%S')
                 return value.strftime(format)
 
             @nested_service.app_template_filter('gemini_round_number')
@@ -55,21 +56,18 @@
                 return floor(value * multiplier + 0.5) / multiplier
 
             @nested_service.route('/', methods=['GET', 'POST'])
             def gemini_init():
                 try:
                     isInstall = _Gemini.get_gemini_config().isinstall
                     if int(isInstall):
-                        if _Gemini.is_valid_license_key():
-                            if session.get('gemini_logged_in'):
-                                return redirect(url_for('nested_service.gemini_dashboard'))
-                            else:
-                                return redirect(url_for('nested_service.gemini_login'))
+                        if session.get('gemini_logged_in'):
+                            return redirect(url_for('nested_service.gemini_dashboard'))
                         else:
-                            return redirect(url_for('nested_service.gemini_update_key'))
+                            return redirect(url_for('nested_service.gemini_login'))
                     else:
                         return redirect(url_for('nested_service.gemini_install'))
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_init', e))
 
             @nested_service.route('/install', methods=['GET', 'POST'])
@@ -106,54 +104,57 @@
                                     "sensitive_value": int(sensitive_value),
                                     "app_path": app_path,
                                     "notification_channel": notification_channel,
                                     "telegram_token": telegram_token,
                                     "telegram_chat_id": telegram_chat_id,
                                     "notification_webhook": notification_webhook,
                                     "predict_server": predict_server,
-                                    "predict_server_key_auth" : predict_server_key_auth
+                                    "predict_server_key_auth": predict_server_key_auth
                                 })
                                 _Gemini.update_gemini_user({
                                     "password": argon2.hash(password),
                                 })
                                 logger.info(
                                     "[+] Install gemini-self-protector successful.!")
-                                flash('Instal gemini-self-protector successful. Login and explore now', 'login')
+                                flash(
+                                    'Instal gemini-self-protector successful. Login and explore now', 'login')
                                 return redirect(url_for('nested_service.gemini_login'))
                         else:
                             sensitive_value = _Gemini.get_gemini_config().sensitive_value
                             app_path = _Gemini.get_gemini_config().app_path
                             return render_template('gemini-protector-gui/install.html', _sensitive_value=sensitive_value, _app_path=app_path)
-                
+
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_install', e))
 
             @nested_service.route('/update-key', methods=['GET', 'POST'])
             def gemini_update_key():
                 try:
                     is_install = _Gemini.get_gemini_config().isinstall
                     if int(is_install) == 0:
                         return redirect(url_for('nested_service.gemini_install'))
 
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     if request.method == 'POST':
                         key = request.form['key']
                         if _Gemini.validator_key_auth(key):
-                            flash('Predict server key auth update successful', 'key_update_success')
+                            flash('Predict server key auth update successful',
+                                  'key_update_success')
                             return redirect(url_for('nested_service.gemini_dashboard'))
                         else:
                             return render_template('gemini-protector-gui/key.html', msg="Invalid predict server key auth")
                     return render_template('gemini-protector-gui/key.html')
 
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_update_key', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_update_key', e))
 
             @nested_service.route('/login', methods=['GET', 'POST'])
             def gemini_login():
                 try:
                     is_install = _Gemini.get_gemini_config().isinstall
                     if int(is_install) == 0:
                         flash('Please install!', 'required')
@@ -166,33 +167,35 @@
                         username = request.form['username']
                         password = request.form['password']
 
                         app_username = _Gemini.get_gemini_user().username
                         app_password = _Gemini.get_gemini_user().password
 
                         password_check = argon2.verify(password, app_password)
-                        
+
                         if username == app_username and password_check:
                             session['gemini_logged_in'] = True
-                            flash('Welcome back {}!'.format(app_username), 'login')
+                            flash('Welcome back {}!'.format(
+                                app_username), 'login')
                             return redirect(url_for('nested_service.gemini_dashboard'))
                         else:
                             return render_template('gemini-protector-gui/accounts/login.html', msg="Incorrect Username / Password")
                     return render_template('gemini-protector-gui/accounts/login.html')
 
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_login', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_login', e))
 
             @nested_service.route('/profile')
             def gemini_profile():
                 try:
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     if request.method == 'POST':
                         password = request.form['pwd']
                         confirm_password = request.form['cpwd']
 
                         if not _Gemini.validator_dashboard_password(password, confirm_password):
                             return render_template('gemini-protector-gui/home/profile.html', msg="Invalid password")
 
@@ -202,38 +205,40 @@
                         logger.info("[+] Update password successful.")
                         return redirect(url_for('nested_service.gemini_login'))
 
                     app_username = _Gemini.get_gemini_user().username
                     return render_template('gemini-protector-gui/home/profile.html', _username=app_username)
 
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_profile', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_profile', e))
 
             @nested_service.route('/dashboard')
             def gemini_dashboard():
                 try:
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     gemini_summary = _Gemini.get_gemini_summary()
                     gemini_config = _Gemini.get_gemini_config()
                     gemini_user = _Gemini.get_gemini_user()
                     request_log = _Gemini.get_gemini_request_log()
                     # predict_server_status = _Gemini.health_check_predict_server()
-                    
-                    sorted_request_log_data = sorted(request_log, key=lambda x: x.time)
+
+                    sorted_request_log_data = sorted(
+                        request_log, key=lambda x: x.time)
                     page = int(request.args.get('page', 1))
                     per_page = 5
                     total_records = len(sorted_request_log_data)
                     total_pages = (total_records + per_page - 1) // per_page
                     start_index = (page - 1) * per_page
                     end_index = start_index + per_page
                     limited_request_log_data = sorted_request_log_data[start_index:end_index]
-                    
+
                     attack_counts = {
                         'Malicious Request': 0,
                         'ACL Block': 0,
                         'Malicious Response': 0,
                         'Unvalidated Redirects': 0,
                         'Large Requests': 0,
                         'HTTP Method Tampering': 0,
@@ -242,34 +247,35 @@
 
                     for log in request_log:
                         attack_type = log.attack_type
                         if attack_type in attack_counts:
                             attack_counts[attack_type] += 1
 
                     return render_template('gemini-protector-gui/home/index.html',
-                                        _username=gemini_user.username,
-                                        _protect_mode=gemini_config.global_protect_mode,
-                                        _total_request=gemini_summary.total_request,
-                                        _normal_request=gemini_summary.normal_request,
-                                        _abnormal_request=gemini_summary.abnormal_request,
-                                        _sensitive_value=gemini_config.sensitive_value,
-                                        _normal_response=gemini_summary.normal_response,
-                                        _abnormal_response=gemini_summary.abnormal_response,
-                                        _gemini_request_log_data=limited_request_log_data,
-                                        _current_page=page,
-                                        _total_pages=total_pages,
-                                        _anti_dos=gemini_config.anti_dos,
-                                        _max_req_per_min=gemini_config.max_requests_per_minute,
-                                        # _gemini_predict_server_status=predict_server_status,
-                                        # _gemini_predict_server=gemini_config.predict_server,
-                                        _gemini_notification_channel=gemini_config.notification_channel,
-                                        _gemini_attack_counts=attack_counts
-                                        )
+                                           _username=gemini_user.username,
+                                           _protect_mode=gemini_config.global_protect_mode,
+                                           _total_request=gemini_summary.total_request,
+                                           _normal_request=gemini_summary.normal_request,
+                                           _abnormal_request=gemini_summary.abnormal_request,
+                                           _sensitive_value=gemini_config.sensitive_value,
+                                           _normal_response=gemini_summary.normal_response,
+                                           _abnormal_response=gemini_summary.abnormal_response,
+                                           _gemini_request_log_data=limited_request_log_data,
+                                           _current_page=page,
+                                           _total_pages=total_pages,
+                                           _anti_dos=gemini_config.anti_dos,
+                                           _max_req_per_min=gemini_config.max_requests_per_minute,
+                                           # _gemini_predict_server_status=predict_server_status,
+                                           # _gemini_predict_server=gemini_config.predict_server,
+                                           _gemini_notification_channel=gemini_config.notification_channel,
+                                           _gemini_attack_counts=attack_counts
+                                           )
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_dashboard', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_dashboard', e))
 
             @nested_service.route('/configurate', methods=['GET', 'POST'])
             def gemini_configurate():
                 try:
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
@@ -277,15 +283,16 @@
                     if request.method == 'POST':
                         predict_server = request.form['predict_server']
                         protect_mode = request.form['protect_mode']
                         sensitive_value = request.form['sensitive_value']
                         max_content_length = request.form['max_content_length']
                         http_method = request.form.getlist('http_method[]')
                         safe_redirect_status = request.form['safe_redirect_status']
-                        trust_domain_list = [d.strip() for d in request.form.get('trust_domain_list').split(',')]
+                        trust_domain_list = [d.strip() for d in request.form.get(
+                            'trust_domain_list').split(',')]
                         protect_response_status = request.form['protect_response_status']
                         acl_status = request.form['acl_status']
                         anti_dos = request.form['anti_dos_status']
                         max_request_per_min = request.form['max_request_per_min']
 
                         if _Gemini.validator_protect_mode(protect_mode) and _Gemini.validator_sensitive_value(sensitive_value) and max_content_length.isdigit() and _Gemini.validator_http_method(http_method) and _Gemini.validator_on_off_status(safe_redirect_status) and _Gemini.validator_trust_domain(trust_domain_list) and _Gemini.validator_on_off_status(protect_response_status) and _Gemini.validator_on_off_status(acl_status) and _Gemini.validator_on_off_status(anti_dos) and max_request_per_min.isdigit():
 
@@ -298,42 +305,48 @@
                                 "safe_redirect": int(safe_redirect_status),
                                 "protect_response": int(protect_response_status),
                                 "trust_domain": json.dumps(trust_domain_list),
                                 "enable_acl": int(acl_status),
                                 "anti_dos": int(anti_dos),
                                 "max_requests_per_minute": int(max_request_per_min)
                             })
-                            flash('Configuration update successful', 'config_update_success')
+                            flash('Configuration update successful',
+                                  'config_update_success')
                         else:
-                            flash('Configuration update failed', 'config_update_fail')
+                            flash('Configuration update failed',
+                                  'config_update_fail')
 
                         return redirect(url_for('nested_service.gemini_configurate'))
-                    
+
                     else:
                         gemini_config = _Gemini.get_gemini_config()
-                        trust_domain_list = ast.literal_eval(gemini_config.trust_domain)
+                        trust_domain_list = ast.literal_eval(
+                            gemini_config.trust_domain)
                         gemini_user = _Gemini.get_gemini_user()
 
                         return render_template('gemini-protector-gui/home/config.html',
-                                            _username=gemini_user.username,
-                                            _protect_mode=gemini_config.global_protect_mode,
-                                            _sensitive_value=gemini_config.sensitive_value,
-                                            _server_name=gemini_config.server_name,
-                                            _max_content_length=int(gemini_config.max_content_length / 1024 / 1024),
-                                            _http_method=gemini_config.http_method_allow,
-                                            _safe_redirect_status=gemini_config.safe_redirect,
-                                            _trust_domain_list=", ".join(trust_domain_list),
-                                            _predict_server=gemini_config.predict_server,
-                                            _protect_response=gemini_config.protect_response,
-                                            _is_enable_acl=gemini_config.enable_acl,
-                                            _is_anti_dos=gemini_config.anti_dos,
-                                            _max_request_per_min=gemini_config.max_requests_per_minute
-                                            )
+                                               _username=gemini_user.username,
+                                               _protect_mode=gemini_config.global_protect_mode,
+                                               _sensitive_value=gemini_config.sensitive_value,
+                                               _server_name=gemini_config.server_name,
+                                               _max_content_length=int(
+                                                   gemini_config.max_content_length / 1024 / 1024),
+                                               _http_method=gemini_config.http_method_allow,
+                                               _safe_redirect_status=gemini_config.safe_redirect,
+                                               _trust_domain_list=", ".join(
+                                                   trust_domain_list),
+                                               _predict_server=gemini_config.predict_server,
+                                               _protect_response=gemini_config.protect_response,
+                                               _is_enable_acl=gemini_config.enable_acl,
+                                               _is_anti_dos=gemini_config.anti_dos,
+                                               _max_request_per_min=gemini_config.max_requests_per_minute
+                                               )
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_configurate', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_configurate', e))
 
             @nested_service.route('/access-control-list', methods=['GET', 'POST'])
             def gemini_access_control_list():
                 try:
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
@@ -345,115 +358,127 @@
 
                         ipv4_pattern = r'^(\d{1,3}\.){3}\d{1,3}$'
                         ipv6_pattern = r'^([0-9a-fA-F]{1,4}:){7}[0-9a-fA-F]{1,4}$'
 
                         if re.match(ipv4_pattern, ip_address) or re.match(ipv6_pattern, ip_address):
                             ip = ipaddress.ip_address(ip_address)
                             if ip:
-                                _Gemini.store_gemini_acl(ipaddress=ip_address, isallow=access_type, desciption=description)
+                                _Gemini.store_gemini_acl(
+                                    ipaddress=ip_address, isallow=access_type, desciption=description)
                                 flash('ACL add successful', 'acl_success')
                             else:
                                 flash('ACL add failed', 'acl_fail')
                         else:
                             flash('ACL add failed', 'acl_fail')
 
                         return redirect(url_for('nested_service.gemini_access_control_list'))
 
                     else:
                         gemini_user = _Gemini.get_gemini_user()
                         gemini_config = _Gemini.get_gemini_config()
                         is_enable_acl = gemini_config.enable_acl
                         access_control_list = _Gemini.get_gemini_acl()
-                        sorted_access_control_list_data = sorted(access_control_list, key=lambda x: x.created_at)
+                        sorted_access_control_list_data = sorted(
+                            access_control_list, key=lambda x: x.created_at)
 
                         page = int(request.args.get('page', 1))
                         per_page = 5
 
                         total_records = len(sorted_access_control_list_data)
-                        total_pages = (total_records + per_page - 1) // per_page
+                        total_pages = (total_records +
+                                       per_page - 1) // per_page
 
                         start_index = (page - 1) * per_page
                         end_index = start_index + per_page
-                        limited_access_control_list = sorted_access_control_list_data[start_index:end_index]
+                        limited_access_control_list = sorted_access_control_list_data[
+                            start_index:end_index]
 
                         return render_template('gemini-protector-gui/home/acl.html',
-                                            _username=gemini_user.username,
-                                            _is_enable_acl=is_enable_acl,
-                                            _gemini_acl=limited_access_control_list,
-                                            _current_page=page,
-                                            _total_pages=total_pages
-                                            )
+                                               _username=gemini_user.username,
+                                               _is_enable_acl=is_enable_acl,
+                                               _gemini_acl=limited_access_control_list,
+                                               _current_page=page,
+                                               _total_pages=total_pages
+                                               )
 
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_access_control_list', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_access_control_list', e))
 
             @nested_service.route('/remove-acl', methods=['POST'])
             def gemini_remove_acl():
                 try:
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
 
                     ip_address = request.form['ip_address']
 
                     try:
                         ip = ipaddress.ip_address(ip_address)
                     except ValueError:
-                        flash('AC remove failed. IP address {} is not valid'.format(ip_address), 'acl_fail')
+                        flash('AC remove failed. IP address {} is not valid'.format(
+                            ip_address), 'acl_fail')
                         return redirect(url_for('nested_service.gemini_access_control_list'))
 
                     _Gemini.remove_gemini_acl(str(ip))
                     flash('AC remove successful', 'acl_success')
                     return redirect(url_for('nested_service.gemini_access_control_list'))
 
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_remove_acl', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_remove_acl', e))
 
             @nested_service.route('/dependency-vulnerability', methods=['GET', 'POST'])
             def gemini_dependency_audit():
                 try:
                     if not session.get('gemini_logged_in'):
                         return redirect(url_for('nested_service.gemini_login'))
 
                     if request.method == 'POST':
                         file_path = request.form['dependency_path']
                         filename = os.path.basename(file_path)
                         if filename == 'requirements.txt':
-                            _Gemini.__audit_dependency_vulnerability__(file_path)
+                            _Gemini.__audit_dependency_vulnerability__(
+                                file_path)
                             flash('Check dependency successful', 'audit_success')
                         else:
                             flash('Check dependency failed', 'audit_fail')
                     else:
                         gemini_user = _Gemini.get_gemini_user()
                         dependency_file = _Gemini.get_dependency_file()
                         dependency_result = _Gemini.get_gemini_audit_dependency()
-                        sorted_dependency_result = sorted(dependency_result, key=lambda x: x.created_at)
+                        sorted_dependency_result = sorted(
+                            dependency_result, key=lambda x: x.created_at)
 
                         page = int(request.args.get('page', 1))
                         per_page = 5
 
                         total_records = len(sorted_dependency_result)
-                        total_pages = (total_records + per_page - 1) // per_page
+                        total_pages = (total_records +
+                                       per_page - 1) // per_page
 
                         start_index = (page - 1) * per_page
                         end_index = start_index + per_page
                         limited_dependency_result = sorted_dependency_result[start_index:end_index]
 
                         return render_template('gemini-protector-gui/home/dependency.html',
-                                            _username=gemini_user.username,
-                                            _gemini_dependency_file=dependency_file,
-                                            _gemini_dependency_result=limited_dependency_result,
-                                            gemini_page_pagination=len(dependency_result),
-                                            _current_page=page,
-                                            _total_pages=total_pages)
+                                               _username=gemini_user.username,
+                                               _gemini_dependency_file=dependency_file,
+                                               _gemini_dependency_result=limited_dependency_result,
+                                               gemini_page_pagination=len(
+                                                   dependency_result),
+                                               _current_page=page,
+                                               _total_pages=total_pages)
 
                     return redirect(url_for('nested_service.gemini_dependency_audit'))
 
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_dependency_audit', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_dependency_audit', e))
 
             @nested_service.route('/event', methods=['POST'])
             def gemini_get_event():
                 try:
                     if not session.get('gemini_logged_in'):
                         flash('Please login', 'required_login')
                         return redirect(url_for('nested_service.gemini_login'))
@@ -477,56 +502,59 @@
                             "res_content": str(record.res_content),
                             "attack_type": record.attack_type,
                             "predict": record.predict,
                             "latitude": record.latitude,
                             "longitude": record.longitude,
                             "created_at": record.created_at,
                             "updated_at": record.updated_at
-                            })
+                        })
                     else:
                         return jsonify({
                             "status": False,
                             "message": "Event ID does not exist"
                         })
                 except Exception as e:
-                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_get_event', e))
+                    logger.error("[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format(
+                        'nested_service.route.gemini_get_event', e))
 
             @nested_service.route('/event-feedback', methods=['POST'])
             def gemini_event_feedback():
                 try:
                     if not session.get('gemini_logged_in'):
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     event_id = request.json['event_id']
                     feedback_value = request.json['feedback_value']
 
                     record = _Gemini.get_gemini_detail_request_log(event_id)
                     if record:
-                        sentence = "{}{}".format(record.request, record.req_body)
-                        _Gemini.store_gemini_feedback(sentence, int(feedback_value))
+                        sentence = "{}{}".format(
+                            record.request, record.req_body)
+                        _Gemini.store_gemini_feedback(
+                            sentence, int(feedback_value))
                         _Gemini.update_gemini_request_log(record.event_id)
                         return jsonify({
                             "status": True,
                             "message": "Update feedback successful"
                         })
                     else:
                         return jsonify({
                             "status": False,
                             "message": "Update feedback failed"
                         })
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_event_feedback', e))
-            
+
             @nested_service.route('/endpoint', methods=['GET'])
             def gemini_endpoint():
                 try:
                     if not session.get('gemini_logged_in'):
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     app_path = _Gemini.get_gemini_config().app_path
                     links = []
                     for rule in flask_app.url_map.iter_rules():
                         options = {}
                         for arg in rule.arguments:
                             options[arg] = "[{0}]".format(arg)
 
@@ -546,73 +574,74 @@
 
                     total_records = len(_sorted_links)
                     total_pages = (total_records + per_page - 1) // per_page
 
                     start_index = (page - 1) * per_page
                     end_index = start_index + per_page
                     limited_links = _sorted_links[start_index:end_index]
-                    return render_template('gemini-protector-gui/home/endpoint.html', 
-                                            _sorted_links=limited_links,
-                                            _current_page=page,
-                                            _total_pages=total_pages
+                    return render_template('gemini-protector-gui/home/endpoint.html',
+                                           _sorted_links=limited_links,
+                                           _current_page=page,
+                                           _total_pages=total_pages
                                            )
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_endpoint', e))
 
             @nested_service.route('/feedback', methods=['GET'])
             def gemini_feedback():
                 try:
                     if not session.get('gemini_logged_in'):
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     feedback = _Gemini.get_gemini_feedback()
 
-                    _sorted_links = sorted(feedback, key=lambda x: x.created_at)
+                    _sorted_links = sorted(
+                        feedback, key=lambda x: x.created_at)
                     page = int(request.args.get('page', 1))
                     per_page = 5
 
                     total_records = len(_sorted_links)
                     total_pages = (total_records + per_page - 1) // per_page
 
                     start_index = (page - 1) * per_page
                     end_index = start_index + per_page
                     limited_links = _sorted_links[start_index:end_index]
-                    return render_template('gemini-protector-gui/home/feedback.html', 
-                                            _sorted_links=limited_links,
-                                            _current_page=page,
-                                            _total_pages=total_pages
+                    return render_template('gemini-protector-gui/home/feedback.html',
+                                           _sorted_links=limited_links,
+                                           _current_page=page,
+                                           _total_pages=total_pages
                                            )
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_endpoint', e))
 
             @nested_service.route('/export-feedback')
             def gemini_export_feedback():
                 try:
                     if not session.get('gemini_logged_in'):
                         return redirect(url_for('nested_service.gemini_login'))
-                    
+
                     csv_file = _Gemini.export_gemini_feedback()
-                    return send_file(csv_file, as_attachment=True) 
+                    return send_file(csv_file, as_attachment=True)
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_export_feedback', e))
 
             @nested_service.route('/logout')
             def gemini_logout():
                 try:
                     app_username = _Gemini.get_gemini_user().username
                     session['gemini_logged_in'] = False
                     flash('Goodbye {}!'.format(app_username), 'logout')
                     return redirect(url_for('nested_service.gemini_login'))
                 except Exception as e:
                     logger.error(
                         "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('nested_service.route.gemini_logout', e))
-            
+
             @nested_service.errorhandler(403)
             def access_forbidden(error):
                 return render_template('gemini-protector-gui/home/page-403.html'), 403
 
             @nested_service.errorhandler(404)
             def not_found_error(error):
                 return render_template('gemini-protector-gui/home/page-404.html'), 404
```

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_logger.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_logger.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_model.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_model.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_protect.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_protect.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_template.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_template.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/_utils.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,20 +233,20 @@
         It checks if the protect_mode is in the array arr_mode. If it is, it returns True. If it isn't,
         it returns False
 
         :param protect_mode: This is the mode that you want to run the script in
         :return: a boolean value.
         """
         try:
-            arr_mode = ['off', 'block', 'monitor']
+            arr_mode = ['off', 'protection', 'monitor']
             if protect_mode in arr_mode:
                 return True
             else:
                 logger.error(
-                    "[x_x] Invalid Protect Mode. Protect mode must be: monitor - block - off")
+                    "[x_x] Invalid Protect Mode. Protect mode must be: monitor - protection - off")
                 return False
         except Exception as e:
             logger.error(
                 "[x_x] Something went wrong at {0}, please check your error message.\n Message - {1}".format('_Validator.validate_protect_mode', e))
 
     def validate_sensitive_value(sensitive_value) -> None:
         """
```

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/gemini_self_protector.py` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/gemini_self_protector.py`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/dark.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/css/dark.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/install.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/css/install.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/css/style.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/datta-icon.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/datta/fonts/pct.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/css/feather.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/feather/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/css/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/fonts/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/chrome.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/chrome.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/firefox.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/firefox.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/ie.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/ie.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/opera.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/opera.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/browser/safari.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/browser/safari.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/favicon.ico` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/gemini-7.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/gemini-7.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-dark.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/logo-dark.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo-thumb.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/logo-thumb.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/logo.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-4.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img-slide-5.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img1.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img2.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/slider/img3.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/slider/img3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-1.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-2.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-3.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-4.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/avatar-5.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/monkey-man.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/profile.jpg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/profile.jpg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-1.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/user-1.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/user/user-2.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/user/user-2.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/box.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/box.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-1.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-2.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-3.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-4.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-5.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/dashborad-6.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/images/widget/emoticon.png` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/images/widget/emoticon.png`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/dark-mode.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/dark-mode.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/install.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/install.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/pages/chart-morris-custom.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pages/google-maps.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/pages/google-maps.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/pcoded.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/pcoded.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/js/vendor-all.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/js/vendor-all.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/amcharts.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/ammap.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/gauge.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/dragIconRoundBig.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/images/lens.svg`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/light.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/pie.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/radar.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/serial.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/usaLow.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/amchart/js/worldLow.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/animation/css/animate.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/bootstrap/js/popover.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/morris.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/chart-morris/js/raphael.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/google-maps/js/gmaps.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/css/jquery.scrollbar.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery-scrollbar/js/jquery.scrollbar.min.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/jquery-ui/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify-js.js`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/plugins/toastify/toastify.min.css`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/assets/scss/dark.scss` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/assets/scss/dark.scss`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/accounts/login.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/accounts/login.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/acl.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/acl.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/config.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/config.html`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,19 @@
                                                     <input type="radio" id="protect-mode-monitor" name="protect_mode"
                                                         value="monitor" class="custom-control-input" {% if
                                                         _protect_mode=='monitor' %}checked{% endif %}>
                                                     <label class="custom-control-label"
                                                         for="protect-mode-monitor">Monitor</label>
                                                 </div>
                                                 <div class="custom-control custom-radio custom-control-inline">
-                                                    <input type="radio" id="protect-mode-block" name="protect_mode"
-                                                        value="block" class="custom-control-input" {% if
-                                                        _protect_mode=='block' %}checked{% endif %}>
+                                                    <input type="radio" id="protect-mode-protection" name="protect_mode"
+                                                        value="protection" class="custom-control-input" {% if
+                                                        _protect_mode=='protection' %}checked{% endif %}>
                                                     <label class="custom-control-label"
-                                                        for="protect-mode-block">Block</label>
+                                                        for="protect-mode-protection">Protection</label>
                                                 </div>
                                                 <div class="custom-control custom-radio custom-control-inline">
                                                     <input type="radio" id="protect-mode-off" name="protect_mode"
                                                         value="off" class="custom-control-input" {% if
                                                         _protect_mode=='off' %}checked{% endif %}>
                                                     <label class="custom-control-label"
                                                         for="protect-mode-off">Off</label>
```

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/dependency.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/dependency.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/endpoint.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/endpoint.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/feedback.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/feedback.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/index.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,15 @@
                                             </div>
                                         </div>
                                         <h2 class="mt-3 f-w-300">{{_protect_mode|title}}<sub
                                                 class="text-muted f-14">Global</sub></h2>
                                         {% if _protect_mode == 'monitor' %}
                                         <h6 class="text-muted mt-4 mb-0">Gemini is monitoring all requests</h6>
                                         <i class="fa fa-binoculars text-c-purple f-50"></i>
-                                        {% elif _protect_mode == 'block' %}
+                                        {% elif _protect_mode == 'protection' %}
                                         <h6 class="text-muted mt-4 mb-0">Gemini is blocking abnormal requests</h6>
                                         <i class="fas fa-ban text-c-purple f-50"></i>
                                         {% else %}
                                         <h6 class="text-muted mt-4 mb-0">Gemini is sleeping</h6>
                                         <i class="fas fa-power-off text-c-red f-50"></i>
                                         {% endif %}
                                     </div>
@@ -488,15 +488,15 @@
             var modalId = $(this).attr('id');
             var eventId = modalId.replace('feedbackGoodBtn', '');
             $("#" + eventId).closest("tr").removeClass().addClass("readed");
             $.ajax({
                 url: "{{url_for('nested_service.gemini_event_feedback')}}",
                 method: 'POST',
                 contentType: 'application/json',
-                data: JSON.stringify({ event_id: eventId, feedback_value: 0 }),
+                data: JSON.stringify({ event_id: eventId, feedback_value: 1 }),
                 success: function (data) {
                     Toastify({
                         text: "Update feedback successful",
                         duration: 3000,
                         gravity: "top", // `top` or `bottom`
                         position: "right", // `left`, `center` or `right`
                         stopOnFocus: true, // Prevents dismissing of toast on hover
@@ -525,15 +525,15 @@
             var modalId = $(this).attr('id');
             var eventId = modalId.replace('feedbackBadBtn', '');
             $("#" + eventId).closest("tr").removeClass().addClass("readed");
             $.ajax({
                 url: "{{url_for('nested_service.gemini_event_feedback')}}",
                 method: 'POST',
                 contentType: 'application/json',
-                data: JSON.stringify({ event_id: eventId, feedback_value: 1 }),
+                data: JSON.stringify({ event_id: eventId, feedback_value: 0 }),
                 success: function (data) {
                     Toastify({
                         text: "Update feedback successful",
                         duration: 3000,
                         gravity: "top", // `top` or `bottom`
                         position: "right", // `left`, `center` or `right`
                         stopOnFocus: true, // Prevents dismissing of toast on hover
```

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-403.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-403.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-404.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-404.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-500.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-500.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/page-blank.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/page-blank.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/home/profile.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/home/profile.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/navigation.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/includes/navigation.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/scripts.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/includes/scripts.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/includes/sidebar.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/includes/sidebar.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/install.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/install.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/key.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/key.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/layouts/base-fullscreen.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/src/gemini_self_protector/resource/templates/layouts/base.html` & `gemini_self_protector-0.1.2a0/src/gemini_self_protector/resource/templates/layouts/base.html`

 * *Files identical despite different names*

### Comparing `gemini_self_protector-0.1.2/PKG-INFO` & `gemini_self_protector-0.1.2a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-self-protector
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Runtime Application Self-Protection
 License: MIT
 Author: lethanhphuc
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

