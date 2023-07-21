# Comparing `tmp/copyparty-1.8.3.tar.gz` & `tmp/copyparty-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyparty-1.8.3.tar", last modified: Sun Jul 16 22:39:55 2023, max compression
+gzip compressed data, was "copyparty-1.8.4.tar", last modified: Tue Jul 18 08:04:10 2023, max compression
```

## Comparing `copyparty-1.8.3.tar` & `copyparty-1.8.4.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.380805 copyparty-1.8.3/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.8.3/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-16 22:39:55.379805 copyparty-1.8.3/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)    96750 2023-07-16 21:23:16.000000 copyparty-1.8.3/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.364805 copyparty-1.8.3/copyparty/
--rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    76501 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      246 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    69349 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/authsrv.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.366805 copyparty-1.8.3/copyparty/bos/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/bos/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/bos/bos.py
--rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/bos/path.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3915 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/broker_mp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/broker_mpw.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/broker_thr.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/broker_util.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7135 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/cert.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7497 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/cfg.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/dxml.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/fsutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15455 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/ftpd.py
--rw-r--r--   0 ed        (1000) ed        (1000)   128151 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/httpcli.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/httpconn.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/httpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3016 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/ico.py
--rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/mdns.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/mtag.py
--rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/multicast.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3859 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/pwhash.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.367805 copyparty-1.8.3/copyparty/res/
--rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/res/COPYING.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/res/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.8.3/copyparty/res/insecure.pem
--rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/smbd.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/ssdp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/star.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.367805 copyparty-1.8.3/copyparty/stolen/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.368805 copyparty-1.8.3/copyparty/stolen/dnslib/
--rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/dnslib/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/dnslib/bimap.py
--rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/dnslib/bit.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/dnslib/buffer.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/dnslib/dns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/dnslib/label.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/dnslib/lex.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/dnslib/ranges.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.369805 copyparty-1.8.3/copyparty/stolen/ifaddr/
--rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/ifaddr/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/ifaddr/_posix.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/ifaddr/_shared.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/stolen/ifaddr/_win32.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/qrcodegen.py
--rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/stolen/surrogateescape.py
--rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/sutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    24336 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/svchub.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/szip.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16753 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/tcpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/th_cli.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22828 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/th_srv.py
--rw-r--r--   0 ed        (1000) ed        (1000)    10589 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/u2idx.py
--rw-r--r--   0 ed        (1000) ed        (1000)   124414 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)    72768 2023-07-16 22:39:38.000000 copyparty-1.8.3/copyparty/util.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.372805 copyparty-1.8.3/copyparty/web/
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.373805 copyparty-1.8.3/copyparty/web/a/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/web/a/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/web/a/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/web/a/u2c.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.8.3/copyparty/web/a/webdav-cfg.bat
--rw-r--r--   0 ed        (1000) ed        (1000)     7309 2023-07-16 17:45:42.000000 copyparty-1.8.3/copyparty/web/baguettebox.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10996 2023-07-13 23:14:15.000000 copyparty-1.8.3/copyparty/web/browser.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.8.3/copyparty/web/browser.html
--rw-r--r--   0 ed        (1000) ed        (1000)    59820 2023-07-16 18:14:02.000000 copyparty-1.8.3/copyparty/web/browser.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.8.3/copyparty/web/browser2.html
--rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.8.3/copyparty/web/cf.html
--rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.8.3/copyparty/web/dbg-audio.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.373805 copyparty-1.8.3/copyparty/web/dd/
--rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.8.3/copyparty/web/dd/2.png
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.3/copyparty/web/dd/3.png
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.8.3/copyparty/web/dd/4.png
--rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.8.3/copyparty/web/dd/5.png
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/web/dd/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.378805 copyparty-1.8.3/copyparty/web/deps/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:39.000000 copyparty-1.8.3/copyparty/web/deps/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.8.3/copyparty/web/deps/easymde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.8.3/copyparty/web/deps/easymde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.8.3/copyparty/web/deps/marked.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.8.3/copyparty/web/deps/mini-fa.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.8.3/copyparty/web/deps/mini-fa.woff
--rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.8.3/copyparty/web/deps/prism.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.8.3/copyparty/web/deps/prism.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.8.3/copyparty/web/deps/prismd.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.8.3/copyparty/web/deps/scp.woff2
--rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.8.3/copyparty/web/deps/sha512.ac.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.8.3/copyparty/web/deps/sha512.hw.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.8.3/copyparty/web/md.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.8.3/copyparty/web/md.html
--rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.8.3/copyparty/web/md.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.8.3/copyparty/web/md2.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.8.3/copyparty/web/md2.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.8.3/copyparty/web/mde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.8.3/copyparty/web/mde.html
--rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.8.3/copyparty/web/mde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.3/copyparty/web/msg.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.8.3/copyparty/web/msg.html
--rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.8.3/copyparty/web/splash.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.8.3/copyparty/web/splash.html
--rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.8.3/copyparty/web/splash.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.8.3/copyparty/web/svcs.html
--rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.8.3/copyparty/web/svcs.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-06-25 23:05:18.000000 copyparty-1.8.3/copyparty/web/ui.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.8.3/copyparty/web/up2k.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    13146 2023-06-25 22:59:55.000000 copyparty-1.8.3/copyparty/web/util.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.8.3/copyparty/web/w.hash.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-16 22:39:55.365805 copyparty-1.8.3/copyparty.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-16 22:39:55.000000 copyparty-1.8.3/copyparty.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2828 2023-07-16 22:39:55.000000 copyparty-1.8.3/copyparty.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-07-16 22:39:55.000000 copyparty-1.8.3/copyparty.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-07-16 22:39:55.000000 copyparty-1.8.3/copyparty.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      139 2023-07-16 22:39:55.000000 copyparty-1.8.3/copyparty.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-07-16 22:39:55.000000 copyparty-1.8.3/copyparty.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)     4032 2023-06-25 19:16:18.000000 copyparty-1.8.3/pyproject.toml
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-07-16 22:39:55.380805 copyparty-1.8.3/setup.cfg
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.056205 copyparty-1.8.4/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.8.4/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-18 08:04:10.056205 copyparty-1.8.4/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)    96750 2023-07-16 21:23:16.000000 copyparty-1.8.4/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.045205 copyparty-1.8.4/copyparty/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    76501 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/__main__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      246 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/__version__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    69349 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/authsrv.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.046205 copyparty-1.8.4/copyparty/bos/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/bos/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/bos/bos.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/bos/path.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3915 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_mp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_mpw.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_thr.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_util.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7135 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/cert.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7564 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/cfg.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/dxml.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/fsutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15455 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/ftpd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   128117 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/httpcli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/httpconn.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/httpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3016 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/ico.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/mdns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/mtag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/multicast.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3859 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/pwhash.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.047205 copyparty-1.8.4/copyparty/res/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/res/COPYING.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/res/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.8.4/copyparty/res/insecure.pem
+-rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/smbd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/ssdp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/star.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.047205 copyparty-1.8.4/copyparty/stolen/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.048205 copyparty-1.8.4/copyparty/stolen/dnslib/
+-rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/bimap.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/bit.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/buffer.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/dns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/label.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/lex.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/ranges.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.048205 copyparty-1.8.4/copyparty/stolen/ifaddr/
+-rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/_posix.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/_shared.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/_win32.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/qrcodegen.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/surrogateescape.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/sutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    24336 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/svchub.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/szip.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16753 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/tcpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/th_cli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22828 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/th_srv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    10589 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/u2idx.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   124800 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    72768 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/util.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.052205 copyparty-1.8.4/copyparty/web/
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.052205 copyparty-1.8.4/copyparty/web/a/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/a/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/a/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/a/u2c.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.8.4/copyparty/web/a/webdav-cfg.bat
+-rw-r--r--   0 ed        (1000) ed        (1000)     7309 2023-07-16 17:45:42.000000 copyparty-1.8.4/copyparty/web/baguettebox.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10996 2023-07-13 23:14:15.000000 copyparty-1.8.4/copyparty/web/browser.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.8.4/copyparty/web/browser.html
+-rw-r--r--   0 ed        (1000) ed        (1000)    59820 2023-07-16 18:14:02.000000 copyparty-1.8.4/copyparty/web/browser.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.8.4/copyparty/web/browser2.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.8.4/copyparty/web/cf.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.8.4/copyparty/web/dbg-audio.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.053205 copyparty-1.8.4/copyparty/web/dd/
+-rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/2.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/3.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/4.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/5.png
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/dd/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.055205 copyparty-1.8.4/copyparty/web/deps/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/deps/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.8.4/copyparty/web/deps/easymde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.8.4/copyparty/web/deps/easymde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.8.4/copyparty/web/deps/marked.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.8.4/copyparty/web/deps/mini-fa.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.8.4/copyparty/web/deps/mini-fa.woff
+-rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.8.4/copyparty/web/deps/prism.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.8.4/copyparty/web/deps/prism.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.8.4/copyparty/web/deps/prismd.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.8.4/copyparty/web/deps/scp.woff2
+-rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.8.4/copyparty/web/deps/sha512.ac.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.8.4/copyparty/web/deps/sha512.hw.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.8.4/copyparty/web/md.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.8.4/copyparty/web/md.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.8.4/copyparty/web/md.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.8.4/copyparty/web/md2.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.8.4/copyparty/web/md2.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.8.4/copyparty/web/mde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.8.4/copyparty/web/mde.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.8.4/copyparty/web/mde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/msg.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.8.4/copyparty/web/msg.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.8.4/copyparty/web/splash.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.8.4/copyparty/web/splash.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.8.4/copyparty/web/splash.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.8.4/copyparty/web/svcs.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.8.4/copyparty/web/svcs.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-06-25 23:05:18.000000 copyparty-1.8.4/copyparty/web/ui.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.8.4/copyparty/web/up2k.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    13146 2023-06-25 22:59:55.000000 copyparty-1.8.4/copyparty/web/util.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.8.4/copyparty/web/w.hash.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.046205 copyparty-1.8.4/copyparty.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     2828 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      139 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)     4032 2023-06-25 19:16:18.000000 copyparty-1.8.4/pyproject.toml
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-07-18 08:04:10.056205 copyparty-1.8.4/setup.cfg
```

### Comparing `copyparty-1.8.3/LICENSE` & `copyparty-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/PKG-INFO` & `copyparty-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.8.3
+Version: 1.8.4
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.8.3/README.md` & `copyparty-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/__init__.py` & `copyparty-1.8.4/copyparty/__init__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/__main__.py` & `copyparty-1.8.4/copyparty/__main__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/authsrv.py` & `copyparty-1.8.4/copyparty/authsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/bos/bos.py` & `copyparty-1.8.4/copyparty/bos/bos.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/bos/path.py` & `copyparty-1.8.4/copyparty/bos/path.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/broker_mp.py` & `copyparty-1.8.4/copyparty/broker_mp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/broker_mpw.py` & `copyparty-1.8.4/copyparty/broker_mpw.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/broker_thr.py` & `copyparty-1.8.4/copyparty/broker_thr.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/broker_util.py` & `copyparty-1.8.4/copyparty/broker_util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/cert.py` & `copyparty-1.8.4/copyparty/cert.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/cfg.py` & `copyparty-1.8.4/copyparty/cfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -105,14 +105,15 @@
         "d2v": "disables file verification, overrides -e2v*",
         "d2d": "disables all database stuff, overrides -e2*",
         "hist=/tmp/cdb": "puts thumbnails and indexes at that location",
         "scan=60": "scan for new files every 60sec, same as --re-maxage",
         "nohash=\\.iso$": "skips hashing file contents if path matches *.iso",
         "noidx=\\.iso$": "fully ignores the contents at paths matching *.iso",
         "noforget": "don't forget files when deleted from disk",
+        "fat32": "avoid excessive reindexing on android sdcardfs",
         "dbd=[acid|swal|wal|yolo]": "database speed-durability tradeoff",
         "xlink": "cross-volume dupe detection / linking",
         "xdev": "do not descend into other filesystems",
         "xvol": "do not follow symlinks leaving the volume root",
         "dotsrch": "show dotfiles in search results",
         "nodotsrch": "hide dotfiles in search results (default)",
     },
```

### Comparing `copyparty-1.8.3/copyparty/dxml.py` & `copyparty-1.8.4/copyparty/dxml.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/fsutil.py` & `copyparty-1.8.4/copyparty/fsutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/ftpd.py` & `copyparty-1.8.4/copyparty/ftpd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/httpcli.py` & `copyparty-1.8.4/copyparty/httpcli.py`

 * *Files 0% similar despite different names*

```diff
@@ -6370,1641 +6370,1639 @@
 00018e10: 2020 2020 7265 7475 726e 2072 6574 2e6c      return ret.l
 00018e20: 6f77 6572 2829 0a0a 2020 2020 2020 2020  ower()..        
 00018e30: 7265 7475 726e 2022 2220 2023 2075 6e68  return ""  # unh
 00018e40: 616e 646c 6564 202f 2066 616c 6c74 6872  andled / fallthr
 00018e50: 6f75 6768 0a0a 2020 2020 6465 6620 7363  ough..    def sc
 00018e60: 616e 766f 6c28 7365 6c66 2920 203a 0a20  anvol(self)  :. 
 00018e70: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00018e80: 6c66 2e63 616e 5f72 6561 6420 6f72 206e  lf.can_read or n
-00018e90: 6f74 2073 656c 662e 6361 6e5f 7772 6974  ot self.can_writ
-00018ea0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00018eb0: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
-00018ec0: 2022 6e6f 7420 616c 6c6f 7765 6420 666f   "not allowed fo
-00018ed0: 7220 7573 6572 2022 202b 2073 656c 662e  r user " + self.
-00018ee0: 756e 616d 6529 0a0a 2020 2020 2020 2020  uname)..        
-00018ef0: 6966 2073 656c 662e 6172 6773 2e6e 6f5f  if self.args.no_
-00018f00: 7265 7363 616e 3a0a 2020 2020 2020 2020  rescan:.        
-00018f10: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
-00018f20: 2834 3033 2c20 2274 6865 2072 6573 6361  (403, "the resca
-00018f30: 6e20 6665 6174 7572 6520 6973 2064 6973  n feature is dis
-00018f40: 6162 6c65 6420 696e 2073 6572 7665 7220  abled in server 
-00018f50: 636f 6e66 6967 2229 0a0a 2020 2020 2020  config")..      
-00018f60: 2020 766e 2c20 5f20 3d20 7365 6c66 2e61    vn, _ = self.a
-00018f70: 7372 762e 7666 732e 6765 7428 7365 6c66  srv.vfs.get(self
-00018f80: 2e76 7061 7468 2c20 7365 6c66 2e75 6e61  .vpath, self.una
-00018f90: 6d65 2c20 5472 7565 2c20 5472 7565 290a  me, True, True).
-00018fa0: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
-00018fb0: 5b73 656c 662e 6173 7276 2e76 6673 2e61  [self.asrv.vfs.a
-00018fc0: 6c6c 5f76 6f6c 732c 205b 766e 2e76 7061  ll_vols, [vn.vpa
-00018fd0: 7468 5d2c 2046 616c 7365 2c20 5472 7565  th], False, True
-00018fe0: 5d0a 0a20 2020 2020 2020 2078 203d 2073  ]..        x = s
-00018ff0: 656c 662e 636f 6e6e 2e68 7372 762e 6272  elf.conn.hsrv.br
-00019000: 6f6b 6572 2e61 736b 2822 7570 326b 2e72  oker.ask("up2k.r
-00019010: 6573 6361 6e22 2c20 2a61 7267 7329 0a20  escan", *args). 
-00019020: 2020 2020 2020 2065 7272 203d 2078 2e67         err = x.g
-00019030: 6574 2829 0a20 2020 2020 2020 2069 6620  et().        if 
-00019040: 6e6f 7420 6572 723a 0a20 2020 2020 2020  not err:.       
-00019050: 2020 2020 2073 656c 662e 7265 6469 7265       self.redire
-00019060: 6374 2822 222c 2022 3f68 2229 0a20 2020  ct("", "?h").   
-00019070: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00019080: 5472 7565 0a0a 2020 2020 2020 2020 7261  True..        ra
-00019090: 6973 6520 5065 626b 6163 2835 3030 2c20  ise Pebkac(500, 
-000190a0: 6572 7229 0a0a 2020 2020 6465 6620 6861  err)..    def ha
-000190b0: 6e64 6c65 5f72 656c 6f61 6428 7365 6c66  ndle_reload(self
-000190c0: 2920 203a 0a20 2020 2020 2020 2061 6374  )  :.        act
-000190d0: 203d 2073 656c 662e 7570 6172 616d 2e67   = self.uparam.g
-000190e0: 6574 2822 7265 6c6f 6164 2229 0a20 2020  et("reload").   
-000190f0: 2020 2020 2069 6620 6163 7420 213d 2022       if act != "
-00019100: 6366 6722 3a0a 2020 2020 2020 2020 2020  cfg":.          
-00019110: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-00019120: 3030 2c20 226f 6e6c 7920 636f 6e66 6967  00, "only config
-00019130: 2066 696c 6573 2028 2763 6667 2729 2063   files ('cfg') c
-00019140: 616e 2062 6520 7265 6c6f 6164 6564 2072  an be reloaded r
-00019150: 6e22 290a 0a20 2020 2020 2020 2069 6620  n")..        if 
-00019160: 6e6f 7420 5b78 2066 6f72 2078 2069 6e20  not [x for x in 
-00019170: 7365 6c66 2e77 766f 6c20 6966 2078 2069  self.wvol if x i
-00019180: 6e20 7365 6c66 2e72 766f 6c5d 3a0a 2020  n self.rvol]:.  
-00019190: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000191a0: 5065 626b 6163 2834 3033 2c20 226e 6f74  Pebkac(403, "not
-000191b0: 2061 6c6c 6f77 6564 2066 6f72 2075 7365   allowed for use
-000191c0: 7220 2220 2b20 7365 6c66 2e75 6e61 6d65  r " + self.uname
-000191d0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-000191e0: 6c66 2e61 7267 732e 6e6f 5f72 656c 6f61  lf.args.no_reloa
-000191f0: 643a 0a20 2020 2020 2020 2020 2020 2072  d:.            r
-00019200: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
-00019210: 2022 7468 6520 7265 6c6f 6164 2066 6561   "the reload fea
-00019220: 7475 7265 2069 7320 6469 7361 626c 6564  ture is disabled
-00019230: 2069 6e20 7365 7276 6572 2063 6f6e 6669   in server confi
-00019240: 6722 290a 0a20 2020 2020 2020 2078 203d  g")..        x =
-00019250: 2073 656c 662e 636f 6e6e 2e68 7372 762e   self.conn.hsrv.
-00019260: 6272 6f6b 6572 2e61 736b 2822 7265 6c6f  broker.ask("relo
-00019270: 6164 2229 0a20 2020 2020 2020 2072 6574  ad").        ret
-00019280: 7572 6e20 7365 6c66 2e72 6564 6972 6563  urn self.redirec
-00019290: 7428 2222 2c20 223f 6822 2c20 782e 6765  t("", "?h", x.ge
-000192a0: 7428 292c 2022 7265 7475 726e 2074 6f22  t(), "return to"
-000192b0: 2c20 4661 6c73 6529 0a0a 2020 2020 6465  , False)..    de
-000192c0: 6620 7478 5f73 7461 636b 2873 656c 6629  f tx_stack(self)
-000192d0: 2020 3a0a 2020 2020 2020 2020 6966 206e    :.        if n
-000192e0: 6f74 205b 7820 666f 7220 7820 696e 2073  ot [x for x in s
-000192f0: 656c 662e 7776 6f6c 2069 6620 7820 696e  elf.wvol if x in
-00019300: 2073 656c 662e 7276 6f6c 5d3a 0a20 2020   self.rvol]:.   
-00019310: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-00019320: 6562 6b61 6328 3430 332c 2022 6e6f 7420  ebkac(403, "not 
-00019330: 616c 6c6f 7765 6420 666f 7220 7573 6572  allowed for user
-00019340: 2022 202b 2073 656c 662e 756e 616d 6529   " + self.uname)
-00019350: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
-00019360: 662e 6172 6773 2e6e 6f5f 7374 6163 6b3a  f.args.no_stack:
-00019370: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00019380: 7365 2050 6562 6b61 6328 3430 332c 2022  se Pebkac(403, "
-00019390: 7468 6520 7374 6163 6b64 756d 7020 6665  the stackdump fe
-000193a0: 6174 7572 6520 6973 2064 6973 6162 6c65  ature is disable
-000193b0: 6420 696e 2073 6572 7665 7220 636f 6e66  d in server conf
-000193c0: 6967 2229 0a0a 2020 2020 2020 2020 7265  ig")..        re
-000193d0: 7420 3d20 223c 7072 653e 7b7d 5c6e 7b7d  t = "<pre>{}\n{}
-000193e0: 222e 666f 726d 6174 2874 696d 652e 7469  ".format(time.ti
-000193f0: 6d65 2829 2c20 6874 6d6c 5f65 7363 6170  me(), html_escap
-00019400: 6528 616c 6c74 7261 6365 2829 2929 0a20  e(alltrace())). 
-00019410: 2020 2020 2020 2073 656c 662e 7265 706c         self.repl
-00019420: 7928 7265 742e 656e 636f 6465 2822 7574  y(ret.encode("ut
-00019430: 662d 3822 2929 0a20 2020 2020 2020 2072  f-8")).        r
-00019440: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-00019450: 6465 6620 7478 5f74 7265 6528 7365 6c66  def tx_tree(self
-00019460: 2920 203a 0a20 2020 2020 2020 2074 6f70  )  :.        top
-00019470: 203d 2073 656c 662e 7570 6172 616d 5b22   = self.uparam["
-00019480: 7472 6565 225d 206f 7220 2222 0a20 2020  tree"] or "".   
-00019490: 2020 2020 2064 7374 203d 2073 656c 662e       dst = self.
-000194a0: 7670 6174 680a 2020 2020 2020 2020 6966  vpath.        if
-000194b0: 2074 6f70 2069 6e20 5b22 2e22 2c20 222e   top in [".", ".
-000194c0: 2e22 5d3a 0a20 2020 2020 2020 2020 2020  ."]:.           
-000194d0: 2074 6f70 203d 2075 6e64 6f74 2873 656c   top = undot(sel
-000194e0: 662e 7670 6174 6820 2b20 222f 2220 2b20  f.vpath + "/" + 
-000194f0: 746f 7029 0a0a 2020 2020 2020 2020 6966  top)..        if
-00019500: 2074 6f70 203d 3d20 6473 743a 0a20 2020   top == dst:.   
-00019510: 2020 2020 2020 2020 2064 7374 203d 2022           dst = "
-00019520: 220a 2020 2020 2020 2020 656c 6966 2074  ".        elif t
-00019530: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
-00019540: 6966 206e 6f74 2064 7374 2e73 7461 7274  if not dst.start
-00019550: 7377 6974 6828 746f 7020 2b20 222f 2229  swith(top + "/")
-00019560: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019570: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
-00019580: 3030 2c20 2261 7267 2066 756e 6b22 290a  00, "arg funk").
-00019590: 0a20 2020 2020 2020 2020 2020 2064 7374  .            dst
-000195a0: 203d 2064 7374 5b6c 656e 2874 6f70 2920   = dst[len(top) 
-000195b0: 2b20 3120 3a5d 0a0a 2020 2020 2020 2020  + 1 :]..        
-000195c0: 7265 7420 3d20 7365 6c66 2e67 656e 5f74  ret = self.gen_t
-000195d0: 7265 6528 746f 702c 2064 7374 290a 2020  ree(top, dst).  
-000195e0: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
-000195f0: 5f76 7072 6f78 6965 643a 0a20 2020 2020  _vproxied:.     
-00019600: 2020 2020 2020 2070 6172 656e 7473 203d         parents =
-00019610: 2073 656c 662e 6172 6773 2e52 2e73 706c   self.args.R.spl
-00019620: 6974 2822 2f22 290a 2020 2020 2020 2020  it("/").        
-00019630: 2020 2020 666f 7220 7061 7265 6e74 2069      for parent i
-00019640: 6e20 7265 7665 7273 6564 2870 6172 656e  n reversed(paren
-00019650: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
-00019660: 2020 2020 2072 6574 203d 207b 226b 2573       ret = {"k%s
-00019670: 2220 2520 2870 6172 656e 742c 293a 2072  " % (parent,): r
-00019680: 6574 2c20 2261 223a 205b 5d7d 0a0a 2020  et, "a": []}..  
-00019690: 2020 2020 2020 7a73 203d 206a 736f 6e2e        zs = json.
-000196a0: 6475 6d70 7328 7265 7429 0a20 2020 2020  dumps(ret).     
-000196b0: 2020 2073 656c 662e 7265 706c 7928 7a73     self.reply(zs
-000196c0: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-000196d0: 2c20 6d69 6d65 3d22 6170 706c 6963 6174  , mime="applicat
-000196e0: 696f 6e2f 6a73 6f6e 2229 0a20 2020 2020  ion/json").     
-000196f0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-00019700: 2020 2020 6465 6620 6765 6e5f 7472 6565      def gen_tree
-00019710: 2873 656c 662c 2074 6f70 202c 2074 6172  (self, top , tar
-00019720: 6765 7420 2920 2020 3a0a 2020 2020 2020  get )   :.      
-00019730: 2020 7265 7420 2020 3d20 7b7d 0a20 2020    ret   = {}.   
-00019740: 2020 2020 2065 7863 6c20 3d20 4e6f 6e65       excl = None
-00019750: 0a20 2020 2020 2020 2069 6620 7461 7267  .        if targ
-00019760: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00019770: 6578 636c 2c20 7461 7267 6574 203d 2028  excl, target = (
-00019780: 7461 7267 6574 2e73 706c 6974 2822 2f22  target.split("/"
-00019790: 2c20 3129 202b 205b 2222 5d29 5b3a 325d  , 1) + [""])[:2]
-000197a0: 0a20 2020 2020 2020 2020 2020 2073 7562  .            sub
-000197b0: 203d 2073 656c 662e 6765 6e5f 7472 6565   = self.gen_tree
-000197c0: 2822 2f22 2e6a 6f69 6e28 5b74 6f70 2c20  ("/".join([top, 
-000197d0: 6578 636c 5d29 2e73 7472 6970 2822 2f22  excl]).strip("/"
-000197e0: 292c 2074 6172 6765 7429 0a20 2020 2020  ), target).     
-000197f0: 2020 2020 2020 2072 6574 5b22 6b22 202b         ret["k" +
-00019800: 2071 756f 7465 7028 6578 636c 295d 203d   quotep(excl)] =
-00019810: 2073 7562 0a0a 2020 2020 2020 2020 7472   sub..        tr
-00019820: 793a 0a20 2020 2020 2020 2020 2020 2076  y:.            v
-00019830: 6e2c 2072 656d 203d 2073 656c 662e 6173  n, rem = self.as
-00019840: 7276 2e76 6673 2e67 6574 2874 6f70 2c20  rv.vfs.get(top, 
-00019850: 7365 6c66 2e75 6e61 6d65 2c20 5472 7565  self.uname, True
-00019860: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
-00019870: 2020 2020 2066 7372 6f6f 742c 2076 6673       fsroot, vfs
-00019880: 5f6c 732c 2076 6673 5f76 6972 7420 3d20  _ls, vfs_virt = 
-00019890: 766e 2e6c 7328 0a20 2020 2020 2020 2020  vn.ls(.         
-000198a0: 2020 2020 2020 2072 656d 2c0a 2020 2020         rem,.    
-000198b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000198c0: 2e75 6e61 6d65 2c0a 2020 2020 2020 2020  .uname,.        
-000198d0: 2020 2020 2020 2020 6e6f 7420 7365 6c66          not self
-000198e0: 2e61 7267 732e 6e6f 5f73 6361 6e64 6972  .args.no_scandir
-000198f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00019900: 2020 5b5b 5472 7565 2c20 4661 6c73 655d    [[True, False]
-00019910: 2c20 5b46 616c 7365 2c20 5472 7565 5d5d  , [False, True]]
-00019920: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00019930: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-00019940: 2020 2020 2020 2020 2020 2020 7666 735f              vfs_
-00019950: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
-00019960: 2020 2020 7666 735f 7669 7274 203d 207b      vfs_virt = {
-00019970: 7d0a 2020 2020 2020 2020 2020 2020 666f  }.            fo
-00019980: 7220 7620 696e 2073 656c 662e 7276 6f6c  r v in self.rvol
-00019990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000199a0: 2020 6431 2c20 6432 203d 2076 2e72 7370    d1, d2 = v.rsp
-000199b0: 6c69 7428 222f 222c 2031 2920 6966 2022  lit("/", 1) if "
-000199c0: 2f22 2069 6e20 7620 656c 7365 205b 2222  /" in v else [""
-000199d0: 2c20 765d 0a20 2020 2020 2020 2020 2020  , v].           
-000199e0: 2020 2020 2069 6620 6431 203d 3d20 746f       if d1 == to
-000199f0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00019a00: 2020 2020 2020 2076 6673 5f76 6972 745b         vfs_virt[
-00019a10: 6432 5d20 3d20 7365 6c66 2e61 7372 762e  d2] = self.asrv.
-00019a20: 7666 7320 2023 2074 7970 6563 686b 2c20  vfs  # typechk, 
-00019a30: 7661 6c75 6520 6e65 7665 7220 7265 6164  value never read
-00019a40: 0a0a 2020 2020 2020 2020 6469 7273 203d  ..        dirs =
-00019a50: 205b 5d0a 0a20 2020 2020 2020 2064 6972   []..        dir
-00019a60: 6e61 6d65 7320 3d20 5b78 5b30 5d20 666f  names = [x[0] fo
-00019a70: 7220 7820 696e 2076 6673 5f6c 7320 6966  r x in vfs_ls if
-00019a80: 2073 7461 742e 535f 4953 4449 5228 785b   stat.S_ISDIR(x[
-00019a90: 315d 2e73 745f 6d6f 6465 295d 0a0a 2020  1].st_mode)]..  
-00019aa0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00019ab0: 662e 6172 6773 2e65 6420 6f72 2022 646f  f.args.ed or "do
-00019ac0: 7473 2220 6e6f 7420 696e 2073 656c 662e  ts" not in self.
-00019ad0: 7570 6172 616d 3a0a 2020 2020 2020 2020  uparam:.        
-00019ae0: 2020 2020 6469 726e 616d 6573 203d 2065      dirnames = e
-00019af0: 7863 6c75 6465 5f64 6f74 6669 6c65 7328  xclude_dotfiles(
-00019b00: 6469 726e 616d 6573 290a 0a20 2020 2020  dirnames)..     
-00019b10: 2020 2066 6f72 2066 6e20 696e 205b 7820     for fn in [x 
-00019b20: 666f 7220 7820 696e 2064 6972 6e61 6d65  for x in dirname
-00019b30: 7320 6966 2078 2021 3d20 6578 636c 5d3a  s if x != excl]:
-00019b40: 0a20 2020 2020 2020 2020 2020 2064 6972  .            dir
-00019b50: 732e 6170 7065 6e64 2871 756f 7465 7028  s.append(quotep(
-00019b60: 666e 2929 0a0a 2020 2020 2020 2020 666f  fn))..        fo
-00019b70: 7220 7820 696e 2076 6673 5f76 6972 743a  r x in vfs_virt:
-00019b80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00019b90: 7820 213d 2065 7863 6c3a 0a20 2020 2020  x != excl:.     
-00019ba0: 2020 2020 2020 2020 2020 2064 6972 732e             dirs.
-00019bb0: 6170 7065 6e64 2878 290a 0a20 2020 2020  append(x)..     
-00019bc0: 2020 2072 6574 5b22 6122 5d20 3d20 6469     ret["a"] = di
-00019bd0: 7273 0a20 2020 2020 2020 2072 6574 7572  rs.        retur
-00019be0: 6e20 7265 740a 0a20 2020 2064 6566 2074  n ret..    def t
-00019bf0: 785f 7570 7328 7365 6c66 2920 203a 0a20  x_ups(self)  :. 
-00019c00: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00019c10: 6c66 2e61 7267 732e 756e 706f 7374 3a0a  lf.args.unpost:.
-00019c20: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00019c30: 6520 5065 626b 6163 2834 3033 2c20 2274  e Pebkac(403, "t
-00019c40: 6865 2075 6e70 6f73 7420 6665 6174 7572  he unpost featur
-00019c50: 6520 6973 2064 6973 6162 6c65 6420 696e  e is disabled in
-00019c60: 2073 6572 7665 7220 636f 6e66 6967 2229   server config")
-00019c70: 0a0a 2020 2020 2020 2020 6964 7820 3d20  ..        idx = 
-00019c80: 7365 6c66 2e63 6f6e 6e2e 6765 745f 7532  self.conn.get_u2
-00019c90: 6964 7828 290a 2020 2020 2020 2020 6966  idx().        if
-00019ca0: 206e 6f74 2069 6478 206f 7220 6e6f 7420   not idx or not 
-00019cb0: 6861 7361 7474 7228 6964 782c 2022 705f  hasattr(idx, "p_
-00019cc0: 656e 6422 293a 0a20 2020 2020 2020 2020  end"):.         
-00019cd0: 2020 2072 6169 7365 2050 6562 6b61 6328     raise Pebkac(
-00019ce0: 3530 302c 2022 7371 6c69 7465 3320 6973  500, "sqlite3 is
-00019cf0: 206e 6f74 2061 7661 696c 6162 6c65 206f   not available o
-00019d00: 6e20 7468 6520 7365 7276 6572 3b20 6361  n the server; ca
-00019d10: 6e6e 6f74 2075 6e70 6f73 7422 290a 0a20  nnot unpost").. 
-00019d20: 2020 2020 2020 2066 696c 7420 3d20 7365         filt = se
-00019d30: 6c66 2e75 7061 7261 6d2e 6765 7428 2266  lf.uparam.get("f
-00019d40: 696c 7465 7222 290a 2020 2020 2020 2020  ilter").        
-00019d50: 6669 6c74 203d 2075 6e71 756f 7465 7028  filt = unquotep(
-00019d60: 6669 6c74 206f 7220 2222 290a 2020 2020  filt or "").    
-00019d70: 2020 2020 6c6d 203d 2022 7570 7320 5b7b      lm = "ups [{
-00019d80: 7d5d 222e 666f 726d 6174 2866 696c 7429  }]".format(filt)
-00019d90: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
-00019da0: 6728 6c6d 290a 0a20 2020 2020 2020 2072  g(lm)..        r
-00019db0: 6574 2020 203d 205b 5d0a 2020 2020 2020  et   = [].      
-00019dc0: 2020 7430 203d 2074 696d 652e 7469 6d65    t0 = time.time
-00019dd0: 2829 0a20 2020 2020 2020 206c 696d 203d  ().        lim =
-00019de0: 2074 696d 652e 7469 6d65 2829 202d 2073   time.time() - s
-00019df0: 656c 662e 6172 6773 2e75 6e70 6f73 740a  elf.args.unpost.
-00019e00: 2020 2020 2020 2020 666b 5f76 6f6c 7320          fk_vols 
-00019e10: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00019e20: 766f 6c3a 2076 6f6c 2e66 6c61 6773 5b22  vol: vol.flags["
-00019e30: 666b 225d 0a20 2020 2020 2020 2020 2020  fk"].           
-00019e40: 2066 6f72 2076 702c 2076 6f6c 2069 6e20   for vp, vol in 
-00019e50: 7365 6c66 2e61 7372 762e 7666 732e 616c  self.asrv.vfs.al
-00019e60: 6c5f 766f 6c73 2e69 7465 6d73 2829 0a20  l_vols.items(). 
-00019e70: 2020 2020 2020 2020 2020 2069 6620 2266             if "f
-00019e80: 6b22 2069 6e20 766f 6c2e 666c 6167 7320  k" in vol.flags 
-00019e90: 616e 6420 2876 7020 696e 2073 656c 662e  and (vp in self.
-00019ea0: 7276 6f6c 206f 7220 7670 2069 6e20 7365  rvol or vp in se
-00019eb0: 6c66 2e75 7076 6f6c 290a 2020 2020 2020  lf.upvol).      
-00019ec0: 2020 7d0a 2020 2020 2020 2020 666f 7220    }.        for 
-00019ed0: 766f 6c20 696e 2073 656c 662e 6173 7276  vol in self.asrv
-00019ee0: 2e76 6673 2e61 6c6c 5f76 6f6c 732e 7661  .vfs.all_vols.va
-00019ef0: 6c75 6573 2829 3a0a 2020 2020 2020 2020  lues():.        
-00019f00: 2020 2020 6375 7220 3d20 6964 782e 6765      cur = idx.ge
-00019f10: 745f 6375 7228 766f 6c2e 7265 616c 7061  t_cur(vol.realpa
-00019f20: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
-00019f30: 6966 206e 6f74 2063 7572 3a0a 2020 2020  if not cur:.    
-00019f40: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00019f50: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-00019f60: 2020 6e66 6b20 3d20 666b 5f76 6f6c 732e    nfk = fk_vols.
-00019f70: 6765 7428 766f 6c2c 2030 290a 0a20 2020  get(vol, 0)..   
-00019f80: 2020 2020 2020 2020 2071 203d 2022 7365           q = "se
-00019f90: 6c65 6374 2073 7a2c 2072 642c 2066 6e2c  lect sz, rd, fn,
-00019fa0: 2061 7420 6672 6f6d 2075 7020 7768 6572   at from up wher
-00019fb0: 6520 6970 3d3f 2061 6e64 2061 743e 3f22  e ip=? and at>?"
-00019fc0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00019fd0: 2073 7a2c 2072 642c 2066 6e2c 2061 7420   sz, rd, fn, at 
-00019fe0: 696e 2063 7572 2e65 7865 6375 7465 2871  in cur.execute(q
-00019ff0: 2c20 2873 656c 662e 6970 2c20 6c69 6d29  , (self.ip, lim)
-0001a000: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001a010: 2020 2076 7020 3d20 222f 2220 2b20 222f     vp = "/" + "/
-0001a020: 222e 6a6f 696e 2878 2066 6f72 2078 2069  ".join(x for x i
-0001a030: 6e20 5b76 6f6c 2e76 7061 7468 2c20 7264  n [vol.vpath, rd
-0001a040: 2c20 666e 5d20 6966 2078 290a 2020 2020  , fn] if x).    
-0001a050: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-0001a060: 696c 7420 616e 6420 6669 6c74 206e 6f74  ilt and filt not
-0001a070: 2069 6e20 7670 3a0a 2020 2020 2020 2020   in vp:.        
-0001a080: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0001a090: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-0001a0a0: 2020 2020 2020 7276 203d 207b 2276 7022        rv = {"vp"
-0001a0b0: 3a20 7175 6f74 6570 2876 7029 2c20 2273  : quotep(vp), "s
-0001a0c0: 7a22 3a20 737a 2c20 2261 7422 3a20 6174  z": sz, "at": at
-0001a0d0: 2c20 226e 666b 223a 206e 666b 7d0a 2020  , "nfk": nfk}.  
-0001a0e0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001a0f0: 206e 666b 3a0a 2020 2020 2020 2020 2020   nfk:.          
-0001a100: 2020 2020 2020 2020 2020 7276 5b22 6170            rv["ap
-0001a110: 225d 203d 2076 6f6c 2e63 616e 6f6e 6963  "] = vol.canonic
-0001a120: 616c 2876 6a6f 696e 2872 642c 2066 6e29  al(vjoin(rd, fn)
-0001a130: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a140: 2020 2072 6574 2e61 7070 656e 6428 7276     ret.append(rv
-0001a150: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001a160: 2020 6966 206c 656e 2872 6574 2920 3e20    if len(ret) > 
-0001a170: 3330 3030 3a0a 2020 2020 2020 2020 2020  3000:.          
-0001a180: 2020 2020 2020 2020 2020 7265 742e 736f            ret.so
-0001a190: 7274 286b 6579 3d6c 616d 6264 6120 783a  rt(key=lambda x:
-0001a1a0: 2078 5b22 6174 225d 2c20 7265 7665 7273   x["at"], revers
-0001a1b0: 653d 5472 7565 2920 2023 2074 7970 653a  e=True)  # type:
-0001a1c0: 2069 676e 6f72 650a 2020 2020 2020 2020   ignore.        
-0001a1d0: 2020 2020 2020 2020 2020 2020 7265 7420              ret 
-0001a1e0: 3d20 7265 745b 3a32 3030 305d 0a0a 2020  = ret[:2000]..  
-0001a1f0: 2020 2020 2020 7265 742e 736f 7274 286b        ret.sort(k
-0001a200: 6579 3d6c 616d 6264 6120 783a 2078 5b22  ey=lambda x: x["
-0001a210: 6174 225d 2c20 7265 7665 7273 653d 5472  at"], reverse=Tr
-0001a220: 7565 2920 2023 2074 7970 653a 2069 676e  ue)  # type: ign
-0001a230: 6f72 650a 2020 2020 2020 2020 6e20 3d20  ore.        n = 
-0001a240: 300a 2020 2020 2020 2020 666f 7220 7276  0.        for rv
-0001a250: 2069 6e20 7265 745b 3a31 3130 3030 5d3a   in ret[:11000]:
-0001a260: 0a20 2020 2020 2020 2020 2020 206e 666b  .            nfk
-0001a270: 203d 2072 762e 706f 7028 226e 666b 2229   = rv.pop("nfk")
-0001a280: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001a290: 6e6f 7420 6e66 6b3a 0a20 2020 2020 2020  not nfk:.       
-0001a2a0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0001a2b0: 650a 0a20 2020 2020 2020 2020 2020 2061  e..            a
-0001a2c0: 7020 3d20 7276 2e70 6f70 2822 6170 2229  p = rv.pop("ap")
-0001a2d0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0001a2e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a2f0: 2020 7374 203d 2062 6f73 2e73 7461 7428    st = bos.stat(
-0001a300: 6170 290a 2020 2020 2020 2020 2020 2020  ap).            
-0001a310: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-0001a320: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-0001a330: 0a0a 2020 2020 2020 2020 2020 2020 666b  ..            fk
-0001a340: 203d 2073 656c 662e 6765 6e5f 666b 280a   = self.gen_fk(.
-0001a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a360: 7365 6c66 2e61 7267 732e 666b 5f73 616c  self.args.fk_sal
-0001a370: 742c 2061 702c 2073 742e 7374 5f73 697a  t, ap, st.st_siz
-0001a380: 652c 2030 2069 6620 414e 5957 494e 2065  e, 0 if ANYWIN e
-0001a390: 6c73 6520 7374 2e73 745f 696e 6f0a 2020  lse st.st_ino.  
-0001a3a0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0001a3b0: 2020 2020 2020 2020 7276 5b22 7670 225d          rv["vp"]
-0001a3c0: 202b 3d20 223f 6b3d 2220 2b20 666b 5b3a   += "?k=" + fk[:
-0001a3d0: 6e66 6b5d 0a0a 2020 2020 2020 2020 2020  nfk]..          
-0001a3e0: 2020 6e20 2b3d 2031 0a20 2020 2020 2020    n += 1.       
-0001a3f0: 2020 2020 2069 6620 6e20 3e20 3230 3030       if n > 2000
-0001a400: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a410: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
-0001a420: 2072 6574 203d 2072 6574 5b3a 3230 3030   ret = ret[:2000
-0001a430: 5d0a 0a20 2020 2020 2020 2069 6620 7365  ]..        if se
-0001a440: 6c66 2e69 735f 7670 726f 7869 6564 3a0a  lf.is_vproxied:.
-0001a450: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001a460: 7620 696e 2072 6574 3a0a 2020 2020 2020  v in ret:.      
-0001a470: 2020 2020 2020 2020 2020 765b 2276 7022            v["vp"
-0001a480: 5d20 3d20 7365 6c66 2e61 7267 732e 5352  ] = self.args.SR
-0001a490: 202b 2076 5b22 7670 225d 0a0a 2020 2020   + v["vp"]..    
-0001a4a0: 2020 2020 6a74 7874 203d 206a 736f 6e2e      jtxt = json.
-0001a4b0: 6475 6d70 7328 7265 742c 2069 6e64 656e  dumps(ret, inden
-0001a4c0: 743d 322c 2073 6f72 745f 6b65 7973 3d54  t=2, sort_keys=T
-0001a4d0: 7275 6529 2e65 6e63 6f64 6528 2275 7466  rue).encode("utf
-0001a4e0: 2d38 222c 2022 7265 706c 6163 6522 290a  -8", "replace").
-0001a4f0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-0001a500: 2822 7b7d 2023 7b7d 207b 3a2e 3266 7d73  ("{} #{} {:.2f}s
-0001a510: 6563 222e 666f 726d 6174 286c 6d2c 206c  ec".format(lm, l
-0001a520: 656e 2872 6574 292c 2074 696d 652e 7469  en(ret), time.ti
-0001a530: 6d65 2829 202d 2074 3029 290a 2020 2020  me() - t0)).    
-0001a540: 2020 2020 7365 6c66 2e72 6570 6c79 286a      self.reply(j
-0001a550: 7478 742c 206d 696d 653d 2261 7070 6c69  txt, mime="appli
-0001a560: 6361 7469 6f6e 2f6a 736f 6e22 290a 2020  cation/json").  
-0001a570: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0001a580: 650a 0a20 2020 2064 6566 2068 616e 646c  e..    def handl
-0001a590: 655f 726d 2873 656c 662c 2072 6571 2029  e_rm(self, req )
-0001a5a0: 2020 3a0a 2020 2020 2020 2020 6966 206e    :.        if n
-0001a5b0: 6f74 2072 6571 2061 6e64 206e 6f74 2073  ot req and not s
-0001a5c0: 656c 662e 6361 6e5f 6465 6c65 7465 3a0a  elf.can_delete:.
-0001a5d0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001a5e0: 6520 5065 626b 6163 2834 3033 2c20 226e  e Pebkac(403, "n
-0001a5f0: 6f74 2061 6c6c 6f77 6564 2066 6f72 2075  ot allowed for u
-0001a600: 7365 7220 2220 2b20 7365 6c66 2e75 6e61  ser " + self.una
-0001a610: 6d65 290a 0a20 2020 2020 2020 2069 6620  me)..        if 
-0001a620: 7365 6c66 2e61 7267 732e 6e6f 5f64 656c  self.args.no_del
-0001a630: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-0001a640: 6973 6520 5065 626b 6163 2834 3033 2c20  ise Pebkac(403, 
-0001a650: 2274 6865 2064 656c 6574 6520 6665 6174  "the delete feat
-0001a660: 7572 6520 6973 2064 6973 6162 6c65 6420  ure is disabled 
-0001a670: 696e 2073 6572 7665 7220 636f 6e66 6967  in server config
-0001a680: 2229 0a0a 2020 2020 2020 2020 6966 206e  ")..        if n
-0001a690: 6f74 2072 6571 3a0a 2020 2020 2020 2020  ot req:.        
-0001a6a0: 2020 2020 7265 7120 3d20 5b73 656c 662e      req = [self.
-0001a6b0: 7670 6174 685d 0a20 2020 2020 2020 2065  vpath].        e
-0001a6c0: 6c69 6620 7365 6c66 2e69 735f 7670 726f  lif self.is_vpro
-0001a6d0: 7869 6564 3a0a 2020 2020 2020 2020 2020  xied:.          
-0001a6e0: 2020 7265 7120 3d20 5b78 5b6c 656e 2873    req = [x[len(s
-0001a6f0: 656c 662e 6172 6773 2e53 5229 203a 5d20  elf.args.SR) :] 
-0001a700: 666f 7220 7820 696e 2072 6571 5d0a 0a20  for x in req].. 
-0001a710: 2020 2020 2020 206e 6c69 6d20 3d20 696e         nlim = in
-0001a720: 7428 7365 6c66 2e75 7061 7261 6d2e 6765  t(self.uparam.ge
-0001a730: 7428 226c 696d 2229 206f 7220 3029 0a20  t("lim") or 0). 
-0001a740: 2020 2020 2020 206c 696d 203d 205b 6e6c         lim = [nl
-0001a750: 696d 2c20 6e6c 696d 5d20 6966 206e 6c69  im, nlim] if nli
-0001a760: 6d20 656c 7365 205b 5d0a 0a20 2020 2020  m else []..     
-0001a770: 2020 2078 203d 2073 656c 662e 636f 6e6e     x = self.conn
-0001a780: 2e68 7372 762e 6272 6f6b 6572 2e61 736b  .hsrv.broker.ask
-0001a790: 280a 2020 2020 2020 2020 2020 2020 2275  (.            "u
-0001a7a0: 7032 6b2e 6861 6e64 6c65 5f72 6d22 2c20  p2k.handle_rm", 
-0001a7b0: 7365 6c66 2e75 6e61 6d65 2c20 7365 6c66  self.uname, self
-0001a7c0: 2e69 702c 2072 6571 2c20 6c69 6d2c 2046  .ip, req, lim, F
-0001a7d0: 616c 7365 0a20 2020 2020 2020 2029 0a20  alse.        ). 
-0001a7e0: 2020 2020 2020 2073 656c 662e 6c6f 7564         self.loud
-0001a7f0: 5f72 6570 6c79 2878 2e67 6574 2829 290a  _reply(x.get()).
-0001a800: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0001a810: 7275 650a 0a20 2020 2064 6566 2068 616e  rue..    def han
-0001a820: 646c 655f 6d76 2873 656c 6629 2020 3a0a  dle_mv(self)  :.
-0001a830: 2020 2020 2020 2020 2320 6675 6c6c 2070          # full p
-0001a840: 6174 6820 6f66 206e 6577 206c 6f63 2028  ath of new loc (
-0001a850: 696e 636c 2066 696c 656e 616d 6529 0a20  incl filename). 
-0001a860: 2020 2020 2020 2064 7374 203d 2073 656c         dst = sel
-0001a870: 662e 7570 6172 616d 2e67 6574 2822 6d6f  f.uparam.get("mo
-0001a880: 7665 2229 0a0a 2020 2020 2020 2020 6966  ve")..        if
-0001a890: 2073 656c 662e 6973 5f76 7072 6f78 6965   self.is_vproxie
-0001a8a0: 6420 616e 6420 6473 7420 616e 6420 6473  d and dst and ds
-0001a8b0: 742e 7374 6172 7473 7769 7468 2873 656c  t.startswith(sel
-0001a8c0: 662e 6172 6773 2e53 5229 3a0a 2020 2020  f.args.SR):.    
-0001a8d0: 2020 2020 2020 2020 6473 7420 3d20 6473          dst = ds
-0001a8e0: 745b 6c65 6e28 7365 6c66 2e61 7267 732e  t[len(self.args.
-0001a8f0: 5253 2920 3a5d 0a0a 2020 2020 2020 2020  RS) :]..        
-0001a900: 6966 206e 6f74 2064 7374 3a0a 2020 2020  if not dst:.    
-0001a910: 2020 2020 2020 2020 7261 6973 6520 5065          raise Pe
-0001a920: 626b 6163 2834 3030 2c20 226e 6565 6420  bkac(400, "need 
-0001a930: 6473 7420 7670 6174 6822 290a 0a20 2020  dst vpath")..   
-0001a940: 2020 2020 2023 2078 2d77 7777 2d66 6f72       # x-www-for
-0001a950: 6d2d 7572 6c65 6e63 6f64 6564 2028 7572  m-urlencoded (ur
-0001a960: 6c20 7175 6572 7920 7061 7274 2920 7573  l query part) us
-0001a970: 6573 0a20 2020 2020 2020 2023 2065 6974  es.        # eit
-0001a980: 6865 7220 2b20 6f72 2025 3230 2066 6f72  her + or %20 for
-0001a990: 2030 7832 3020 736f 2068 616e 646c 6520   0x20 so handle 
-0001a9a0: 626f 7468 0a20 2020 2020 2020 2064 7374  both.        dst
-0001a9b0: 203d 2075 6e71 756f 7465 7028 6473 742e   = unquotep(dst.
-0001a9c0: 7265 706c 6163 6528 222b 222c 2022 2022  replace("+", " "
-0001a9d0: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-0001a9e0: 6e20 7365 6c66 2e5f 6d76 2873 656c 662e  n self._mv(self.
-0001a9f0: 7670 6174 682c 2064 7374 2e6c 7374 7269  vpath, dst.lstri
-0001aa00: 7028 222f 2229 290a 0a20 2020 2064 6566  p("/"))..    def
-0001aa10: 205f 6d76 2873 656c 662c 2076 7372 6320   _mv(self, vsrc 
-0001aa20: 2c20 7664 7374 2029 2020 3a0a 2020 2020  , vdst )  :.    
-0001aa30: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0001aa40: 6361 6e5f 6d6f 7665 3a0a 2020 2020 2020  can_move:.      
-0001aa50: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-0001aa60: 6163 2834 3033 2c20 226e 6f74 2061 6c6c  ac(403, "not all
-0001aa70: 6f77 6564 2066 6f72 2075 7365 7220 2220  owed for user " 
-0001aa80: 2b20 7365 6c66 2e75 6e61 6d65 290a 0a20  + self.uname).. 
-0001aa90: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0001aaa0: 7267 732e 6e6f 5f6d 763a 0a20 2020 2020  rgs.no_mv:.     
-0001aab0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-0001aac0: 6b61 6328 3430 332c 2022 7468 6520 7265  kac(403, "the re
-0001aad0: 6e61 6d65 2f6d 6f76 6520 6665 6174 7572  name/move featur
-0001aae0: 6520 6973 2064 6973 6162 6c65 6420 696e  e is disabled in
-0001aaf0: 2073 6572 7665 7220 636f 6e66 6967 2229   server config")
-0001ab00: 0a0a 2020 2020 2020 2020 7820 3d20 7365  ..        x = se
-0001ab10: 6c66 2e63 6f6e 6e2e 6873 7276 2e62 726f  lf.conn.hsrv.bro
-0001ab20: 6b65 722e 6173 6b28 2275 7032 6b2e 6861  ker.ask("up2k.ha
-0001ab30: 6e64 6c65 5f6d 7622 2c20 7365 6c66 2e75  ndle_mv", self.u
-0001ab40: 6e61 6d65 2c20 7673 7263 2c20 7664 7374  name, vsrc, vdst
-0001ab50: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
-0001ab60: 6f75 645f 7265 706c 7928 782e 6765 7428  oud_reply(x.get(
-0001ab70: 292c 2073 7461 7475 733d 3230 3129 0a20  ), status=201). 
-0001ab80: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0001ab90: 7565 0a0a 2020 2020 6465 6620 7478 5f6c  ue..    def tx_l
-0001aba0: 7328 7365 6c66 2c20 6c73 2020 2920 203a  s(self, ls  )  :
-0001abb0: 0a20 2020 2020 2020 2064 6972 7320 3d20  .        dirs = 
-0001abc0: 6c73 5b22 6469 7273 225d 0a20 2020 2020  ls["dirs"].     
-0001abd0: 2020 2066 696c 6573 203d 206c 735b 2266     files = ls["f
-0001abe0: 696c 6573 225d 0a20 2020 2020 2020 2061  iles"].        a
-0001abf0: 7267 203d 2073 656c 662e 7570 6172 616d  rg = self.uparam
-0001ac00: 5b22 6c73 225d 0a20 2020 2020 2020 2069  ["ls"].        i
-0001ac10: 6620 6172 6720 696e 205b 2276 222c 2022  f arg in ["v", "
-0001ac20: 7422 2c20 2274 7874 225d 3a0a 2020 2020  t", "txt"]:.    
-0001ac30: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001ac40: 2020 2020 2020 2020 2020 2020 2062 6967               big
-0001ac50: 6765 7374 203d 206d 6178 286c 735b 2266  gest = max(ls["f
-0001ac60: 696c 6573 225d 202b 206c 735b 2264 6972  iles"] + ls["dir
-0001ac70: 7322 5d2c 206b 6579 3d69 7465 6d67 6574  s"], key=itemget
-0001ac80: 7465 7228 2273 7a22 2929 5b22 737a 225d  ter("sz"))["sz"]
-0001ac90: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0001aca0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-0001acb0: 2020 2020 2062 6967 6765 7374 203d 2030       biggest = 0
-0001acc0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001acd0: 2061 7267 203d 3d20 2276 223a 0a20 2020   arg == "v":.   
-0001ace0: 2020 2020 2020 2020 2020 2020 2066 6d74               fmt
-0001acf0: 203d 2022 5c30 3333 5b30 3b37 3b33 366d   = "\033[0;7;36m
-0001ad00: 7b7b 7d7d 7b7b 3a3e 7b7d 7d7d 5c30 3333  {{}}{{:>{}}}\033
-0001ad10: 5b30 6d20 7b7b 7d7d 220a 2020 2020 2020  [0m {{}}".      
-0001ad20: 2020 2020 2020 2020 2020 6e66 6d74 203d            nfmt =
-0001ad30: 2022 7b7d 220a 2020 2020 2020 2020 2020   "{}".          
-0001ad40: 2020 2020 2020 6269 6767 6573 7420 3d20        biggest = 
-0001ad50: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
-0001ad60: 2020 6632 203d 2022 222e 6a6f 696e 280a    f2 = "".join(.
-0001ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad80: 2020 2020 227b 7d7b 7b7d 7d22 2e66 6f72      "{}{{}}".for
-0001ad90: 6d61 7428 7829 0a20 2020 2020 2020 2020  mat(x).         
-0001ada0: 2020 2020 2020 2020 2020 2066 6f72 2078             for x
-0001adb0: 2069 6e20 5b0a 2020 2020 2020 2020 2020   in [.          
-0001adc0: 2020 2020 2020 2020 2020 2020 2020 225c                "\
-0001add0: 3033 335b 376d 222c 0a20 2020 2020 2020  033[7m",.       
+00018e80: 6c66 2e63 616e 5f61 646d 696e 3a0a 2020  lf.can_admin:.  
+00018e90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00018ea0: 5065 626b 6163 2834 3033 2c20 226e 6f74  Pebkac(403, "not
+00018eb0: 2061 6c6c 6f77 6564 2066 6f72 2075 7365   allowed for use
+00018ec0: 7220 2220 2b20 7365 6c66 2e75 6e61 6d65  r " + self.uname
+00018ed0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+00018ee0: 6c66 2e61 7267 732e 6e6f 5f72 6573 6361  lf.args.no_resca
+00018ef0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
+00018f00: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
+00018f10: 2022 7468 6520 7265 7363 616e 2066 6561   "the rescan fea
+00018f20: 7475 7265 2069 7320 6469 7361 626c 6564  ture is disabled
+00018f30: 2069 6e20 7365 7276 6572 2063 6f6e 6669   in server confi
+00018f40: 6722 290a 0a20 2020 2020 2020 2076 6e2c  g")..        vn,
+00018f50: 205f 203d 2073 656c 662e 6173 7276 2e76   _ = self.asrv.v
+00018f60: 6673 2e67 6574 2873 656c 662e 7670 6174  fs.get(self.vpat
+00018f70: 682c 2073 656c 662e 756e 616d 652c 2054  h, self.uname, T
+00018f80: 7275 652c 2054 7275 6529 0a0a 2020 2020  rue, True)..    
+00018f90: 2020 2020 6172 6773 203d 205b 7365 6c66      args = [self
+00018fa0: 2e61 7372 762e 7666 732e 616c 6c5f 766f  .asrv.vfs.all_vo
+00018fb0: 6c73 2c20 5b76 6e2e 7670 6174 685d 2c20  ls, [vn.vpath], 
+00018fc0: 4661 6c73 652c 2054 7275 655d 0a0a 2020  False, True]..  
+00018fd0: 2020 2020 2020 7820 3d20 7365 6c66 2e63        x = self.c
+00018fe0: 6f6e 6e2e 6873 7276 2e62 726f 6b65 722e  onn.hsrv.broker.
+00018ff0: 6173 6b28 2275 7032 6b2e 7265 7363 616e  ask("up2k.rescan
+00019000: 222c 202a 6172 6773 290a 2020 2020 2020  ", *args).      
+00019010: 2020 6572 7220 3d20 782e 6765 7428 290a    err = x.get().
+00019020: 2020 2020 2020 2020 6966 206e 6f74 2065          if not e
+00019030: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
+00019040: 7365 6c66 2e72 6564 6972 6563 7428 2222  self.redirect(""
+00019050: 2c20 223f 6822 290a 2020 2020 2020 2020  , "?h").        
+00019060: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00019070: 0a20 2020 2020 2020 2072 6169 7365 2050  .        raise P
+00019080: 6562 6b61 6328 3530 302c 2065 7272 290a  ebkac(500, err).
+00019090: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
+000190a0: 7265 6c6f 6164 2873 656c 6629 2020 3a0a  reload(self)  :.
+000190b0: 2020 2020 2020 2020 6163 7420 3d20 7365          act = se
+000190c0: 6c66 2e75 7061 7261 6d2e 6765 7428 2272  lf.uparam.get("r
+000190d0: 656c 6f61 6422 290a 2020 2020 2020 2020  eload").        
+000190e0: 6966 2061 6374 2021 3d20 2263 6667 223a  if act != "cfg":
+000190f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00019100: 7365 2050 6562 6b61 6328 3430 302c 2022  se Pebkac(400, "
+00019110: 6f6e 6c79 2063 6f6e 6669 6720 6669 6c65  only config file
+00019120: 7320 2827 6366 6727 2920 6361 6e20 6265  s ('cfg') can be
+00019130: 2072 656c 6f61 6465 6420 726e 2229 0a0a   reloaded rn")..
+00019140: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00019150: 656c 662e 6176 6f6c 3a0a 2020 2020 2020  elf.avol:.      
+00019160: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
+00019170: 6163 2834 3033 2c20 226e 6f74 2061 6c6c  ac(403, "not all
+00019180: 6f77 6564 2066 6f72 2075 7365 7220 2220  owed for user " 
+00019190: 2b20 7365 6c66 2e75 6e61 6d65 290a 0a20  + self.uname).. 
+000191a0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
+000191b0: 7267 732e 6e6f 5f72 656c 6f61 643a 0a20  rgs.no_reload:. 
+000191c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+000191d0: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
+000191e0: 6520 7265 6c6f 6164 2066 6561 7475 7265  e reload feature
+000191f0: 2069 7320 6469 7361 626c 6564 2069 6e20   is disabled in 
+00019200: 7365 7276 6572 2063 6f6e 6669 6722 290a  server config").
+00019210: 0a20 2020 2020 2020 2078 203d 2073 656c  .        x = sel
+00019220: 662e 636f 6e6e 2e68 7372 762e 6272 6f6b  f.conn.hsrv.brok
+00019230: 6572 2e61 736b 2822 7265 6c6f 6164 2229  er.ask("reload")
+00019240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019250: 7365 6c66 2e72 6564 6972 6563 7428 2222  self.redirect(""
+00019260: 2c20 223f 6822 2c20 782e 6765 7428 292c  , "?h", x.get(),
+00019270: 2022 7265 7475 726e 2074 6f22 2c20 4661   "return to", Fa
+00019280: 6c73 6529 0a0a 2020 2020 6465 6620 7478  lse)..    def tx
+00019290: 5f73 7461 636b 2873 656c 6629 2020 3a0a  _stack(self)  :.
+000192a0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+000192b0: 656c 662e 6176 6f6c 2061 6e64 206e 6f74  elf.avol and not
+000192c0: 205b 7820 666f 7220 7820 696e 2073 656c   [x for x in sel
+000192d0: 662e 7776 6f6c 2069 6620 7820 696e 2073  f.wvol if x in s
+000192e0: 656c 662e 7276 6f6c 5d3a 0a20 2020 2020  elf.rvol]:.     
+000192f0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+00019300: 6b61 6328 3430 332c 2022 6e6f 7420 616c  kac(403, "not al
+00019310: 6c6f 7765 6420 666f 7220 7573 6572 2022  lowed for user "
+00019320: 202b 2073 656c 662e 756e 616d 6529 0a0a   + self.uname)..
+00019330: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00019340: 6172 6773 2e6e 6f5f 7374 6163 6b3a 0a20  args.no_stack:. 
+00019350: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00019360: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
+00019370: 6520 7374 6163 6b64 756d 7020 6665 6174  e stackdump feat
+00019380: 7572 6520 6973 2064 6973 6162 6c65 6420  ure is disabled 
+00019390: 696e 2073 6572 7665 7220 636f 6e66 6967  in server config
+000193a0: 2229 0a0a 2020 2020 2020 2020 7265 7420  ")..        ret 
+000193b0: 3d20 223c 7072 653e 7b7d 5c6e 7b7d 222e  = "<pre>{}\n{}".
+000193c0: 666f 726d 6174 2874 696d 652e 7469 6d65  format(time.time
+000193d0: 2829 2c20 6874 6d6c 5f65 7363 6170 6528  (), html_escape(
+000193e0: 616c 6c74 7261 6365 2829 2929 0a20 2020  alltrace())).   
+000193f0: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
+00019400: 7265 742e 656e 636f 6465 2822 7574 662d  ret.encode("utf-
+00019410: 3822 2929 0a20 2020 2020 2020 2072 6574  8")).        ret
+00019420: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+00019430: 6620 7478 5f74 7265 6528 7365 6c66 2920  f tx_tree(self) 
+00019440: 203a 0a20 2020 2020 2020 2074 6f70 203d   :.        top =
+00019450: 2073 656c 662e 7570 6172 616d 5b22 7472   self.uparam["tr
+00019460: 6565 225d 206f 7220 2222 0a20 2020 2020  ee"] or "".     
+00019470: 2020 2064 7374 203d 2073 656c 662e 7670     dst = self.vp
+00019480: 6174 680a 2020 2020 2020 2020 6966 2074  ath.        if t
+00019490: 6f70 2069 6e20 5b22 2e22 2c20 222e 2e22  op in [".", ".."
+000194a0: 5d3a 0a20 2020 2020 2020 2020 2020 2074  ]:.            t
+000194b0: 6f70 203d 2075 6e64 6f74 2873 656c 662e  op = undot(self.
+000194c0: 7670 6174 6820 2b20 222f 2220 2b20 746f  vpath + "/" + to
+000194d0: 7029 0a0a 2020 2020 2020 2020 6966 2074  p)..        if t
+000194e0: 6f70 203d 3d20 6473 743a 0a20 2020 2020  op == dst:.     
+000194f0: 2020 2020 2020 2064 7374 203d 2022 220a         dst = "".
+00019500: 2020 2020 2020 2020 656c 6966 2074 6f70          elif top
+00019510: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00019520: 206e 6f74 2064 7374 2e73 7461 7274 7377   not dst.startsw
+00019530: 6974 6828 746f 7020 2b20 222f 2229 3a0a  ith(top + "/"):.
+00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019550: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
+00019560: 2c20 2261 7267 2066 756e 6b22 290a 0a20  , "arg funk").. 
+00019570: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
+00019580: 2064 7374 5b6c 656e 2874 6f70 2920 2b20   dst[len(top) + 
+00019590: 3120 3a5d 0a0a 2020 2020 2020 2020 7265  1 :]..        re
+000195a0: 7420 3d20 7365 6c66 2e67 656e 5f74 7265  t = self.gen_tre
+000195b0: 6528 746f 702c 2064 7374 290a 2020 2020  e(top, dst).    
+000195c0: 2020 2020 6966 2073 656c 662e 6973 5f76      if self.is_v
+000195d0: 7072 6f78 6965 643a 0a20 2020 2020 2020  proxied:.       
+000195e0: 2020 2020 2070 6172 656e 7473 203d 2073       parents = s
+000195f0: 656c 662e 6172 6773 2e52 2e73 706c 6974  elf.args.R.split
+00019600: 2822 2f22 290a 2020 2020 2020 2020 2020  ("/").          
+00019610: 2020 666f 7220 7061 7265 6e74 2069 6e20    for parent in 
+00019620: 7265 7665 7273 6564 2870 6172 656e 7473  reversed(parents
+00019630: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00019640: 2020 2072 6574 203d 207b 226b 2573 2220     ret = {"k%s" 
+00019650: 2520 2870 6172 656e 742c 293a 2072 6574  % (parent,): ret
+00019660: 2c20 2261 223a 205b 5d7d 0a0a 2020 2020  , "a": []}..    
+00019670: 2020 2020 7a73 203d 206a 736f 6e2e 6475      zs = json.du
+00019680: 6d70 7328 7265 7429 0a20 2020 2020 2020  mps(ret).       
+00019690: 2073 656c 662e 7265 706c 7928 7a73 2e65   self.reply(zs.e
+000196a0: 6e63 6f64 6528 2275 7466 2d38 2229 2c20  ncode("utf-8"), 
+000196b0: 6d69 6d65 3d22 6170 706c 6963 6174 696f  mime="applicatio
+000196c0: 6e2f 6a73 6f6e 2229 0a20 2020 2020 2020  n/json").       
+000196d0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+000196e0: 2020 6465 6620 6765 6e5f 7472 6565 2873    def gen_tree(s
+000196f0: 656c 662c 2074 6f70 202c 2074 6172 6765  elf, top , targe
+00019700: 7420 2920 2020 3a0a 2020 2020 2020 2020  t )   :.        
+00019710: 7265 7420 2020 3d20 7b7d 0a20 2020 2020  ret   = {}.     
+00019720: 2020 2065 7863 6c20 3d20 4e6f 6e65 0a20     excl = None. 
+00019730: 2020 2020 2020 2069 6620 7461 7267 6574         if target
+00019740: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
+00019750: 636c 2c20 7461 7267 6574 203d 2028 7461  cl, target = (ta
+00019760: 7267 6574 2e73 706c 6974 2822 2f22 2c20  rget.split("/", 
+00019770: 3129 202b 205b 2222 5d29 5b3a 325d 0a20  1) + [""])[:2]. 
+00019780: 2020 2020 2020 2020 2020 2073 7562 203d             sub =
+00019790: 2073 656c 662e 6765 6e5f 7472 6565 2822   self.gen_tree("
+000197a0: 2f22 2e6a 6f69 6e28 5b74 6f70 2c20 6578  /".join([top, ex
+000197b0: 636c 5d29 2e73 7472 6970 2822 2f22 292c  cl]).strip("/"),
+000197c0: 2074 6172 6765 7429 0a20 2020 2020 2020   target).       
+000197d0: 2020 2020 2072 6574 5b22 6b22 202b 2071       ret["k" + q
+000197e0: 756f 7465 7028 6578 636c 295d 203d 2073  uotep(excl)] = s
+000197f0: 7562 0a0a 2020 2020 2020 2020 7472 793a  ub..        try:
+00019800: 0a20 2020 2020 2020 2020 2020 2076 6e2c  .            vn,
+00019810: 2072 656d 203d 2073 656c 662e 6173 7276   rem = self.asrv
+00019820: 2e76 6673 2e67 6574 2874 6f70 2c20 7365  .vfs.get(top, se
+00019830: 6c66 2e75 6e61 6d65 2c20 5472 7565 2c20  lf.uname, True, 
+00019840: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00019850: 2020 2066 7372 6f6f 742c 2076 6673 5f6c     fsroot, vfs_l
+00019860: 732c 2076 6673 5f76 6972 7420 3d20 766e  s, vfs_virt = vn
+00019870: 2e6c 7328 0a20 2020 2020 2020 2020 2020  .ls(.           
+00019880: 2020 2020 2072 656d 2c0a 2020 2020 2020       rem,.      
+00019890: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+000198a0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+000198b0: 2020 2020 2020 6e6f 7420 7365 6c66 2e61        not self.a
+000198c0: 7267 732e 6e6f 5f73 6361 6e64 6972 2c0a  rgs.no_scandir,.
+000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198e0: 5b5b 5472 7565 2c20 4661 6c73 655d 2c20  [[True, False], 
+000198f0: 5b46 616c 7365 2c20 5472 7565 5d5d 2c0a  [False, True]],.
+00019900: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00019910: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00019920: 2020 2020 2020 2020 2020 7666 735f 6c73            vfs_ls
+00019930: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00019940: 2020 7666 735f 7669 7274 203d 207b 7d0a    vfs_virt = {}.
+00019950: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00019960: 7620 696e 2073 656c 662e 7276 6f6c 3a0a  v in self.rvol:.
+00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019980: 6431 2c20 6432 203d 2076 2e72 7370 6c69  d1, d2 = v.rspli
+00019990: 7428 222f 222c 2031 2920 6966 2022 2f22  t("/", 1) if "/"
+000199a0: 2069 6e20 7620 656c 7365 205b 2222 2c20   in v else ["", 
+000199b0: 765d 0a20 2020 2020 2020 2020 2020 2020  v].             
+000199c0: 2020 2069 6620 6431 203d 3d20 746f 703a     if d1 == top:
+000199d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000199e0: 2020 2020 2076 6673 5f76 6972 745b 6432       vfs_virt[d2
+000199f0: 5d20 3d20 7365 6c66 2e61 7372 762e 7666  ] = self.asrv.vf
+00019a00: 7320 2023 2074 7970 6563 686b 2c20 7661  s  # typechk, va
+00019a10: 6c75 6520 6e65 7665 7220 7265 6164 0a0a  lue never read..
+00019a20: 2020 2020 2020 2020 6469 7273 203d 205b          dirs = [
+00019a30: 5d0a 0a20 2020 2020 2020 2064 6972 6e61  ]..        dirna
+00019a40: 6d65 7320 3d20 5b78 5b30 5d20 666f 7220  mes = [x[0] for 
+00019a50: 7820 696e 2076 6673 5f6c 7320 6966 2073  x in vfs_ls if s
+00019a60: 7461 742e 535f 4953 4449 5228 785b 315d  tat.S_ISDIR(x[1]
+00019a70: 2e73 745f 6d6f 6465 295d 0a0a 2020 2020  .st_mode)]..    
+00019a80: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00019a90: 6172 6773 2e65 6420 6f72 2022 646f 7473  args.ed or "dots
+00019aa0: 2220 6e6f 7420 696e 2073 656c 662e 7570  " not in self.up
+00019ab0: 6172 616d 3a0a 2020 2020 2020 2020 2020  aram:.          
+00019ac0: 2020 6469 726e 616d 6573 203d 2065 7863    dirnames = exc
+00019ad0: 6c75 6465 5f64 6f74 6669 6c65 7328 6469  lude_dotfiles(di
+00019ae0: 726e 616d 6573 290a 0a20 2020 2020 2020  rnames)..       
+00019af0: 2066 6f72 2066 6e20 696e 205b 7820 666f   for fn in [x fo
+00019b00: 7220 7820 696e 2064 6972 6e61 6d65 7320  r x in dirnames 
+00019b10: 6966 2078 2021 3d20 6578 636c 5d3a 0a20  if x != excl]:. 
+00019b20: 2020 2020 2020 2020 2020 2064 6972 732e             dirs.
+00019b30: 6170 7065 6e64 2871 756f 7465 7028 666e  append(quotep(fn
+00019b40: 2929 0a0a 2020 2020 2020 2020 666f 7220  ))..        for 
+00019b50: 7820 696e 2076 6673 5f76 6972 743a 0a20  x in vfs_virt:. 
+00019b60: 2020 2020 2020 2020 2020 2069 6620 7820             if x 
+00019b70: 213d 2065 7863 6c3a 0a20 2020 2020 2020  != excl:.       
+00019b80: 2020 2020 2020 2020 2064 6972 732e 6170           dirs.ap
+00019b90: 7065 6e64 2878 290a 0a20 2020 2020 2020  pend(x)..       
+00019ba0: 2072 6574 5b22 6122 5d20 3d20 6469 7273   ret["a"] = dirs
+00019bb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00019bc0: 7265 740a 0a20 2020 2064 6566 2074 785f  ret..    def tx_
+00019bd0: 7570 7328 7365 6c66 2920 203a 0a20 2020  ups(self)  :.   
+00019be0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00019bf0: 2e61 7267 732e 756e 706f 7374 3a0a 2020  .args.unpost:.  
+00019c00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00019c10: 5065 626b 6163 2834 3033 2c20 2274 6865  Pebkac(403, "the
+00019c20: 2075 6e70 6f73 7420 6665 6174 7572 6520   unpost feature 
+00019c30: 6973 2064 6973 6162 6c65 6420 696e 2073  is disabled in s
+00019c40: 6572 7665 7220 636f 6e66 6967 2229 0a0a  erver config")..
+00019c50: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
+00019c60: 6c66 2e63 6f6e 6e2e 6765 745f 7532 6964  lf.conn.get_u2id
+00019c70: 7828 290a 2020 2020 2020 2020 6966 206e  x().        if n
+00019c80: 6f74 2069 6478 206f 7220 6e6f 7420 6861  ot idx or not ha
+00019c90: 7361 7474 7228 6964 782c 2022 705f 656e  sattr(idx, "p_en
+00019ca0: 6422 293a 0a20 2020 2020 2020 2020 2020  d"):.           
+00019cb0: 2072 6169 7365 2050 6562 6b61 6328 3530   raise Pebkac(50
+00019cc0: 302c 2022 7371 6c69 7465 3320 6973 206e  0, "sqlite3 is n
+00019cd0: 6f74 2061 7661 696c 6162 6c65 206f 6e20  ot available on 
+00019ce0: 7468 6520 7365 7276 6572 3b20 6361 6e6e  the server; cann
+00019cf0: 6f74 2075 6e70 6f73 7422 290a 0a20 2020  ot unpost")..   
+00019d00: 2020 2020 2066 696c 7420 3d20 7365 6c66       filt = self
+00019d10: 2e75 7061 7261 6d2e 6765 7428 2266 696c  .uparam.get("fil
+00019d20: 7465 7222 290a 2020 2020 2020 2020 6669  ter").        fi
+00019d30: 6c74 203d 2075 6e71 756f 7465 7028 6669  lt = unquotep(fi
+00019d40: 6c74 206f 7220 2222 290a 2020 2020 2020  lt or "").      
+00019d50: 2020 6c6d 203d 2022 7570 7320 5b7b 7d5d    lm = "ups [{}]
+00019d60: 222e 666f 726d 6174 2866 696c 7429 0a20  ".format(filt). 
+00019d70: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+00019d80: 6c6d 290a 0a20 2020 2020 2020 2072 6574  lm)..        ret
+00019d90: 2020 203d 205b 5d0a 2020 2020 2020 2020     = [].        
+00019da0: 7430 203d 2074 696d 652e 7469 6d65 2829  t0 = time.time()
+00019db0: 0a20 2020 2020 2020 206c 696d 203d 2074  .        lim = t
+00019dc0: 696d 652e 7469 6d65 2829 202d 2073 656c  ime.time() - sel
+00019dd0: 662e 6172 6773 2e75 6e70 6f73 740a 2020  f.args.unpost.  
+00019de0: 2020 2020 2020 666b 5f76 6f6c 7320 3d20        fk_vols = 
+00019df0: 7b0a 2020 2020 2020 2020 2020 2020 766f  {.            vo
+00019e00: 6c3a 2076 6f6c 2e66 6c61 6773 5b22 666b  l: vol.flags["fk
+00019e10: 225d 0a20 2020 2020 2020 2020 2020 2066  "].            f
+00019e20: 6f72 2076 702c 2076 6f6c 2069 6e20 7365  or vp, vol in se
+00019e30: 6c66 2e61 7372 762e 7666 732e 616c 6c5f  lf.asrv.vfs.all_
+00019e40: 766f 6c73 2e69 7465 6d73 2829 0a20 2020  vols.items().   
+00019e50: 2020 2020 2020 2020 2069 6620 2266 6b22           if "fk"
+00019e60: 2069 6e20 766f 6c2e 666c 6167 7320 616e   in vol.flags an
+00019e70: 6420 2876 7020 696e 2073 656c 662e 7276  d (vp in self.rv
+00019e80: 6f6c 206f 7220 7670 2069 6e20 7365 6c66  ol or vp in self
+00019e90: 2e75 7076 6f6c 290a 2020 2020 2020 2020  .upvol).        
+00019ea0: 7d0a 2020 2020 2020 2020 666f 7220 766f  }.        for vo
+00019eb0: 6c20 696e 2073 656c 662e 6173 7276 2e76  l in self.asrv.v
+00019ec0: 6673 2e61 6c6c 5f76 6f6c 732e 7661 6c75  fs.all_vols.valu
+00019ed0: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
+00019ee0: 2020 6375 7220 3d20 6964 782e 6765 745f    cur = idx.get_
+00019ef0: 6375 7228 766f 6c2e 7265 616c 7061 7468  cur(vol.realpath
+00019f00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00019f10: 206e 6f74 2063 7572 3a0a 2020 2020 2020   not cur:.      
+00019f20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+00019f30: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00019f40: 6e66 6b20 3d20 666b 5f76 6f6c 732e 6765  nfk = fk_vols.ge
+00019f50: 7428 766f 6c2c 2030 290a 0a20 2020 2020  t(vol, 0)..     
+00019f60: 2020 2020 2020 2071 203d 2022 7365 6c65         q = "sele
+00019f70: 6374 2073 7a2c 2072 642c 2066 6e2c 2061  ct sz, rd, fn, a
+00019f80: 7420 6672 6f6d 2075 7020 7768 6572 6520  t from up where 
+00019f90: 6970 3d3f 2061 6e64 2061 743e 3f22 0a20  ip=? and at>?". 
+00019fa0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
+00019fb0: 7a2c 2072 642c 2066 6e2c 2061 7420 696e  z, rd, fn, at in
+00019fc0: 2063 7572 2e65 7865 6375 7465 2871 2c20   cur.execute(q, 
+00019fd0: 2873 656c 662e 6970 2c20 6c69 6d29 293a  (self.ip, lim)):
+00019fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019ff0: 2076 7020 3d20 222f 2220 2b20 222f 222e   vp = "/" + "/".
+0001a000: 6a6f 696e 2878 2066 6f72 2078 2069 6e20  join(x for x in 
+0001a010: 5b76 6f6c 2e76 7061 7468 2c20 7264 2c20  [vol.vpath, rd, 
+0001a020: 666e 5d20 6966 2078 290a 2020 2020 2020  fn] if x).      
+0001a030: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
+0001a040: 7420 616e 6420 6669 6c74 206e 6f74 2069  t and filt not i
+0001a050: 6e20 7670 3a0a 2020 2020 2020 2020 2020  n vp:.          
+0001a060: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0001a070: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+0001a080: 2020 2020 7276 203d 207b 2276 7022 3a20      rv = {"vp": 
+0001a090: 7175 6f74 6570 2876 7029 2c20 2273 7a22  quotep(vp), "sz"
+0001a0a0: 3a20 737a 2c20 2261 7422 3a20 6174 2c20  : sz, "at": at, 
+0001a0b0: 226e 666b 223a 206e 666b 7d0a 2020 2020  "nfk": nfk}.    
+0001a0c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001a0d0: 666b 3a0a 2020 2020 2020 2020 2020 2020  fk:.            
+0001a0e0: 2020 2020 2020 2020 7276 5b22 6170 225d          rv["ap"]
+0001a0f0: 203d 2076 6f6c 2e63 616e 6f6e 6963 616c   = vol.canonical
+0001a100: 2876 6a6f 696e 2872 642c 2066 6e29 290a  (vjoin(rd, fn)).
+0001a110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a120: 2072 6574 2e61 7070 656e 6428 7276 290a   ret.append(rv).
+0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a140: 6966 206c 656e 2872 6574 2920 3e20 3330  if len(ret) > 30
+0001a150: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
+0001a160: 2020 2020 2020 2020 7265 742e 736f 7274          ret.sort
+0001a170: 286b 6579 3d6c 616d 6264 6120 783a 2078  (key=lambda x: x
+0001a180: 5b22 6174 225d 2c20 7265 7665 7273 653d  ["at"], reverse=
+0001a190: 5472 7565 2920 2023 2074 7970 653a 2069  True)  # type: i
+0001a1a0: 676e 6f72 650a 2020 2020 2020 2020 2020  gnore.          
+0001a1b0: 2020 2020 2020 2020 2020 7265 7420 3d20            ret = 
+0001a1c0: 7265 745b 3a32 3030 305d 0a0a 2020 2020  ret[:2000]..    
+0001a1d0: 2020 2020 7265 742e 736f 7274 286b 6579      ret.sort(key
+0001a1e0: 3d6c 616d 6264 6120 783a 2078 5b22 6174  =lambda x: x["at
+0001a1f0: 225d 2c20 7265 7665 7273 653d 5472 7565  "], reverse=True
+0001a200: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
+0001a210: 650a 2020 2020 2020 2020 6e20 3d20 300a  e.        n = 0.
+0001a220: 2020 2020 2020 2020 666f 7220 7276 2069          for rv i
+0001a230: 6e20 7265 745b 3a31 3130 3030 5d3a 0a20  n ret[:11000]:. 
+0001a240: 2020 2020 2020 2020 2020 206e 666b 203d             nfk =
+0001a250: 2072 762e 706f 7028 226e 666b 2229 0a20   rv.pop("nfk"). 
+0001a260: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001a270: 7420 6e66 6b3a 0a20 2020 2020 2020 2020  t nfk:.         
+0001a280: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0001a290: 0a20 2020 2020 2020 2020 2020 2061 7020  .            ap 
+0001a2a0: 3d20 7276 2e70 6f70 2822 6170 2229 0a20  = rv.pop("ap"). 
+0001a2b0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0001a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2d0: 7374 203d 2062 6f73 2e73 7461 7428 6170  st = bos.stat(ap
+0001a2e0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0001a2f0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0001a300: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
+0001a310: 2020 2020 2020 2020 2020 2020 666b 203d              fk =
+0001a320: 2073 656c 662e 6765 6e5f 666b 280a 2020   self.gen_fk(.  
+0001a330: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a340: 6c66 2e61 7267 732e 666b 5f73 616c 742c  lf.args.fk_salt,
+0001a350: 2061 702c 2073 742e 7374 5f73 697a 652c   ap, st.st_size,
+0001a360: 2030 2069 6620 414e 5957 494e 2065 6c73   0 if ANYWIN els
+0001a370: 6520 7374 2e73 745f 696e 6f0a 2020 2020  e st.st_ino.    
+0001a380: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0001a390: 2020 2020 2020 7276 5b22 7670 225d 202b        rv["vp"] +
+0001a3a0: 3d20 223f 6b3d 2220 2b20 666b 5b3a 6e66  = "?k=" + fk[:nf
+0001a3b0: 6b5d 0a0a 2020 2020 2020 2020 2020 2020  k]..            
+0001a3c0: 6e20 2b3d 2031 0a20 2020 2020 2020 2020  n += 1.         
+0001a3d0: 2020 2069 6620 6e20 3e20 3230 3030 3a0a     if n > 2000:.
+0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a3f0: 6272 6561 6b0a 0a20 2020 2020 2020 2072  break..        r
+0001a400: 6574 203d 2072 6574 5b3a 3230 3030 5d0a  et = ret[:2000].
+0001a410: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001a420: 2e69 735f 7670 726f 7869 6564 3a0a 2020  .is_vproxied:.  
+0001a430: 2020 2020 2020 2020 2020 666f 7220 7620            for v 
+0001a440: 696e 2072 6574 3a0a 2020 2020 2020 2020  in ret:.        
+0001a450: 2020 2020 2020 2020 765b 2276 7022 5d20          v["vp"] 
+0001a460: 3d20 7365 6c66 2e61 7267 732e 5352 202b  = self.args.SR +
+0001a470: 2076 5b22 7670 225d 0a0a 2020 2020 2020   v["vp"]..      
+0001a480: 2020 6a74 7874 203d 206a 736f 6e2e 6475    jtxt = json.du
+0001a490: 6d70 7328 7265 742c 2069 6e64 656e 743d  mps(ret, indent=
+0001a4a0: 322c 2073 6f72 745f 6b65 7973 3d54 7275  2, sort_keys=Tru
+0001a4b0: 6529 2e65 6e63 6f64 6528 2275 7466 2d38  e).encode("utf-8
+0001a4c0: 222c 2022 7265 706c 6163 6522 290a 2020  ", "replace").  
+0001a4d0: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
+0001a4e0: 7b7d 2023 7b7d 207b 3a2e 3266 7d73 6563  {} #{} {:.2f}sec
+0001a4f0: 222e 666f 726d 6174 286c 6d2c 206c 656e  ".format(lm, len
+0001a500: 2872 6574 292c 2074 696d 652e 7469 6d65  (ret), time.time
+0001a510: 2829 202d 2074 3029 290a 2020 2020 2020  () - t0)).      
+0001a520: 2020 7365 6c66 2e72 6570 6c79 286a 7478    self.reply(jtx
+0001a530: 742c 206d 696d 653d 2261 7070 6c69 6361  t, mime="applica
+0001a540: 7469 6f6e 2f6a 736f 6e22 290a 2020 2020  tion/json").    
+0001a550: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0001a560: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
+0001a570: 726d 2873 656c 662c 2072 6571 2029 2020  rm(self, req )  
+0001a580: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+0001a590: 2072 6571 2061 6e64 206e 6f74 2073 656c   req and not sel
+0001a5a0: 662e 6361 6e5f 6465 6c65 7465 3a0a 2020  f.can_delete:.  
+0001a5b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001a5c0: 5065 626b 6163 2834 3033 2c20 226e 6f74  Pebkac(403, "not
+0001a5d0: 2061 6c6c 6f77 6564 2066 6f72 2075 7365   allowed for use
+0001a5e0: 7220 2220 2b20 7365 6c66 2e75 6e61 6d65  r " + self.uname
+0001a5f0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
+0001a600: 6c66 2e61 7267 732e 6e6f 5f64 656c 3a0a  lf.args.no_del:.
+0001a610: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001a620: 6520 5065 626b 6163 2834 3033 2c20 2274  e Pebkac(403, "t
+0001a630: 6865 2064 656c 6574 6520 6665 6174 7572  he delete featur
+0001a640: 6520 6973 2064 6973 6162 6c65 6420 696e  e is disabled in
+0001a650: 2073 6572 7665 7220 636f 6e66 6967 2229   server config")
+0001a660: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+0001a670: 2072 6571 3a0a 2020 2020 2020 2020 2020   req:.          
+0001a680: 2020 7265 7120 3d20 5b73 656c 662e 7670    req = [self.vp
+0001a690: 6174 685d 0a20 2020 2020 2020 2065 6c69  ath].        eli
+0001a6a0: 6620 7365 6c66 2e69 735f 7670 726f 7869  f self.is_vproxi
+0001a6b0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+0001a6c0: 7265 7120 3d20 5b78 5b6c 656e 2873 656c  req = [x[len(sel
+0001a6d0: 662e 6172 6773 2e53 5229 203a 5d20 666f  f.args.SR) :] fo
+0001a6e0: 7220 7820 696e 2072 6571 5d0a 0a20 2020  r x in req]..   
+0001a6f0: 2020 2020 206e 6c69 6d20 3d20 696e 7428       nlim = int(
+0001a700: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
+0001a710: 226c 696d 2229 206f 7220 3029 0a20 2020  "lim") or 0).   
+0001a720: 2020 2020 206c 696d 203d 205b 6e6c 696d       lim = [nlim
+0001a730: 2c20 6e6c 696d 5d20 6966 206e 6c69 6d20  , nlim] if nlim 
+0001a740: 656c 7365 205b 5d0a 0a20 2020 2020 2020  else []..       
+0001a750: 2078 203d 2073 656c 662e 636f 6e6e 2e68   x = self.conn.h
+0001a760: 7372 762e 6272 6f6b 6572 2e61 736b 280a  srv.broker.ask(.
+0001a770: 2020 2020 2020 2020 2020 2020 2275 7032              "up2
+0001a780: 6b2e 6861 6e64 6c65 5f72 6d22 2c20 7365  k.handle_rm", se
+0001a790: 6c66 2e75 6e61 6d65 2c20 7365 6c66 2e69  lf.uname, self.i
+0001a7a0: 702c 2072 6571 2c20 6c69 6d2c 2046 616c  p, req, lim, Fal
+0001a7b0: 7365 0a20 2020 2020 2020 2029 0a20 2020  se.        ).   
+0001a7c0: 2020 2020 2073 656c 662e 6c6f 7564 5f72       self.loud_r
+0001a7d0: 6570 6c79 2878 2e67 6574 2829 290a 2020  eply(x.get()).  
+0001a7e0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0001a7f0: 650a 0a20 2020 2064 6566 2068 616e 646c  e..    def handl
+0001a800: 655f 6d76 2873 656c 6629 2020 3a0a 2020  e_mv(self)  :.  
+0001a810: 2020 2020 2020 2320 6675 6c6c 2070 6174        # full pat
+0001a820: 6820 6f66 206e 6577 206c 6f63 2028 696e  h of new loc (in
+0001a830: 636c 2066 696c 656e 616d 6529 0a20 2020  cl filename).   
+0001a840: 2020 2020 2064 7374 203d 2073 656c 662e       dst = self.
+0001a850: 7570 6172 616d 2e67 6574 2822 6d6f 7665  uparam.get("move
+0001a860: 2229 0a0a 2020 2020 2020 2020 6966 2073  ")..        if s
+0001a870: 656c 662e 6973 5f76 7072 6f78 6965 6420  elf.is_vproxied 
+0001a880: 616e 6420 6473 7420 616e 6420 6473 742e  and dst and dst.
+0001a890: 7374 6172 7473 7769 7468 2873 656c 662e  startswith(self.
+0001a8a0: 6172 6773 2e53 5229 3a0a 2020 2020 2020  args.SR):.      
+0001a8b0: 2020 2020 2020 6473 7420 3d20 6473 745b        dst = dst[
+0001a8c0: 6c65 6e28 7365 6c66 2e61 7267 732e 5253  len(self.args.RS
+0001a8d0: 2920 3a5d 0a0a 2020 2020 2020 2020 6966  ) :]..        if
+0001a8e0: 206e 6f74 2064 7374 3a0a 2020 2020 2020   not dst:.      
+0001a8f0: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
+0001a900: 6163 2834 3030 2c20 226e 6565 6420 6473  ac(400, "need ds
+0001a910: 7420 7670 6174 6822 290a 0a20 2020 2020  t vpath")..     
+0001a920: 2020 2023 2078 2d77 7777 2d66 6f72 6d2d     # x-www-form-
+0001a930: 7572 6c65 6e63 6f64 6564 2028 7572 6c20  urlencoded (url 
+0001a940: 7175 6572 7920 7061 7274 2920 7573 6573  query part) uses
+0001a950: 0a20 2020 2020 2020 2023 2065 6974 6865  .        # eithe
+0001a960: 7220 2b20 6f72 2025 3230 2066 6f72 2030  r + or %20 for 0
+0001a970: 7832 3020 736f 2068 616e 646c 6520 626f  x20 so handle bo
+0001a980: 7468 0a20 2020 2020 2020 2064 7374 203d  th.        dst =
+0001a990: 2075 6e71 756f 7465 7028 6473 742e 7265   unquotep(dst.re
+0001a9a0: 706c 6163 6528 222b 222c 2022 2022 2929  place("+", " "))
+0001a9b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a9c0: 7365 6c66 2e5f 6d76 2873 656c 662e 7670  self._mv(self.vp
+0001a9d0: 6174 682c 2064 7374 2e6c 7374 7269 7028  ath, dst.lstrip(
+0001a9e0: 222f 2229 290a 0a20 2020 2064 6566 205f  "/"))..    def _
+0001a9f0: 6d76 2873 656c 662c 2076 7372 6320 2c20  mv(self, vsrc , 
+0001aa00: 7664 7374 2029 2020 3a0a 2020 2020 2020  vdst )  :.      
+0001aa10: 2020 6966 206e 6f74 2073 656c 662e 6361    if not self.ca
+0001aa20: 6e5f 6d6f 7665 3a0a 2020 2020 2020 2020  n_move:.        
+0001aa30: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
+0001aa40: 2834 3033 2c20 226e 6f74 2061 6c6c 6f77  (403, "not allow
+0001aa50: 6564 2066 6f72 2075 7365 7220 2220 2b20  ed for user " + 
+0001aa60: 7365 6c66 2e75 6e61 6d65 290a 0a20 2020  self.uname)..   
+0001aa70: 2020 2020 2069 6620 7365 6c66 2e61 7267       if self.arg
+0001aa80: 732e 6e6f 5f6d 763a 0a20 2020 2020 2020  s.no_mv:.       
+0001aa90: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
+0001aaa0: 6328 3430 332c 2022 7468 6520 7265 6e61  c(403, "the rena
+0001aab0: 6d65 2f6d 6f76 6520 6665 6174 7572 6520  me/move feature 
+0001aac0: 6973 2064 6973 6162 6c65 6420 696e 2073  is disabled in s
+0001aad0: 6572 7665 7220 636f 6e66 6967 2229 0a0a  erver config")..
+0001aae0: 2020 2020 2020 2020 7820 3d20 7365 6c66          x = self
+0001aaf0: 2e63 6f6e 6e2e 6873 7276 2e62 726f 6b65  .conn.hsrv.broke
+0001ab00: 722e 6173 6b28 2275 7032 6b2e 6861 6e64  r.ask("up2k.hand
+0001ab10: 6c65 5f6d 7622 2c20 7365 6c66 2e75 6e61  le_mv", self.una
+0001ab20: 6d65 2c20 7673 7263 2c20 7664 7374 290a  me, vsrc, vdst).
+0001ab30: 2020 2020 2020 2020 7365 6c66 2e6c 6f75          self.lou
+0001ab40: 645f 7265 706c 7928 782e 6765 7428 292c  d_reply(x.get(),
+0001ab50: 2073 7461 7475 733d 3230 3129 0a20 2020   status=201).   
+0001ab60: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+0001ab70: 0a0a 2020 2020 6465 6620 7478 5f6c 7328  ..    def tx_ls(
+0001ab80: 7365 6c66 2c20 6c73 2020 2920 203a 0a20  self, ls  )  :. 
+0001ab90: 2020 2020 2020 2064 6972 7320 3d20 6c73         dirs = ls
+0001aba0: 5b22 6469 7273 225d 0a20 2020 2020 2020  ["dirs"].       
+0001abb0: 2066 696c 6573 203d 206c 735b 2266 696c   files = ls["fil
+0001abc0: 6573 225d 0a20 2020 2020 2020 2061 7267  es"].        arg
+0001abd0: 203d 2073 656c 662e 7570 6172 616d 5b22   = self.uparam["
+0001abe0: 6c73 225d 0a20 2020 2020 2020 2069 6620  ls"].        if 
+0001abf0: 6172 6720 696e 205b 2276 222c 2022 7422  arg in ["v", "t"
+0001ac00: 2c20 2274 7874 225d 3a0a 2020 2020 2020  , "txt"]:.      
+0001ac10: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+0001ac20: 2020 2020 2020 2020 2020 2062 6967 6765             bigge
+0001ac30: 7374 203d 206d 6178 286c 735b 2266 696c  st = max(ls["fil
+0001ac40: 6573 225d 202b 206c 735b 2264 6972 7322  es"] + ls["dirs"
+0001ac50: 5d2c 206b 6579 3d69 7465 6d67 6574 7465  ], key=itemgette
+0001ac60: 7228 2273 7a22 2929 5b22 737a 225d 0a20  r("sz"))["sz"]. 
+0001ac70: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001ac80: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001ac90: 2020 2062 6967 6765 7374 203d 2030 0a0a     biggest = 0..
+0001aca0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0001acb0: 7267 203d 3d20 2276 223a 0a20 2020 2020  rg == "v":.     
+0001acc0: 2020 2020 2020 2020 2020 2066 6d74 203d             fmt =
+0001acd0: 2022 5c30 3333 5b30 3b37 3b33 366d 7b7b   "\033[0;7;36m{{
+0001ace0: 7d7d 7b7b 3a3e 7b7d 7d7d 5c30 3333 5b30  }}{{:>{}}}\033[0
+0001acf0: 6d20 7b7b 7d7d 220a 2020 2020 2020 2020  m {{}}".        
+0001ad00: 2020 2020 2020 2020 6e66 6d74 203d 2022          nfmt = "
+0001ad10: 7b7d 220a 2020 2020 2020 2020 2020 2020  {}".            
+0001ad20: 2020 2020 6269 6767 6573 7420 3d20 300a      biggest = 0.
+0001ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad40: 6632 203d 2022 222e 6a6f 696e 280a 2020  f2 = "".join(.  
+0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad60: 2020 227b 7d7b 7b7d 7d22 2e66 6f72 6d61    "{}{{}}".forma
+0001ad70: 7428 7829 0a20 2020 2020 2020 2020 2020  t(x).           
+0001ad80: 2020 2020 2020 2020 2066 6f72 2078 2069           for x i
+0001ad90: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
+0001ada0: 2020 2020 2020 2020 2020 2020 225c 3033              "\03
+0001adb0: 335b 376d 222c 0a20 2020 2020 2020 2020  3[7m",.         
+0001adc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001add0: 5c30 3333 5b32 376d 222c 0a20 2020 2020  \033[27m",.     
 0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adf0: 2022 5c30 3333 5b32 376d 222c 0a20 2020   "\033[27m",.   
-0001ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae10: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
+0001adf0: 2020 2022 222c 0a20 2020 2020 2020 2020     "",.         
+0001ae00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001ae10: 5c30 3333 5b30 3b31 6d22 2c0a 2020 2020  \033[0;1m",.    
 0001ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae30: 2022 5c30 3333 5b30 3b31 6d22 2c0a 2020   "\033[0;1m",.  
-0001ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae50: 2020 2020 2020 225c 3033 335b 303b 3336        "\033[0;36
-0001ae60: 6d22 2c0a 2020 2020 2020 2020 2020 2020  m",.            
-0001ae70: 2020 2020 2020 2020 2020 2020 225c 3033              "\03
-0001ae80: 335b 306d 222c 0a20 2020 2020 2020 2020  3[0m",.         
-0001ae90: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
-0001aea0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001aec0: 7461 6220 3d20 7b22 4222 3a20 362c 2022  tab = {"B": 6, "
-0001aed0: 4b22 3a20 352c 2022 4d22 3a20 312c 2022  K": 5, "M": 1, "
-0001aee0: 4722 3a20 337d 0a20 2020 2020 2020 2020  G": 3}.         
-0001aef0: 2020 2020 2020 2066 6f72 206c 7374 2069         for lst i
-0001af00: 6e20 5b64 6972 732c 2066 696c 6573 5d3a  n [dirs, files]:
+0001ae30: 2020 2020 225c 3033 335b 303b 3336 6d22      "\033[0;36m"
+0001ae40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001ae50: 2020 2020 2020 2020 2020 225c 3033 335b            "\033[
+0001ae60: 306d 222c 0a20 2020 2020 2020 2020 2020  0m",.           
+0001ae70: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+0001ae80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001ae90: 2020 2020 2020 2020 2020 2020 2063 7461               cta
+0001aea0: 6220 3d20 7b22 4222 3a20 362c 2022 4b22  b = {"B": 6, "K"
+0001aeb0: 3a20 352c 2022 4d22 3a20 312c 2022 4722  : 5, "M": 1, "G"
+0001aec0: 3a20 337d 0a20 2020 2020 2020 2020 2020  : 3}.           
+0001aed0: 2020 2020 2066 6f72 206c 7374 2069 6e20       for lst in 
+0001aee0: 5b64 6972 732c 2066 696c 6573 5d3a 0a20  [dirs, files]:. 
+0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af00: 2020 2066 6f72 2078 2069 6e20 6c73 743a     for x in lst:
 0001af10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001af20: 2020 2020 2066 6f72 2078 2069 6e20 6c73       for x in ls
-0001af30: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0001af40: 2020 2020 2020 2020 2020 2061 203d 2078             a = x
-0001af50: 5b22 6474 225d 2e72 6570 6c61 6365 2822  ["dt"].replace("
-0001af60: 2d22 2c20 2220 2229 2e72 6570 6c61 6365  -", " ").replace
-0001af70: 2822 3a22 2c20 2220 2229 2e73 706c 6974  (":", " ").split
-0001af80: 2822 2022 290a 2020 2020 2020 2020 2020  (" ").          
-0001af90: 2020 2020 2020 2020 2020 2020 2020 785b                x[
-0001afa0: 2264 7422 5d20 3d20 6632 2e66 6f72 6d61  "dt"] = f2.forma
-0001afb0: 7428 2a6c 6973 7428 6129 290a 2020 2020  t(*list(a)).    
-0001afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afd0: 2020 2020 737a 203d 2068 756d 616e 7369      sz = humansi
-0001afe0: 7a65 2878 5b22 737a 225d 2c20 5472 7565  ze(x["sz"], True
-0001aff0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001b000: 2020 2020 2020 2020 2020 785b 2273 7a22            x["sz"
-0001b010: 5d20 3d20 225c 3033 335b 303b 337b 7d6d  ] = "\033[0;3{}m
-0001b020: 207b 3a3e 357d 222e 666f 726d 6174 2863   {:>5}".format(c
-0001b030: 7461 622e 6765 7428 737a 5b2d 313a 5d2c  tab.get(sz[-1:],
-0001b040: 2030 292c 2073 7a29 0a20 2020 2020 2020   0), sz).       
-0001b050: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0001b060: 2020 2020 2020 2020 2020 2066 6d74 203d             fmt =
-0001b070: 2022 7b7b 7d7d 2020 7b7b 3a7b 7d2c 7d7d   "{{}}  {{:{},}}
-0001b080: 2020 7b7b 7d7d 220a 2020 2020 2020 2020    {{}}".        
-0001b090: 2020 2020 2020 2020 6e66 6d74 203d 2022          nfmt = "
-0001b0a0: 7b3a 2c7d 220a 0a20 2020 2020 2020 2020  {:,}"..         
-0001b0b0: 2020 2066 6f72 2078 2069 6e20 6469 7273     for x in dirs
-0001b0c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b0d0: 2020 6e20 3d20 785b 226e 616d 6522 5d20    n = x["name"] 
-0001b0e0: 2b20 222f 220a 2020 2020 2020 2020 2020  + "/".          
-0001b0f0: 2020 2020 2020 6966 2061 7267 203d 3d20        if arg == 
-0001b100: 2276 223a 0a20 2020 2020 2020 2020 2020  "v":.           
-0001b110: 2020 2020 2020 2020 206e 203d 2022 5c30           n = "\0
-0001b120: 3333 5b39 346d 2220 2b20 6e0a 0a20 2020  33[94m" + n..   
-0001b130: 2020 2020 2020 2020 2020 2020 2078 5b22               x["
-0001b140: 6e61 6d65 225d 203d 206e 0a0a 2020 2020  name"] = n..    
-0001b150: 2020 2020 2020 2020 666d 7420 3d20 666d          fmt = fm
-0001b160: 742e 666f 726d 6174 286c 656e 286e 666d  t.format(len(nfm
-0001b170: 742e 666f 726d 6174 2862 6967 6765 7374  t.format(biggest
-0001b180: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0001b190: 7265 746c 203d 205b 0a20 2020 2020 2020  retl = [.       
-0001b1a0: 2020 2020 2020 2020 2022 2320 7b7d 3a20           "# {}: 
-0001b1b0: 7b7d 222e 666f 726d 6174 2878 2c20 6c73  {}".format(x, ls
-0001b1c0: 5b78 5d29 0a20 2020 2020 2020 2020 2020  [x]).           
-0001b1d0: 2020 2020 2066 6f72 2078 2069 6e20 5b22       for x in ["
-0001b1e0: 6163 6374 222c 2022 7065 726d 7322 2c20  acct", "perms", 
-0001b1f0: 2273 7276 696e 6622 5d0a 2020 2020 2020  "srvinf"].      
-0001b200: 2020 2020 2020 2020 2020 6966 2078 2069            if x i
-0001b210: 6e20 6c73 0a20 2020 2020 2020 2020 2020  n ls.           
-0001b220: 205d 0a20 2020 2020 2020 2020 2020 2072   ].            r
-0001b230: 6574 6c20 2b3d 205b 0a20 2020 2020 2020  etl += [.       
-0001b240: 2020 2020 2020 2020 2066 6d74 2e66 6f72           fmt.for
-0001b250: 6d61 7428 785b 2264 7422 5d2c 2078 5b22  mat(x["dt"], x["
-0001b260: 737a 225d 2c20 785b 226e 616d 6522 5d29  sz"], x["name"])
-0001b270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b280: 2066 6f72 2079 2069 6e20 5b64 6972 732c   for y in [dirs,
-0001b290: 2066 696c 6573 5d0a 2020 2020 2020 2020   files].        
-0001b2a0: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
-0001b2b0: 2079 0a20 2020 2020 2020 2020 2020 205d   y.            ]
-0001b2c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001b2d0: 203d 2022 5c6e 222e 6a6f 696e 2872 6574   = "\n".join(ret
-0001b2e0: 6c29 0a20 2020 2020 2020 2020 2020 206d  l).            m
-0001b2f0: 696d 6520 3d20 2274 6578 742f 706c 6169  ime = "text/plai
-0001b300: 6e3b 2063 6861 7273 6574 3d75 7466 2d38  n; charset=utf-8
-0001b310: 220a 2020 2020 2020 2020 656c 7365 3a0a  ".        else:.
-0001b320: 2020 2020 2020 2020 2020 2020 5b78 2e70              [x.p
-0001b330: 6f70 286b 2920 666f 7220 6b20 696e 205b  op(k) for k in [
-0001b340: 226e 616d 6522 2c20 2264 7422 5d20 666f  "name", "dt"] fo
-0001b350: 7220 7920 696e 205b 6469 7273 2c20 6669  r y in [dirs, fi
-0001b360: 6c65 735d 2066 6f72 2078 2069 6e20 795d  les] for x in y]
-0001b370: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-0001b380: 7420 3d20 6a73 6f6e 2e64 756d 7073 286c  t = json.dumps(l
-0001b390: 7329 0a20 2020 2020 2020 2020 2020 206d  s).            m
-0001b3a0: 696d 6520 3d20 2261 7070 6c69 6361 7469  ime = "applicati
-0001b3b0: 6f6e 2f6a 736f 6e22 0a0a 2020 2020 2020  on/json"..      
-0001b3c0: 2020 7265 7420 2b3d 2022 5c6e 5c30 3333    ret += "\n\033
-0001b3d0: 5b30 6d22 2069 6620 6172 6720 3d3d 2022  [0m" if arg == "
-0001b3e0: 7622 2065 6c73 6520 225c 6e22 0a20 2020  v" else "\n".   
-0001b3f0: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
-0001b400: 7265 742e 656e 636f 6465 2822 7574 662d  ret.encode("utf-
-0001b410: 3822 2c20 2272 6570 6c61 6365 2229 2c20  8", "replace"), 
-0001b420: 6d69 6d65 3d6d 696d 6529 0a20 2020 2020  mime=mime).     
-0001b430: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-0001b440: 2020 2020 6465 6620 7478 5f62 726f 7773      def tx_brows
-0001b450: 6572 2873 656c 6629 2020 3a0a 2020 2020  er(self)  :.    
-0001b460: 2020 2020 7670 6174 6820 3d20 2222 0a20      vpath = "". 
-0001b470: 2020 2020 2020 2076 706e 6f64 6573 203d         vpnodes =
-0001b480: 205b 5b22 222c 2022 2f22 5d5d 0a20 2020   [["", "/"]].   
-0001b490: 2020 2020 2069 6620 7365 6c66 2e76 7061       if self.vpa
-0001b4a0: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-0001b4b0: 666f 7220 6e6f 6465 2069 6e20 7365 6c66  for node in self
-0001b4c0: 2e76 7061 7468 2e73 706c 6974 2822 2f22  .vpath.split("/"
-0001b4d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001b4e0: 2020 2069 6620 6e6f 7420 7670 6174 683a     if not vpath:
-0001b4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b500: 2020 2020 2076 7061 7468 203d 206e 6f64       vpath = nod
-0001b510: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0001b520: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001b530: 2020 2020 2020 2020 2020 2020 7670 6174              vpat
-0001b540: 6820 2b3d 2022 2f22 202b 206e 6f64 650a  h += "/" + node.
-0001b550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b560: 2076 706e 6f64 6573 2e61 7070 656e 6428   vpnodes.append(
-0001b570: 5b71 756f 7465 7028 7670 6174 6829 202b  [quotep(vpath) +
-0001b580: 2022 2f22 2c20 6874 6d6c 5f65 7363 6170   "/", html_escap
-0001b590: 6528 6e6f 6465 2c20 6372 6c66 3d54 7275  e(node, crlf=Tru
-0001b5a0: 6529 5d29 0a0a 2020 2020 2020 2020 766e  e)])..        vn
-0001b5b0: 203d 2073 656c 662e 766e 0a20 2020 2020   = self.vn.     
-0001b5c0: 2020 2072 656d 203d 2073 656c 662e 7265     rem = self.re
-0001b5d0: 6d0a 2020 2020 2020 2020 6162 7370 6174  m.        abspat
-0001b5e0: 6820 3d20 766e 2e64 6361 6e6f 6e69 6361  h = vn.dcanonica
-0001b5f0: 6c28 7265 6d29 0a20 2020 2020 2020 2064  l(rem).        d
-0001b600: 6276 2c20 7672 656d 203d 2076 6e2e 6765  bv, vrem = vn.ge
-0001b610: 745f 6462 7628 7265 6d29 0a0a 2020 2020  t_dbv(rem)..    
-0001b620: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0001b630: 2020 2020 2073 7420 3d20 626f 732e 7374       st = bos.st
-0001b640: 6174 2861 6273 7061 7468 290a 2020 2020  at(abspath).    
-0001b650: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-0001b660: 2020 2020 2020 2020 6966 2022 6f6e 3430          if "on40
-0001b670: 3422 206e 6f74 2069 6e20 766e 2e66 6c61  4" not in vn.fla
-0001b680: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-0001b690: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001b6a0: 7478 5f34 3034 2829 0a0a 2020 2020 2020  tx_404()..      
-0001b6b0: 2020 2020 2020 7265 7420 3d20 7365 6c66        ret = self
-0001b6c0: 2e6f 6e34 3078 2876 6e2e 666c 6167 735b  .on40x(vn.flags[
-0001b6d0: 226f 6e34 3034 225d 2c20 766e 2c20 7265  "on404"], vn, re
-0001b6e0: 6d29 0a20 2020 2020 2020 2020 2020 2069  m).            i
-0001b6f0: 6620 7265 7420 3d3d 2022 7472 7565 223a  f ret == "true":
-0001b700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b710: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-0001b720: 2020 2020 2020 2020 2065 6c69 6620 7265           elif re
-0001b730: 7420 3d3d 2022 6661 6c73 6522 3a0a 2020  t == "false":.  
-0001b740: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001b750: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-0001b760: 2020 2020 2020 2065 6c69 6620 7265 7420         elif ret 
-0001b770: 3d3d 2022 7265 7472 7922 3a0a 2020 2020  == "retry":.    
-0001b780: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0001b790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b7a0: 2020 2020 2073 7420 3d20 626f 732e 7374       st = bos.st
-0001b7b0: 6174 2861 6273 7061 7468 290a 2020 2020  at(abspath).    
-0001b7c0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0001b7d0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-0001b7e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001b7f0: 656c 662e 7478 5f34 3034 2829 0a20 2020  elf.tx_404().   
-0001b800: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0001b810: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001b820: 6574 7572 6e20 7365 6c66 2e74 785f 3430  eturn self.tx_40
-0001b830: 3428 290a 0a20 2020 2020 2020 2069 6620  4()..        if 
-0001b840: 7265 6d2e 7374 6172 7473 7769 7468 2822  rem.startswith("
-0001b850: 2e68 6973 742f 7570 326b 2e22 2920 6f72  .hist/up2k.") or
-0001b860: 2028 0a20 2020 2020 2020 2020 2020 2072   (.            r
-0001b870: 656d 2e65 6e64 7377 6974 6828 222f 6469  em.endswith("/di
-0001b880: 722e 7478 7422 2920 616e 6420 7265 6d2e  r.txt") and rem.
-0001b890: 7374 6172 7473 7769 7468 2822 2e68 6973  startswith(".his
-0001b8a0: 742f 7468 2f22 290a 2020 2020 2020 2020  t/th/").        
-0001b8b0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0001b8c0: 6169 7365 2050 6562 6b61 6328 3430 3329  aise Pebkac(403)
-0001b8d0: 0a0a 2020 2020 2020 2020 6532 6420 3d20  ..        e2d = 
-0001b8e0: 2265 3264 2220 696e 2076 6e2e 666c 6167  "e2d" in vn.flag
-0001b8f0: 730a 2020 2020 2020 2020 6532 7420 3d20  s.        e2t = 
-0001b900: 2265 3274 2220 696e 2076 6e2e 666c 6167  "e2t" in vn.flag
-0001b910: 730a 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-0001b920: 6874 6d6c 5f68 6561 6420 3d20 766e 2e66  html_head = vn.f
-0001b930: 6c61 6773 2e67 6574 2822 6874 6d6c 5f68  lags.get("html_h
-0001b940: 6561 6422 2c20 2222 290a 2020 2020 2020  ead", "").      
-0001b950: 2020 6966 2076 6e2e 666c 6167 732e 6765    if vn.flags.ge
-0001b960: 7428 226e 6f72 6f62 6f74 7322 2920 6f72  t("norobots") or
-0001b970: 2022 6222 2069 6e20 7365 6c66 2e75 7061   "b" in self.upa
-0001b980: 7261 6d3a 0a20 2020 2020 2020 2020 2020  ram:.           
-0001b990: 2073 656c 662e 6f75 745f 6865 6164 6572   self.out_header
-0001b9a0: 735b 2258 2d52 6f62 6f74 732d 5461 6722  s["X-Robots-Tag"
-0001b9b0: 5d20 3d20 226e 6f69 6e64 6578 2c20 6e6f  ] = "noindex, no
-0001b9c0: 666f 6c6c 6f77 220a 2020 2020 2020 2020  follow".        
-0001b9d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001b9e0: 2020 7365 6c66 2e6f 7574 5f68 6561 6465    self.out_heade
-0001b9f0: 7273 2e70 6f70 2822 582d 526f 626f 7473  rs.pop("X-Robots
-0001ba00: 2d54 6167 222c 204e 6f6e 6529 0a0a 2020  -Tag", None)..  
-0001ba10: 2020 2020 2020 6973 5f64 6972 203d 2073        is_dir = s
-0001ba20: 7461 742e 535f 4953 4449 5228 7374 2e73  tat.S_ISDIR(st.s
-0001ba30: 745f 6d6f 6465 290a 2020 2020 2020 2020  t_mode).        
-0001ba40: 6963 7572 203d 204e 6f6e 650a 2020 2020  icur = None.    
-0001ba50: 2020 2020 6966 2069 735f 6469 7220 616e      if is_dir an
-0001ba60: 6420 2865 3274 206f 7220 6532 6429 3a0a  d (e2t or e2d):.
-0001ba70: 2020 2020 2020 2020 2020 2020 6964 7820              idx 
-0001ba80: 3d20 7365 6c66 2e63 6f6e 6e2e 6765 745f  = self.conn.get_
-0001ba90: 7532 6964 7828 290a 2020 2020 2020 2020  u2idx().        
-0001baa0: 2020 2020 6966 2069 6478 2061 6e64 2068      if idx and h
-0001bab0: 6173 6174 7472 2869 6478 2c20 2270 5f65  asattr(idx, "p_e
-0001bac0: 6e64 2229 3a0a 2020 2020 2020 2020 2020  nd"):.          
-0001bad0: 2020 2020 2020 6963 7572 203d 2069 6478        icur = idx
-0001bae0: 2e67 6574 5f63 7572 2864 6276 2e72 6561  .get_cur(dbv.rea
-0001baf0: 6c70 6174 6829 0a0a 2020 2020 2020 2020  lpath)..        
-0001bb00: 6966 2073 656c 662e 6361 6e5f 7265 6164  if self.can_read
-0001bb10: 3a0a 2020 2020 2020 2020 2020 2020 7468  :.            th
-0001bb20: 5f66 6d74 203d 2073 656c 662e 7570 6172  _fmt = self.upar
-0001bb30: 616d 2e67 6574 2822 7468 2229 0a20 2020  am.get("th").   
-0001bb40: 2020 2020 2020 2020 2069 6620 7468 5f66           if th_f
-0001bb50: 6d74 2069 7320 6e6f 7420 4e6f 6e65 3a0a  mt is not None:.
-0001bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb70: 6966 2069 735f 6469 723a 0a20 2020 2020  if is_dir:.     
-0001bb80: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0001bb90: 7265 6d20 3d20 7672 656d 2e72 7374 7269  rem = vrem.rstri
-0001bba0: 7028 222f 2229 0a20 2020 2020 2020 2020  p("/").         
-0001bbb0: 2020 2020 2020 2020 2020 2069 6620 6963             if ic
-0001bbc0: 7572 2061 6e64 2076 7265 6d3a 0a20 2020  ur and vrem:.   
-0001bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbe0: 2020 2020 2071 203d 2022 7365 6c65 6374       q = "select
-0001bbf0: 2066 6e20 6672 6f6d 2063 7620 7768 6572   fn from cv wher
-0001bc00: 6520 7264 3d3f 2061 6e64 2064 6e3d 3f22  e rd=? and dn=?"
-0001bc10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bc20: 2020 2020 2020 2020 2063 7264 2c20 6364           crd, cd
-0001bc30: 6e20 3d20 7672 656d 2e72 7370 6c69 7428  n = vrem.rsplit(
-0001bc40: 222f 222c 2031 2920 6966 2022 2f22 2069  "/", 1) if "/" i
-0001bc50: 6e20 7672 656d 2065 6c73 6520 2822 222c  n vrem else ("",
-0001bc60: 2076 7265 6d29 0a20 2020 2020 2020 2020   vrem).         
-0001bc70: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001bc80: 206e 6f20 6d6f 6a69 6261 6b65 2073 7570   no mojibake sup
-0001bc90: 706f 7274 3a0a 2020 2020 2020 2020 2020  port:.          
-0001bca0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0001bcb0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001bcc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001bcd0: 666e 203d 2069 6375 722e 6578 6563 7574  fn = icur.execut
-0001bce0: 6528 712c 2028 6372 642c 2063 646e 2929  e(q, (crd, cdn))
-0001bcf0: 2e66 6574 6368 6f6e 6528 290a 2020 2020  .fetchone().    
+0001af20: 2020 2020 2020 2020 2061 203d 2078 5b22           a = x["
+0001af30: 6474 225d 2e72 6570 6c61 6365 2822 2d22  dt"].replace("-"
+0001af40: 2c20 2220 2229 2e72 6570 6c61 6365 2822  , " ").replace("
+0001af50: 3a22 2c20 2220 2229 2e73 706c 6974 2822  :", " ").split("
+0001af60: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
+0001af70: 2020 2020 2020 2020 2020 2020 785b 2264              x["d
+0001af80: 7422 5d20 3d20 6632 2e66 6f72 6d61 7428  t"] = f2.format(
+0001af90: 2a6c 6973 7428 6129 290a 2020 2020 2020  *list(a)).      
+0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afb0: 2020 737a 203d 2068 756d 616e 7369 7a65    sz = humansize
+0001afc0: 2878 5b22 737a 225d 2c20 5472 7565 290a  (x["sz"], True).
+0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001afe0: 2020 2020 2020 2020 785b 2273 7a22 5d20          x["sz"] 
+0001aff0: 3d20 225c 3033 335b 303b 337b 7d6d 207b  = "\033[0;3{}m {
+0001b000: 3a3e 357d 222e 666f 726d 6174 2863 7461  :>5}".format(cta
+0001b010: 622e 6765 7428 737a 5b2d 313a 5d2c 2030  b.get(sz[-1:], 0
+0001b020: 292c 2073 7a29 0a20 2020 2020 2020 2020  ), sz).         
+0001b030: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001b040: 2020 2020 2020 2020 2066 6d74 203d 2022           fmt = "
+0001b050: 7b7b 7d7d 2020 7b7b 3a7b 7d2c 7d7d 2020  {{}}  {{:{},}}  
+0001b060: 7b7b 7d7d 220a 2020 2020 2020 2020 2020  {{}}".          
+0001b070: 2020 2020 2020 6e66 6d74 203d 2022 7b3a        nfmt = "{:
+0001b080: 2c7d 220a 0a20 2020 2020 2020 2020 2020  ,}"..           
+0001b090: 2066 6f72 2078 2069 6e20 6469 7273 3a0a   for x in dirs:.
+0001b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0b0: 6e20 3d20 785b 226e 616d 6522 5d20 2b20  n = x["name"] + 
+0001b0c0: 222f 220a 2020 2020 2020 2020 2020 2020  "/".            
+0001b0d0: 2020 2020 6966 2061 7267 203d 3d20 2276      if arg == "v
+0001b0e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0001b0f0: 2020 2020 2020 206e 203d 2022 5c30 3333         n = "\033
+0001b100: 5b39 346d 2220 2b20 6e0a 0a20 2020 2020  [94m" + n..     
+0001b110: 2020 2020 2020 2020 2020 2078 5b22 6e61             x["na
+0001b120: 6d65 225d 203d 206e 0a0a 2020 2020 2020  me"] = n..      
+0001b130: 2020 2020 2020 666d 7420 3d20 666d 742e        fmt = fmt.
+0001b140: 666f 726d 6174 286c 656e 286e 666d 742e  format(len(nfmt.
+0001b150: 666f 726d 6174 2862 6967 6765 7374 2929  format(biggest))
+0001b160: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+0001b170: 746c 203d 205b 0a20 2020 2020 2020 2020  tl = [.         
+0001b180: 2020 2020 2020 2022 2320 7b7d 3a20 7b7d         "# {}: {}
+0001b190: 222e 666f 726d 6174 2878 2c20 6c73 5b78  ".format(x, ls[x
+0001b1a0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0001b1b0: 2020 2066 6f72 2078 2069 6e20 5b22 6163     for x in ["ac
+0001b1c0: 6374 222c 2022 7065 726d 7322 2c20 2273  ct", "perms", "s
+0001b1d0: 7276 696e 6622 5d0a 2020 2020 2020 2020  rvinf"].        
+0001b1e0: 2020 2020 2020 2020 6966 2078 2069 6e20          if x in 
+0001b1f0: 6c73 0a20 2020 2020 2020 2020 2020 205d  ls.            ]
+0001b200: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0001b210: 6c20 2b3d 205b 0a20 2020 2020 2020 2020  l += [.         
+0001b220: 2020 2020 2020 2066 6d74 2e66 6f72 6d61         fmt.forma
+0001b230: 7428 785b 2264 7422 5d2c 2078 5b22 737a  t(x["dt"], x["sz
+0001b240: 225d 2c20 785b 226e 616d 6522 5d29 0a20  "], x["name"]). 
+0001b250: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001b260: 6f72 2079 2069 6e20 5b64 6972 732c 2066  or y in [dirs, f
+0001b270: 696c 6573 5d0a 2020 2020 2020 2020 2020  iles].          
+0001b280: 2020 2020 2020 666f 7220 7820 696e 2079        for x in y
+0001b290: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+0001b2a0: 2020 2020 2020 2020 2020 2072 6574 203d             ret =
+0001b2b0: 2022 5c6e 222e 6a6f 696e 2872 6574 6c29   "\n".join(retl)
+0001b2c0: 0a20 2020 2020 2020 2020 2020 206d 696d  .            mim
+0001b2d0: 6520 3d20 2274 6578 742f 706c 6169 6e3b  e = "text/plain;
+0001b2e0: 2063 6861 7273 6574 3d75 7466 2d38 220a   charset=utf-8".
+0001b2f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001b300: 2020 2020 2020 2020 2020 5b78 2e70 6f70            [x.pop
+0001b310: 286b 2920 666f 7220 6b20 696e 205b 226e  (k) for k in ["n
+0001b320: 616d 6522 2c20 2264 7422 5d20 666f 7220  ame", "dt"] for 
+0001b330: 7920 696e 205b 6469 7273 2c20 6669 6c65  y in [dirs, file
+0001b340: 735d 2066 6f72 2078 2069 6e20 795d 0a0a  s] for x in y]..
+0001b350: 2020 2020 2020 2020 2020 2020 7265 7420              ret 
+0001b360: 3d20 6a73 6f6e 2e64 756d 7073 286c 7329  = json.dumps(ls)
+0001b370: 0a20 2020 2020 2020 2020 2020 206d 696d  .            mim
+0001b380: 6520 3d20 2261 7070 6c69 6361 7469 6f6e  e = "application
+0001b390: 2f6a 736f 6e22 0a0a 2020 2020 2020 2020  /json"..        
+0001b3a0: 7265 7420 2b3d 2022 5c6e 5c30 3333 5b30  ret += "\n\033[0
+0001b3b0: 6d22 2069 6620 6172 6720 3d3d 2022 7622  m" if arg == "v"
+0001b3c0: 2065 6c73 6520 225c 6e22 0a20 2020 2020   else "\n".     
+0001b3d0: 2020 2073 656c 662e 7265 706c 7928 7265     self.reply(re
+0001b3e0: 742e 656e 636f 6465 2822 7574 662d 3822  t.encode("utf-8"
+0001b3f0: 2c20 2272 6570 6c61 6365 2229 2c20 6d69  , "replace"), mi
+0001b400: 6d65 3d6d 696d 6529 0a20 2020 2020 2020  me=mime).       
+0001b410: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
+0001b420: 2020 6465 6620 7478 5f62 726f 7773 6572    def tx_browser
+0001b430: 2873 656c 6629 2020 3a0a 2020 2020 2020  (self)  :.      
+0001b440: 2020 7670 6174 6820 3d20 2222 0a20 2020    vpath = "".   
+0001b450: 2020 2020 2076 706e 6f64 6573 203d 205b       vpnodes = [
+0001b460: 5b22 222c 2022 2f22 5d5d 0a20 2020 2020  ["", "/"]].     
+0001b470: 2020 2069 6620 7365 6c66 2e76 7061 7468     if self.vpath
+0001b480: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+0001b490: 7220 6e6f 6465 2069 6e20 7365 6c66 2e76  r node in self.v
+0001b4a0: 7061 7468 2e73 706c 6974 2822 2f22 293a  path.split("/"):
+0001b4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b4c0: 2069 6620 6e6f 7420 7670 6174 683a 0a20   if not vpath:. 
+0001b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4e0: 2020 2076 7061 7468 203d 206e 6f64 650a     vpath = node.
+0001b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b500: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001b510: 2020 2020 2020 2020 2020 7670 6174 6820            vpath 
+0001b520: 2b3d 2022 2f22 202b 206e 6f64 650a 0a20  += "/" + node.. 
+0001b530: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0001b540: 706e 6f64 6573 2e61 7070 656e 6428 5b71  pnodes.append([q
+0001b550: 756f 7465 7028 7670 6174 6829 202b 2022  uotep(vpath) + "
+0001b560: 2f22 2c20 6874 6d6c 5f65 7363 6170 6528  /", html_escape(
+0001b570: 6e6f 6465 2c20 6372 6c66 3d54 7275 6529  node, crlf=True)
+0001b580: 5d29 0a0a 2020 2020 2020 2020 766e 203d  ])..        vn =
+0001b590: 2073 656c 662e 766e 0a20 2020 2020 2020   self.vn.       
+0001b5a0: 2072 656d 203d 2073 656c 662e 7265 6d0a   rem = self.rem.
+0001b5b0: 2020 2020 2020 2020 6162 7370 6174 6820          abspath 
+0001b5c0: 3d20 766e 2e64 6361 6e6f 6e69 6361 6c28  = vn.dcanonical(
+0001b5d0: 7265 6d29 0a20 2020 2020 2020 2064 6276  rem).        dbv
+0001b5e0: 2c20 7672 656d 203d 2076 6e2e 6765 745f  , vrem = vn.get_
+0001b5f0: 6462 7628 7265 6d29 0a0a 2020 2020 2020  dbv(rem)..      
+0001b600: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0001b610: 2020 2073 7420 3d20 626f 732e 7374 6174     st = bos.stat
+0001b620: 2861 6273 7061 7468 290a 2020 2020 2020  (abspath).      
+0001b630: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+0001b640: 2020 2020 2020 6966 2022 6f6e 3430 3422        if "on404"
+0001b650: 206e 6f74 2069 6e20 766e 2e66 6c61 6773   not in vn.flags
+0001b660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b670: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+0001b680: 5f34 3034 2829 0a0a 2020 2020 2020 2020  _404()..        
+0001b690: 2020 2020 7265 7420 3d20 7365 6c66 2e6f      ret = self.o
+0001b6a0: 6e34 3078 2876 6e2e 666c 6167 735b 226f  n40x(vn.flags["o
+0001b6b0: 6e34 3034 225d 2c20 766e 2c20 7265 6d29  n404"], vn, rem)
+0001b6c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001b6d0: 7265 7420 3d3d 2022 7472 7565 223a 0a20  ret == "true":. 
+0001b6e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001b6f0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0001b700: 2020 2020 2020 2065 6c69 6620 7265 7420         elif ret 
+0001b710: 3d3d 2022 6661 6c73 6522 3a0a 2020 2020  == "false":.    
+0001b720: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001b730: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0001b740: 2020 2020 2065 6c69 6620 7265 7420 3d3d       elif ret ==
+0001b750: 2022 7265 7472 7922 3a0a 2020 2020 2020   "retry":.      
+0001b760: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0001b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b780: 2020 2073 7420 3d20 626f 732e 7374 6174     st = bos.stat
+0001b790: 2861 6273 7061 7468 290a 2020 2020 2020  (abspath).      
+0001b7a0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0001b7b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b7c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001b7d0: 662e 7478 5f34 3034 2829 0a20 2020 2020  f.tx_404().     
+0001b7e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001b7f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001b800: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
+0001b810: 290a 0a20 2020 2020 2020 2069 6620 7265  )..        if re
+0001b820: 6d2e 7374 6172 7473 7769 7468 2822 2e68  m.startswith(".h
+0001b830: 6973 742f 7570 326b 2e22 2920 6f72 2028  ist/up2k.") or (
+0001b840: 0a20 2020 2020 2020 2020 2020 2072 656d  .            rem
+0001b850: 2e65 6e64 7377 6974 6828 222f 6469 722e  .endswith("/dir.
+0001b860: 7478 7422 2920 616e 6420 7265 6d2e 7374  txt") and rem.st
+0001b870: 6172 7473 7769 7468 2822 2e68 6973 742f  artswith(".hist/
+0001b880: 7468 2f22 290a 2020 2020 2020 2020 293a  th/").        ):
+0001b890: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001b8a0: 7365 2050 6562 6b61 6328 3430 3329 0a0a  se Pebkac(403)..
+0001b8b0: 2020 2020 2020 2020 6532 6420 3d20 2265          e2d = "e
+0001b8c0: 3264 2220 696e 2076 6e2e 666c 6167 730a  2d" in vn.flags.
+0001b8d0: 2020 2020 2020 2020 6532 7420 3d20 2265          e2t = "e
+0001b8e0: 3274 2220 696e 2076 6e2e 666c 6167 730a  2t" in vn.flags.
+0001b8f0: 0a20 2020 2020 2020 2073 656c 662e 6874  .        self.ht
+0001b900: 6d6c 5f68 6561 6420 3d20 766e 2e66 6c61  ml_head = vn.fla
+0001b910: 6773 2e67 6574 2822 6874 6d6c 5f68 6561  gs.get("html_hea
+0001b920: 6422 2c20 2222 290a 2020 2020 2020 2020  d", "").        
+0001b930: 6966 2076 6e2e 666c 6167 732e 6765 7428  if vn.flags.get(
+0001b940: 226e 6f72 6f62 6f74 7322 2920 6f72 2022  "norobots") or "
+0001b950: 6222 2069 6e20 7365 6c66 2e75 7061 7261  b" in self.upara
+0001b960: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
+0001b970: 656c 662e 6f75 745f 6865 6164 6572 735b  elf.out_headers[
+0001b980: 2258 2d52 6f62 6f74 732d 5461 6722 5d20  "X-Robots-Tag"] 
+0001b990: 3d20 226e 6f69 6e64 6578 2c20 6e6f 666f  = "noindex, nofo
+0001b9a0: 6c6c 6f77 220a 2020 2020 2020 2020 656c  llow".        el
+0001b9b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001b9c0: 7365 6c66 2e6f 7574 5f68 6561 6465 7273  self.out_headers
+0001b9d0: 2e70 6f70 2822 582d 526f 626f 7473 2d54  .pop("X-Robots-T
+0001b9e0: 6167 222c 204e 6f6e 6529 0a0a 2020 2020  ag", None)..    
+0001b9f0: 2020 2020 6973 5f64 6972 203d 2073 7461      is_dir = sta
+0001ba00: 742e 535f 4953 4449 5228 7374 2e73 745f  t.S_ISDIR(st.st_
+0001ba10: 6d6f 6465 290a 2020 2020 2020 2020 6963  mode).        ic
+0001ba20: 7572 203d 204e 6f6e 650a 2020 2020 2020  ur = None.      
+0001ba30: 2020 6966 2069 735f 6469 7220 616e 6420    if is_dir and 
+0001ba40: 2865 3274 206f 7220 6532 6429 3a0a 2020  (e2t or e2d):.  
+0001ba50: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
+0001ba60: 7365 6c66 2e63 6f6e 6e2e 6765 745f 7532  self.conn.get_u2
+0001ba70: 6964 7828 290a 2020 2020 2020 2020 2020  idx().          
+0001ba80: 2020 6966 2069 6478 2061 6e64 2068 6173    if idx and has
+0001ba90: 6174 7472 2869 6478 2c20 2270 5f65 6e64  attr(idx, "p_end
+0001baa0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0001bab0: 2020 2020 6963 7572 203d 2069 6478 2e67      icur = idx.g
+0001bac0: 6574 5f63 7572 2864 6276 2e72 6561 6c70  et_cur(dbv.realp
+0001bad0: 6174 6829 0a0a 2020 2020 2020 2020 6966  ath)..        if
+0001bae0: 2073 656c 662e 6361 6e5f 7265 6164 3a0a   self.can_read:.
+0001baf0: 2020 2020 2020 2020 2020 2020 7468 5f66              th_f
+0001bb00: 6d74 203d 2073 656c 662e 7570 6172 616d  mt = self.uparam
+0001bb10: 2e67 6574 2822 7468 2229 0a20 2020 2020  .get("th").     
+0001bb20: 2020 2020 2020 2069 6620 7468 5f66 6d74         if th_fmt
+0001bb30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0001bb40: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001bb50: 2069 735f 6469 723a 0a20 2020 2020 2020   is_dir:.       
+0001bb60: 2020 2020 2020 2020 2020 2020 2076 7265               vre
+0001bb70: 6d20 3d20 7672 656d 2e72 7374 7269 7028  m = vrem.rstrip(
+0001bb80: 222f 2229 0a20 2020 2020 2020 2020 2020  "/").           
+0001bb90: 2020 2020 2020 2020 2069 6620 6963 7572           if icur
+0001bba0: 2061 6e64 2076 7265 6d3a 0a20 2020 2020   and vrem:.     
+0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bbc0: 2020 2071 203d 2022 7365 6c65 6374 2066     q = "select f
+0001bbd0: 6e20 6672 6f6d 2063 7620 7768 6572 6520  n from cv where 
+0001bbe0: 7264 3d3f 2061 6e64 2064 6e3d 3f22 0a20  rd=? and dn=?". 
+0001bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc00: 2020 2020 2020 2063 7264 2c20 6364 6e20         crd, cdn 
+0001bc10: 3d20 7672 656d 2e72 7370 6c69 7428 222f  = vrem.rsplit("/
+0001bc20: 222c 2031 2920 6966 2022 2f22 2069 6e20  ", 1) if "/" in 
+0001bc30: 7672 656d 2065 6c73 6520 2822 222c 2076  vrem else ("", v
+0001bc40: 7265 6d29 0a20 2020 2020 2020 2020 2020  rem).           
+0001bc50: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+0001bc60: 6f20 6d6f 6a69 6261 6b65 2073 7570 706f  o mojibake suppo
+0001bc70: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
+0001bc80: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0001bc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bca0: 2020 2020 2020 2020 2020 2020 2063 666e               cfn
+0001bcb0: 203d 2069 6375 722e 6578 6563 7574 6528   = icur.execute(
+0001bcc0: 712c 2028 6372 642c 2063 646e 2929 2e66  q, (crd, cdn)).f
+0001bcd0: 6574 6368 6f6e 6528 290a 2020 2020 2020  etchone().      
+0001bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcf0: 2020 2020 2020 6966 2063 666e 3a0a 2020        if cfn:.  
 0001bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd10: 2020 2020 2020 2020 6966 2063 666e 3a0a          if cfn:.
-0001bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd10: 2020 2020 2020 2020 2020 2020 2020 666e                fn
+0001bd20: 203d 2063 666e 5b30 5d0a 2020 2020 2020   = cfn[0].      
 0001bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd40: 666e 203d 2063 666e 5b30 5d0a 2020 2020  fn = cfn[0].    
-0001bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd60: 2020 2020 2020 2020 2020 2020 6670 203d              fp =
-0001bd70: 206f 732e 7061 7468 2e6a 6f69 6e28 6162   os.path.join(ab
-0001bd80: 7370 6174 682c 2066 6e29 0a20 2020 2020  spath, fn).     
-0001bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bda0: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
-0001bdb0: 732e 7061 7468 2e65 7869 7374 7328 6670  s.path.exists(fp
-0001bdc0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bde0: 2020 2020 2020 2076 7265 6d20 3d20 227b         vrem = "{
-0001bdf0: 7d2f 7b7d 222e 666f 726d 6174 2876 7265  }/{}".format(vre
-0001be00: 6d2c 2066 6e29 2e73 7472 6970 2822 2f22  m, fn).strip("/"
-0001be10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be30: 2020 2020 2020 6973 5f64 6972 203d 2046        is_dir = F
-0001be40: 616c 7365 0a20 2020 2020 2020 2020 2020  alse.           
-0001be50: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-0001be60: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-0001be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be80: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
-0001be90: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001beb0: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
-0001bec0: 6e20 7365 6c66 2e61 7267 732e 7468 5f63  n self.args.th_c
-0001bed0: 6f76 6572 733a 0a20 2020 2020 2020 2020  overs:.         
-0001bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bef0: 2020 2066 7020 3d20 6f73 2e70 6174 682e     fp = os.path.
-0001bf00: 6a6f 696e 2861 6273 7061 7468 2c20 666e  join(abspath, fn
-0001bf10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001bf20: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001bf30: 2062 6f73 2e70 6174 682e 6578 6973 7473   bos.path.exists
-0001bf40: 2866 7029 3a0a 2020 2020 2020 2020 2020  (fp):.          
-0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf60: 2020 2020 2020 7672 656d 203d 2022 7b7d        vrem = "{}
-0001bf70: 2f7b 7d22 2e66 6f72 6d61 7428 7672 656d  /{}".format(vrem
-0001bf80: 2c20 666e 292e 7374 7269 7028 222f 2229  , fn).strip("/")
-0001bf90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bd40: 2020 2020 2020 2020 2020 6670 203d 206f            fp = o
+0001bd50: 732e 7061 7468 2e6a 6f69 6e28 6162 7370  s.path.join(absp
+0001bd60: 6174 682c 2066 6e29 0a20 2020 2020 2020  ath, fn).       
+0001bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd80: 2020 2020 2020 2020 2069 6620 626f 732e           if bos.
+0001bd90: 7061 7468 2e65 7869 7374 7328 6670 293a  path.exists(fp):
+0001bda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bdc0: 2020 2020 2076 7265 6d20 3d20 227b 7d2f       vrem = "{}/
+0001bdd0: 7b7d 222e 666f 726d 6174 2876 7265 6d2c  {}".format(vrem,
+0001bde0: 2066 6e29 2e73 7472 6970 2822 2f22 290a   fn).strip("/").
+0001bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be10: 2020 2020 6973 5f64 6972 203d 2046 616c      is_dir = Fal
+0001be20: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0001be30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+0001be40: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0001be50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001be60: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+0001be70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be90: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+0001bea0: 7365 6c66 2e61 7267 732e 7468 5f63 6f76  self.args.th_cov
+0001beb0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+0001bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bed0: 2066 7020 3d20 6f73 2e70 6174 682e 6a6f   fp = os.path.jo
+0001bee0: 696e 2861 6273 7061 7468 2c20 666e 290a  in(abspath, fn).
+0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf00: 2020 2020 2020 2020 2020 2020 6966 2062              if b
+0001bf10: 6f73 2e70 6174 682e 6578 6973 7473 2866  os.path.exists(f
+0001bf20: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
+0001bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf40: 2020 2020 7672 656d 203d 2022 7b7d 2f7b      vrem = "{}/{
+0001bf50: 7d22 2e66 6f72 6d61 7428 7672 656d 2c20  }".format(vrem, 
+0001bf60: 666e 292e 7374 7269 7028 222f 2229 0a20  fn).strip("/"). 
+0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001bf90: 735f 6469 7220 3d20 4661 6c73 650a 2020  s_dir = False.  
 0001bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfb0: 2069 735f 6469 7220 3d20 4661 6c73 650a   is_dir = False.
-0001bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfe0: 6272 6561 6b0a 0a20 2020 2020 2020 2020  break..         
-0001bff0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0001c000: 5f64 6972 3a0a 2020 2020 2020 2020 2020  _dir:.          
-0001c010: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001c020: 7475 726e 2073 656c 662e 7478 5f69 636f  turn self.tx_ico
-0001c030: 2822 612e 666f 6c64 6572 2229 0a0a 2020  ("a.folder")..  
-0001c040: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0001c050: 7020 3d20 4e6f 6e65 0a20 2020 2020 2020  p = None.       
-0001c060: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0001c070: 2e74 6875 6d62 636c 693a 0a20 2020 2020  .thumbcli:.     
-0001c080: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001c090: 6870 203d 2073 656c 662e 7468 756d 6263  hp = self.thumbc
-0001c0a0: 6c69 2e67 6574 2864 6276 2c20 7672 656d  li.get(dbv, vrem
-0001c0b0: 2c20 696e 7428 7374 2e73 745f 6d74 696d  , int(st.st_mtim
-0001c0c0: 6529 2c20 7468 5f66 6d74 290a 0a20 2020  e), th_fmt)..   
-0001c0d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001c0e0: 7468 703a 0a20 2020 2020 2020 2020 2020  thp:.           
-0001c0f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0001c100: 7365 6c66 2e74 785f 6669 6c65 2874 6870  self.tx_file(thp
-0001c110: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001c120: 2020 2069 6620 7468 5f66 6d74 203d 3d20     if th_fmt == 
-0001c130: 2270 223a 0a20 2020 2020 2020 2020 2020  "p":.           
-0001c140: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
-0001c150: 6562 6b61 6328 3430 3429 0a0a 2020 2020  ebkac(404)..    
-0001c160: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001c170: 726e 2073 656c 662e 7478 5f69 636f 2872  rn self.tx_ico(r
-0001c180: 656d 290a 0a20 2020 2020 2020 2069 6620  em)..        if 
-0001c190: 6e6f 7420 6973 5f64 6972 2061 6e64 2028  not is_dir and (
-0001c1a0: 7365 6c66 2e63 616e 5f72 6561 6420 6f72  self.can_read or
-0001c1b0: 2073 656c 662e 6361 6e5f 6765 7429 3a0a   self.can_get):.
-0001c1c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001c1d0: 6f74 2073 656c 662e 6361 6e5f 7265 6164  ot self.can_read
-0001c1e0: 2061 6e64 2022 666b 2220 696e 2076 6e2e   and "fk" in vn.
-0001c1f0: 666c 6167 733a 0a20 2020 2020 2020 2020  flags:.         
-0001c200: 2020 2020 2020 2063 6f72 7265 6374 203d         correct =
-0001c210: 2073 656c 662e 6765 6e5f 666b 280a 2020   self.gen_fk(.  
-0001c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c230: 2020 7365 6c66 2e61 7267 732e 666b 5f73    self.args.fk_s
-0001c240: 616c 742c 2061 6273 7061 7468 2c20 7374  alt, abspath, st
-0001c250: 2e73 745f 7369 7a65 2c20 3020 6966 2041  .st_size, 0 if A
-0001c260: 4e59 5749 4e20 656c 7365 2073 742e 7374  NYWIN else st.st
-0001c270: 5f69 6e6f 0a20 2020 2020 2020 2020 2020  _ino.           
-0001c280: 2020 2020 2029 5b3a 2076 6e2e 666c 6167       )[: vn.flag
-0001c290: 735b 2266 6b22 5d5d 0a20 2020 2020 2020  s["fk"]].       
-0001c2a0: 2020 2020 2020 2020 2067 6f74 203d 2073           got = s
-0001c2b0: 656c 662e 7570 6172 616d 2e67 6574 2822  elf.uparam.get("
-0001c2c0: 6b22 290a 2020 2020 2020 2020 2020 2020  k").            
-0001c2d0: 2020 2020 6966 2067 6f74 2021 3d20 636f      if got != co
-0001c2e0: 7272 6563 743a 0a20 2020 2020 2020 2020  rrect:.         
-0001c2f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001c300: 6c6f 6728 2277 726f 6e67 2066 696c 656b  log("wrong filek
-0001c310: 6579 2c20 7761 6e74 207b 7d2c 2067 6f74  ey, want {}, got
-0001c320: 207b 7d22 2e66 6f72 6d61 7428 636f 7272   {}".format(corr
-0001c330: 6563 742c 2067 6f74 2929 0a20 2020 2020  ect, got)).     
-0001c340: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001c350: 6574 7572 6e20 7365 6c66 2e74 785f 3430  eturn self.tx_40
-0001c360: 3428 290a 0a20 2020 2020 2020 2020 2020  4()..           
-0001c370: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
-0001c380: 2020 2020 2020 6162 7370 6174 682e 656e        abspath.en
-0001c390: 6473 7769 7468 2822 2e6d 6422 290a 2020  dswith(".md").  
-0001c3a0: 2020 2020 2020 2020 2020 2020 2020 616e                an
-0001c3b0: 6420 226e 6f68 746d 6c22 206e 6f74 2069  d "nohtml" not i
-0001c3c0: 6e20 766e 2e66 6c61 6773 0a20 2020 2020  n vn.flags.     
-0001c3d0: 2020 2020 2020 2020 2020 2061 6e64 2028             and (
-0001c3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c3f0: 2020 2020 2022 7622 2069 6e20 7365 6c66       "v" in self
-0001c400: 2e75 7061 7261 6d0a 2020 2020 2020 2020  .uparam.        
-0001c410: 2020 2020 2020 2020 2020 2020 6f72 2022              or "
-0001c420: 6564 6974 2220 696e 2073 656c 662e 7570  edit" in self.up
-0001c430: 6172 616d 0a20 2020 2020 2020 2020 2020  aram.           
-0001c440: 2020 2020 2020 2020 206f 7220 2265 6469           or "edi
-0001c450: 7432 2220 696e 2073 656c 662e 7570 6172  t2" in self.upar
-0001c460: 616d 0a20 2020 2020 2020 2020 2020 2020  am.             
-0001c470: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0001c480: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0001c490: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001c4a0: 7478 5f6d 6428 6162 7370 6174 6829 0a0a  tx_md(abspath)..
-0001c4b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001c4c0: 726e 2073 656c 662e 7478 5f66 696c 6528  rn self.tx_file(
-0001c4d0: 6162 7370 6174 6829 0a0a 2020 2020 2020  abspath)..      
-0001c4e0: 2020 656c 6966 2069 735f 6469 7220 616e    elif is_dir an
-0001c4f0: 6420 6e6f 7420 7365 6c66 2e63 616e 5f72  d not self.can_r
-0001c500: 6561 6420 616e 6420 6e6f 7420 7365 6c66  ead and not self
-0001c510: 2e63 616e 5f77 7269 7465 3a0a 2020 2020  .can_write:.    
-0001c520: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001c530: 656c 662e 7478 5f34 3034 2854 7275 6529  elf.tx_404(True)
-0001c540: 0a0a 2020 2020 2020 2020 7372 765f 696e  ..        srv_in
-0001c550: 666f 203d 205b 5d0a 0a20 2020 2020 2020  fo = []..       
-0001c560: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-0001c570: 2020 6966 206e 6f74 2073 656c 662e 6172    if not self.ar
-0001c580: 6773 2e6e 6968 3a0a 2020 2020 2020 2020  gs.nih:.        
-0001c590: 2020 2020 2020 2020 7372 765f 696e 666f          srv_info
-0001c5a0: 2e61 7070 656e 6428 7365 6c66 2e61 7267  .append(self.arg
-0001c5b0: 732e 6e61 6d65 290a 2020 2020 2020 2020  s.name).        
-0001c5c0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-0001c5d0: 2020 2020 7365 6c66 2e6c 6f67 2822 2377      self.log("#w
-0001c5e0: 6f77 2023 7768 6f61 2229 0a0a 2020 2020  ow #whoa")..    
-0001c5f0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0001c600: 6172 6773 2e6e 6964 3a0a 2020 2020 2020  args.nid:.      
-0001c610: 2020 2020 2020 6672 6565 2c20 746f 7461        free, tota
-0001c620: 6c20 3d20 6765 745f 6466 2861 6273 7061  l = get_df(abspa
-0001c630: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
-0001c640: 6966 2074 6f74 616c 2069 7320 6e6f 7420  if total is not 
-0001c650: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001c660: 2020 2020 2020 6831 203d 2068 756d 616e        h1 = human
-0001c670: 7369 7a65 2866 7265 6520 6f72 2030 290a  size(free or 0).
-0001c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c690: 6832 203d 2068 756d 616e 7369 7a65 2874  h2 = humansize(t
-0001c6a0: 6f74 616c 290a 2020 2020 2020 2020 2020  otal).          
-0001c6b0: 2020 2020 2020 7372 765f 696e 666f 2e61        srv_info.a
-0001c6c0: 7070 656e 6428 227b 7d20 6672 6565 206f  ppend("{} free o
-0001c6d0: 6620 7b7d 222e 666f 726d 6174 2868 312c  f {}".format(h1,
-0001c6e0: 2068 3229 290a 2020 2020 2020 2020 2020   h2)).          
-0001c6f0: 2020 656c 6966 2066 7265 6520 6973 206e    elif free is n
-0001c700: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0001c710: 2020 2020 2020 2020 2073 7276 5f69 6e66           srv_inf
-0001c720: 6f2e 6170 7065 6e64 2868 756d 616e 7369  o.append(humansi
-0001c730: 7a65 2866 7265 652c 2054 7275 6529 202b  ze(free, True) +
-0001c740: 2022 2066 7265 6522 290a 0a20 2020 2020   " free")..     
-0001c750: 2020 2073 7276 5f69 6e66 6f74 203d 2022     srv_infot = "
-0001c760: 3c2f 7370 616e 3e20 2f2f 203c 7370 616e  </span> // <span
-0001c770: 3e22 2e6a 6f69 6e28 7372 765f 696e 666f  >".join(srv_info
-0001c780: 290a 0a20 2020 2020 2020 2070 6572 6d73  )..        perms
-0001c790: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
-0001c7a0: 2073 656c 662e 6361 6e5f 7265 6164 3a0a   self.can_read:.
-0001c7b0: 2020 2020 2020 2020 2020 2020 7065 726d              perm
-0001c7c0: 732e 6170 7065 6e64 2822 7265 6164 2229  s.append("read")
-0001c7d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001c7e0: 2e63 616e 5f77 7269 7465 3a0a 2020 2020  .can_write:.    
-0001c7f0: 2020 2020 2020 2020 7065 726d 732e 6170          perms.ap
-0001c800: 7065 6e64 2822 7772 6974 6522 290a 2020  pend("write").  
-0001c810: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
-0001c820: 6e5f 6d6f 7665 3a0a 2020 2020 2020 2020  n_move:.        
-0001c830: 2020 2020 7065 726d 732e 6170 7065 6e64      perms.append
-0001c840: 2822 6d6f 7665 2229 0a20 2020 2020 2020  ("move").       
-0001c850: 2069 6620 7365 6c66 2e63 616e 5f64 656c   if self.can_del
-0001c860: 6574 653a 0a20 2020 2020 2020 2020 2020  ete:.           
-0001c870: 2070 6572 6d73 2e61 7070 656e 6428 2264   perms.append("d
-0001c880: 656c 6574 6522 290a 2020 2020 2020 2020  elete").        
-0001c890: 6966 2073 656c 662e 6361 6e5f 6765 743a  if self.can_get:
-0001c8a0: 0a20 2020 2020 2020 2020 2020 2070 6572  .            per
-0001c8b0: 6d73 2e61 7070 656e 6428 2267 6574 2229  ms.append("get")
-0001c8c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001c8d0: 2e63 616e 5f75 7067 6574 3a0a 2020 2020  .can_upget:.    
-0001c8e0: 2020 2020 2020 2020 7065 726d 732e 6170          perms.ap
-0001c8f0: 7065 6e64 2822 7570 6765 7422 290a 2020  pend("upget").  
-0001c900: 2020 2020 2020 6966 2073 656c 662e 6361        if self.ca
-0001c910: 6e5f 6164 6d69 6e3a 0a20 2020 2020 2020  n_admin:.       
-0001c920: 2020 2020 2070 6572 6d73 2e61 7070 656e       perms.appen
-0001c930: 6428 2261 646d 696e 2229 0a0a 2020 2020  d("admin")..    
-0001c940: 2020 2020 7572 6c5f 7375 6620 3d20 7365      url_suf = se
-0001c950: 6c66 2e75 726c 7128 7b7d 2c20 5b22 6b22  lf.urlq({}, ["k"
-0001c960: 5d29 0a20 2020 2020 2020 2069 735f 6c73  ]).        is_ls
-0001c970: 203d 2022 6c73 2220 696e 2073 656c 662e   = "ls" in self.
-0001c980: 7570 6172 616d 0a20 2020 2020 2020 2069  uparam.        i
-0001c990: 735f 6a73 203d 2073 656c 662e 6172 6773  s_js = self.args
-0001c9a0: 2e66 6f72 6365 5f6a 7320 6f72 2073 656c  .force_js or sel
-0001c9b0: 662e 636f 6f6b 6965 732e 6765 7428 226a  f.cookies.get("j
-0001c9c0: 7322 2920 3d3d 2022 7922 0a0a 2020 2020  s") == "y"..    
-0001c9d0: 2020 2020 6966 206e 6f74 2069 735f 6c73      if not is_ls
-0001c9e0: 2061 6e64 2028 7365 6c66 2e75 612e 7374   and (self.ua.st
-0001c9f0: 6172 7473 7769 7468 2822 6375 726c 2f22  artswith("curl/"
-0001ca00: 2920 6f72 2073 656c 662e 7561 2e73 7461  ) or self.ua.sta
-0001ca10: 7274 7377 6974 6828 2266 6574 6368 2229  rtswith("fetch")
-0001ca20: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-0001ca30: 656c 662e 7570 6172 616d 5b22 6c73 225d  elf.uparam["ls"]
-0001ca40: 203d 2022 7622 0a20 2020 2020 2020 2020   = "v".         
-0001ca50: 2020 2069 735f 6c73 203d 2054 7275 650a     is_ls = True.
-0001ca60: 0a20 2020 2020 2020 2074 706c 203d 2022  .        tpl = "
-0001ca70: 6272 6f77 7365 7222 0a20 2020 2020 2020  browser".       
-0001ca80: 2069 6620 2262 2220 696e 2073 656c 662e   if "b" in self.
-0001ca90: 7570 6172 616d 3a0a 2020 2020 2020 2020  uparam:.        
-0001caa0: 2020 2020 7470 6c20 3d20 2262 726f 7773      tpl = "brows
-0001cab0: 6572 3222 0a20 2020 2020 2020 2020 2020  er2".           
-0001cac0: 2069 735f 6a73 203d 2046 616c 7365 0a0a   is_js = False..
-0001cad0: 2020 2020 2020 2020 6c6f 6775 6573 203d          logues =
-0001cae0: 205b 2222 2c20 2222 5d0a 2020 2020 2020   ["", ""].      
-0001caf0: 2020 6966 206e 6f74 2073 656c 662e 6172    if not self.ar
-0001cb00: 6773 2e6e 6f5f 6c6f 6775 6573 3a0a 2020  gs.no_logues:.  
-0001cb10: 2020 2020 2020 2020 2020 666f 7220 6e2c            for n,
-0001cb20: 2066 6e20 696e 2065 6e75 6d65 7261 7465   fn in enumerate
-0001cb30: 285b 222e 7072 6f6c 6f67 7565 2e68 746d  ([".prologue.htm
-0001cb40: 6c22 2c20 222e 6570 696c 6f67 7565 2e68  l", ".epilogue.h
-0001cb50: 746d 6c22 5d29 3a0a 2020 2020 2020 2020  tml"]):.        
-0001cb60: 2020 2020 2020 2020 666e 203d 206f 732e          fn = os.
-0001cb70: 7061 7468 2e6a 6f69 6e28 6162 7370 6174  path.join(abspat
-0001cb80: 682c 2066 6e29 0a20 2020 2020 2020 2020  h, fn).         
-0001cb90: 2020 2020 2020 2069 6620 626f 732e 7061         if bos.pa
-0001cba0: 7468 2e65 7869 7374 7328 666e 293a 0a20  th.exists(fn):. 
-0001cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cbc0: 2020 2077 6974 6820 6f70 656e 2866 7365     with open(fse
-0001cbd0: 6e63 2866 6e29 2c20 2272 6222 2920 6173  nc(fn), "rb") as
-0001cbe0: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
-0001cbf0: 2020 2020 2020 2020 2020 2020 6c6f 6775              logu
-0001cc00: 6573 5b6e 5d20 3d20 662e 7265 6164 2829  es[n] = f.read()
-0001cc10: 2e64 6563 6f64 6528 2275 7466 2d38 2229  .decode("utf-8")
-0001cc20: 0a0a 2020 2020 2020 2020 7265 6164 6d65  ..        readme
-0001cc30: 203d 2022 220a 2020 2020 2020 2020 6966   = "".        if
-0001cc40: 206e 6f74 2073 656c 662e 6172 6773 2e6e   not self.args.n
-0001cc50: 6f5f 7265 6164 6d65 2061 6e64 206e 6f74  o_readme and not
-0001cc60: 206c 6f67 7565 735b 315d 3a0a 2020 2020   logues[1]:.    
-0001cc70: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
-0001cc80: 6e20 5b22 5245 4144 4d45 2e6d 6422 2c20  n ["README.md", 
-0001cc90: 2272 6561 646d 652e 6d64 225d 3a0a 2020  "readme.md"]:.  
-0001cca0: 2020 2020 2020 2020 2020 2020 2020 666e                fn
-0001ccb0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0001ccc0: 6162 7370 6174 682c 2066 6e29 0a20 2020  abspath, fn).   
-0001ccd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001cce0: 626f 732e 7061 7468 2e69 7366 696c 6528  bos.path.isfile(
-0001ccf0: 666e 293a 0a20 2020 2020 2020 2020 2020  fn):.           
-0001cd00: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-0001cd10: 656e 2866 7365 6e63 2866 6e29 2c20 2272  en(fsenc(fn), "r
-0001cd20: 6222 2920 6173 2066 3a0a 2020 2020 2020  b") as f:.      
-0001cd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd40: 2020 7265 6164 6d65 203d 2066 2e72 6561    readme = f.rea
-0001cd50: 6428 292e 6465 636f 6465 2822 7574 662d  d().decode("utf-
-0001cd60: 3822 290a 2020 2020 2020 2020 2020 2020  8").            
-0001cd70: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-0001cd80: 6b0a 0a20 2020 2020 2020 2076 6620 3d20  k..        vf = 
-0001cd90: 766e 2e66 6c61 6773 0a20 2020 2020 2020  vn.flags.       
-0001cda0: 2075 6e6c 6973 7420 3d20 7666 2e67 6574   unlist = vf.get
-0001cdb0: 2822 756e 6c69 7374 222c 2022 2229 0a20  ("unlist", ""). 
-0001cdc0: 2020 2020 2020 206c 735f 7265 7420 3d20         ls_ret = 
-0001cdd0: 7b0a 2020 2020 2020 2020 2020 2020 2264  {.            "d
-0001cde0: 6972 7322 3a20 5b5d 2c0a 2020 2020 2020  irs": [],.      
-0001cdf0: 2020 2020 2020 2266 696c 6573 223a 205b        "files": [
-0001ce00: 5d2c 0a20 2020 2020 2020 2020 2020 2022  ],.            "
-0001ce10: 7461 676c 6973 7422 3a20 5b5d 2c0a 2020  taglist": [],.  
-0001ce20: 2020 2020 2020 2020 2020 2273 7276 696e            "srvin
-0001ce30: 6622 3a20 7372 765f 696e 666f 742c 0a20  f": srv_infot,. 
-0001ce40: 2020 2020 2020 2020 2020 2022 6163 6374             "acct
-0001ce50: 223a 2073 656c 662e 756e 616d 652c 0a20  ": self.uname,. 
-0001ce60: 2020 2020 2020 2020 2020 2022 6964 7822             "idx"
-0001ce70: 3a20 6532 642c 0a20 2020 2020 2020 2020  : e2d,.         
-0001ce80: 2020 2022 6974 6167 223a 2065 3274 2c0a     "itag": e2t,.
-0001ce90: 2020 2020 2020 2020 2020 2020 226c 6966              "lif
-0001cea0: 6574 696d 6522 3a20 766e 2e66 6c61 6773  etime": vn.flags
-0001ceb0: 2e67 6574 2822 6c69 6665 7469 6d65 2229  .get("lifetime")
-0001cec0: 206f 7220 302c 0a20 2020 2020 2020 2020   or 0,.         
-0001ced0: 2020 2022 6672 616e 6422 3a20 626f 6f6c     "frand": bool
-0001cee0: 2876 6e2e 666c 6167 732e 6765 7428 2272  (vn.flags.get("r
-0001cef0: 616e 6422 2929 2c0a 2020 2020 2020 2020  and")),.        
-0001cf00: 2020 2020 2275 6e6c 6973 7422 3a20 756e      "unlist": un
-0001cf10: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
-0001cf20: 2020 2270 6572 6d73 223a 2070 6572 6d73    "perms": perms
-0001cf30: 2c0a 2020 2020 2020 2020 2020 2020 226c  ,.            "l
-0001cf40: 6f67 7565 7322 3a20 6c6f 6775 6573 2c0a  ogues": logues,.
-0001cf50: 2020 2020 2020 2020 2020 2020 2272 6561              "rea
-0001cf60: 646d 6522 3a20 7265 6164 6d65 2c0a 2020  dme": readme,.  
-0001cf70: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-0001cf80: 6a32 6120 3d20 7b0a 2020 2020 2020 2020  j2a = {.        
-0001cf90: 2020 2020 2276 6469 7222 3a20 7175 6f74      "vdir": quot
-0001cfa0: 6570 2873 656c 662e 7670 6174 6829 2c0a  ep(self.vpath),.
-0001cfb0: 2020 2020 2020 2020 2020 2020 2276 706e              "vpn
-0001cfc0: 6f64 6573 223a 2076 706e 6f64 6573 2c0a  odes": vpnodes,.
-0001cfd0: 2020 2020 2020 2020 2020 2020 2266 696c              "fil
-0001cfe0: 6573 223a 205b 5d2c 0a20 2020 2020 2020  es": [],.       
-0001cff0: 2020 2020 2022 6c73 3022 3a20 4e6f 6e65       "ls0": None
-0001d000: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
-0001d010: 6363 7422 3a20 7365 6c66 2e75 6e61 6d65  cct": self.uname
-0001d020: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
-0001d030: 6572 6d73 223a 206a 736f 6e2e 6475 6d70  erms": json.dump
-0001d040: 7328 7065 726d 7329 2c0a 2020 2020 2020  s(perms),.      
-0001d050: 2020 2020 2020 226c 6966 6574 696d 6522        "lifetime"
-0001d060: 3a20 6c73 5f72 6574 5b22 6c69 6665 7469  : ls_ret["lifeti
-0001d070: 6d65 225d 2c0a 2020 2020 2020 2020 2020  me"],.          
-0001d080: 2020 2266 7261 6e64 223a 2062 6f6f 6c28    "frand": bool(
-0001d090: 766e 2e66 6c61 6773 2e67 6574 2822 7261  vn.flags.get("ra
-0001d0a0: 6e64 2229 292c 0a20 2020 2020 2020 2020  nd")),.         
-0001d0b0: 2020 2022 7461 676c 6973 7422 3a20 5b5d     "taglist": []
-0001d0c0: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
-0001d0d0: 6566 5f68 636f 6c73 223a 205b 5d2c 0a20  ef_hcols": [],. 
-0001d0e0: 2020 2020 2020 2020 2020 2022 6861 7665             "have
-0001d0f0: 5f65 6d70 223a 2073 656c 662e 6172 6773  _emp": self.args
-0001d100: 2e65 6d70 2c0a 2020 2020 2020 2020 2020  .emp,.          
-0001d110: 2020 2268 6176 655f 7570 326b 5f69 6478    "have_up2k_idx
-0001d120: 223a 2065 3264 2c0a 2020 2020 2020 2020  ": e2d,.        
-0001d130: 2020 2020 2268 6176 655f 7461 6773 5f69      "have_tags_i
-0001d140: 6478 223a 2065 3274 2c0a 2020 2020 2020  dx": e2t,.      
-0001d150: 2020 2020 2020 2268 6176 655f 6163 6f64        "have_acod
-0001d160: 6522 3a20 286e 6f74 2073 656c 662e 6172  e": (not self.ar
-0001d170: 6773 2e6e 6f5f 6163 6f64 6529 2c0a 2020  gs.no_acode),.  
-0001d180: 2020 2020 2020 2020 2020 2268 6176 655f            "have_
-0001d190: 6d76 223a 2028 6e6f 7420 7365 6c66 2e61  mv": (not self.a
-0001d1a0: 7267 732e 6e6f 5f6d 7629 2c0a 2020 2020  rgs.no_mv),.    
-0001d1b0: 2020 2020 2020 2020 2268 6176 655f 6465          "have_de
-0001d1c0: 6c22 3a20 286e 6f74 2073 656c 662e 6172  l": (not self.ar
-0001d1d0: 6773 2e6e 6f5f 6465 6c29 2c0a 2020 2020  gs.no_del),.    
-0001d1e0: 2020 2020 2020 2020 2268 6176 655f 7a69          "have_zi
-0001d1f0: 7022 3a20 286e 6f74 2073 656c 662e 6172  p": (not self.ar
-0001d200: 6773 2e6e 6f5f 7a69 7029 2c0a 2020 2020  gs.no_zip),.    
-0001d210: 2020 2020 2020 2020 2268 6176 655f 756e          "have_un
-0001d220: 706f 7374 223a 2069 6e74 2873 656c 662e  post": int(self.
-0001d230: 6172 6773 2e75 6e70 6f73 7429 2c0a 2020  args.unpost),.  
-0001d240: 2020 2020 2020 2020 2020 2268 6176 655f            "have_
-0001d250: 625f 7522 3a20 2873 656c 662e 6361 6e5f  b_u": (self.can_
-0001d260: 7772 6974 6520 616e 6420 7365 6c66 2e75  write and self.u
-0001d270: 7061 7261 6d2e 6765 7428 2262 2229 203d  param.get("b") =
-0001d280: 3d20 2275 2229 2c0a 2020 2020 2020 2020  = "u"),.        
-0001d290: 2020 2020 2273 625f 6d64 223a 2022 2220      "sb_md": "" 
-0001d2a0: 6966 2022 6e6f 5f73 625f 6d64 2220 696e  if "no_sb_md" in
-0001d2b0: 2076 6620 656c 7365 2028 7666 2e67 6574   vf else (vf.get
-0001d2c0: 2822 6d64 5f73 6266 2229 206f 7220 2279  ("md_sbf") or "y
-0001d2d0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-0001d2e0: 2273 625f 6c67 223a 2022 2220 6966 2022  "sb_lg": "" if "
-0001d2f0: 6e6f 5f73 625f 6c67 2220 696e 2076 6620  no_sb_lg" in vf 
-0001d300: 656c 7365 2028 7666 2e67 6574 2822 6c67  else (vf.get("lg
-0001d310: 5f73 6266 2229 206f 7220 2279 2229 2c0a  _sbf") or "y"),.
-0001d320: 2020 2020 2020 2020 2020 2020 2275 726c              "url
-0001d330: 5f73 7566 223a 2075 726c 5f73 7566 2c0a  _suf": url_suf,.
-0001d340: 2020 2020 2020 2020 2020 2020 226c 6f67              "log
-0001d350: 7565 7322 3a20 6c6f 6775 6573 2c0a 2020  ues": logues,.  
-0001d360: 2020 2020 2020 2020 2020 2272 6561 646d            "readm
-0001d370: 6522 3a20 7265 6164 6d65 2c0a 2020 2020  e": readme,.    
-0001d380: 2020 2020 2020 2020 2274 6974 6c65 223a          "title":
-0001d390: 2068 746d 6c5f 6573 6361 7065 2873 656c   html_escape(sel
-0001d3a0: 662e 7670 6174 682c 2063 726c 663d 5472  f.vpath, crlf=Tr
-0001d3b0: 7565 2920 6f72 2022 f09f 92be f09f 8e89  ue) or "........
-0001d3c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-0001d3d0: 7372 765f 696e 666f 223a 2073 7276 5f69  srv_info": srv_i
-0001d3e0: 6e66 6f74 2c0a 2020 2020 2020 2020 2020  nfot,.          
-0001d3f0: 2020 2264 6772 6964 223a 2022 6772 6964    "dgrid": "grid
-0001d400: 2220 696e 2076 662c 0a20 2020 2020 2020  " in vf,.       
-0001d410: 2020 2020 2022 756e 6c69 7374 223a 2075       "unlist": u
-0001d420: 6e6c 6973 742c 0a20 2020 2020 2020 2020  nlist,.         
-0001d430: 2020 2022 6474 6865 6d65 223a 2073 656c     "dtheme": sel
-0001d440: 662e 6172 6773 2e74 6865 6d65 2c0a 2020  f.args.theme,.  
-0001d450: 2020 2020 2020 2020 2020 2274 6865 6d65            "theme
-0001d460: 7322 3a20 7365 6c66 2e61 7267 732e 7468  s": self.args.th
-0001d470: 656d 6573 2c0a 2020 2020 2020 2020 2020  emes,.          
-0001d480: 2020 2274 7572 626f 6c76 6c22 3a20 7365    "turbolvl": se
-0001d490: 6c66 2e61 7267 732e 7475 7262 6f2c 0a20  lf.args.turbo,. 
-0001d4a0: 2020 2020 2020 2020 2020 2022 6964 7868             "idxh
-0001d4b0: 223a 2069 6e74 2873 656c 662e 6172 6773  ": int(self.args
-0001d4c0: 2e69 6829 2c0a 2020 2020 2020 2020 2020  .ih),.          
-0001d4d0: 2020 2275 3273 6f72 7422 3a20 7365 6c66    "u2sort": self
-0001d4e0: 2e61 7267 732e 7532 736f 7274 2c0a 2020  .args.u2sort,.  
-0001d4f0: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
-0001d500: 2069 6620 7365 6c66 2e61 7267 732e 6a73   if self.args.js
-0001d510: 5f62 726f 7773 6572 3a0a 2020 2020 2020  _browser:.      
-0001d520: 2020 2020 2020 6a32 615b 226a 7322 5d20        j2a["js"] 
-0001d530: 3d20 7365 6c66 2e61 7267 732e 6a73 5f62  = self.args.js_b
-0001d540: 726f 7773 6572 0a0a 2020 2020 2020 2020  rowser..        
-0001d550: 6966 2073 656c 662e 6172 6773 2e63 7373  if self.args.css
-0001d560: 5f62 726f 7773 6572 3a0a 2020 2020 2020  _browser:.      
-0001d570: 2020 2020 2020 6a32 615b 2263 7373 225d        j2a["css"]
-0001d580: 203d 2073 656c 662e 6172 6773 2e63 7373   = self.args.css
-0001d590: 5f62 726f 7773 6572 0a0a 2020 2020 2020  _browser..      
-0001d5a0: 2020 6966 206e 6f74 2073 656c 662e 636f    if not self.co
-0001d5b0: 6e6e 2e68 7372 762e 7072 6973 6d3a 0a20  nn.hsrv.prism:. 
-0001d5c0: 2020 2020 2020 2020 2020 206a 3261 5b22             j2a["
-0001d5d0: 6e6f 5f70 7269 736d 225d 203d 2054 7275  no_prism"] = Tru
-0001d5e0: 650a 0a20 2020 2020 2020 2069 6620 6e6f  e..        if no
-0001d5f0: 7420 7365 6c66 2e63 616e 5f72 6561 643a  t self.can_read:
-0001d600: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001d610: 6973 5f6c 733a 0a20 2020 2020 2020 2020  is_ls:.         
-0001d620: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001d630: 6c66 2e74 785f 6c73 286c 735f 7265 7429  lf.tx_ls(ls_ret)
-0001d640: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001d650: 206e 6f74 2073 7461 742e 535f 4953 4449   not stat.S_ISDI
-0001d660: 5228 7374 2e73 745f 6d6f 6465 293a 0a20  R(st.st_mode):. 
-0001d670: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001d680: 6574 7572 6e20 7365 6c66 2e74 785f 3430  eturn self.tx_40
-0001d690: 3428 5472 7565 290a 0a20 2020 2020 2020  4(True)..       
-0001d6a0: 2020 2020 2069 6620 227a 6970 2220 696e       if "zip" in
-0001d6b0: 2073 656c 662e 7570 6172 616d 206f 7220   self.uparam or 
-0001d6c0: 2274 6172 2220 696e 2073 656c 662e 7570  "tar" in self.up
-0001d6d0: 6172 616d 3a0a 2020 2020 2020 2020 2020  aram:.          
-0001d6e0: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-0001d6f0: 6163 2834 3033 290a 0a20 2020 2020 2020  ac(403)..       
-0001d700: 2020 2020 2068 746d 6c20 3d20 7365 6c66       html = self
-0001d710: 2e6a 3273 2874 706c 2c20 2a2a 6a32 6129  .j2s(tpl, **j2a)
-0001d720: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001d730: 662e 7265 706c 7928 6874 6d6c 2e65 6e63  f.reply(html.enc
-0001d740: 6f64 6528 2275 7466 2d38 222c 2022 7265  ode("utf-8", "re
-0001d750: 706c 6163 6522 2929 0a20 2020 2020 2020  place")).       
-0001d760: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-0001d770: 0a0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
-0001d780: 696e 205b 227a 6970 222c 2022 7461 7222  in ["zip", "tar"
-0001d790: 5d3a 0a20 2020 2020 2020 2020 2020 2076  ]:.            v
-0001d7a0: 203d 2073 656c 662e 7570 6172 616d 2e67   = self.uparam.g
-0001d7b0: 6574 286b 290a 2020 2020 2020 2020 2020  et(k).          
-0001d7c0: 2020 6966 2076 2069 7320 6e6f 7420 4e6f    if v is not No
-0001d7d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001d7e0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-0001d7f0: 7478 5f7a 6970 286b 2c20 762c 2073 656c  tx_zip(k, v, sel
-0001d800: 662e 7670 6174 682c 2076 6e2c 2072 656d  f.vpath, vn, rem
-0001d810: 2c20 5b5d 2c20 7365 6c66 2e61 7267 732e  , [], self.args.
-0001d820: 6564 290a 0a20 2020 2020 2020 2066 7372  ed)..        fsr
-0001d830: 6f6f 742c 2076 6673 5f6c 732c 2076 6673  oot, vfs_ls, vfs
-0001d840: 5f76 6972 7420 3d20 766e 2e6c 7328 0a20  _virt = vn.ls(. 
-0001d850: 2020 2020 2020 2020 2020 2072 656d 2c0a             rem,.
-0001d860: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001d870: 2e75 6e61 6d65 2c0a 2020 2020 2020 2020  .uname,.        
-0001d880: 2020 2020 6e6f 7420 7365 6c66 2e61 7267      not self.arg
-0001d890: 732e 6e6f 5f73 6361 6e64 6972 2c0a 2020  s.no_scandir,.  
-0001d8a0: 2020 2020 2020 2020 2020 5b5b 5472 7565            [[True
-0001d8b0: 2c20 4661 6c73 655d 2c20 5b46 616c 7365  , False], [False
-0001d8c0: 2c20 5472 7565 5d5d 2c0a 2020 2020 2020  , True]],.      
-0001d8d0: 2020 2020 2020 6c73 7461 743d 226c 7422        lstat="lt"
-0001d8e0: 2069 6e20 7365 6c66 2e75 7061 7261 6d2c   in self.uparam,
-0001d8f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0001d900: 2020 2073 7461 7473 203d 207b 6b3a 2076     stats = {k: v
-0001d910: 2066 6f72 206b 2c20 7620 696e 2076 6673   for k, v in vfs
-0001d920: 5f6c 737d 0a20 2020 2020 2020 206c 735f  _ls}.        ls_
-0001d930: 6e61 6d65 7320 3d20 5b78 5b30 5d20 666f  names = [x[0] fo
-0001d940: 7220 7820 696e 2076 6673 5f6c 735d 0a20  r x in vfs_ls]. 
-0001d950: 2020 2020 2020 206c 735f 6e61 6d65 732e         ls_names.
-0001d960: 6578 7465 6e64 286c 6973 7428 7666 735f  extend(list(vfs_
-0001d970: 7669 7274 2e6b 6579 7328 2929 290a 0a20  virt.keys())).. 
-0001d980: 2020 2020 2020 2023 2063 6865 636b 2066         # check f
-0001d990: 6f72 206f 6c64 2076 6572 7369 6f6e 7320  or old versions 
-0001d9a0: 6f66 2066 696c 6573 2c0a 2020 2020 2020  of files,.      
-0001d9b0: 2020 2320 5b6e 756d 2d62 6163 6b75 7073    # [num-backups
-0001d9c0: 2c20 6d6f 7374 2d72 6563 656e 742c 2068  , most-recent, h
-0001d9d0: 6973 742d 7061 7468 5d0a 2020 2020 2020  ist-path].      
-0001d9e0: 2020 6869 7374 2020 2020 203d 207b 7d0a    hist     = {}.
-0001d9f0: 2020 2020 2020 2020 6869 7374 6469 7220          histdir 
-0001da00: 3d20 6f73 2e70 6174 682e 6a6f 696e 2866  = os.path.join(f
-0001da10: 7372 6f6f 742c 2022 2e68 6973 7422 290a  sroot, ".hist").
-0001da20: 2020 2020 2020 2020 7074 6e20 3d20 7265          ptn = re
-0001da30: 2e63 6f6d 7069 6c65 2872 2228 2e2a 295c  .compile(r"(.*)\
-0001da40: 2e28 5b30 2d39 5d2b 5c2e 5b30 2d39 5d7b  .([0-9]+\.[0-9]{
-0001da50: 337d 2928 5c2e 5b5e 5c2e 5d2b 2924 2229  3})(\.[^\.]+)$")
-0001da60: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0001da70: 2020 2020 2020 2020 2020 666f 7220 6866            for hf
-0001da80: 6e20 696e 2062 6f73 2e6c 6973 7464 6972  n in bos.listdir
-0001da90: 2868 6973 7464 6972 293a 0a20 2020 2020  (histdir):.     
-0001daa0: 2020 2020 2020 2020 2020 206d 203d 2070             m = p
-0001dab0: 746e 2e6d 6174 6368 2868 666e 290a 2020  tn.match(hfn).  
-0001dac0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001dad0: 206e 6f74 206d 3a0a 2020 2020 2020 2020   not m:.        
-0001dae0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0001daf0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-0001db00: 2020 2020 2020 666e 203d 206d 2e67 726f        fn = m.gro
-0001db10: 7570 2831 2920 2b20 6d2e 6772 6f75 7028  up(1) + m.group(
-0001db20: 3329 0a20 2020 2020 2020 2020 2020 2020  3).             
-0001db30: 2020 206e 2c20 7473 2c20 5f20 3d20 6869     n, ts, _ = hi
-0001db40: 7374 2e67 6574 2866 6e2c 2028 302c 2030  st.get(fn, (0, 0
-0001db50: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
-0001db60: 2020 2020 2020 2068 6973 745b 666e 5d20         hist[fn] 
-0001db70: 3d20 286e 202b 2031 2c20 6d61 7828 7473  = (n + 1, max(ts
-0001db80: 2c20 666c 6f61 7428 6d2e 6772 6f75 7028  , float(m.group(
-0001db90: 3229 2929 2c20 6866 6e29 0a20 2020 2020  2))), hfn).     
-0001dba0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
-0001dbb0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-0001dbc0: 2020 2020 2023 2073 686f 7720 646f 7466       # show dotf
-0001dbd0: 696c 6573 2069 6620 7065 726d 6974 7465  iles if permitte
-0001dbe0: 6420 616e 6420 7265 7175 6573 7465 640a  d and requested.
-0001dbf0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-0001dc00: 656c 662e 6172 6773 2e65 6420 6f72 2022  elf.args.ed or "
-0001dc10: 646f 7473 2220 6e6f 7420 696e 2073 656c  dots" not in sel
-0001dc20: 662e 7570 6172 616d 3a0a 2020 2020 2020  f.uparam:.      
-0001dc30: 2020 2020 2020 6c73 5f6e 616d 6573 203d        ls_names =
-0001dc40: 2065 7863 6c75 6465 5f64 6f74 6669 6c65   exclude_dotfile
-0001dc50: 7328 6c73 5f6e 616d 6573 290a 0a20 2020  s(ls_names)..   
-0001dc60: 2020 2020 2061 6464 5f66 6b20 3d20 766e       add_fk = vn
-0001dc70: 2e66 6c61 6773 2e67 6574 2822 666b 2229  .flags.get("fk")
-0001dc80: 0a0a 2020 2020 2020 2020 6469 7273 203d  ..        dirs =
-0001dc90: 205b 5d0a 2020 2020 2020 2020 6669 6c65   [].        file
-0001dca0: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
-0001dcb0: 6f72 2066 6e20 696e 206c 735f 6e61 6d65  or fn in ls_name
-0001dcc0: 733a 0a20 2020 2020 2020 2020 2020 2062  s:.            b
-0001dcd0: 6173 6520 3d20 2222 0a20 2020 2020 2020  ase = "".       
-0001dce0: 2020 2020 2068 7265 6620 3d20 666e 0a20       href = fn. 
-0001dcf0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0001dd00: 7420 6973 5f6c 7320 616e 6420 6e6f 7420  t is_ls and not 
-0001dd10: 6973 5f6a 7320 616e 6420 6e6f 7420 7365  is_js and not se
-0001dd20: 6c66 2e74 7261 696c 696e 675f 736c 6173  lf.trailing_slas
-0001dd30: 6820 616e 6420 7670 6174 683a 0a20 2020  h and vpath:.   
-0001dd40: 2020 2020 2020 2020 2020 2020 2062 6173               bas
-0001dd50: 6520 3d20 222f 2220 2b20 7670 6174 6820  e = "/" + vpath 
-0001dd60: 2b20 222f 220a 2020 2020 2020 2020 2020  + "/".          
-0001dd70: 2020 2020 2020 6872 6566 203d 2062 6173        href = bas
-0001dd80: 6520 2b20 666e 0a0a 2020 2020 2020 2020  e + fn..        
-0001dd90: 2020 2020 6966 2066 6e20 696e 2076 6673      if fn in vfs
-0001dda0: 5f76 6972 743a 0a20 2020 2020 2020 2020  _virt:.         
-0001ddb0: 2020 2020 2020 2066 7370 6174 6820 3d20         fspath = 
-0001ddc0: 7666 735f 7669 7274 5b66 6e5d 2e72 6561  vfs_virt[fn].rea
-0001ddd0: 6c70 6174 680a 2020 2020 2020 2020 2020  lpath.          
-0001dde0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001ddf0: 2020 2020 2020 2020 6673 7061 7468 203d          fspath =
-0001de00: 2066 7372 6f6f 7420 2b20 222f 2220 2b20   fsroot + "/" + 
-0001de10: 666e 0a0a 2020 2020 2020 2020 2020 2020  fn..            
-0001de20: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-0001de30: 2020 2020 206c 696e 6620 3d20 7374 6174       linf = stat
-0001de40: 732e 6765 7428 666e 2920 6f72 2062 6f73  s.get(fn) or bos
-0001de50: 2e6c 7374 6174 2866 7370 6174 6829 0a20  .lstat(fspath). 
-0001de60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001de70: 6e66 203d 2062 6f73 2e73 7461 7428 6673  nf = bos.stat(fs
-0001de80: 7061 7468 2920 6966 2073 7461 742e 535f  path) if stat.S_
-0001de90: 4953 4c4e 4b28 6c69 6e66 2e73 745f 6d6f  ISLNK(linf.st_mo
-0001dea0: 6465 2920 656c 7365 206c 696e 660a 2020  de) else linf.  
-0001deb0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0001dec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001ded0: 2020 7365 6c66 2e6c 6f67 2822 6272 6f6b    self.log("brok
-0001dee0: 656e 2073 796d 6c69 6e6b 3a20 7b7d 222e  en symlink: {}".
-0001def0: 666f 726d 6174 2872 6570 7228 6673 7061  format(repr(fspa
-0001df00: 7468 2929 290a 2020 2020 2020 2020 2020  th))).          
-0001df10: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-0001df20: 2020 2020 2020 2020 2020 2020 6973 5f64              is_d
-0001df30: 6972 203d 2073 7461 742e 535f 4953 4449  ir = stat.S_ISDI
-0001df40: 5228 696e 662e 7374 5f6d 6f64 6529 0a20  R(inf.st_mode). 
-0001df50: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0001df60: 5f64 6972 3a0a 2020 2020 2020 2020 2020  _dir:.          
-0001df70: 2020 2020 2020 6872 6566 202b 3d20 222f        href += "/
-0001df80: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001df90: 2020 6966 2073 656c 662e 6172 6773 2e6e    if self.args.n
-0001dfa0: 6f5f 7a69 703a 0a20 2020 2020 2020 2020  o_zip:.         
-0001dfb0: 2020 2020 2020 2020 2020 206d 6172 6769             margi
-0001dfc0: 6e20 3d20 2244 4952 220a 2020 2020 2020  n = "DIR".      
-0001dfd0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dff0: 2020 2020 6d61 7267 696e 203d 2027 3c61      margin = '<a
-0001e000: 2068 7265 663d 2225 733f 7a69 7022 2072   href="%s?zip" r
-0001e010: 656c 3d22 6e6f 666f 6c6c 6f77 223e 7a69  el="nofollow">zi
-0001e020: 703c 2f61 3e27 2025 2028 7175 6f74 6570  p</a>' % (quotep
-0001e030: 2868 7265 6629 2c29 0a20 2020 2020 2020  (href),).       
-0001e040: 2020 2020 2065 6c69 6620 666e 2069 6e20       elif fn in 
-0001e050: 6869 7374 3a0a 2020 2020 2020 2020 2020  hist:.          
-0001e060: 2020 2020 2020 6d61 7267 696e 203d 2027        margin = '
-0001e070: 3c61 2068 7265 663d 2225 732e 6869 7374  <a href="%s.hist
-0001e080: 2f25 7322 3e23 2573 3c2f 613e 2720 2520  /%s">#%s</a>' % 
-0001e090: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0001e0a0: 2020 2020 2020 6261 7365 2c0a 2020 2020        base,.    
-0001e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0c0: 6874 6d6c 5f65 7363 6170 6528 6869 7374  html_escape(hist
-0001e0d0: 5b66 6e5d 5b32 5d2c 2071 756f 743d 5472  [fn][2], quot=Tr
-0001e0e0: 7565 2c20 6372 6c66 3d54 7275 6529 2c0a  ue, crlf=True),.
-0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e100: 2020 2020 6869 7374 5b66 6e5d 5b30 5d2c      hist[fn][0],
-0001e110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e120: 2029 0a20 2020 2020 2020 2020 2020 2065   ).            e
-0001e130: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001e140: 2020 2020 206d 6172 6769 6e20 3d20 222d       margin = "-
-0001e150: 220a 0a20 2020 2020 2020 2020 2020 2073  "..            s
-0001e160: 7a20 3d20 696e 662e 7374 5f73 697a 650a  z = inf.st_size.
-0001e170: 2020 2020 2020 2020 2020 2020 7a64 203d              zd =
-0001e180: 2064 6174 6574 696d 652e 7574 6366 726f   datetime.utcfro
-0001e190: 6d74 696d 6573 7461 6d70 286c 696e 662e  mtimestamp(linf.
-0001e1a0: 7374 5f6d 7469 6d65 290a 2020 2020 2020  st_mtime).      
-0001e1b0: 2020 2020 2020 6474 203d 2022 2530 3464        dt = "%04d
-0001e1c0: 2d25 3032 642d 2530 3264 2025 3032 643a  -%02d-%02d %02d:
-0001e1d0: 2530 3264 3a25 3032 6422 2025 2028 0a20  %02d:%02d" % (. 
-0001e1e0: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-0001e1f0: 642e 7965 6172 2c0a 2020 2020 2020 2020  d.year,.        
-0001e200: 2020 2020 2020 2020 7a64 2e6d 6f6e 7468          zd.month
-0001e210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001e220: 2020 7a64 2e64 6179 2c0a 2020 2020 2020    zd.day,.      
-0001e230: 2020 2020 2020 2020 2020 7a64 2e68 6f75            zd.hou
-0001e240: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0001e250: 2020 207a 642e 6d69 6e75 7465 2c0a 2020     zd.minute,.  
-0001e260: 2020 2020 2020 2020 2020 2020 2020 7a64                zd
-0001e270: 2e73 6563 6f6e 642c 0a20 2020 2020 2020  .second,.       
-0001e280: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0001e290: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0001e2a0: 2020 2020 2020 2020 2065 7874 203d 2022           ext = "
-0001e2b0: 2d2d 2d22 2069 6620 6973 5f64 6972 2065  ---" if is_dir e
-0001e2c0: 6c73 6520 666e 2e72 7370 6c69 7428 222e  lse fn.rsplit(".
-0001e2d0: 222c 2031 295b 315d 0a20 2020 2020 2020  ", 1)[1].       
-0001e2e0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-0001e2f0: 6578 7429 203e 2031 363a 0a20 2020 2020  ext) > 16:.     
-0001e300: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0001e310: 7874 203d 2065 7874 5b3a 3136 5d0a 2020  xt = ext[:16].  
-0001e320: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0001e330: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e340: 2020 6578 7420 3d20 2225 220a 0a20 2020    ext = "%"..   
-0001e350: 2020 2020 2020 2020 2069 6620 6164 645f           if add_
-0001e360: 666b 3a0a 2020 2020 2020 2020 2020 2020  fk:.            
-0001e370: 2020 2020 6872 6566 203d 2022 2573 3f6b      href = "%s?k
-0001e380: 3d25 7322 2025 2028 0a20 2020 2020 2020  =%s" % (.       
-0001e390: 2020 2020 2020 2020 2020 2020 2071 756f               quo
-0001e3a0: 7465 7028 6872 6566 292c 0a20 2020 2020  tep(href),.     
-0001e3b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001e3c0: 656c 662e 6765 6e5f 666b 280a 2020 2020  elf.gen_fk(.    
-0001e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3e0: 2020 2020 7365 6c66 2e61 7267 732e 666b      self.args.fk
-0001e3f0: 5f73 616c 742c 2066 7370 6174 682c 2073  _salt, fspath, s
-0001e400: 7a2c 2030 2069 6620 414e 5957 494e 2065  z, 0 if ANYWIN e
-0001e410: 6c73 6520 696e 662e 7374 5f69 6e6f 0a20  lse inf.st_ino. 
-0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e430: 2020 2029 5b3a 6164 645f 666b 5d2c 0a20     )[:add_fk],. 
-0001e440: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001e450: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001e460: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001e470: 2020 2068 7265 6620 3d20 7175 6f74 6570     href = quotep
-0001e480: 2868 7265 6629 0a0a 2020 2020 2020 2020  (href)..        
-0001e490: 2020 2020 6974 656d 203d 207b 0a20 2020      item = {.   
-0001e4a0: 2020 2020 2020 2020 2020 2020 2022 6c65               "le
-0001e4b0: 6164 223a 206d 6172 6769 6e2c 0a20 2020  ad": margin,.   
-0001e4c0: 2020 2020 2020 2020 2020 2020 2022 6872               "hr
-0001e4d0: 6566 223a 2068 7265 662c 0a20 2020 2020  ef": href,.     
-0001e4e0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-0001e4f0: 223a 2066 6e2c 0a20 2020 2020 2020 2020  ": fn,.         
-0001e500: 2020 2020 2020 2022 737a 223a 2073 7a2c         "sz": sz,
-0001e510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e520: 2022 6578 7422 3a20 6578 742c 0a20 2020   "ext": ext,.   
-0001e530: 2020 2020 2020 2020 2020 2020 2022 6474               "dt
-0001e540: 223a 2064 742c 0a20 2020 2020 2020 2020  ": dt,.         
-0001e550: 2020 2020 2020 2022 7473 223a 2069 6e74         "ts": int
-0001e560: 286c 696e 662e 7374 5f6d 7469 6d65 292c  (linf.st_mtime),
-0001e570: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
-0001e580: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0001e590: 5f64 6972 3a0a 2020 2020 2020 2020 2020  _dir:.          
-0001e5a0: 2020 2020 2020 6469 7273 2e61 7070 656e        dirs.appen
-0001e5b0: 6428 6974 656d 290a 2020 2020 2020 2020  d(item).        
-0001e5c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0001e5d0: 2020 2020 2020 2020 2020 6669 6c65 732e            files.
-0001e5e0: 6170 7065 6e64 2869 7465 6d29 0a20 2020  append(item).   
-0001e5f0: 2020 2020 2020 2020 2020 2020 2069 7465               ite
-0001e600: 6d5b 2272 6422 5d20 3d20 7265 6d0a 0a20  m["rd"] = rem.. 
-0001e610: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0001e620: 2020 2020 2020 2020 7365 6c66 2e63 6f6f          self.coo
-0001e630: 6b69 6573 2e67 6574 2822 6964 7868 2229  kies.get("idxh")
-0001e640: 203d 3d20 2279 220a 2020 2020 2020 2020   == "y".        
-0001e650: 2020 2020 616e 6420 226c 7322 206e 6f74      and "ls" not
-0001e660: 2069 6e20 7365 6c66 2e75 7061 7261 6d0a   in self.uparam.
-0001e670: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001e680: 2276 2220 6e6f 7420 696e 2073 656c 662e  "v" not in self.
-0001e690: 7570 6172 616d 0a20 2020 2020 2020 2029  uparam.        )
-0001e6a0: 3a0a 2020 2020 2020 2020 2020 2020 6964  :.            id
-0001e6b0: 785f 6874 6d6c 203d 2073 6574 285b 2269  x_html = set(["i
-0001e6c0: 6e64 6578 2e68 746d 222c 2022 696e 6465  ndex.htm", "inde
-0001e6d0: 782e 6874 6d6c 225d 290a 2020 2020 2020  x.html"]).      
-0001e6e0: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-0001e6f0: 6e20 6669 6c65 733a 0a20 2020 2020 2020  n files:.       
-0001e700: 2020 2020 2020 2020 2069 6620 6974 656d           if item
-0001e710: 5b22 6e61 6d65 225d 2069 6e20 6964 785f  ["name"] in idx_
-0001e720: 6874 6d6c 3a0a 2020 2020 2020 2020 2020  html:.          
-0001e730: 2020 2020 2020 2020 2020 2320 646f 2066            # do f
-0001e740: 756c 6c20 7265 736f 6c76 6520 696e 2063  ull resolve in c
-0001e750: 6173 6520 6f66 2073 6861 646f 7765 6420  ase of shadowed 
-0001e760: 6669 6c65 0a20 2020 2020 2020 2020 2020  file.           
-0001e770: 2020 2020 2020 2020 2076 7020 3d20 766a           vp = vj
-0001e780: 6f69 6e28 7365 6c66 2e76 7061 7468 2e73  oin(self.vpath.s
-0001e790: 706c 6974 2822 3f22 295b 305d 2c20 6974  plit("?")[0], it
-0001e7a0: 656d 5b22 6e61 6d65 225d 290a 2020 2020  em["name"]).    
-0001e7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7c0: 766e 2c20 7265 6d20 3d20 7365 6c66 2e61  vn, rem = self.a
-0001e7d0: 7372 762e 7666 732e 6765 7428 7670 2c20  srv.vfs.get(vp, 
-0001e7e0: 7365 6c66 2e75 6e61 6d65 2c20 5472 7565  self.uname, True
-0001e7f0: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
-0001e800: 2020 2020 2020 2020 2020 2020 2061 7020               ap 
-0001e810: 3d20 766e 2e63 616e 6f6e 6963 616c 2872  = vn.canonical(r
-0001e820: 656d 290a 2020 2020 2020 2020 2020 2020  em).            
-0001e830: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0001e840: 656c 662e 7478 5f66 696c 6528 6170 2920  elf.tx_file(ap) 
-0001e850: 2023 2069 7320 6e6f 2d63 6163 6865 0a0a   # is no-cache..
-0001e860: 2020 2020 2020 2020 7461 6773 6574 2020          tagset  
-0001e870: 3d20 7365 7428 290a 2020 2020 2020 2020  = set().        
-0001e880: 666f 7220 6665 2069 6e20 6669 6c65 733a  for fe in files:
-0001e890: 0a20 2020 2020 2020 2020 2020 2066 6e20  .            fn 
-0001e8a0: 3d20 6665 5b22 6e61 6d65 225d 0a20 2020  = fe["name"].   
-0001e8b0: 2020 2020 2020 2020 2072 6420 3d20 6665           rd = fe
-0001e8c0: 5b22 7264 225d 0a20 2020 2020 2020 2020  ["rd"].         
-0001e8d0: 2020 2064 656c 2066 655b 2272 6422 5d0a     del fe["rd"].
-0001e8e0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001e8f0: 6f74 2069 6375 723a 0a20 2020 2020 2020  ot icur:.       
-0001e900: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0001e910: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
-0001e920: 6620 766e 2021 3d20 6462 763a 0a20 2020  f vn != dbv:.   
-0001e930: 2020 2020 2020 2020 2020 2020 205f 2c20               _, 
-0001e940: 7264 203d 2076 6e2e 6765 745f 6462 7628  rd = vn.get_dbv(
-0001e950: 7264 290a 0a20 2020 2020 2020 2020 2020  rd)..           
-0001e960: 2065 7264 5f65 666e 203d 2028 7264 2c20   erd_efn = (rd, 
-0001e970: 666e 290a 2020 2020 2020 2020 2020 2020  fn).            
-0001e980: 7120 3d20 2273 656c 6563 7420 6d74 2e6b  q = "select mt.k
-0001e990: 2c20 6d74 2e76 2066 726f 6d20 7570 2069  , mt.v from up i
-0001e9a0: 6e6e 6572 206a 6f69 6e20 6d74 206f 6e20  nner join mt on 
-0001e9b0: 6d74 2e77 203d 2073 7562 7374 7228 7570  mt.w = substr(up
-0001e9c0: 2e77 2c31 2c31 3629 2077 6865 7265 2075  .w,1,16) where u
-0001e9d0: 702e 7264 203d 203f 2061 6e64 2075 702e  p.rd = ? and up.
-0001e9e0: 666e 203d 203f 2061 6e64 202b 6d74 2e6b  fn = ? and +mt.k
-0001e9f0: 2021 3d20 2778 2722 0a20 2020 2020 2020   != 'x'".       
-0001ea00: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0001ea10: 2020 2020 2020 2020 2020 7220 3d20 6963            r = ic
-0001ea20: 7572 2e65 7865 6375 7465 2871 2c20 6572  ur.execute(q, er
-0001ea30: 645f 6566 6e29 0a20 2020 2020 2020 2020  d_efn).         
-0001ea40: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0001ea50: 696f 6e20 6173 2065 783a 0a20 2020 2020  ion as ex:.     
-0001ea60: 2020 2020 2020 2020 2020 2069 6620 2264             if "d
-0001ea70: 6174 6162 6173 6520 6973 206c 6f63 6b65  atabase is locke
-0001ea80: 6422 2069 6e20 7374 7228 6578 293a 0a20  d" in str(ex):. 
-0001ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eaa0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-0001eab0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0001eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ead0: 2020 2065 7264 5f65 666e 203d 2073 3365     erd_efn = s3e
-0001eae0: 6e63 2869 6478 2e6d 656d 5f63 7572 2c20  nc(idx.mem_cur, 
-0001eaf0: 7264 2c20 666e 290a 2020 2020 2020 2020  rd, fn).        
-0001eb00: 2020 2020 2020 2020 2020 2020 7220 3d20              r = 
-0001eb10: 6963 7572 2e65 7865 6375 7465 2871 2c20  icur.execute(q, 
-0001eb20: 6572 645f 6566 6e29 0a20 2020 2020 2020  erd_efn).       
-0001eb30: 2020 2020 2020 2020 2065 7863 6570 743a           except:
-0001eb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001eb50: 2020 2020 2074 203d 2022 7461 6720 7265       t = "tag re
-0001eb60: 6164 2065 7272 6f72 2c20 7b7d 2f7b 7d5c  ad error, {}/{}\
-0001eb70: 6e7b 7d22 0a20 2020 2020 2020 2020 2020  n{}".           
-0001eb80: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0001eb90: 6728 742e 666f 726d 6174 2872 642c 2066  g(t.format(rd, f
-0001eba0: 6e2c 206d 696e 5f65 7828 2929 290a 2020  n, min_ex())).  
-0001ebb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ebc0: 2020 6272 6561 6b0a 0a20 2020 2020 2020    break..       
-0001ebd0: 2020 2020 2066 655b 2274 6167 7322 5d20       fe["tags"] 
-0001ebe0: 3d20 7b6b 3a20 7620 666f 7220 6b2c 2076  = {k: v for k, v
-0001ebf0: 2069 6e20 727d 0a0a 2020 2020 2020 2020   in r}..        
-0001ec00: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
-0001ec10: 6164 6d69 6e3a 0a20 2020 2020 2020 2020  admin:.         
-0001ec20: 2020 2020 2020 2071 203d 2022 7365 6c65         q = "sele
-0001ec30: 6374 2069 702c 2061 7420 6672 6f6d 2075  ct ip, at from u
-0001ec40: 7020 7768 6572 6520 7264 3d3f 2061 6e64  p where rd=? and
-0001ec50: 2066 6e3d 3f22 0a20 2020 2020 2020 2020   fn=?".         
-0001ec60: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0001ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec80: 7a73 312c 207a 7332 203d 2069 6375 722e  zs1, zs2 = icur.
-0001ec90: 6578 6563 7574 6528 712c 2065 7264 5f65  execute(q, erd_e
-0001eca0: 666e 292e 6665 7463 686f 6e65 2829 0a20  fn).fetchone(). 
-0001ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ecc0: 2020 2066 655b 2274 6167 7322 5d5b 2275     fe["tags"]["u
-0001ecd0: 705f 6970 225d 203d 207a 7331 0a20 2020  p_ip"] = zs1.   
-0001ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ecf0: 2066 655b 2274 6167 7322 5d5b 222e 7570   fe["tags"][".up
-0001ed00: 5f61 7422 5d20 3d20 7a73 320a 2020 2020  _at"] = zs2.    
-0001ed10: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0001ed20: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-0001ed30: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-0001ed40: 2020 2020 2020 2020 2020 5f20 3d20 5b74            _ = [t
-0001ed50: 6167 7365 742e 6164 6428 6b29 2066 6f72  agset.add(k) for
-0001ed60: 206b 2069 6e20 6665 5b22 7461 6773 225d   k in fe["tags"]
-0001ed70: 5d0a 0a20 2020 2020 2020 2069 6620 6963  ]..        if ic
-0001ed80: 7572 3a0a 2020 2020 2020 2020 2020 2020  ur:.            
-0001ed90: 6d74 6520 3d20 766e 2e66 6c61 6773 2e67  mte = vn.flags.g
-0001eda0: 6574 2822 6d74 6522 2920 6f72 2022 7570  et("mte") or "up
-0001edb0: 5f69 702c 2e75 705f 6174 220a 2020 2020  _ip,.up_at".    
-0001edc0: 2020 2020 2020 2020 7461 676c 6973 7420          taglist 
-0001edd0: 3d20 5b6b 2066 6f72 206b 2069 6e20 6d74  = [k for k in mt
-0001ede0: 652e 7370 6c69 7428 222c 2229 2069 6620  e.split(",") if 
-0001edf0: 6b20 696e 2074 6167 7365 745d 0a20 2020  k in tagset].   
-0001ee00: 2020 2020 2020 2020 2066 6f72 2066 6520           for fe 
-0001ee10: 696e 2064 6972 733a 0a20 2020 2020 2020  in dirs:.       
-0001ee20: 2020 2020 2020 2020 2066 655b 2274 6167           fe["tag
-0001ee30: 7322 5d20 3d20 7b7d 0a20 2020 2020 2020  s"] = {}.       
-0001ee40: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001ee50: 2020 2074 6167 6c69 7374 203d 206c 6973     taglist = lis
-0001ee60: 7428 7461 6773 6574 290a 0a20 2020 2020  t(tagset)..     
-0001ee70: 2020 2069 6620 6973 5f6c 733a 0a20 2020     if is_ls:.   
+0001bfb0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0001bfc0: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
+0001bfd0: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
+0001bfe0: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
+0001bff0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001c000: 726e 2073 656c 662e 7478 5f69 636f 2822  rn self.tx_ico("
+0001c010: 612e 666f 6c64 6572 2229 0a0a 2020 2020  a.folder")..    
+0001c020: 2020 2020 2020 2020 2020 2020 7468 7020              thp 
+0001c030: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0001c040: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+0001c050: 6875 6d62 636c 693a 0a20 2020 2020 2020  humbcli:.       
+0001c060: 2020 2020 2020 2020 2020 2020 2074 6870               thp
+0001c070: 203d 2073 656c 662e 7468 756d 6263 6c69   = self.thumbcli
+0001c080: 2e67 6574 2864 6276 2c20 7672 656d 2c20  .get(dbv, vrem, 
+0001c090: 696e 7428 7374 2e73 745f 6d74 696d 6529  int(st.st_mtime)
+0001c0a0: 2c20 7468 5f66 6d74 290a 0a20 2020 2020  , th_fmt)..     
+0001c0b0: 2020 2020 2020 2020 2020 2069 6620 7468             if th
+0001c0c0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+0001c0d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001c0e0: 6c66 2e74 785f 6669 6c65 2874 6870 290a  lf.tx_file(thp).
+0001c0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c100: 2069 6620 7468 5f66 6d74 203d 3d20 2270   if th_fmt == "p
+0001c110: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0001c120: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
+0001c130: 6b61 6328 3430 3429 0a0a 2020 2020 2020  kac(404)..      
+0001c140: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001c150: 2073 656c 662e 7478 5f69 636f 2872 656d   self.tx_ico(rem
+0001c160: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
+0001c170: 7420 6973 5f64 6972 2061 6e64 2028 7365  t is_dir and (se
+0001c180: 6c66 2e63 616e 5f72 6561 6420 6f72 2073  lf.can_read or s
+0001c190: 656c 662e 6361 6e5f 6765 7429 3a0a 2020  elf.can_get):.  
+0001c1a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0001c1b0: 2073 656c 662e 6361 6e5f 7265 6164 2061   self.can_read a
+0001c1c0: 6e64 2022 666b 2220 696e 2076 6e2e 666c  nd "fk" in vn.fl
+0001c1d0: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+0001c1e0: 2020 2020 2063 6f72 7265 6374 203d 2073       correct = s
+0001c1f0: 656c 662e 6765 6e5f 666b 280a 2020 2020  elf.gen_fk(.    
+0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c210: 7365 6c66 2e61 7267 732e 666b 5f73 616c  self.args.fk_sal
+0001c220: 742c 2061 6273 7061 7468 2c20 7374 2e73  t, abspath, st.s
+0001c230: 745f 7369 7a65 2c20 3020 6966 2041 4e59  t_size, 0 if ANY
+0001c240: 5749 4e20 656c 7365 2073 742e 7374 5f69  WIN else st.st_i
+0001c250: 6e6f 0a20 2020 2020 2020 2020 2020 2020  no.             
+0001c260: 2020 2029 5b3a 2076 6e2e 666c 6167 735b     )[: vn.flags[
+0001c270: 2266 6b22 5d5d 0a20 2020 2020 2020 2020  "fk"]].         
+0001c280: 2020 2020 2020 2067 6f74 203d 2073 656c         got = sel
+0001c290: 662e 7570 6172 616d 2e67 6574 2822 6b22  f.uparam.get("k"
+0001c2a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001c2b0: 2020 6966 2067 6f74 2021 3d20 636f 7272    if got != corr
+0001c2c0: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
+0001c2d0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+0001c2e0: 6728 2277 726f 6e67 2066 696c 656b 6579  g("wrong filekey
+0001c2f0: 2c20 7761 6e74 207b 7d2c 2067 6f74 207b  , want {}, got {
+0001c300: 7d22 2e66 6f72 6d61 7428 636f 7272 6563  }".format(correc
+0001c310: 742c 2067 6f74 2929 0a20 2020 2020 2020  t, got)).       
+0001c320: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001c330: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
+0001c340: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0001c350: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+0001c360: 2020 2020 6162 7370 6174 682e 656e 6473      abspath.ends
+0001c370: 7769 7468 2822 2e6d 6422 290a 2020 2020  with(".md").    
+0001c380: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+0001c390: 226e 6f68 746d 6c22 206e 6f74 2069 6e20  "nohtml" not in 
+0001c3a0: 766e 2e66 6c61 6773 0a20 2020 2020 2020  vn.flags.       
+0001c3b0: 2020 2020 2020 2020 2061 6e64 2028 0a20           and (. 
+0001c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3d0: 2020 2022 7622 2069 6e20 7365 6c66 2e75     "v" in self.u
+0001c3e0: 7061 7261 6d0a 2020 2020 2020 2020 2020  param.          
+0001c3f0: 2020 2020 2020 2020 2020 6f72 2022 6564            or "ed
+0001c400: 6974 2220 696e 2073 656c 662e 7570 6172  it" in self.upar
+0001c410: 616d 0a20 2020 2020 2020 2020 2020 2020  am.             
+0001c420: 2020 2020 2020 206f 7220 2265 6469 7432         or "edit2
+0001c430: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
+0001c440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c450: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+0001c460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001c470: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+0001c480: 5f6d 6428 6162 7370 6174 6829 0a0a 2020  _md(abspath)..  
+0001c490: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001c4a0: 2073 656c 662e 7478 5f66 696c 6528 6162   self.tx_file(ab
+0001c4b0: 7370 6174 6829 0a0a 2020 2020 2020 2020  spath)..        
+0001c4c0: 656c 6966 2069 735f 6469 7220 616e 6420  elif is_dir and 
+0001c4d0: 6e6f 7420 7365 6c66 2e63 616e 5f72 6561  not self.can_rea
+0001c4e0: 6420 616e 6420 6e6f 7420 7365 6c66 2e63  d and not self.c
+0001c4f0: 616e 5f77 7269 7465 3a0a 2020 2020 2020  an_write:.      
+0001c500: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001c510: 662e 7478 5f34 3034 2854 7275 6529 0a0a  f.tx_404(True)..
+0001c520: 2020 2020 2020 2020 7372 765f 696e 666f          srv_info
+0001c530: 203d 205b 5d0a 0a20 2020 2020 2020 2074   = []..        t
+0001c540: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0001c550: 6966 206e 6f74 2073 656c 662e 6172 6773  if not self.args
+0001c560: 2e6e 6968 3a0a 2020 2020 2020 2020 2020  .nih:.          
+0001c570: 2020 2020 2020 7372 765f 696e 666f 2e61        srv_info.a
+0001c580: 7070 656e 6428 7365 6c66 2e61 7267 732e  ppend(self.args.
+0001c590: 6e61 6d65 290a 2020 2020 2020 2020 6578  name).        ex
+0001c5a0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+0001c5b0: 2020 7365 6c66 2e6c 6f67 2822 2377 6f77    self.log("#wow
+0001c5c0: 2023 7768 6f61 2229 0a0a 2020 2020 2020   #whoa")..      
+0001c5d0: 2020 6966 206e 6f74 2073 656c 662e 6172    if not self.ar
+0001c5e0: 6773 2e6e 6964 3a0a 2020 2020 2020 2020  gs.nid:.        
+0001c5f0: 2020 2020 6672 6565 2c20 746f 7461 6c20      free, total 
+0001c600: 3d20 6765 745f 6466 2861 6273 7061 7468  = get_df(abspath
+0001c610: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001c620: 2074 6f74 616c 2069 7320 6e6f 7420 4e6f   total is not No
+0001c630: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0001c640: 2020 2020 6831 203d 2068 756d 616e 7369      h1 = humansi
+0001c650: 7a65 2866 7265 6520 6f72 2030 290a 2020  ze(free or 0).  
+0001c660: 2020 2020 2020 2020 2020 2020 2020 6832                h2
+0001c670: 203d 2068 756d 616e 7369 7a65 2874 6f74   = humansize(tot
+0001c680: 616c 290a 2020 2020 2020 2020 2020 2020  al).            
+0001c690: 2020 2020 7372 765f 696e 666f 2e61 7070      srv_info.app
+0001c6a0: 656e 6428 227b 7d20 6672 6565 206f 6620  end("{} free of 
+0001c6b0: 7b7d 222e 666f 726d 6174 2868 312c 2068  {}".format(h1, h
+0001c6c0: 3229 290a 2020 2020 2020 2020 2020 2020  2)).            
+0001c6d0: 656c 6966 2066 7265 6520 6973 206e 6f74  elif free is not
+0001c6e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001c6f0: 2020 2020 2020 2073 7276 5f69 6e66 6f2e         srv_info.
+0001c700: 6170 7065 6e64 2868 756d 616e 7369 7a65  append(humansize
+0001c710: 2866 7265 652c 2054 7275 6529 202b 2022  (free, True) + "
+0001c720: 2066 7265 6522 290a 0a20 2020 2020 2020   free")..       
+0001c730: 2073 7276 5f69 6e66 6f74 203d 2022 3c2f   srv_infot = "</
+0001c740: 7370 616e 3e20 2f2f 203c 7370 616e 3e22  span> // <span>"
+0001c750: 2e6a 6f69 6e28 7372 765f 696e 666f 290a  .join(srv_info).
+0001c760: 0a20 2020 2020 2020 2070 6572 6d73 203d  .        perms =
+0001c770: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
+0001c780: 656c 662e 6361 6e5f 7265 6164 3a0a 2020  elf.can_read:.  
+0001c790: 2020 2020 2020 2020 2020 7065 726d 732e            perms.
+0001c7a0: 6170 7065 6e64 2822 7265 6164 2229 0a20  append("read"). 
+0001c7b0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0001c7c0: 616e 5f77 7269 7465 3a0a 2020 2020 2020  an_write:.      
+0001c7d0: 2020 2020 2020 7065 726d 732e 6170 7065        perms.appe
+0001c7e0: 6e64 2822 7772 6974 6522 290a 2020 2020  nd("write").    
+0001c7f0: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
+0001c800: 6d6f 7665 3a0a 2020 2020 2020 2020 2020  move:.          
+0001c810: 2020 7065 726d 732e 6170 7065 6e64 2822    perms.append("
+0001c820: 6d6f 7665 2229 0a20 2020 2020 2020 2069  move").        i
+0001c830: 6620 7365 6c66 2e63 616e 5f64 656c 6574  f self.can_delet
+0001c840: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+0001c850: 6572 6d73 2e61 7070 656e 6428 2264 656c  erms.append("del
+0001c860: 6574 6522 290a 2020 2020 2020 2020 6966  ete").        if
+0001c870: 2073 656c 662e 6361 6e5f 6765 743a 0a20   self.can_get:. 
+0001c880: 2020 2020 2020 2020 2020 2070 6572 6d73             perms
+0001c890: 2e61 7070 656e 6428 2267 6574 2229 0a20  .append("get"). 
+0001c8a0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0001c8b0: 616e 5f75 7067 6574 3a0a 2020 2020 2020  an_upget:.      
+0001c8c0: 2020 2020 2020 7065 726d 732e 6170 7065        perms.appe
+0001c8d0: 6e64 2822 7570 6765 7422 290a 2020 2020  nd("upget").    
+0001c8e0: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
+0001c8f0: 6164 6d69 6e3a 0a20 2020 2020 2020 2020  admin:.         
+0001c900: 2020 2070 6572 6d73 2e61 7070 656e 6428     perms.append(
+0001c910: 2261 646d 696e 2229 0a0a 2020 2020 2020  "admin")..      
+0001c920: 2020 7572 6c5f 7375 6620 3d20 7365 6c66    url_suf = self
+0001c930: 2e75 726c 7128 7b7d 2c20 5b22 6b22 5d29  .urlq({}, ["k"])
+0001c940: 0a20 2020 2020 2020 2069 735f 6c73 203d  .        is_ls =
+0001c950: 2022 6c73 2220 696e 2073 656c 662e 7570   "ls" in self.up
+0001c960: 6172 616d 0a20 2020 2020 2020 2069 735f  aram.        is_
+0001c970: 6a73 203d 2073 656c 662e 6172 6773 2e66  js = self.args.f
+0001c980: 6f72 6365 5f6a 7320 6f72 2073 656c 662e  orce_js or self.
+0001c990: 636f 6f6b 6965 732e 6765 7428 226a 7322  cookies.get("js"
+0001c9a0: 2920 3d3d 2022 7922 0a0a 2020 2020 2020  ) == "y"..      
+0001c9b0: 2020 6966 206e 6f74 2069 735f 6c73 2061    if not is_ls a
+0001c9c0: 6e64 2028 7365 6c66 2e75 612e 7374 6172  nd (self.ua.star
+0001c9d0: 7473 7769 7468 2822 6375 726c 2f22 2920  tswith("curl/") 
+0001c9e0: 6f72 2073 656c 662e 7561 2e73 7461 7274  or self.ua.start
+0001c9f0: 7377 6974 6828 2266 6574 6368 2229 293a  swith("fetch")):
+0001ca00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001ca10: 662e 7570 6172 616d 5b22 6c73 225d 203d  f.uparam["ls"] =
+0001ca20: 2022 7622 0a20 2020 2020 2020 2020 2020   "v".           
+0001ca30: 2069 735f 6c73 203d 2054 7275 650a 0a20   is_ls = True.. 
+0001ca40: 2020 2020 2020 2074 706c 203d 2022 6272         tpl = "br
+0001ca50: 6f77 7365 7222 0a20 2020 2020 2020 2069  owser".        i
+0001ca60: 6620 2262 2220 696e 2073 656c 662e 7570  f "b" in self.up
+0001ca70: 6172 616d 3a0a 2020 2020 2020 2020 2020  aram:.          
+0001ca80: 2020 7470 6c20 3d20 2262 726f 7773 6572    tpl = "browser
+0001ca90: 3222 0a20 2020 2020 2020 2020 2020 2069  2".            i
+0001caa0: 735f 6a73 203d 2046 616c 7365 0a0a 2020  s_js = False..  
+0001cab0: 2020 2020 2020 6c6f 6775 6573 203d 205b        logues = [
+0001cac0: 2222 2c20 2222 5d0a 2020 2020 2020 2020  "", ""].        
+0001cad0: 6966 206e 6f74 2073 656c 662e 6172 6773  if not self.args
+0001cae0: 2e6e 6f5f 6c6f 6775 6573 3a0a 2020 2020  .no_logues:.    
+0001caf0: 2020 2020 2020 2020 666f 7220 6e2c 2066          for n, f
+0001cb00: 6e20 696e 2065 6e75 6d65 7261 7465 285b  n in enumerate([
+0001cb10: 222e 7072 6f6c 6f67 7565 2e68 746d 6c22  ".prologue.html"
+0001cb20: 2c20 222e 6570 696c 6f67 7565 2e68 746d  , ".epilogue.htm
+0001cb30: 6c22 5d29 3a0a 2020 2020 2020 2020 2020  l"]):.          
+0001cb40: 2020 2020 2020 666e 203d 206f 732e 7061        fn = os.pa
+0001cb50: 7468 2e6a 6f69 6e28 6162 7370 6174 682c  th.join(abspath,
+0001cb60: 2066 6e29 0a20 2020 2020 2020 2020 2020   fn).           
+0001cb70: 2020 2020 2069 6620 626f 732e 7061 7468       if bos.path
+0001cb80: 2e65 7869 7374 7328 666e 293a 0a20 2020  .exists(fn):.   
+0001cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cba0: 2077 6974 6820 6f70 656e 2866 7365 6e63   with open(fsenc
+0001cbb0: 2866 6e29 2c20 2272 6222 2920 6173 2066  (fn), "rb") as f
+0001cbc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001cbd0: 2020 2020 2020 2020 2020 6c6f 6775 6573            logues
+0001cbe0: 5b6e 5d20 3d20 662e 7265 6164 2829 2e64  [n] = f.read().d
+0001cbf0: 6563 6f64 6528 2275 7466 2d38 2229 0a0a  ecode("utf-8")..
+0001cc00: 2020 2020 2020 2020 7265 6164 6d65 203d          readme =
+0001cc10: 2022 220a 2020 2020 2020 2020 6966 206e   "".        if n
+0001cc20: 6f74 2073 656c 662e 6172 6773 2e6e 6f5f  ot self.args.no_
+0001cc30: 7265 6164 6d65 2061 6e64 206e 6f74 206c  readme and not l
+0001cc40: 6f67 7565 735b 315d 3a0a 2020 2020 2020  ogues[1]:.      
+0001cc50: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+0001cc60: 5b22 5245 4144 4d45 2e6d 6422 2c20 2272  ["README.md", "r
+0001cc70: 6561 646d 652e 6d64 225d 3a0a 2020 2020  eadme.md"]:.    
+0001cc80: 2020 2020 2020 2020 2020 2020 666e 203d              fn =
+0001cc90: 206f 732e 7061 7468 2e6a 6f69 6e28 6162   os.path.join(ab
+0001cca0: 7370 6174 682c 2066 6e29 0a20 2020 2020  spath, fn).     
+0001ccb0: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
+0001ccc0: 732e 7061 7468 2e69 7366 696c 6528 666e  s.path.isfile(fn
+0001ccd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001cce0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+0001ccf0: 2866 7365 6e63 2866 6e29 2c20 2272 6222  (fsenc(fn), "rb"
+0001cd00: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
+0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd20: 7265 6164 6d65 203d 2066 2e72 6561 6428  readme = f.read(
+0001cd30: 292e 6465 636f 6465 2822 7574 662d 3822  ).decode("utf-8"
+0001cd40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001cd50: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+0001cd60: 0a20 2020 2020 2020 2076 6620 3d20 766e  .        vf = vn
+0001cd70: 2e66 6c61 6773 0a20 2020 2020 2020 2075  .flags.        u
+0001cd80: 6e6c 6973 7420 3d20 7666 2e67 6574 2822  nlist = vf.get("
+0001cd90: 756e 6c69 7374 222c 2022 2229 0a20 2020  unlist", "").   
+0001cda0: 2020 2020 206c 735f 7265 7420 3d20 7b0a       ls_ret = {.
+0001cdb0: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
+0001cdc0: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
+0001cdd0: 2020 2020 2266 696c 6573 223a 205b 5d2c      "files": [],
+0001cde0: 0a20 2020 2020 2020 2020 2020 2022 7461  .            "ta
+0001cdf0: 676c 6973 7422 3a20 5b5d 2c0a 2020 2020  glist": [],.    
+0001ce00: 2020 2020 2020 2020 2273 7276 696e 6622          "srvinf"
+0001ce10: 3a20 7372 765f 696e 666f 742c 0a20 2020  : srv_infot,.   
+0001ce20: 2020 2020 2020 2020 2022 6163 6374 223a           "acct":
+0001ce30: 2073 656c 662e 756e 616d 652c 0a20 2020   self.uname,.   
+0001ce40: 2020 2020 2020 2020 2022 6964 7822 3a20           "idx": 
+0001ce50: 6532 642c 0a20 2020 2020 2020 2020 2020  e2d,.           
+0001ce60: 2022 6974 6167 223a 2065 3274 2c0a 2020   "itag": e2t,.  
+0001ce70: 2020 2020 2020 2020 2020 226c 6966 6574            "lifet
+0001ce80: 696d 6522 3a20 766e 2e66 6c61 6773 2e67  ime": vn.flags.g
+0001ce90: 6574 2822 6c69 6665 7469 6d65 2229 206f  et("lifetime") o
+0001cea0: 7220 302c 0a20 2020 2020 2020 2020 2020  r 0,.           
+0001ceb0: 2022 6672 616e 6422 3a20 626f 6f6c 2876   "frand": bool(v
+0001cec0: 6e2e 666c 6167 732e 6765 7428 2272 616e  n.flags.get("ran
+0001ced0: 6422 2929 2c0a 2020 2020 2020 2020 2020  d")),.          
+0001cee0: 2020 2275 6e6c 6973 7422 3a20 756e 6c69    "unlist": unli
+0001cef0: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
+0001cf00: 2270 6572 6d73 223a 2070 6572 6d73 2c0a  "perms": perms,.
+0001cf10: 2020 2020 2020 2020 2020 2020 226c 6f67              "log
+0001cf20: 7565 7322 3a20 6c6f 6775 6573 2c0a 2020  ues": logues,.  
+0001cf30: 2020 2020 2020 2020 2020 2272 6561 646d            "readm
+0001cf40: 6522 3a20 7265 6164 6d65 2c0a 2020 2020  e": readme,.    
+0001cf50: 2020 2020 7d0a 2020 2020 2020 2020 6a32      }.        j2
+0001cf60: 6120 3d20 7b0a 2020 2020 2020 2020 2020  a = {.          
+0001cf70: 2020 2276 6469 7222 3a20 7175 6f74 6570    "vdir": quotep
+0001cf80: 2873 656c 662e 7670 6174 6829 2c0a 2020  (self.vpath),.  
+0001cf90: 2020 2020 2020 2020 2020 2276 706e 6f64            "vpnod
+0001cfa0: 6573 223a 2076 706e 6f64 6573 2c0a 2020  es": vpnodes,.  
+0001cfb0: 2020 2020 2020 2020 2020 2266 696c 6573            "files
+0001cfc0: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
+0001cfd0: 2020 2022 6c73 3022 3a20 4e6f 6e65 2c0a     "ls0": None,.
+0001cfe0: 2020 2020 2020 2020 2020 2020 2261 6363              "acc
+0001cff0: 7422 3a20 7365 6c66 2e75 6e61 6d65 2c0a  t": self.uname,.
+0001d000: 2020 2020 2020 2020 2020 2020 2270 6572              "per
+0001d010: 6d73 223a 206a 736f 6e2e 6475 6d70 7328  ms": json.dumps(
+0001d020: 7065 726d 7329 2c0a 2020 2020 2020 2020  perms),.        
+0001d030: 2020 2020 226c 6966 6574 696d 6522 3a20      "lifetime": 
+0001d040: 6c73 5f72 6574 5b22 6c69 6665 7469 6d65  ls_ret["lifetime
+0001d050: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+0001d060: 2266 7261 6e64 223a 2062 6f6f 6c28 766e  "frand": bool(vn
+0001d070: 2e66 6c61 6773 2e67 6574 2822 7261 6e64  .flags.get("rand
+0001d080: 2229 292c 0a20 2020 2020 2020 2020 2020  ")),.           
+0001d090: 2022 7461 676c 6973 7422 3a20 5b5d 2c0a   "taglist": [],.
+0001d0a0: 2020 2020 2020 2020 2020 2020 2264 6566              "def
+0001d0b0: 5f68 636f 6c73 223a 205b 5d2c 0a20 2020  _hcols": [],.   
+0001d0c0: 2020 2020 2020 2020 2022 6861 7665 5f65           "have_e
+0001d0d0: 6d70 223a 2073 656c 662e 6172 6773 2e65  mp": self.args.e
+0001d0e0: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
+0001d0f0: 2268 6176 655f 7570 326b 5f69 6478 223a  "have_up2k_idx":
+0001d100: 2065 3264 2c0a 2020 2020 2020 2020 2020   e2d,.          
+0001d110: 2020 2268 6176 655f 7461 6773 5f69 6478    "have_tags_idx
+0001d120: 223a 2065 3274 2c0a 2020 2020 2020 2020  ": e2t,.        
+0001d130: 2020 2020 2268 6176 655f 6163 6f64 6522      "have_acode"
+0001d140: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
+0001d150: 2e6e 6f5f 6163 6f64 6529 2c0a 2020 2020  .no_acode),.    
+0001d160: 2020 2020 2020 2020 2268 6176 655f 6d76          "have_mv
+0001d170: 223a 2028 6e6f 7420 7365 6c66 2e61 7267  ": (not self.arg
+0001d180: 732e 6e6f 5f6d 7629 2c0a 2020 2020 2020  s.no_mv),.      
+0001d190: 2020 2020 2020 2268 6176 655f 6465 6c22        "have_del"
+0001d1a0: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
+0001d1b0: 2e6e 6f5f 6465 6c29 2c0a 2020 2020 2020  .no_del),.      
+0001d1c0: 2020 2020 2020 2268 6176 655f 7a69 7022        "have_zip"
+0001d1d0: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
+0001d1e0: 2e6e 6f5f 7a69 7029 2c0a 2020 2020 2020  .no_zip),.      
+0001d1f0: 2020 2020 2020 2268 6176 655f 756e 706f        "have_unpo
+0001d200: 7374 223a 2069 6e74 2873 656c 662e 6172  st": int(self.ar
+0001d210: 6773 2e75 6e70 6f73 7429 2c0a 2020 2020  gs.unpost),.    
+0001d220: 2020 2020 2020 2020 2268 6176 655f 625f          "have_b_
+0001d230: 7522 3a20 2873 656c 662e 6361 6e5f 7772  u": (self.can_wr
+0001d240: 6974 6520 616e 6420 7365 6c66 2e75 7061  ite and self.upa
+0001d250: 7261 6d2e 6765 7428 2262 2229 203d 3d20  ram.get("b") == 
+0001d260: 2275 2229 2c0a 2020 2020 2020 2020 2020  "u"),.          
+0001d270: 2020 2273 625f 6d64 223a 2022 2220 6966    "sb_md": "" if
+0001d280: 2022 6e6f 5f73 625f 6d64 2220 696e 2076   "no_sb_md" in v
+0001d290: 6620 656c 7365 2028 7666 2e67 6574 2822  f else (vf.get("
+0001d2a0: 6d64 5f73 6266 2229 206f 7220 2279 2229  md_sbf") or "y")
+0001d2b0: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+0001d2c0: 625f 6c67 223a 2022 2220 6966 2022 6e6f  b_lg": "" if "no
+0001d2d0: 5f73 625f 6c67 2220 696e 2076 6620 656c  _sb_lg" in vf el
+0001d2e0: 7365 2028 7666 2e67 6574 2822 6c67 5f73  se (vf.get("lg_s
+0001d2f0: 6266 2229 206f 7220 2279 2229 2c0a 2020  bf") or "y"),.  
+0001d300: 2020 2020 2020 2020 2020 2275 726c 5f73            "url_s
+0001d310: 7566 223a 2075 726c 5f73 7566 2c0a 2020  uf": url_suf,.  
+0001d320: 2020 2020 2020 2020 2020 226c 6f67 7565            "logue
+0001d330: 7322 3a20 6c6f 6775 6573 2c0a 2020 2020  s": logues,.    
+0001d340: 2020 2020 2020 2020 2272 6561 646d 6522          "readme"
+0001d350: 3a20 7265 6164 6d65 2c0a 2020 2020 2020  : readme,.      
+0001d360: 2020 2020 2020 2274 6974 6c65 223a 2068        "title": h
+0001d370: 746d 6c5f 6573 6361 7065 2873 656c 662e  tml_escape(self.
+0001d380: 7670 6174 682c 2063 726c 663d 5472 7565  vpath, crlf=True
+0001d390: 2920 6f72 2022 f09f 92be f09f 8e89 222c  ) or "........",
+0001d3a0: 0a20 2020 2020 2020 2020 2020 2022 7372  .            "sr
+0001d3b0: 765f 696e 666f 223a 2073 7276 5f69 6e66  v_info": srv_inf
+0001d3c0: 6f74 2c0a 2020 2020 2020 2020 2020 2020  ot,.            
+0001d3d0: 2264 6772 6964 223a 2022 6772 6964 2220  "dgrid": "grid" 
+0001d3e0: 696e 2076 662c 0a20 2020 2020 2020 2020  in vf,.         
+0001d3f0: 2020 2022 756e 6c69 7374 223a 2075 6e6c     "unlist": unl
+0001d400: 6973 742c 0a20 2020 2020 2020 2020 2020  ist,.           
+0001d410: 2022 6474 6865 6d65 223a 2073 656c 662e   "dtheme": self.
+0001d420: 6172 6773 2e74 6865 6d65 2c0a 2020 2020  args.theme,.    
+0001d430: 2020 2020 2020 2020 2274 6865 6d65 7322          "themes"
+0001d440: 3a20 7365 6c66 2e61 7267 732e 7468 656d  : self.args.them
+0001d450: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0001d460: 2274 7572 626f 6c76 6c22 3a20 7365 6c66  "turbolvl": self
+0001d470: 2e61 7267 732e 7475 7262 6f2c 0a20 2020  .args.turbo,.   
+0001d480: 2020 2020 2020 2020 2022 6964 7868 223a           "idxh":
+0001d490: 2069 6e74 2873 656c 662e 6172 6773 2e69   int(self.args.i
+0001d4a0: 6829 2c0a 2020 2020 2020 2020 2020 2020  h),.            
+0001d4b0: 2275 3273 6f72 7422 3a20 7365 6c66 2e61  "u2sort": self.a
+0001d4c0: 7267 732e 7532 736f 7274 2c0a 2020 2020  rgs.u2sort,.    
+0001d4d0: 2020 2020 7d0a 0a20 2020 2020 2020 2069      }..        i
+0001d4e0: 6620 7365 6c66 2e61 7267 732e 6a73 5f62  f self.args.js_b
+0001d4f0: 726f 7773 6572 3a0a 2020 2020 2020 2020  rowser:.        
+0001d500: 2020 2020 6a32 615b 226a 7322 5d20 3d20      j2a["js"] = 
+0001d510: 7365 6c66 2e61 7267 732e 6a73 5f62 726f  self.args.js_bro
+0001d520: 7773 6572 0a0a 2020 2020 2020 2020 6966  wser..        if
+0001d530: 2073 656c 662e 6172 6773 2e63 7373 5f62   self.args.css_b
+0001d540: 726f 7773 6572 3a0a 2020 2020 2020 2020  rowser:.        
+0001d550: 2020 2020 6a32 615b 2263 7373 225d 203d      j2a["css"] =
+0001d560: 2073 656c 662e 6172 6773 2e63 7373 5f62   self.args.css_b
+0001d570: 726f 7773 6572 0a0a 2020 2020 2020 2020  rowser..        
+0001d580: 6966 206e 6f74 2073 656c 662e 636f 6e6e  if not self.conn
+0001d590: 2e68 7372 762e 7072 6973 6d3a 0a20 2020  .hsrv.prism:.   
+0001d5a0: 2020 2020 2020 2020 206a 3261 5b22 6e6f           j2a["no
+0001d5b0: 5f70 7269 736d 225d 203d 2054 7275 650a  _prism"] = True.
+0001d5c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0001d5d0: 7365 6c66 2e63 616e 5f72 6561 643a 0a20  self.can_read:. 
+0001d5e0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+0001d5f0: 5f6c 733a 0a20 2020 2020 2020 2020 2020  _ls:.           
+0001d600: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001d610: 2e74 785f 6c73 286c 735f 7265 7429 0a0a  .tx_ls(ls_ret)..
+0001d620: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001d630: 6f74 2073 7461 742e 535f 4953 4449 5228  ot stat.S_ISDIR(
+0001d640: 7374 2e73 745f 6d6f 6465 293a 0a20 2020  st.st_mode):.   
+0001d650: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001d660: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
+0001d670: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
+0001d680: 2020 2069 6620 227a 6970 2220 696e 2073     if "zip" in s
+0001d690: 656c 662e 7570 6172 616d 206f 7220 2274  elf.uparam or "t
+0001d6a0: 6172 2220 696e 2073 656c 662e 7570 6172  ar" in self.upar
+0001d6b0: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
+0001d6c0: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
+0001d6d0: 2834 3033 290a 0a20 2020 2020 2020 2020  (403)..         
+0001d6e0: 2020 2068 746d 6c20 3d20 7365 6c66 2e6a     html = self.j
+0001d6f0: 3273 2874 706c 2c20 2a2a 6a32 6129 0a20  2s(tpl, **j2a). 
+0001d700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001d710: 7265 706c 7928 6874 6d6c 2e65 6e63 6f64  reply(html.encod
+0001d720: 6528 2275 7466 2d38 222c 2022 7265 706c  e("utf-8", "repl
+0001d730: 6163 6522 2929 0a20 2020 2020 2020 2020  ace")).         
+0001d740: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+0001d750: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+0001d760: 205b 227a 6970 222c 2022 7461 7222 5d3a   ["zip", "tar"]:
+0001d770: 0a20 2020 2020 2020 2020 2020 2076 203d  .            v =
+0001d780: 2073 656c 662e 7570 6172 616d 2e67 6574   self.uparam.get
+0001d790: 286b 290a 2020 2020 2020 2020 2020 2020  (k).            
+0001d7a0: 6966 2076 2069 7320 6e6f 7420 4e6f 6e65  if v is not None
+0001d7b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d7c0: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+0001d7d0: 5f7a 6970 286b 2c20 762c 2073 656c 662e  _zip(k, v, self.
+0001d7e0: 7670 6174 682c 2076 6e2c 2072 656d 2c20  vpath, vn, rem, 
+0001d7f0: 5b5d 2c20 7365 6c66 2e61 7267 732e 6564  [], self.args.ed
+0001d800: 290a 0a20 2020 2020 2020 2066 7372 6f6f  )..        fsroo
+0001d810: 742c 2076 6673 5f6c 732c 2076 6673 5f76  t, vfs_ls, vfs_v
+0001d820: 6972 7420 3d20 766e 2e6c 7328 0a20 2020  irt = vn.ls(.   
+0001d830: 2020 2020 2020 2020 2072 656d 2c0a 2020           rem,.  
+0001d840: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
+0001d850: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+0001d860: 2020 6e6f 7420 7365 6c66 2e61 7267 732e    not self.args.
+0001d870: 6e6f 5f73 6361 6e64 6972 2c0a 2020 2020  no_scandir,.    
+0001d880: 2020 2020 2020 2020 5b5b 5472 7565 2c20          [[True, 
+0001d890: 4661 6c73 655d 2c20 5b46 616c 7365 2c20  False], [False, 
+0001d8a0: 5472 7565 5d5d 2c0a 2020 2020 2020 2020  True]],.        
+0001d8b0: 2020 2020 6c73 7461 743d 226c 7422 2069      lstat="lt" i
+0001d8c0: 6e20 7365 6c66 2e75 7061 7261 6d2c 0a20  n self.uparam,. 
+0001d8d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0001d8e0: 2073 7461 7473 203d 207b 6b3a 2076 2066   stats = {k: v f
+0001d8f0: 6f72 206b 2c20 7620 696e 2076 6673 5f6c  or k, v in vfs_l
+0001d900: 737d 0a20 2020 2020 2020 206c 735f 6e61  s}.        ls_na
+0001d910: 6d65 7320 3d20 5b78 5b30 5d20 666f 7220  mes = [x[0] for 
+0001d920: 7820 696e 2076 6673 5f6c 735d 0a20 2020  x in vfs_ls].   
+0001d930: 2020 2020 206c 735f 6e61 6d65 732e 6578       ls_names.ex
+0001d940: 7465 6e64 286c 6973 7428 7666 735f 7669  tend(list(vfs_vi
+0001d950: 7274 2e6b 6579 7328 2929 290a 0a20 2020  rt.keys()))..   
+0001d960: 2020 2020 2023 2063 6865 636b 2066 6f72       # check for
+0001d970: 206f 6c64 2076 6572 7369 6f6e 7320 6f66   old versions of
+0001d980: 2066 696c 6573 2c0a 2020 2020 2020 2020   files,.        
+0001d990: 2320 5b6e 756d 2d62 6163 6b75 7073 2c20  # [num-backups, 
+0001d9a0: 6d6f 7374 2d72 6563 656e 742c 2068 6973  most-recent, his
+0001d9b0: 742d 7061 7468 5d0a 2020 2020 2020 2020  t-path].        
+0001d9c0: 6869 7374 2020 2020 203d 207b 7d0a 2020  hist     = {}.  
+0001d9d0: 2020 2020 2020 6869 7374 6469 7220 3d20        histdir = 
+0001d9e0: 6f73 2e70 6174 682e 6a6f 696e 2866 7372  os.path.join(fsr
+0001d9f0: 6f6f 742c 2022 2e68 6973 7422 290a 2020  oot, ".hist").  
+0001da00: 2020 2020 2020 7074 6e20 3d20 7265 2e63        ptn = re.c
+0001da10: 6f6d 7069 6c65 2872 2228 2e2a 295c 2e28  ompile(r"(.*)\.(
+0001da20: 5b30 2d39 5d2b 5c2e 5b30 2d39 5d7b 337d  [0-9]+\.[0-9]{3}
+0001da30: 2928 5c2e 5b5e 5c2e 5d2b 2924 2229 0a20  )(\.[^\.]+)$"). 
+0001da40: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001da50: 2020 2020 2020 2020 666f 7220 6866 6e20          for hfn 
+0001da60: 696e 2062 6f73 2e6c 6973 7464 6972 2868  in bos.listdir(h
+0001da70: 6973 7464 6972 293a 0a20 2020 2020 2020  istdir):.       
+0001da80: 2020 2020 2020 2020 206d 203d 2070 746e           m = ptn
+0001da90: 2e6d 6174 6368 2868 666e 290a 2020 2020  .match(hfn).    
+0001daa0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001dab0: 6f74 206d 3a0a 2020 2020 2020 2020 2020  ot m:.          
+0001dac0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
+0001dad0: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+0001dae0: 2020 2020 666e 203d 206d 2e67 726f 7570      fn = m.group
+0001daf0: 2831 2920 2b20 6d2e 6772 6f75 7028 3329  (1) + m.group(3)
+0001db00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001db10: 206e 2c20 7473 2c20 5f20 3d20 6869 7374   n, ts, _ = hist
+0001db20: 2e67 6574 2866 6e2c 2028 302c 2030 2c20  .get(fn, (0, 0, 
+0001db30: 2222 2929 0a20 2020 2020 2020 2020 2020  "")).           
+0001db40: 2020 2020 2068 6973 745b 666e 5d20 3d20       hist[fn] = 
+0001db50: 286e 202b 2031 2c20 6d61 7828 7473 2c20  (n + 1, max(ts, 
+0001db60: 666c 6f61 7428 6d2e 6772 6f75 7028 3229  float(m.group(2)
+0001db70: 2929 2c20 6866 6e29 0a20 2020 2020 2020  )), hfn).       
+0001db80: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+0001db90: 2020 2020 2070 6173 730a 0a20 2020 2020       pass..     
+0001dba0: 2020 2023 2073 686f 7720 646f 7466 696c     # show dotfil
+0001dbb0: 6573 2069 6620 7065 726d 6974 7465 6420  es if permitted 
+0001dbc0: 616e 6420 7265 7175 6573 7465 640a 2020  and requested.  
+0001dbd0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
+0001dbe0: 662e 6172 6773 2e65 6420 6f72 2022 646f  f.args.ed or "do
+0001dbf0: 7473 2220 6e6f 7420 696e 2073 656c 662e  ts" not in self.
+0001dc00: 7570 6172 616d 3a0a 2020 2020 2020 2020  uparam:.        
+0001dc10: 2020 2020 6c73 5f6e 616d 6573 203d 2065      ls_names = e
+0001dc20: 7863 6c75 6465 5f64 6f74 6669 6c65 7328  xclude_dotfiles(
+0001dc30: 6c73 5f6e 616d 6573 290a 0a20 2020 2020  ls_names)..     
+0001dc40: 2020 2061 6464 5f66 6b20 3d20 766e 2e66     add_fk = vn.f
+0001dc50: 6c61 6773 2e67 6574 2822 666b 2229 0a0a  lags.get("fk")..
+0001dc60: 2020 2020 2020 2020 6469 7273 203d 205b          dirs = [
+0001dc70: 5d0a 2020 2020 2020 2020 6669 6c65 7320  ].        files 
+0001dc80: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0001dc90: 2066 6e20 696e 206c 735f 6e61 6d65 733a   fn in ls_names:
+0001dca0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0001dcb0: 6520 3d20 2222 0a20 2020 2020 2020 2020  e = "".         
+0001dcc0: 2020 2068 7265 6620 3d20 666e 0a20 2020     href = fn.   
+0001dcd0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0001dce0: 6973 5f6c 7320 616e 6420 6e6f 7420 6973  is_ls and not is
+0001dcf0: 5f6a 7320 616e 6420 6e6f 7420 7365 6c66  _js and not self
+0001dd00: 2e74 7261 696c 696e 675f 736c 6173 6820  .trailing_slash 
+0001dd10: 616e 6420 7670 6174 683a 0a20 2020 2020  and vpath:.     
+0001dd20: 2020 2020 2020 2020 2020 2062 6173 6520             base 
+0001dd30: 3d20 222f 2220 2b20 7670 6174 6820 2b20  = "/" + vpath + 
+0001dd40: 222f 220a 2020 2020 2020 2020 2020 2020  "/".            
+0001dd50: 2020 2020 6872 6566 203d 2062 6173 6520      href = base 
+0001dd60: 2b20 666e 0a0a 2020 2020 2020 2020 2020  + fn..          
+0001dd70: 2020 6966 2066 6e20 696e 2076 6673 5f76    if fn in vfs_v
+0001dd80: 6972 743a 0a20 2020 2020 2020 2020 2020  irt:.           
+0001dd90: 2020 2020 2066 7370 6174 6820 3d20 7666       fspath = vf
+0001dda0: 735f 7669 7274 5b66 6e5d 2e72 6561 6c70  s_virt[fn].realp
+0001ddb0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+0001ddc0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001ddd0: 2020 2020 2020 6673 7061 7468 203d 2066        fspath = f
+0001dde0: 7372 6f6f 7420 2b20 222f 2220 2b20 666e  sroot + "/" + fn
+0001ddf0: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
+0001de00: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0001de10: 2020 206c 696e 6620 3d20 7374 6174 732e     linf = stats.
+0001de20: 6765 7428 666e 2920 6f72 2062 6f73 2e6c  get(fn) or bos.l
+0001de30: 7374 6174 2866 7370 6174 6829 0a20 2020  stat(fspath).   
+0001de40: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+0001de50: 203d 2062 6f73 2e73 7461 7428 6673 7061   = bos.stat(fspa
+0001de60: 7468 2920 6966 2073 7461 742e 535f 4953  th) if stat.S_IS
+0001de70: 4c4e 4b28 6c69 6e66 2e73 745f 6d6f 6465  LNK(linf.st_mode
+0001de80: 2920 656c 7365 206c 696e 660a 2020 2020  ) else linf.    
+0001de90: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+0001dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001deb0: 7365 6c66 2e6c 6f67 2822 6272 6f6b 656e  self.log("broken
+0001dec0: 2073 796d 6c69 6e6b 3a20 7b7d 222e 666f   symlink: {}".fo
+0001ded0: 726d 6174 2872 6570 7228 6673 7061 7468  rmat(repr(fspath
+0001dee0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
+0001def0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+0001df00: 2020 2020 2020 2020 2020 6973 5f64 6972            is_dir
+0001df10: 203d 2073 7461 742e 535f 4953 4449 5228   = stat.S_ISDIR(
+0001df20: 696e 662e 7374 5f6d 6f64 6529 0a20 2020  inf.st_mode).   
+0001df30: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
+0001df40: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
+0001df50: 2020 2020 6872 6566 202b 3d20 222f 220a      href += "/".
+0001df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df70: 6966 2073 656c 662e 6172 6773 2e6e 6f5f  if self.args.no_
+0001df80: 7a69 703a 0a20 2020 2020 2020 2020 2020  zip:.           
+0001df90: 2020 2020 2020 2020 206d 6172 6769 6e20           margin 
+0001dfa0: 3d20 2244 4952 220a 2020 2020 2020 2020  = "DIR".        
+0001dfb0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dfd0: 2020 6d61 7267 696e 203d 2027 3c61 2068    margin = '<a h
+0001dfe0: 7265 663d 2225 733f 7a69 7022 2072 656c  ref="%s?zip" rel
+0001dff0: 3d22 6e6f 666f 6c6c 6f77 223e 7a69 703c  ="nofollow">zip<
+0001e000: 2f61 3e27 2025 2028 7175 6f74 6570 2868  /a>' % (quotep(h
+0001e010: 7265 6629 2c29 0a20 2020 2020 2020 2020  ref),).         
+0001e020: 2020 2065 6c69 6620 666e 2069 6e20 6869     elif fn in hi
+0001e030: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+0001e040: 2020 2020 6d61 7267 696e 203d 2027 3c61      margin = '<a
+0001e050: 2068 7265 663d 2225 732e 6869 7374 2f25   href="%s.hist/%
+0001e060: 7322 3e23 2573 3c2f 613e 2720 2520 280a  s">#%s</a>' % (.
+0001e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e080: 2020 2020 6261 7365 2c0a 2020 2020 2020      base,.      
+0001e090: 2020 2020 2020 2020 2020 2020 2020 6874                ht
+0001e0a0: 6d6c 5f65 7363 6170 6528 6869 7374 5b66  ml_escape(hist[f
+0001e0b0: 6e5d 5b32 5d2c 2071 756f 743d 5472 7565  n][2], quot=True
+0001e0c0: 2c20 6372 6c66 3d54 7275 6529 2c0a 2020  , crlf=True),.  
+0001e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e0e0: 2020 6869 7374 5b66 6e5d 5b30 5d2c 0a20    hist[fn][0],. 
+0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001e100: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001e110: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001e120: 2020 206d 6172 6769 6e20 3d20 222d 220a     margin = "-".
+0001e130: 0a20 2020 2020 2020 2020 2020 2073 7a20  .            sz 
+0001e140: 3d20 696e 662e 7374 5f73 697a 650a 2020  = inf.st_size.  
+0001e150: 2020 2020 2020 2020 2020 7a64 203d 2064            zd = d
+0001e160: 6174 6574 696d 652e 7574 6366 726f 6d74  atetime.utcfromt
+0001e170: 696d 6573 7461 6d70 286c 696e 662e 7374  imestamp(linf.st
+0001e180: 5f6d 7469 6d65 290a 2020 2020 2020 2020  _mtime).        
+0001e190: 2020 2020 6474 203d 2022 2530 3464 2d25      dt = "%04d-%
+0001e1a0: 3032 642d 2530 3264 2025 3032 643a 2530  02d-%02d %02d:%0
+0001e1b0: 3264 3a25 3032 6422 2025 2028 0a20 2020  2d:%02d" % (.   
+0001e1c0: 2020 2020 2020 2020 2020 2020 207a 642e               zd.
+0001e1d0: 7965 6172 2c0a 2020 2020 2020 2020 2020  year,.          
+0001e1e0: 2020 2020 2020 7a64 2e6d 6f6e 7468 2c0a        zd.month,.
+0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e200: 7a64 2e64 6179 2c0a 2020 2020 2020 2020  zd.day,.        
+0001e210: 2020 2020 2020 2020 7a64 2e68 6f75 722c          zd.hour,
+0001e220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e230: 207a 642e 6d69 6e75 7465 2c0a 2020 2020   zd.minute,.    
+0001e240: 2020 2020 2020 2020 2020 2020 7a64 2e73              zd.s
+0001e250: 6563 6f6e 642c 0a20 2020 2020 2020 2020  econd,.         
+0001e260: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+0001e270: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+0001e280: 2020 2020 2020 2065 7874 203d 2022 2d2d         ext = "--
+0001e290: 2d22 2069 6620 6973 5f64 6972 2065 6c73  -" if is_dir els
+0001e2a0: 6520 666e 2e72 7370 6c69 7428 222e 222c  e fn.rsplit(".",
+0001e2b0: 2031 295b 315d 0a20 2020 2020 2020 2020   1)[1].         
+0001e2c0: 2020 2020 2020 2069 6620 6c65 6e28 6578         if len(ex
+0001e2d0: 7429 203e 2031 363a 0a20 2020 2020 2020  t) > 16:.       
+0001e2e0: 2020 2020 2020 2020 2020 2020 2065 7874               ext
+0001e2f0: 203d 2065 7874 5b3a 3136 5d0a 2020 2020   = ext[:16].    
+0001e300: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+0001e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e320: 6578 7420 3d20 2225 220a 0a20 2020 2020  ext = "%"..     
+0001e330: 2020 2020 2020 2069 6620 6164 645f 666b         if add_fk
+0001e340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001e350: 2020 6872 6566 203d 2022 2573 3f6b 3d25    href = "%s?k=%
+0001e360: 7322 2025 2028 0a20 2020 2020 2020 2020  s" % (.         
+0001e370: 2020 2020 2020 2020 2020 2071 756f 7465             quote
+0001e380: 7028 6872 6566 292c 0a20 2020 2020 2020  p(href),.       
+0001e390: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+0001e3a0: 662e 6765 6e5f 666b 280a 2020 2020 2020  f.gen_fk(.      
+0001e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3c0: 2020 7365 6c66 2e61 7267 732e 666b 5f73    self.args.fk_s
+0001e3d0: 616c 742c 2066 7370 6174 682c 2073 7a2c  alt, fspath, sz,
+0001e3e0: 2030 2069 6620 414e 5957 494e 2065 6c73   0 if ANYWIN els
+0001e3f0: 6520 696e 662e 7374 5f69 6e6f 0a20 2020  e inf.st_ino.   
+0001e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e410: 2029 5b3a 6164 645f 666b 5d2c 0a20 2020   )[:add_fk],.   
+0001e420: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0001e430: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001e440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e450: 2068 7265 6620 3d20 7175 6f74 6570 2868   href = quotep(h
+0001e460: 7265 6629 0a0a 2020 2020 2020 2020 2020  ref)..          
+0001e470: 2020 6974 656d 203d 207b 0a20 2020 2020    item = {.     
+0001e480: 2020 2020 2020 2020 2020 2022 6c65 6164             "lead
+0001e490: 223a 206d 6172 6769 6e2c 0a20 2020 2020  ": margin,.     
+0001e4a0: 2020 2020 2020 2020 2020 2022 6872 6566             "href
+0001e4b0: 223a 2068 7265 662c 0a20 2020 2020 2020  ": href,.       
+0001e4c0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+0001e4d0: 2066 6e2c 0a20 2020 2020 2020 2020 2020   fn,.           
+0001e4e0: 2020 2020 2022 737a 223a 2073 7a2c 0a20       "sz": sz,. 
+0001e4f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001e500: 6578 7422 3a20 6578 742c 0a20 2020 2020  ext": ext,.     
+0001e510: 2020 2020 2020 2020 2020 2022 6474 223a             "dt":
+0001e520: 2064 742c 0a20 2020 2020 2020 2020 2020   dt,.           
+0001e530: 2020 2020 2022 7473 223a 2069 6e74 286c       "ts": int(l
+0001e540: 696e 662e 7374 5f6d 7469 6d65 292c 0a20  inf.st_mtime),. 
+0001e550: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+0001e560: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
+0001e570: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
+0001e580: 2020 2020 6469 7273 2e61 7070 656e 6428      dirs.append(
+0001e590: 6974 656d 290a 2020 2020 2020 2020 2020  item).          
+0001e5a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001e5b0: 2020 2020 2020 2020 6669 6c65 732e 6170          files.ap
+0001e5c0: 7065 6e64 2869 7465 6d29 0a20 2020 2020  pend(item).     
+0001e5d0: 2020 2020 2020 2020 2020 2069 7465 6d5b             item[
+0001e5e0: 2272 6422 5d20 3d20 7265 6d0a 0a20 2020  "rd"] = rem..   
+0001e5f0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+0001e600: 2020 2020 2020 7365 6c66 2e63 6f6f 6b69        self.cooki
+0001e610: 6573 2e67 6574 2822 6964 7868 2229 203d  es.get("idxh") =
+0001e620: 3d20 2279 220a 2020 2020 2020 2020 2020  = "y".          
+0001e630: 2020 616e 6420 226c 7322 206e 6f74 2069    and "ls" not i
+0001e640: 6e20 7365 6c66 2e75 7061 7261 6d0a 2020  n self.uparam.  
+0001e650: 2020 2020 2020 2020 2020 616e 6420 2276            and "v
+0001e660: 2220 6e6f 7420 696e 2073 656c 662e 7570  " not in self.up
+0001e670: 6172 616d 0a20 2020 2020 2020 2029 3a0a  aram.        ):.
+0001e680: 2020 2020 2020 2020 2020 2020 6964 785f              idx_
+0001e690: 6874 6d6c 203d 2073 6574 285b 2269 6e64  html = set(["ind
+0001e6a0: 6578 2e68 746d 222c 2022 696e 6465 782e  ex.htm", "index.
+0001e6b0: 6874 6d6c 225d 290a 2020 2020 2020 2020  html"]).        
+0001e6c0: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
+0001e6d0: 6669 6c65 733a 0a20 2020 2020 2020 2020  files:.         
+0001e6e0: 2020 2020 2020 2069 6620 6974 656d 5b22         if item["
+0001e6f0: 6e61 6d65 225d 2069 6e20 6964 785f 6874  name"] in idx_ht
+0001e700: 6d6c 3a0a 2020 2020 2020 2020 2020 2020  ml:.            
+0001e710: 2020 2020 2020 2020 2320 646f 2066 756c          # do ful
+0001e720: 6c20 7265 736f 6c76 6520 696e 2063 6173  l resolve in cas
+0001e730: 6520 6f66 2073 6861 646f 7765 6420 6669  e of shadowed fi
+0001e740: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+0001e750: 2020 2020 2020 2076 7020 3d20 766a 6f69         vp = vjoi
+0001e760: 6e28 7365 6c66 2e76 7061 7468 2e73 706c  n(self.vpath.spl
+0001e770: 6974 2822 3f22 295b 305d 2c20 6974 656d  it("?")[0], item
+0001e780: 5b22 6e61 6d65 225d 290a 2020 2020 2020  ["name"]).      
+0001e790: 2020 2020 2020 2020 2020 2020 2020 766e                vn
+0001e7a0: 2c20 7265 6d20 3d20 7365 6c66 2e61 7372  , rem = self.asr
+0001e7b0: 762e 7666 732e 6765 7428 7670 2c20 7365  v.vfs.get(vp, se
+0001e7c0: 6c66 2e75 6e61 6d65 2c20 5472 7565 2c20  lf.uname, True, 
+0001e7d0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+0001e7e0: 2020 2020 2020 2020 2020 2061 7020 3d20             ap = 
+0001e7f0: 766e 2e63 616e 6f6e 6963 616c 2872 656d  vn.canonical(rem
+0001e800: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001e810: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0001e820: 662e 7478 5f66 696c 6528 6170 2920 2023  f.tx_file(ap)  #
+0001e830: 2069 7320 6e6f 2d63 6163 6865 0a0a 2020   is no-cache..  
+0001e840: 2020 2020 2020 7461 6773 6574 2020 3d20        tagset  = 
+0001e850: 7365 7428 290a 2020 2020 2020 2020 666f  set().        fo
+0001e860: 7220 6665 2069 6e20 6669 6c65 733a 0a20  r fe in files:. 
+0001e870: 2020 2020 2020 2020 2020 2066 6e20 3d20             fn = 
+0001e880: 6665 5b22 6e61 6d65 225d 0a20 2020 2020  fe["name"].     
+0001e890: 2020 2020 2020 2072 6420 3d20 6665 5b22         rd = fe["
+0001e8a0: 7264 225d 0a20 2020 2020 2020 2020 2020  rd"].           
+0001e8b0: 2064 656c 2066 655b 2272 6422 5d0a 2020   del fe["rd"].  
+0001e8c0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0001e8d0: 2069 6375 723a 0a20 2020 2020 2020 2020   icur:.         
+0001e8e0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0001e8f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001e900: 766e 2021 3d20 6462 763a 0a20 2020 2020  vn != dbv:.     
+0001e910: 2020 2020 2020 2020 2020 205f 2c20 7264             _, rd
+0001e920: 203d 2076 6e2e 6765 745f 6462 7628 7264   = vn.get_dbv(rd
+0001e930: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
+0001e940: 7264 5f65 666e 203d 2028 7264 2c20 666e  rd_efn = (rd, fn
+0001e950: 290a 2020 2020 2020 2020 2020 2020 7120  ).            q 
+0001e960: 3d20 2273 656c 6563 7420 6d74 2e6b 2c20  = "select mt.k, 
+0001e970: 6d74 2e76 2066 726f 6d20 7570 2069 6e6e  mt.v from up inn
+0001e980: 6572 206a 6f69 6e20 6d74 206f 6e20 6d74  er join mt on mt
+0001e990: 2e77 203d 2073 7562 7374 7228 7570 2e77  .w = substr(up.w
+0001e9a0: 2c31 2c31 3629 2077 6865 7265 2075 702e  ,1,16) where up.
+0001e9b0: 7264 203d 203f 2061 6e64 2075 702e 666e  rd = ? and up.fn
+0001e9c0: 203d 203f 2061 6e64 202b 6d74 2e6b 2021   = ? and +mt.k !
+0001e9d0: 3d20 2778 2722 0a20 2020 2020 2020 2020  = 'x'".         
+0001e9e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001e9f0: 2020 2020 2020 2020 7220 3d20 6963 7572          r = icur
+0001ea00: 2e65 7865 6375 7465 2871 2c20 6572 645f  .execute(q, erd_
+0001ea10: 6566 6e29 0a20 2020 2020 2020 2020 2020  efn).           
+0001ea20: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0001ea30: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
+0001ea40: 2020 2020 2020 2020 2069 6620 2264 6174           if "dat
+0001ea50: 6162 6173 6520 6973 206c 6f63 6b65 6422  abase is locked"
+0001ea60: 2069 6e20 7374 7228 6578 293a 0a20 2020   in str(ex):.   
+0001ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea80: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
+0001ea90: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0001eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eab0: 2065 7264 5f65 666e 203d 2073 3365 6e63   erd_efn = s3enc
+0001eac0: 2869 6478 2e6d 656d 5f63 7572 2c20 7264  (idx.mem_cur, rd
+0001ead0: 2c20 666e 290a 2020 2020 2020 2020 2020  , fn).          
+0001eae0: 2020 2020 2020 2020 2020 7220 3d20 6963            r = ic
+0001eaf0: 7572 2e65 7865 6375 7465 2871 2c20 6572  ur.execute(q, er
+0001eb00: 645f 6566 6e29 0a20 2020 2020 2020 2020  d_efn).         
+0001eb10: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+0001eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb30: 2020 2074 203d 2022 7461 6720 7265 6164     t = "tag read
+0001eb40: 2065 7272 6f72 2c20 7b7d 2f7b 7d5c 6e7b   error, {}/{}\n{
+0001eb50: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0001eb60: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+0001eb70: 742e 666f 726d 6174 2872 642c 2066 6e2c  t.format(rd, fn,
+0001eb80: 206d 696e 5f65 7828 2929 290a 2020 2020   min_ex())).    
+0001eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eba0: 6272 6561 6b0a 0a20 2020 2020 2020 2020  break..         
+0001ebb0: 2020 2066 655b 2274 6167 7322 5d20 3d20     fe["tags"] = 
+0001ebc0: 7b6b 3a20 7620 666f 7220 6b2c 2076 2069  {k: v for k, v i
+0001ebd0: 6e20 727d 0a0a 2020 2020 2020 2020 2020  n r}..          
+0001ebe0: 2020 6966 2073 656c 662e 6361 6e5f 6164    if self.can_ad
+0001ebf0: 6d69 6e3a 0a20 2020 2020 2020 2020 2020  min:.           
+0001ec00: 2020 2020 2071 203d 2022 7365 6c65 6374       q = "select
+0001ec10: 2069 702c 2061 7420 6672 6f6d 2075 7020   ip, at from up 
+0001ec20: 7768 6572 6520 7264 3d3f 2061 6e64 2066  where rd=? and f
+0001ec30: 6e3d 3f22 0a20 2020 2020 2020 2020 2020  n=?".           
+0001ec40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0001ec50: 2020 2020 2020 2020 2020 2020 2020 7a73                zs
+0001ec60: 312c 207a 7332 203d 2069 6375 722e 6578  1, zs2 = icur.ex
+0001ec70: 6563 7574 6528 712c 2065 7264 5f65 666e  ecute(q, erd_efn
+0001ec80: 292e 6665 7463 686f 6e65 2829 0a20 2020  ).fetchone().   
+0001ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eca0: 2066 655b 2274 6167 7322 5d5b 2275 705f   fe["tags"]["up_
+0001ecb0: 6970 225d 203d 207a 7331 0a20 2020 2020  ip"] = zs1.     
+0001ecc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001ecd0: 655b 2274 6167 7322 5d5b 222e 7570 5f61  e["tags"][".up_a
+0001ece0: 7422 5d20 3d20 7a73 320a 2020 2020 2020  t"] = zs2.      
+0001ecf0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0001ed00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ed10: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0001ed20: 2020 2020 2020 2020 5f20 3d20 5b74 6167          _ = [tag
+0001ed30: 7365 742e 6164 6428 6b29 2066 6f72 206b  set.add(k) for k
+0001ed40: 2069 6e20 6665 5b22 7461 6773 225d 5d0a   in fe["tags"]].
+0001ed50: 0a20 2020 2020 2020 2069 6620 6963 7572  .        if icur
+0001ed60: 3a0a 2020 2020 2020 2020 2020 2020 6d74  :.            mt
+0001ed70: 6520 3d20 766e 2e66 6c61 6773 2e67 6574  e = vn.flags.get
+0001ed80: 2822 6d74 6522 2920 6f72 2022 7570 5f69  ("mte") or "up_i
+0001ed90: 702c 2e75 705f 6174 220a 2020 2020 2020  p,.up_at".      
+0001eda0: 2020 2020 2020 7461 676c 6973 7420 3d20        taglist = 
+0001edb0: 5b6b 2066 6f72 206b 2069 6e20 6d74 652e  [k for k in mte.
+0001edc0: 7370 6c69 7428 222c 2229 2069 6620 6b20  split(",") if k 
+0001edd0: 696e 2074 6167 7365 745d 0a20 2020 2020  in tagset].     
+0001ede0: 2020 2020 2020 2066 6f72 2066 6520 696e         for fe in
+0001edf0: 2064 6972 733a 0a20 2020 2020 2020 2020   dirs:.         
+0001ee00: 2020 2020 2020 2066 655b 2274 6167 7322         fe["tags"
+0001ee10: 5d20 3d20 7b7d 0a20 2020 2020 2020 2065  ] = {}.        e
+0001ee20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001ee30: 2074 6167 6c69 7374 203d 206c 6973 7428   taglist = list(
+0001ee40: 7461 6773 6574 290a 0a20 2020 2020 2020  tagset)..       
+0001ee50: 2069 6620 6973 5f6c 733a 0a20 2020 2020   if is_ls:.     
+0001ee60: 2020 2020 2020 206c 735f 7265 745b 2264         ls_ret["d
+0001ee70: 6972 7322 5d20 3d20 6469 7273 0a20 2020  irs"] = dirs.   
 0001ee80: 2020 2020 2020 2020 206c 735f 7265 745b           ls_ret[
-0001ee90: 2264 6972 7322 5d20 3d20 6469 7273 0a20  "dirs"] = dirs. 
-0001eea0: 2020 2020 2020 2020 2020 206c 735f 7265             ls_re
-0001eeb0: 745b 2266 696c 6573 225d 203d 2066 696c  t["files"] = fil
-0001eec0: 6573 0a20 2020 2020 2020 2020 2020 206c  es.            l
-0001eed0: 735f 7265 745b 2274 6167 6c69 7374 225d  s_ret["taglist"]
-0001eee0: 203d 2074 6167 6c69 7374 0a20 2020 2020   = taglist.     
-0001eef0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001ef00: 6c66 2e74 785f 6c73 286c 735f 7265 7429  lf.tx_ls(ls_ret)
-0001ef10: 0a0a 2020 2020 2020 2020 646f 6320 3d20  ..        doc = 
-0001ef20: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
-0001ef30: 2264 6f63 2229 2069 6620 7365 6c66 2e63  "doc") if self.c
-0001ef40: 616e 5f72 6561 6420 656c 7365 204e 6f6e  an_read else Non
-0001ef50: 650a 2020 2020 2020 2020 6966 2064 6f63  e.        if doc
-0001ef60: 3a0a 2020 2020 2020 2020 2020 2020 646f  :.            do
-0001ef70: 6320 3d20 756e 7175 6f74 6570 2864 6f63  c = unquotep(doc
-0001ef80: 2e72 6570 6c61 6365 2822 2b22 2c20 2220  .replace("+", " 
-0001ef90: 2229 2e73 706c 6974 2822 3f22 295b 305d  ").split("?")[0]
-0001efa0: 290a 2020 2020 2020 2020 2020 2020 6a32  ).            j2
-0001efb0: 615b 2264 6f63 6e61 6d65 225d 203d 2064  a["docname"] = d
-0001efc0: 6f63 0a20 2020 2020 2020 2020 2020 2064  oc.            d
-0001efd0: 6f63 7478 7420 3d20 4e6f 6e65 0a20 2020  octxt = None.   
-0001efe0: 2020 2020 2020 2020 2069 6620 6e65 7874           if next
-0001eff0: 2828 7820 666f 7220 7820 696e 2066 696c  ((x for x in fil
-0001f000: 6573 2069 6620 785b 226e 616d 6522 5d20  es if x["name"] 
-0001f010: 3d3d 2064 6f63 292c 204e 6f6e 6529 3a0a  == doc), None):.
-0001f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f030: 646f 6370 6174 6820 3d20 6f73 2e70 6174  docpath = os.pat
-0001f040: 682e 6a6f 696e 2861 6273 7061 7468 2c20  h.join(abspath, 
-0001f050: 646f 6329 0a20 2020 2020 2020 2020 2020  doc).           
-0001f060: 2020 2020 2073 7a20 3d20 626f 732e 7061       sz = bos.pa
-0001f070: 7468 2e67 6574 7369 7a65 2864 6f63 7061  th.getsize(docpa
-0001f080: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
-0001f090: 2020 2020 6966 2073 7a20 3c20 3130 3234      if sz < 1024
-0001f0a0: 202a 2073 656c 662e 6172 6773 2e74 7874   * self.args.txt
-0001f0b0: 5f6d 6178 3a0a 2020 2020 2020 2020 2020  _max:.          
-0001f0c0: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-0001f0d0: 7065 6e28 6673 656e 6328 646f 6370 6174  pen(fsenc(docpat
-0001f0e0: 6829 2c20 2272 6222 2920 6173 2066 3a0a  h), "rb") as f:.
-0001f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f100: 2020 2020 2020 2020 646f 6374 7874 203d          doctxt =
-0001f110: 2066 2e72 6561 6428 292e 6465 636f 6465   f.read().decode
-0001f120: 2822 7574 662d 3822 2c20 2272 6570 6c61  ("utf-8", "repla
-0001f130: 6365 2229 0a20 2020 2020 2020 2020 2020  ce").           
-0001f140: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0001f150: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
-0001f160: 2264 6f63 2034 3034 3a20 5b7b 7d5d 222e  "doc 404: [{}]".
-0001f170: 666f 726d 6174 2864 6f63 292c 2063 3d36  format(doc), c=6
-0001f180: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001f190: 2020 646f 6374 7874 203d 2022 2820 7465    doctxt = "( te
-0001f1a0: 7874 6669 6c65 206e 6f74 2066 6f75 6e64  xtfile not found
-0001f1b0: 2029 220a 0a20 2020 2020 2020 2020 2020   )"..           
-0001f1c0: 2069 6620 646f 6374 7874 2069 7320 6e6f   if doctxt is no
-0001f1d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0001f1e0: 2020 2020 2020 2020 6a32 615b 2264 6f63          j2a["doc
-0001f1f0: 225d 203d 2064 6f63 7478 740a 0a20 2020  "] = doctxt..   
-0001f200: 2020 2020 2066 6f72 2064 2069 6e20 6469       for d in di
-0001f210: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0001f220: 645b 226e 616d 6522 5d20 2b3d 2022 2f22  d["name"] += "/"
-0001f230: 0a0a 2020 2020 2020 2020 6469 7273 2e73  ..        dirs.s
-0001f240: 6f72 7428 6b65 793d 6974 656d 6765 7474  ort(key=itemgett
-0001f250: 6572 2822 6e61 6d65 2229 290a 0a20 2020  er("name"))..   
-0001f260: 2020 2020 2069 6620 6973 5f6a 733a 0a20       if is_js:. 
-0001f270: 2020 2020 2020 2020 2020 206a 3261 5b22             j2a["
-0001f280: 6c73 3022 5d20 3d20 7b0a 2020 2020 2020  ls0"] = {.      
-0001f290: 2020 2020 2020 2020 2020 2264 6972 7322            "dirs"
-0001f2a0: 3a20 6469 7273 2c0a 2020 2020 2020 2020  : dirs,.        
-0001f2b0: 2020 2020 2020 2020 2266 696c 6573 223a          "files":
-0001f2c0: 2066 696c 6573 2c0a 2020 2020 2020 2020   files,.        
-0001f2d0: 2020 2020 2020 2020 2274 6167 6c69 7374          "taglist
-0001f2e0: 223a 2074 6167 6c69 7374 2c0a 2020 2020  ": taglist,.    
-0001f2f0: 2020 2020 2020 2020 2020 2020 2275 6e6c              "unl
-0001f300: 6973 7422 3a20 756e 6c69 7374 2c0a 2020  ist": unlist,.  
-0001f310: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-0001f320: 2020 2020 2020 2020 6a32 615b 2266 696c          j2a["fil
-0001f330: 6573 225d 203d 205b 5d0a 2020 2020 2020  es"] = [].      
-0001f340: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001f350: 2020 2020 6a32 615b 2266 696c 6573 225d      j2a["files"]
-0001f360: 203d 2064 6972 7320 2b20 6669 6c65 730a   = dirs + files.
-0001f370: 0a20 2020 2020 2020 206a 3261 5b22 7461  .        j2a["ta
-0001f380: 676c 6973 7422 5d20 3d20 7461 676c 6973  glist"] = taglis
-0001f390: 740a 2020 2020 2020 2020 6a32 615b 2274  t.        j2a["t
-0001f3a0: 7874 5f65 7874 225d 203d 2073 656c 662e  xt_ext"] = self.
-0001f3b0: 6172 6773 2e74 6578 7466 696c 6573 2e72  args.textfiles.r
-0001f3c0: 6570 6c61 6365 2822 2c22 2c20 2220 2229  eplace(",", " ")
-0001f3d0: 0a0a 2020 2020 2020 2020 6966 2022 6d74  ..        if "mt
-0001f3e0: 6822 2069 6e20 766e 2e66 6c61 6773 3a0a  h" in vn.flags:.
-0001f3f0: 2020 2020 2020 2020 2020 2020 6a32 615b              j2a[
-0001f400: 2264 6566 5f68 636f 6c73 225d 203d 2076  "def_hcols"] = v
-0001f410: 6e2e 666c 6167 735b 226d 7468 225d 2e73  n.flags["mth"].s
-0001f420: 706c 6974 2822 2c22 290a 0a20 2020 2020  plit(",")..     
-0001f430: 2020 2068 746d 6c20 3d20 7365 6c66 2e6a     html = self.j
-0001f440: 3273 2874 706c 2c20 2a2a 6a32 6129 0a20  2s(tpl, **j2a). 
-0001f450: 2020 2020 2020 2073 656c 662e 7265 706c         self.repl
-0001f460: 7928 6874 6d6c 2e65 6e63 6f64 6528 2275  y(html.encode("u
-0001f470: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
-0001f480: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-0001f490: 6e20 5472 7565 0a                        n True.
+0001ee90: 2266 696c 6573 225d 203d 2066 696c 6573  "files"] = files
+0001eea0: 0a20 2020 2020 2020 2020 2020 206c 735f  .            ls_
+0001eeb0: 7265 745b 2274 6167 6c69 7374 225d 203d  ret["taglist"] =
+0001eec0: 2074 6167 6c69 7374 0a20 2020 2020 2020   taglist.       
+0001eed0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0001eee0: 2e74 785f 6c73 286c 735f 7265 7429 0a0a  .tx_ls(ls_ret)..
+0001eef0: 2020 2020 2020 2020 646f 6320 3d20 7365          doc = se
+0001ef00: 6c66 2e75 7061 7261 6d2e 6765 7428 2264  lf.uparam.get("d
+0001ef10: 6f63 2229 2069 6620 7365 6c66 2e63 616e  oc") if self.can
+0001ef20: 5f72 6561 6420 656c 7365 204e 6f6e 650a  _read else None.
+0001ef30: 2020 2020 2020 2020 6966 2064 6f63 3a0a          if doc:.
+0001ef40: 2020 2020 2020 2020 2020 2020 646f 6320              doc 
+0001ef50: 3d20 756e 7175 6f74 6570 2864 6f63 2e72  = unquotep(doc.r
+0001ef60: 6570 6c61 6365 2822 2b22 2c20 2220 2229  eplace("+", " ")
+0001ef70: 2e73 706c 6974 2822 3f22 295b 305d 290a  .split("?")[0]).
+0001ef80: 2020 2020 2020 2020 2020 2020 6a32 615b              j2a[
+0001ef90: 2264 6f63 6e61 6d65 225d 203d 2064 6f63  "docname"] = doc
+0001efa0: 0a20 2020 2020 2020 2020 2020 2064 6f63  .            doc
+0001efb0: 7478 7420 3d20 4e6f 6e65 0a20 2020 2020  txt = None.     
+0001efc0: 2020 2020 2020 2069 6620 6e65 7874 2828         if next((
+0001efd0: 7820 666f 7220 7820 696e 2066 696c 6573  x for x in files
+0001efe0: 2069 6620 785b 226e 616d 6522 5d20 3d3d   if x["name"] ==
+0001eff0: 2064 6f63 292c 204e 6f6e 6529 3a0a 2020   doc), None):.  
+0001f000: 2020 2020 2020 2020 2020 2020 2020 646f                do
+0001f010: 6370 6174 6820 3d20 6f73 2e70 6174 682e  cpath = os.path.
+0001f020: 6a6f 696e 2861 6273 7061 7468 2c20 646f  join(abspath, do
+0001f030: 6329 0a20 2020 2020 2020 2020 2020 2020  c).             
+0001f040: 2020 2073 7a20 3d20 626f 732e 7061 7468     sz = bos.path
+0001f050: 2e67 6574 7369 7a65 2864 6f63 7061 7468  .getsize(docpath
+0001f060: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001f070: 2020 6966 2073 7a20 3c20 3130 3234 202a    if sz < 1024 *
+0001f080: 2073 656c 662e 6172 6773 2e74 7874 5f6d   self.args.txt_m
+0001f090: 6178 3a0a 2020 2020 2020 2020 2020 2020  ax:.            
+0001f0a0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+0001f0b0: 6e28 6673 656e 6328 646f 6370 6174 6829  n(fsenc(docpath)
+0001f0c0: 2c20 2272 6222 2920 6173 2066 3a0a 2020  , "rb") as f:.  
+0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f0e0: 2020 2020 2020 646f 6374 7874 203d 2066        doctxt = f
+0001f0f0: 2e72 6561 6428 292e 6465 636f 6465 2822  .read().decode("
+0001f100: 7574 662d 3822 2c20 2272 6570 6c61 6365  utf-8", "replace
+0001f110: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+0001f120: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001f130: 2020 2020 2073 656c 662e 6c6f 6728 2264       self.log("d
+0001f140: 6f63 2034 3034 3a20 5b7b 7d5d 222e 666f  oc 404: [{}]".fo
+0001f150: 726d 6174 2864 6f63 292c 2063 3d36 290a  rmat(doc), c=6).
+0001f160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f170: 646f 6374 7874 203d 2022 2820 7465 7874  doctxt = "( text
+0001f180: 6669 6c65 206e 6f74 2066 6f75 6e64 2029  file not found )
+0001f190: 220a 0a20 2020 2020 2020 2020 2020 2069  "..            i
+0001f1a0: 6620 646f 6374 7874 2069 7320 6e6f 7420  f doctxt is not 
+0001f1b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0001f1c0: 2020 2020 2020 6a32 615b 2264 6f63 225d        j2a["doc"]
+0001f1d0: 203d 2064 6f63 7478 740a 0a20 2020 2020   = doctxt..     
+0001f1e0: 2020 2066 6f72 2064 2069 6e20 6469 7273     for d in dirs
+0001f1f0: 3a0a 2020 2020 2020 2020 2020 2020 645b  :.            d[
+0001f200: 226e 616d 6522 5d20 2b3d 2022 2f22 0a0a  "name"] += "/"..
+0001f210: 2020 2020 2020 2020 6469 7273 2e73 6f72          dirs.sor
+0001f220: 7428 6b65 793d 6974 656d 6765 7474 6572  t(key=itemgetter
+0001f230: 2822 6e61 6d65 2229 290a 0a20 2020 2020  ("name"))..     
+0001f240: 2020 2069 6620 6973 5f6a 733a 0a20 2020     if is_js:.   
+0001f250: 2020 2020 2020 2020 206a 3261 5b22 6c73           j2a["ls
+0001f260: 3022 5d20 3d20 7b0a 2020 2020 2020 2020  0"] = {.        
+0001f270: 2020 2020 2020 2020 2264 6972 7322 3a20          "dirs": 
+0001f280: 6469 7273 2c0a 2020 2020 2020 2020 2020  dirs,.          
+0001f290: 2020 2020 2020 2266 696c 6573 223a 2066        "files": f
+0001f2a0: 696c 6573 2c0a 2020 2020 2020 2020 2020  iles,.          
+0001f2b0: 2020 2020 2020 2274 6167 6c69 7374 223a        "taglist":
+0001f2c0: 2074 6167 6c69 7374 2c0a 2020 2020 2020   taglist,.      
+0001f2d0: 2020 2020 2020 2020 2020 2275 6e6c 6973            "unlis
+0001f2e0: 7422 3a20 756e 6c69 7374 2c0a 2020 2020  t": unlist,.    
+0001f2f0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0001f300: 2020 2020 2020 6a32 615b 2266 696c 6573        j2a["files
+0001f310: 225d 203d 205b 5d0a 2020 2020 2020 2020  "] = [].        
+0001f320: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001f330: 2020 6a32 615b 2266 696c 6573 225d 203d    j2a["files"] =
+0001f340: 2064 6972 7320 2b20 6669 6c65 730a 0a20   dirs + files.. 
+0001f350: 2020 2020 2020 206a 3261 5b22 7461 676c         j2a["tagl
+0001f360: 6973 7422 5d20 3d20 7461 676c 6973 740a  ist"] = taglist.
+0001f370: 2020 2020 2020 2020 6a32 615b 2274 7874          j2a["txt
+0001f380: 5f65 7874 225d 203d 2073 656c 662e 6172  _ext"] = self.ar
+0001f390: 6773 2e74 6578 7466 696c 6573 2e72 6570  gs.textfiles.rep
+0001f3a0: 6c61 6365 2822 2c22 2c20 2220 2229 0a0a  lace(",", " ")..
+0001f3b0: 2020 2020 2020 2020 6966 2022 6d74 6822          if "mth"
+0001f3c0: 2069 6e20 766e 2e66 6c61 6773 3a0a 2020   in vn.flags:.  
+0001f3d0: 2020 2020 2020 2020 2020 6a32 615b 2264            j2a["d
+0001f3e0: 6566 5f68 636f 6c73 225d 203d 2076 6e2e  ef_hcols"] = vn.
+0001f3f0: 666c 6167 735b 226d 7468 225d 2e73 706c  flags["mth"].spl
+0001f400: 6974 2822 2c22 290a 0a20 2020 2020 2020  it(",")..       
+0001f410: 2068 746d 6c20 3d20 7365 6c66 2e6a 3273   html = self.j2s
+0001f420: 2874 706c 2c20 2a2a 6a32 6129 0a20 2020  (tpl, **j2a).   
+0001f430: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
+0001f440: 6874 6d6c 2e65 6e63 6f64 6528 2275 7466  html.encode("utf
+0001f450: 2d38 222c 2022 7265 706c 6163 6522 2929  -8", "replace"))
+0001f460: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001f470: 5472 7565 0a                             True.
```

### Comparing `copyparty-1.8.3/copyparty/httpconn.py` & `copyparty-1.8.4/copyparty/httpconn.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/httpsrv.py` & `copyparty-1.8.4/copyparty/httpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/ico.py` & `copyparty-1.8.4/copyparty/ico.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/mdns.py` & `copyparty-1.8.4/copyparty/mdns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/mtag.py` & `copyparty-1.8.4/copyparty/mtag.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/multicast.py` & `copyparty-1.8.4/copyparty/multicast.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/pwhash.py` & `copyparty-1.8.4/copyparty/pwhash.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/res/COPYING.txt` & `copyparty-1.8.4/copyparty/res/COPYING.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/res/insecure.pem` & `copyparty-1.8.4/copyparty/res/insecure.pem`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/smbd.py` & `copyparty-1.8.4/copyparty/smbd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/ssdp.py` & `copyparty-1.8.4/copyparty/ssdp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/star.py` & `copyparty-1.8.4/copyparty/star.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/dnslib/bimap.py` & `copyparty-1.8.4/copyparty/stolen/dnslib/bimap.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/dnslib/buffer.py` & `copyparty-1.8.4/copyparty/stolen/dnslib/buffer.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/dnslib/dns.py` & `copyparty-1.8.4/copyparty/stolen/dnslib/dns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/dnslib/label.py` & `copyparty-1.8.4/copyparty/stolen/dnslib/label.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/dnslib/lex.py` & `copyparty-1.8.4/copyparty/stolen/dnslib/lex.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/dnslib/ranges.py` & `copyparty-1.8.4/copyparty/stolen/dnslib/ranges.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/ifaddr/_posix.py` & `copyparty-1.8.4/copyparty/stolen/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/ifaddr/_shared.py` & `copyparty-1.8.4/copyparty/stolen/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/ifaddr/_win32.py` & `copyparty-1.8.4/copyparty/stolen/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/qrcodegen.py` & `copyparty-1.8.4/copyparty/stolen/qrcodegen.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/stolen/surrogateescape.py` & `copyparty-1.8.4/copyparty/stolen/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/sutil.py` & `copyparty-1.8.4/copyparty/sutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/svchub.py` & `copyparty-1.8.4/copyparty/svchub.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/szip.py` & `copyparty-1.8.4/copyparty/szip.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/tcpsrv.py` & `copyparty-1.8.4/copyparty/tcpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/th_cli.py` & `copyparty-1.8.4/copyparty/th_cli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/th_srv.py` & `copyparty-1.8.4/copyparty/th_srv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/u2idx.py` & `copyparty-1.8.4/copyparty/u2idx.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/up2k.py` & `copyparty-1.8.4/copyparty/up2k.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,14 +876,15 @@
 
     def _build_file_index(self, vol , all_vols )   :
         do_vac = False
         top = vol.realpath
         rei = vol.flags.get("noidx")
         reh = vol.flags.get("nohash")
         n4g = bool(vol.flags.get("noforget"))
+        ffat = "fat32" in vol.flags
         cst = bos.stat(top)
         dev = cst.st_dev if vol.flags.get("xdev") else 0
 
         with self.mutex:
             reg = self.register_vpath(top, vol.flags)
             assert reg and self.pp
             cur, db_path = reg
@@ -912,14 +913,15 @@
                     top,
                     set(excl),
                     top,
                     rtop,
                     rei,
                     reh,
                     n4g,
+                    ffat,
                     [],
                     cst,
                     dev,
                     bool(vol.flags.get("xvol")),
                 )
                 if not n4g:
                     n_rm = self._drop_lost(db.c, top, excl)
@@ -967,14 +969,15 @@
         top ,
         excl ,
         cdir ,
         rcdir ,
         rei ,
         reh ,
         n4g ,
+        ffat ,
         seen ,
         cst ,
         dev ,
         xvol ,
     )  :
         if xvol and not rcdir.startswith(top):
             self.log("skip xvol: [{}] -> [{}]".format(cdir, rcdir), 6)
@@ -1011,15 +1014,15 @@
 
             if rei and rei.search(abspath):
                 unreg.append(rp)
                 continue
 
             lmod = int(inf.st_mtime)
             sz = inf.st_size
-            if fat32 and inf.st_mtime % 2:
+            if fat32 and not ffat and inf.st_mtime % 2:
                 fat32 = False
 
             if stat.S_ISDIR(inf.st_mode):
                 rap = absreal(abspath)
                 if dev and inf.st_dev != dev:
                     self.log("skip xdev {}->{}: {}".format(dev, inf.st_dev, abspath), 6)
                     continue
@@ -1028,15 +1031,27 @@
                     continue
                 if iname == ".th" and bos.path.isdir(os.path.join(abspath, "top")):
                     # abandoned or foreign, skip
                     continue
                 # self.log(" dir: {}".format(abspath))
                 try:
                     ret += self._build_dir(
-                        db, top, excl, abspath, rap, rei, reh, n4g, seen, inf, dev, xvol
+                        db,
+                        top,
+                        excl,
+                        abspath,
+                        rap,
+                        rei,
+                        reh,
+                        n4g,
+                        fat32,
+                        seen,
+                        inf,
+                        dev,
+                        xvol,
                     )
                 except:
                     t = "failed to index subdir [{}]:\n{}"
                     self.log(t.format(abspath, min_ex()), c=1)
             elif not stat.S_ISREG(inf.st_mode):
                 self.log("skip type-{:x} file [{}]".format(inf.st_mode, abspath))
             else:
```

### Comparing `copyparty-1.8.3/copyparty/util.py` & `copyparty-1.8.4/copyparty/util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/a/partyfuse.py` & `copyparty-1.8.4/copyparty/web/a/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/a/u2c.py` & `copyparty-1.8.4/copyparty/web/a/u2c.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/a/webdav-cfg.bat` & `copyparty-1.8.4/copyparty/web/a/webdav-cfg.bat`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/baguettebox.js.gz` & `copyparty-1.8.4/copyparty/web/baguettebox.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/browser.css.gz` & `copyparty-1.8.4/copyparty/web/browser.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/browser.html` & `copyparty-1.8.4/copyparty/web/browser.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/browser.js.gz` & `copyparty-1.8.4/copyparty/web/browser.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/browser2.html` & `copyparty-1.8.4/copyparty/web/browser2.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/cf.html` & `copyparty-1.8.4/copyparty/web/cf.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/dbg-audio.js.gz` & `copyparty-1.8.4/copyparty/web/dbg-audio.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/easymde.css.gz` & `copyparty-1.8.4/copyparty/web/deps/easymde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/easymde.js.gz` & `copyparty-1.8.4/copyparty/web/deps/easymde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/marked.js.gz` & `copyparty-1.8.4/copyparty/web/deps/marked.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/mini-fa.css.gz` & `copyparty-1.8.4/copyparty/web/deps/mini-fa.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/mini-fa.woff` & `copyparty-1.8.4/copyparty/web/deps/mini-fa.woff`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/prism.css.gz` & `copyparty-1.8.4/copyparty/web/deps/prism.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/prism.js.gz` & `copyparty-1.8.4/copyparty/web/deps/prism.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/prismd.css.gz` & `copyparty-1.8.4/copyparty/web/deps/prismd.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/scp.woff2` & `copyparty-1.8.4/copyparty/web/deps/scp.woff2`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/sha512.ac.js.gz` & `copyparty-1.8.4/copyparty/web/deps/sha512.ac.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/deps/sha512.hw.js.gz` & `copyparty-1.8.4/copyparty/web/deps/sha512.hw.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/md.css.gz` & `copyparty-1.8.4/copyparty/web/md.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/md.html` & `copyparty-1.8.4/copyparty/web/md.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/md.js.gz` & `copyparty-1.8.4/copyparty/web/md.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/md2.css.gz` & `copyparty-1.8.4/copyparty/web/md2.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/md2.js.gz` & `copyparty-1.8.4/copyparty/web/md2.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/mde.css.gz` & `copyparty-1.8.4/copyparty/web/mde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/mde.html` & `copyparty-1.8.4/copyparty/web/mde.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/mde.js.gz` & `copyparty-1.8.4/copyparty/web/mde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/msg.html` & `copyparty-1.8.4/copyparty/web/msg.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/splash.css.gz` & `copyparty-1.8.4/copyparty/web/splash.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/splash.html` & `copyparty-1.8.4/copyparty/web/splash.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/splash.js.gz` & `copyparty-1.8.4/copyparty/web/splash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/svcs.html` & `copyparty-1.8.4/copyparty/web/svcs.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/svcs.js.gz` & `copyparty-1.8.4/copyparty/web/svcs.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/ui.css.gz` & `copyparty-1.8.4/copyparty/web/ui.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/up2k.js.gz` & `copyparty-1.8.4/copyparty/web/up2k.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/util.js.gz` & `copyparty-1.8.4/copyparty/web/util.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty/web/w.hash.js.gz` & `copyparty-1.8.4/copyparty/web/w.hash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/copyparty.egg-info/PKG-INFO` & `copyparty-1.8.4/copyparty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.8.3
+Version: 1.8.4
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.8.3/copyparty.egg-info/SOURCES.txt` & `copyparty-1.8.4/copyparty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.3/pyproject.toml` & `copyparty-1.8.4/pyproject.toml`

 * *Files identical despite different names*

