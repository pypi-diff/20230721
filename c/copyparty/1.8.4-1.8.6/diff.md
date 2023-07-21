# Comparing `tmp/copyparty-1.8.4.tar.gz` & `tmp/copyparty-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyparty-1.8.4.tar", last modified: Tue Jul 18 08:04:10 2023, max compression
+gzip compressed data, was "copyparty-1.8.6.tar", last modified: Fri Jul 21 00:58:32 2023, max compression
```

## Comparing `copyparty-1.8.4.tar` & `copyparty-1.8.6.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.056205 copyparty-1.8.4/
--rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.8.4/LICENSE
--rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-18 08:04:10.056205 copyparty-1.8.4/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)    96750 2023-07-16 21:23:16.000000 copyparty-1.8.4/README.md
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.045205 copyparty-1.8.4/copyparty/
--rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    76501 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/__main__.py
--rw-r--r--   0 ed        (1000) ed        (1000)      246 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/__version__.py
--rw-r--r--   0 ed        (1000) ed        (1000)    69349 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/authsrv.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.046205 copyparty-1.8.4/copyparty/bos/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/bos/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/bos/bos.py
--rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/bos/path.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3915 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_mp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_mpw.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_thr.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/broker_util.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7135 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/cert.py
--rw-r--r--   0 ed        (1000) ed        (1000)     7564 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/cfg.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/dxml.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/fsutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15455 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/ftpd.py
--rw-r--r--   0 ed        (1000) ed        (1000)   128117 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/httpcli.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/httpconn.py
--rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/httpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3016 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/ico.py
--rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/mdns.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/mtag.py
--rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/multicast.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3859 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/pwhash.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.047205 copyparty-1.8.4/copyparty/res/
--rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/res/COPYING.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/res/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.8.4/copyparty/res/insecure.pem
--rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/smbd.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/ssdp.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/star.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.047205 copyparty-1.8.4/copyparty/stolen/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.048205 copyparty-1.8.4/copyparty/stolen/dnslib/
--rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/bimap.py
--rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/bit.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/buffer.py
--rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/dns.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/label.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/lex.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/dnslib/ranges.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.048205 copyparty-1.8.4/copyparty/stolen/ifaddr/
--rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/_posix.py
--rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/_shared.py
--rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/ifaddr/_win32.py
--rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/qrcodegen.py
--rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/stolen/surrogateescape.py
--rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/sutil.py
--rw-r--r--   0 ed        (1000) ed        (1000)    24336 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/svchub.py
--rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/szip.py
--rw-r--r--   0 ed        (1000) ed        (1000)    16753 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/tcpsrv.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/th_cli.py
--rw-r--r--   0 ed        (1000) ed        (1000)    22828 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/th_srv.py
--rw-r--r--   0 ed        (1000) ed        (1000)    10589 2023-07-18 08:03:52.000000 copyparty-1.8.4/copyparty/u2idx.py
--rw-r--r--   0 ed        (1000) ed        (1000)   124800 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/up2k.py
--rw-r--r--   0 ed        (1000) ed        (1000)    72768 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/util.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.052205 copyparty-1.8.4/copyparty/web/
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.052205 copyparty-1.8.4/copyparty/web/a/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/a/__init__.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/a/partyfuse.py
--rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/a/u2c.py
--rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.8.4/copyparty/web/a/webdav-cfg.bat
--rw-r--r--   0 ed        (1000) ed        (1000)     7309 2023-07-16 17:45:42.000000 copyparty-1.8.4/copyparty/web/baguettebox.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10996 2023-07-13 23:14:15.000000 copyparty-1.8.4/copyparty/web/browser.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.8.4/copyparty/web/browser.html
--rw-r--r--   0 ed        (1000) ed        (1000)    59820 2023-07-16 18:14:02.000000 copyparty-1.8.4/copyparty/web/browser.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.8.4/copyparty/web/browser2.html
--rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.8.4/copyparty/web/cf.html
--rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.8.4/copyparty/web/dbg-audio.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.053205 copyparty-1.8.4/copyparty/web/dd/
--rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/2.png
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/3.png
--rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/4.png
--rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/dd/5.png
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/dd/__init__.py
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.055205 copyparty-1.8.4/copyparty/web/deps/
--rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-18 08:03:53.000000 copyparty-1.8.4/copyparty/web/deps/__init__.py
--rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.8.4/copyparty/web/deps/easymde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.8.4/copyparty/web/deps/easymde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.8.4/copyparty/web/deps/marked.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.8.4/copyparty/web/deps/mini-fa.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.8.4/copyparty/web/deps/mini-fa.woff
--rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.8.4/copyparty/web/deps/prism.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.8.4/copyparty/web/deps/prism.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.8.4/copyparty/web/deps/prismd.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.8.4/copyparty/web/deps/scp.woff2
--rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.8.4/copyparty/web/deps/sha512.ac.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.8.4/copyparty/web/deps/sha512.hw.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.8.4/copyparty/web/md.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.8.4/copyparty/web/md.html
--rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.8.4/copyparty/web/md.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.8.4/copyparty/web/md2.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.8.4/copyparty/web/md2.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.8.4/copyparty/web/mde.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.8.4/copyparty/web/mde.html
--rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.8.4/copyparty/web/mde.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.4/copyparty/web/msg.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.8.4/copyparty/web/msg.html
--rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.8.4/copyparty/web/splash.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.8.4/copyparty/web/splash.html
--rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.8.4/copyparty/web/splash.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-05-07 15:13:28.000000 copyparty-1.8.4/copyparty/web/svcs.html
--rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.8.4/copyparty/web/svcs.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-06-25 23:05:18.000000 copyparty-1.8.4/copyparty/web/ui.css.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.8.4/copyparty/web/up2k.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)    13146 2023-06-25 22:59:55.000000 copyparty-1.8.4/copyparty/web/util.js.gz
--rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.8.4/copyparty/web/w.hash.js.gz
-drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-18 08:04:10.046205 copyparty-1.8.4/copyparty.egg-info/
--rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/PKG-INFO
--rw-r--r--   0 ed        (1000) ed        (1000)     2828 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/SOURCES.txt
--rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/dependency_links.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/entry_points.txt
--rw-r--r--   0 ed        (1000) ed        (1000)      139 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/requires.txt
--rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-07-18 08:04:10.000000 copyparty-1.8.4/copyparty.egg-info/top_level.txt
--rw-r--r--   0 ed        (1000) ed        (1000)     4032 2023-06-25 19:16:18.000000 copyparty-1.8.4/pyproject.toml
--rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-07-18 08:04:10.056205 copyparty-1.8.4/setup.cfg
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.217768 copyparty-1.8.6/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1059 2021-09-11 12:44:53.000000 copyparty-1.8.6/LICENSE
+-rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-21 00:58:32.217768 copyparty-1.8.6/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)    96750 2023-07-16 21:23:16.000000 copyparty-1.8.6/README.md
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.206768 copyparty-1.8.6/copyparty/
+-rw-r--r--   0 ed        (1000) ed        (1000)     1812 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    76501 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/__main__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      246 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/__version__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    69349 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/authsrv.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.207768 copyparty-1.8.6/copyparty/bos/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/bos/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1560 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/bos/bos.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      777 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/bos/path.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3915 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/broker_mp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3200 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/broker_mpw.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1759 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/broker_thr.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1489 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/broker_util.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7135 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/cert.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     7564 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/cfg.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1548 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/dxml.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3932 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/fsutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15455 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/ftpd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   128266 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/httpcli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6825 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/httpconn.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    15372 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/httpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3016 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/ico.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    17205 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/mdns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16844 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/mtag.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    11520 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/multicast.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3859 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/pwhash.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.208768 copyparty-1.8.6/copyparty/res/
+-rw-r--r--   0 ed        (1000) ed        (1000)    10570 2023-07-21 00:58:14.000000 copyparty-1.8.6/copyparty/res/COPYING.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/res/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2876 2023-04-23 21:16:05.000000 copyparty-1.8.6/copyparty/res/insecure.pem
+-rw-r--r--   0 ed        (1000) ed        (1000)    10623 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/smbd.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6379 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/ssdp.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2699 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/star.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.208768 copyparty-1.8.6/copyparty/stolen/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.209768 copyparty-1.8.6/copyparty/stolen/dnslib/
+-rw-r--r--   0 ed        (1000) ed        (1000)      159 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1182 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/bimap.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      348 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/bit.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1407 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/buffer.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    20956 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/dns.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4893 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/label.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2615 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/lex.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1810 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/dnslib/ranges.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.209768 copyparty-1.8.6/copyparty/stolen/ifaddr/
+-rw-r--r--   0 ed        (1000) ed        (1000)      463 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/ifaddr/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     2626 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/ifaddr/_posix.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     6111 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/ifaddr/_shared.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     4026 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/ifaddr/_win32.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    21469 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/qrcodegen.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     5573 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/stolen/surrogateescape.py
+-rw-r--r--   0 ed        (1000) ed        (1000)      972 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/sutil.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    24336 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/svchub.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     8166 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/szip.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    16753 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/tcpsrv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3826 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/th_cli.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    22828 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/th_srv.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    10589 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/u2idx.py
+-rw-r--r--   0 ed        (1000) ed        (1000)   124800 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/up2k.py
+-rw-r--r--   0 ed        (1000) ed        (1000)    72768 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/util.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.213768 copyparty-1.8.6/copyparty/web/
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.213768 copyparty-1.8.6/copyparty/web/a/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/web/a/__init__.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    32276 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/web/a/partyfuse.py
+-rwxr-xr-x   0 ed        (1000) ed        (1000)    36247 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/web/a/u2c.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     1449 2023-02-20 20:21:49.000000 copyparty-1.8.6/copyparty/web/a/webdav-cfg.bat
+-rw-r--r--   0 ed        (1000) ed        (1000)     7309 2023-07-16 17:45:42.000000 copyparty-1.8.6/copyparty/web/baguettebox.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10996 2023-07-13 23:14:15.000000 copyparty-1.8.6/copyparty/web/browser.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     5317 2023-06-02 21:39:24.000000 copyparty-1.8.6/copyparty/web/browser.html
+-rw-r--r--   0 ed        (1000) ed        (1000)    59820 2023-07-16 18:14:02.000000 copyparty-1.8.6/copyparty/web/browser.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1604 2022-12-10 19:54:48.000000 copyparty-1.8.6/copyparty/web/browser2.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      585 2022-07-03 13:28:49.000000 copyparty-1.8.6/copyparty/web/cf.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      688 2022-07-14 21:26:48.000000 copyparty-1.8.6/copyparty/web/dbg-audio.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.214769 copyparty-1.8.6/copyparty/web/dd/
+-rw-r--r--   0 ed        (1000) ed        (1000)      258 2021-09-11 12:44:53.000000 copyparty-1.8.6/copyparty/web/dd/2.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.6/copyparty/web/dd/3.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      248 2021-09-11 12:44:53.000000 copyparty-1.8.6/copyparty/web/dd/4.png
+-rw-r--r--   0 ed        (1000) ed        (1000)      250 2021-09-11 12:44:53.000000 copyparty-1.8.6/copyparty/web/dd/5.png
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/web/dd/__init__.py
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.217768 copyparty-1.8.6/copyparty/web/deps/
+-rw-r--r--   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:15.000000 copyparty-1.8.6/copyparty/web/deps/__init__.py
+-rw-r--r--   0 ed        (1000) ed        (1000)     3053 2023-02-20 10:55:39.000000 copyparty-1.8.6/copyparty/web/deps/easymde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    76953 2023-04-01 14:48:07.000000 copyparty-1.8.6/copyparty/web/deps/easymde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    14819 2023-04-01 14:47:51.000000 copyparty-1.8.6/copyparty/web/deps/marked.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      584 2023-04-01 14:48:09.000000 copyparty-1.8.6/copyparty/web/deps/mini-fa.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2784 2023-04-01 14:48:09.000000 copyparty-1.8.6/copyparty/web/deps/mini-fa.woff
+-rw-r--r--   0 ed        (1000) ed        (1000)     1478 2022-12-29 03:41:18.000000 copyparty-1.8.6/copyparty/web/deps/prism.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    41428 2022-12-29 03:41:18.000000 copyparty-1.8.6/copyparty/web/deps/prism.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1647 2022-12-29 03:41:18.000000 copyparty-1.8.6/copyparty/web/deps/prismd.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8612 2023-04-01 14:48:10.000000 copyparty-1.8.6/copyparty/web/deps/scp.woff2
+-rw-r--r--   0 ed        (1000) ed        (1000)     7043 2023-04-01 14:23:12.000000 copyparty-1.8.6/copyparty/web/deps/sha512.ac.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8119 2021-07-22 23:48:12.000000 copyparty-1.8.6/copyparty/web/deps/sha512.hw.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2011 2022-10-30 15:38:07.000000 copyparty-1.8.6/copyparty/web/md.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     4063 2022-12-10 20:27:29.000000 copyparty-1.8.6/copyparty/web/md.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     4121 2023-03-26 01:52:00.000000 copyparty-1.8.6/copyparty/web/md.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      681 2022-12-01 22:41:28.000000 copyparty-1.8.6/copyparty/web/md2.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     8213 2023-01-25 20:58:01.000000 copyparty-1.8.6/copyparty/web/md2.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      929 2022-04-15 15:07:16.000000 copyparty-1.8.6/copyparty/web/mde.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1640 2022-12-10 20:27:33.000000 copyparty-1.8.6/copyparty/web/mde.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     2219 2022-12-01 07:23:41.000000 copyparty-1.8.6/copyparty/web/mde.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      252 2021-09-11 12:44:53.000000 copyparty-1.8.6/copyparty/web/msg.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)      898 2022-12-10 19:57:40.000000 copyparty-1.8.6/copyparty/web/msg.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      927 2023-02-17 22:46:57.000000 copyparty-1.8.6/copyparty/web/splash.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     3741 2023-02-19 19:41:20.000000 copyparty-1.8.6/copyparty/web/splash.html
+-rw-r--r--   0 ed        (1000) ed        (1000)     1235 2023-02-17 22:28:18.000000 copyparty-1.8.6/copyparty/web/splash.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    10610 2023-07-21 00:24:03.000000 copyparty-1.8.6/copyparty/web/svcs.html
+-rw-r--r--   0 ed        (1000) ed        (1000)      520 2022-12-04 17:10:33.000000 copyparty-1.8.6/copyparty/web/svcs.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     2419 2023-06-25 23:05:18.000000 copyparty-1.8.6/copyparty/web/ui.css.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    21544 2023-05-12 23:46:23.000000 copyparty-1.8.6/copyparty/web/up2k.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)    13146 2023-06-25 22:59:55.000000 copyparty-1.8.6/copyparty/web/util.js.gz
+-rw-r--r--   0 ed        (1000) ed        (1000)     1060 2023-03-02 22:42:45.000000 copyparty-1.8.6/copyparty/web/w.hash.js.gz
+drwxr-xr-x   0 ed        (1000) ed        (1000)        0 2023-07-21 00:58:32.207768 copyparty-1.8.6/copyparty.egg-info/
+-rw-r--r--   0 ed        (1000) ed        (1000)    98723 2023-07-21 00:58:32.000000 copyparty-1.8.6/copyparty.egg-info/PKG-INFO
+-rw-r--r--   0 ed        (1000) ed        (1000)     2828 2023-07-21 00:58:32.000000 copyparty-1.8.6/copyparty.egg-info/SOURCES.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)        1 2023-07-21 00:58:32.000000 copyparty-1.8.6/copyparty.egg-info/dependency_links.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      128 2023-07-21 00:58:32.000000 copyparty-1.8.6/copyparty.egg-info/entry_points.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)      139 2023-07-21 00:58:32.000000 copyparty-1.8.6/copyparty.egg-info/requires.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)       10 2023-07-21 00:58:32.000000 copyparty-1.8.6/copyparty.egg-info/top_level.txt
+-rw-r--r--   0 ed        (1000) ed        (1000)     4032 2023-06-25 19:16:18.000000 copyparty-1.8.6/pyproject.toml
+-rw-r--r--   0 ed        (1000) ed        (1000)       38 2023-07-21 00:58:32.218768 copyparty-1.8.6/setup.cfg
```

### Comparing `copyparty-1.8.4/LICENSE` & `copyparty-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/PKG-INFO` & `copyparty-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.8.4
+Version: 1.8.6
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.8.4/README.md` & `copyparty-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/__init__.py` & `copyparty-1.8.6/copyparty/__init__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/__main__.py` & `copyparty-1.8.6/copyparty/__main__.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/authsrv.py` & `copyparty-1.8.6/copyparty/authsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/bos/bos.py` & `copyparty-1.8.6/copyparty/bos/bos.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/bos/path.py` & `copyparty-1.8.6/copyparty/bos/path.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/broker_mp.py` & `copyparty-1.8.6/copyparty/broker_mp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/broker_mpw.py` & `copyparty-1.8.6/copyparty/broker_mpw.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/broker_thr.py` & `copyparty-1.8.6/copyparty/broker_thr.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/broker_util.py` & `copyparty-1.8.6/copyparty/broker_util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/cert.py` & `copyparty-1.8.6/copyparty/cert.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/cfg.py` & `copyparty-1.8.6/copyparty/cfg.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/dxml.py` & `copyparty-1.8.6/copyparty/dxml.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/fsutil.py` & `copyparty-1.8.6/copyparty/fsutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/ftpd.py` & `copyparty-1.8.6/copyparty/ftpd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/httpcli.py` & `copyparty-1.8.6/copyparty/httpcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,15 +844,15 @@
 000034b0: 656c 662e 6361 6e5f 7570 6765 742c 0a20  elf.can_upget,. 
 000034c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
 000034d0: 6361 6e5f 6164 6d69 6e2c 0a20 2020 2020  can_admin,.     
 000034e0: 2020 2029 203d 2028 0a20 2020 2020 2020     ) = (.       
 000034f0: 2020 2020 2061 766e 2e63 616e 5f61 6363       avn.can_acc
 00003500: 6573 7328 2222 2c20 7365 6c66 2e75 6e61  ess("", self.una
 00003510: 6d65 2920 6966 2061 766e 2065 6c73 6520  me) if avn else 
-00003520: 5b46 616c 7365 5d20 2a20 360a 2020 2020  [False] * 6.    
+00003520: 5b46 616c 7365 5d20 2a20 370a 2020 2020  [False] * 7.    
 00003530: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
 00003540: 6c66 2e61 766e 203d 2061 766e 0a20 2020  lf.avn = avn.   
 00003550: 2020 2020 2073 656c 662e 766e 203d 2076       self.vn = v
 00003560: 6e0a 2020 2020 2020 2020 7365 6c66 2e72  n.        self.r
 00003570: 656d 203d 2072 656d 0a0a 2020 2020 2020  em = rem..      
 00003580: 2020 7365 6c66 2e73 2e73 6574 7469 6d65    self.s.settime
 00003590: 6f75 7428 7365 6c66 2e61 7267 732e 735f  out(self.args.s_
@@ -6077,1932 +6077,1941 @@
 00017bc0: 6c66 2e61 7267 732e 7263 6c6f 6e65 5f6d  lf.args.rclone_m
 00017bd0: 646e 7320 6f72 206e 6f74 2073 656c 662e  dns or not self.
 00017be0: 6172 6773 2e7a 6d0a 2020 2020 2020 2020  args.zm.        
 00017bf0: 2020 2020 656c 7365 2073 656c 662e 636f      else self.co
 00017c00: 6e6e 2e68 7372 762e 6e6d 2e6d 6170 2873  nn.hsrv.nm.map(s
 00017c10: 656c 662e 6970 2920 6f72 2068 6f73 740a  elf.ip) or host.
 00017c20: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00017c30: 2020 7670 203d 2028 7365 6c66 2e75 7061    vp = (self.upa
-00017c40: 7261 6d5b 2268 6322 5d20 6f72 2022 2229  ram["hc"] or "")
-00017c50: 2e6c 7374 7269 7028 222f 2229 0a20 2020  .lstrip("/").   
-00017c60: 2020 2020 2068 746d 6c20 3d20 7365 6c66       html = self
-00017c70: 2e6a 3273 280a 2020 2020 2020 2020 2020  .j2s(.          
-00017c80: 2020 2273 7663 7322 2c0a 2020 2020 2020    "svcs",.      
-00017c90: 2020 2020 2020 6172 6773 3d73 656c 662e        args=self.
-00017ca0: 6172 6773 2c0a 2020 2020 2020 2020 2020  args,.          
-00017cb0: 2020 6163 6373 3d62 6f6f 6c28 7365 6c66    accs=bool(self
-00017cc0: 2e61 7372 762e 6163 6374 292c 0a20 2020  .asrv.acct),.   
-00017cd0: 2020 2020 2020 2020 2073 3d22 7322 2069           s="s" i
-00017ce0: 6620 7365 6c66 2e69 735f 6874 7470 7320  f self.is_https 
-00017cf0: 656c 7365 2022 222c 0a20 2020 2020 2020  else "",.       
-00017d00: 2020 2020 2072 6970 3d72 6970 2c0a 2020       rip=rip,.  
-00017d10: 2020 2020 2020 2020 2020 6570 3d65 702c            ep=ep,
-00017d20: 0a20 2020 2020 2020 2020 2020 2076 703d  .            vp=
-00017d30: 7670 2c0a 2020 2020 2020 2020 2020 2020  vp,.            
-00017d40: 7276 703d 766a 6f69 6e28 7365 6c66 2e61  rvp=vjoin(self.a
-00017d50: 7267 732e 522c 2076 7029 2c0a 2020 2020  rgs.R, vp),.    
-00017d60: 2020 2020 2020 2020 686f 7374 3d68 6f73          host=hos
-00017d70: 742c 0a20 2020 2020 2020 2020 2020 2068  t,.            h
-00017d80: 706f 7274 3d68 706f 7274 2c0a 2020 2020  port=hport,.    
-00017d90: 2020 2020 2020 2020 616e 616d 653d 616e          aname=an
-00017da0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-00017db0: 2070 773d 7365 6c66 2e70 7720 6f72 2022   pw=self.pw or "
-00017dc0: 7077 222c 0a20 2020 2020 2020 2029 0a20  pw",.        ). 
-00017dd0: 2020 2020 2020 2073 656c 662e 7265 706c         self.repl
-00017de0: 7928 6874 6d6c 2e65 6e63 6f64 6528 2275  y(html.encode("u
-00017df0: 7466 2d38 2229 290a 2020 2020 2020 2020  tf-8")).        
-00017e00: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
-00017e10: 2064 6566 2074 785f 6d6f 756e 7473 2873   def tx_mounts(s
-00017e20: 656c 6629 2020 3a0a 2020 2020 2020 2020  elf)  :.        
-00017e30: 7375 6620 3d20 7365 6c66 2e75 726c 7128  suf = self.urlq(
-00017e40: 7b7d 2c20 5b22 6822 5d29 0a20 2020 2020  {}, ["h"]).     
-00017e50: 2020 2072 766f 6c2c 2077 766f 6c2c 2061     rvol, wvol, a
-00017e60: 766f 6c20 3d20 5b0a 2020 2020 2020 2020  vol = [.        
-00017e70: 2020 2020 5b28 222f 2220 2b20 7829 2e72      [("/" + x).r
-00017e80: 7374 7269 7028 222f 2229 202b 2022 2f22  strip("/") + "/"
-00017e90: 2066 6f72 2078 2069 6e20 795d 0a20 2020   for x in y].   
-00017ea0: 2020 2020 2020 2020 2066 6f72 2079 2069           for y i
-00017eb0: 6e20 5b73 656c 662e 7276 6f6c 2c20 7365  n [self.rvol, se
-00017ec0: 6c66 2e77 766f 6c2c 2073 656c 662e 6176  lf.wvol, self.av
-00017ed0: 6f6c 5d0a 2020 2020 2020 2020 5d0a 0a20  ol].        ].. 
-00017ee0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-00017ef0: 766f 6c20 616e 6420 6e6f 7420 7365 6c66  vol and not self
-00017f00: 2e61 7267 732e 6e6f 5f72 6573 6361 6e3a  .args.no_rescan:
-00017f10: 0a20 2020 2020 2020 2020 2020 2078 203d  .            x =
-00017f20: 2073 656c 662e 636f 6e6e 2e68 7372 762e   self.conn.hsrv.
-00017f30: 6272 6f6b 6572 2e61 736b 2822 7570 326b  broker.ask("up2k
-00017f40: 2e67 6574 5f73 7461 7465 2229 0a20 2020  .get_state").   
-00017f50: 2020 2020 2020 2020 2076 7320 3d20 6a73           vs = js
-00017f60: 6f6e 2e6c 6f61 6473 2878 2e67 6574 2829  on.loads(x.get()
-00017f70: 290a 2020 2020 2020 2020 2020 2020 7673  ).            vs
-00017f80: 7461 7465 203d 207b 2822 2f22 202b 206b  tate = {("/" + k
-00017f90: 292e 7273 7472 6970 2822 2f22 2920 2b20  ).rstrip("/") + 
-00017fa0: 222f 223a 2076 2066 6f72 206b 2c20 7620  "/": v for k, v 
-00017fb0: 696e 2076 735b 2276 6f6c 7374 6174 6522  in vs["volstate"
-00017fc0: 5d2e 6974 656d 7328 297d 0a20 2020 2020  ].items()}.     
-00017fd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00017fe0: 2020 2020 2076 7374 6174 6520 3d20 7b7d       vstate = {}
-00017ff0: 0a20 2020 2020 2020 2020 2020 2076 7320  .            vs 
-00018000: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
-00018010: 2020 2020 2273 6361 6e6e 696e 6722 3a20      "scanning": 
-00018020: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00018030: 2020 2020 2020 2268 6173 6871 223a 204e        "hashq": N
-00018040: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00018050: 2020 2020 2022 7461 6771 223a 204e 6f6e       "tagq": Non
-00018060: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00018070: 2020 2022 6d74 7071 223a 204e 6f6e 652c     "mtpq": None,
-00018080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018090: 2022 6462 7774 223a 204e 6f6e 652c 0a20   "dbwt": None,. 
-000180a0: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
-000180b0: 2020 2020 2020 666d 7420 3d20 7365 6c66        fmt = self
-000180c0: 2e75 7061 7261 6d2e 6765 7428 226c 7322  .uparam.get("ls"
-000180d0: 2c20 2222 290a 2020 2020 2020 2020 6966  , "").        if
-000180e0: 206e 6f74 2066 6d74 2061 6e64 2028 7365   not fmt and (se
-000180f0: 6c66 2e75 612e 7374 6172 7473 7769 7468  lf.ua.startswith
-00018100: 2822 6375 726c 2f22 2920 6f72 2073 656c  ("curl/") or sel
-00018110: 662e 7561 2e73 7461 7274 7377 6974 6828  f.ua.startswith(
-00018120: 2266 6574 6368 2229 293a 0a20 2020 2020  "fetch")):.     
-00018130: 2020 2020 2020 2066 6d74 203d 2022 7622         fmt = "v"
-00018140: 0a0a 2020 2020 2020 2020 6966 2066 6d74  ..        if fmt
-00018150: 2069 6e20 5b22 7622 2c20 2274 222c 2022   in ["v", "t", "
-00018160: 7478 7422 5d3a 0a20 2020 2020 2020 2020  txt"]:.         
-00018170: 2020 2069 6620 7365 6c66 2e75 6e61 6d65     if self.uname
-00018180: 203d 3d20 222a 223a 0a20 2020 2020 2020   == "*":.       
-00018190: 2020 2020 2020 2020 2074 7874 203d 2022           txt = "
-000181a0: 686f 7764 7920 7374 7261 6e67 6572 2028  howdy stranger (
-000181b0: 796f 7527 7265 206e 6f74 206c 6f67 6765  you're not logge
-000181c0: 6420 696e 2922 0a20 2020 2020 2020 2020  d in)".         
-000181d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000181e0: 2020 2020 2020 2020 2074 7874 203d 2022           txt = "
-000181f0: 7765 6c63 6f6d 6520 6261 636b 207b 7d22  welcome back {}"
-00018200: 2e66 6f72 6d61 7428 7365 6c66 2e75 6e61  .format(self.una
-00018210: 6d65 290a 0a20 2020 2020 2020 2020 2020  me)..           
-00018220: 2069 6620 7673 7461 7465 3a0a 2020 2020   if vstate:.    
-00018230: 2020 2020 2020 2020 2020 2020 7478 7420              txt 
-00018240: 2b3d 2022 5c6e 7374 6174 7573 3a22 0a20  += "\nstatus:". 
-00018250: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00018260: 6f72 206b 2069 6e20 5b22 7363 616e 6e69  or k in ["scanni
-00018270: 6e67 222c 2022 6861 7368 7122 2c20 2274  ng", "hashq", "t
-00018280: 6167 7122 2c20 226d 7470 7122 2c20 2264  agq", "mtpq", "d
-00018290: 6277 7422 5d3a 0a20 2020 2020 2020 2020  bwt"]:.         
-000182a0: 2020 2020 2020 2020 2020 2074 7874 202b             txt +
-000182b0: 3d20 2220 7b7d 287b 7d29 222e 666f 726d  = " {}({})".form
-000182c0: 6174 286b 2c20 7673 5b6b 5d29 0a0a 2020  at(k, vs[k])..  
-000182d0: 2020 2020 2020 2020 2020 6966 2072 766f            if rvo
-000182e0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-000182f0: 2020 2074 7874 202b 3d20 225c 6e79 6f75     txt += "\nyou
-00018300: 2063 616e 2062 726f 7773 653a 220a 2020   can browse:".  
-00018310: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00018320: 7220 7620 696e 2072 766f 6c3a 0a20 2020  r v in rvol:.   
+00017c30: 2020 2320 7361 6665 7220 7468 616e 2068    # safer than h
+00017c40: 746d 6c5f 6573 6361 7065 2f71 756f 7465  tml_escape/quote
+00017c50: 7020 7369 6e63 6520 7468 6973 2061 766f  p since this avo
+00017c60: 6964 7320 626f 7468 2058 5353 2061 6e64  ids both XSS and
+00017c70: 2073 6865 6c6c 2d73 7475 6666 0a20 2020   shell-stuff.   
+00017c80: 2020 2020 2070 7720 3d20 7265 2e73 7562       pw = re.sub
+00017c90: 2872 225b 3c3e 2624 3f60 5d22 2c20 225f  (r"[<>&$?`]", "_
+00017ca0: 222c 2073 656c 662e 7077 206f 7220 2270  ", self.pw or "p
+00017cb0: 7722 290a 2020 2020 2020 2020 7670 203d  w").        vp =
+00017cc0: 2072 652e 7375 6228 7222 5b3c 3e26 243f   re.sub(r"[<>&$?
+00017cd0: 605d 222c 2022 5f22 2c20 7365 6c66 2e75  `]", "_", self.u
+00017ce0: 7061 7261 6d5b 2268 6322 5d20 6f72 2022  param["hc"] or "
+00017cf0: 2229 2e6c 7374 7269 7028 222f 2229 0a20  ").lstrip("/"). 
+00017d00: 2020 2020 2020 2068 746d 6c20 3d20 7365         html = se
+00017d10: 6c66 2e6a 3273 280a 2020 2020 2020 2020  lf.j2s(.        
+00017d20: 2020 2020 2273 7663 7322 2c0a 2020 2020      "svcs",.    
+00017d30: 2020 2020 2020 2020 6172 6773 3d73 656c          args=sel
+00017d40: 662e 6172 6773 2c0a 2020 2020 2020 2020  f.args,.        
+00017d50: 2020 2020 6163 6373 3d62 6f6f 6c28 7365      accs=bool(se
+00017d60: 6c66 2e61 7372 762e 6163 6374 292c 0a20  lf.asrv.acct),. 
+00017d70: 2020 2020 2020 2020 2020 2073 3d22 7322             s="s"
+00017d80: 2069 6620 7365 6c66 2e69 735f 6874 7470   if self.is_http
+00017d90: 7320 656c 7365 2022 222c 0a20 2020 2020  s else "",.     
+00017da0: 2020 2020 2020 2072 6970 3d72 6970 2c0a         rip=rip,.
+00017db0: 2020 2020 2020 2020 2020 2020 6570 3d65              ep=e
+00017dc0: 702c 0a20 2020 2020 2020 2020 2020 2076  p,.            v
+00017dd0: 703d 7670 2c0a 2020 2020 2020 2020 2020  p=vp,.          
+00017de0: 2020 7276 703d 766a 6f69 6e28 7365 6c66    rvp=vjoin(self
+00017df0: 2e61 7267 732e 522c 2076 7029 2c0a 2020  .args.R, vp),.  
+00017e00: 2020 2020 2020 2020 2020 686f 7374 3d68            host=h
+00017e10: 6f73 742c 0a20 2020 2020 2020 2020 2020  ost,.           
+00017e20: 2068 706f 7274 3d68 706f 7274 2c0a 2020   hport=hport,.  
+00017e30: 2020 2020 2020 2020 2020 616e 616d 653d            aname=
+00017e40: 616e 616d 652c 0a20 2020 2020 2020 2020  aname,.         
+00017e50: 2020 2070 773d 7077 2c0a 2020 2020 2020     pw=pw,.      
+00017e60: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
+00017e70: 2e72 6570 6c79 2868 746d 6c2e 656e 636f  .reply(html.enco
+00017e80: 6465 2822 7574 662d 3822 2929 0a20 2020  de("utf-8")).   
+00017e90: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00017ea0: 0a0a 2020 2020 6465 6620 7478 5f6d 6f75  ..    def tx_mou
+00017eb0: 6e74 7328 7365 6c66 2920 203a 0a20 2020  nts(self)  :.   
+00017ec0: 2020 2020 2073 7566 203d 2073 656c 662e       suf = self.
+00017ed0: 7572 6c71 287b 7d2c 205b 2268 225d 290a  urlq({}, ["h"]).
+00017ee0: 2020 2020 2020 2020 7276 6f6c 2c20 7776          rvol, wv
+00017ef0: 6f6c 2c20 6176 6f6c 203d 205b 0a20 2020  ol, avol = [.   
+00017f00: 2020 2020 2020 2020 205b 2822 2f22 202b           [("/" +
+00017f10: 2078 292e 7273 7472 6970 2822 2f22 2920   x).rstrip("/") 
+00017f20: 2b20 222f 2220 666f 7220 7820 696e 2079  + "/" for x in y
+00017f30: 5d0a 2020 2020 2020 2020 2020 2020 666f  ].            fo
+00017f40: 7220 7920 696e 205b 7365 6c66 2e72 766f  r y in [self.rvo
+00017f50: 6c2c 2073 656c 662e 7776 6f6c 2c20 7365  l, self.wvol, se
+00017f60: 6c66 2e61 766f 6c5d 0a20 2020 2020 2020  lf.avol].       
+00017f70: 205d 0a0a 2020 2020 2020 2020 6966 2073   ]..        if s
+00017f80: 656c 662e 6176 6f6c 2061 6e64 206e 6f74  elf.avol and not
+00017f90: 2073 656c 662e 6172 6773 2e6e 6f5f 7265   self.args.no_re
+00017fa0: 7363 616e 3a0a 2020 2020 2020 2020 2020  scan:.          
+00017fb0: 2020 7820 3d20 7365 6c66 2e63 6f6e 6e2e    x = self.conn.
+00017fc0: 6873 7276 2e62 726f 6b65 722e 6173 6b28  hsrv.broker.ask(
+00017fd0: 2275 7032 6b2e 6765 745f 7374 6174 6522  "up2k.get_state"
+00017fe0: 290a 2020 2020 2020 2020 2020 2020 7673  ).            vs
+00017ff0: 203d 206a 736f 6e2e 6c6f 6164 7328 782e   = json.loads(x.
+00018000: 6765 7428 2929 0a20 2020 2020 2020 2020  get()).         
+00018010: 2020 2076 7374 6174 6520 3d20 7b28 222f     vstate = {("/
+00018020: 2220 2b20 6b29 2e72 7374 7269 7028 222f  " + k).rstrip("/
+00018030: 2229 202b 2022 2f22 3a20 7620 666f 7220  ") + "/": v for 
+00018040: 6b2c 2076 2069 6e20 7673 5b22 766f 6c73  k, v in vs["vols
+00018050: 7461 7465 225d 2e69 7465 6d73 2829 7d0a  tate"].items()}.
+00018060: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018070: 2020 2020 2020 2020 2020 7673 7461 7465            vstate
+00018080: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00018090: 2020 7673 203d 207b 0a20 2020 2020 2020    vs = {.       
+000180a0: 2020 2020 2020 2020 2022 7363 616e 6e69           "scanni
+000180b0: 6e67 223a 204e 6f6e 652c 0a20 2020 2020  ng": None,.     
+000180c0: 2020 2020 2020 2020 2020 2022 6861 7368             "hash
+000180d0: 7122 3a20 4e6f 6e65 2c0a 2020 2020 2020  q": None,.      
+000180e0: 2020 2020 2020 2020 2020 2274 6167 7122            "tagq"
+000180f0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+00018100: 2020 2020 2020 2020 226d 7470 7122 3a20          "mtpq": 
+00018110: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+00018120: 2020 2020 2020 2264 6277 7422 3a20 4e6f        "dbwt": No
+00018130: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00018140: 7d0a 0a20 2020 2020 2020 2066 6d74 203d  }..        fmt =
+00018150: 2073 656c 662e 7570 6172 616d 2e67 6574   self.uparam.get
+00018160: 2822 6c73 222c 2022 2229 0a20 2020 2020  ("ls", "").     
+00018170: 2020 2069 6620 6e6f 7420 666d 7420 616e     if not fmt an
+00018180: 6420 2873 656c 662e 7561 2e73 7461 7274  d (self.ua.start
+00018190: 7377 6974 6828 2263 7572 6c2f 2229 206f  swith("curl/") o
+000181a0: 7220 7365 6c66 2e75 612e 7374 6172 7473  r self.ua.starts
+000181b0: 7769 7468 2822 6665 7463 6822 2929 3a0a  with("fetch")):.
+000181c0: 2020 2020 2020 2020 2020 2020 666d 7420              fmt 
+000181d0: 3d20 2276 220a 0a20 2020 2020 2020 2069  = "v"..        i
+000181e0: 6620 666d 7420 696e 205b 2276 222c 2022  f fmt in ["v", "
+000181f0: 7422 2c20 2274 7874 225d 3a0a 2020 2020  t", "txt"]:.    
+00018200: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00018210: 756e 616d 6520 3d3d 2022 2a22 3a0a 2020  uname == "*":.  
+00018220: 2020 2020 2020 2020 2020 2020 2020 7478                tx
+00018230: 7420 3d20 2268 6f77 6479 2073 7472 616e  t = "howdy stran
+00018240: 6765 7220 2879 6f75 2772 6520 6e6f 7420  ger (you're not 
+00018250: 6c6f 6767 6564 2069 6e29 220a 2020 2020  logged in)".    
+00018260: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00018270: 2020 2020 2020 2020 2020 2020 2020 7478                tx
+00018280: 7420 3d20 2277 656c 636f 6d65 2062 6163  t = "welcome bac
+00018290: 6b20 7b7d 222e 666f 726d 6174 2873 656c  k {}".format(sel
+000182a0: 662e 756e 616d 6529 0a0a 2020 2020 2020  f.uname)..      
+000182b0: 2020 2020 2020 6966 2076 7374 6174 653a        if vstate:
+000182c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000182d0: 2074 7874 202b 3d20 225c 6e73 7461 7475   txt += "\nstatu
+000182e0: 733a 220a 2020 2020 2020 2020 2020 2020  s:".            
+000182f0: 2020 2020 666f 7220 6b20 696e 205b 2273      for k in ["s
+00018300: 6361 6e6e 696e 6722 2c20 2268 6173 6871  canning", "hashq
+00018310: 222c 2022 7461 6771 222c 2022 6d74 7071  ", "tagq", "mtpq
+00018320: 222c 2022 6462 7774 225d 3a0a 2020 2020  ", "dbwt"]:.    
 00018330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018340: 2074 7874 202b 3d20 225c 6e20 2022 202b   txt += "\n  " +
-00018350: 2076 0a0a 2020 2020 2020 2020 2020 2020   v..            
-00018360: 6966 2077 766f 6c3a 0a20 2020 2020 2020  if wvol:.       
-00018370: 2020 2020 2020 2020 2074 7874 202b 3d20           txt += 
-00018380: 225c 6e79 6f75 2063 616e 2075 706c 6f61  "\nyou can uploa
-00018390: 6420 746f 3a22 0a20 2020 2020 2020 2020  d to:".         
-000183a0: 2020 2020 2020 2066 6f72 2076 2069 6e20         for v in 
-000183b0: 7776 6f6c 3a0a 2020 2020 2020 2020 2020  wvol:.          
-000183c0: 2020 2020 2020 2020 2020 7478 7420 2b3d            txt +=
-000183d0: 2022 5c6e 2020 2220 2b20 760a 0a20 2020   "\n  " + v..   
-000183e0: 2020 2020 2020 2020 207a 6220 3d20 7478           zb = tx
-000183f0: 742e 656e 636f 6465 2822 7574 662d 3822  t.encode("utf-8"
-00018400: 2c20 2272 6570 6c61 6365 2229 202b 2062  , "replace") + b
-00018410: 225c 6e22 0a20 2020 2020 2020 2020 2020  "\n".           
-00018420: 2073 656c 662e 7265 706c 7928 7a62 2c20   self.reply(zb, 
-00018430: 6d69 6d65 3d22 7465 7874 2f70 6c61 696e  mime="text/plain
-00018440: 3b20 6368 6172 7365 743d 7574 662d 3822  ; charset=utf-8"
-00018450: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00018460: 7475 726e 2054 7275 650a 0a20 2020 2020  turn True..     
-00018470: 2020 2068 746d 6c20 3d20 7365 6c66 2e6a     html = self.j
-00018480: 3273 280a 2020 2020 2020 2020 2020 2020  2s(.            
-00018490: 2273 706c 6173 6822 2c0a 2020 2020 2020  "splash",.      
-000184a0: 2020 2020 2020 7468 6973 3d73 656c 662c        this=self,
-000184b0: 0a20 2020 2020 2020 2020 2020 2071 7670  .            qvp
-000184c0: 6174 683d 7175 6f74 6570 2873 656c 662e  ath=quotep(self.
-000184d0: 7670 6174 6829 2c0a 2020 2020 2020 2020  vpath),.        
-000184e0: 2020 2020 7276 6f6c 3d72 766f 6c2c 0a20      rvol=rvol,. 
-000184f0: 2020 2020 2020 2020 2020 2077 766f 6c3d             wvol=
-00018500: 7776 6f6c 2c0a 2020 2020 2020 2020 2020  wvol,.          
-00018510: 2020 6176 6f6c 3d61 766f 6c2c 0a20 2020    avol=avol,.   
-00018520: 2020 2020 2020 2020 2076 7374 6174 653d           vstate=
-00018530: 7673 7461 7465 2c0a 2020 2020 2020 2020  vstate,.        
-00018540: 2020 2020 7363 616e 6e69 6e67 3d76 735b      scanning=vs[
-00018550: 2273 6361 6e6e 696e 6722 5d2c 0a20 2020  "scanning"],.   
-00018560: 2020 2020 2020 2020 2068 6173 6871 3d76           hashq=v
-00018570: 735b 2268 6173 6871 225d 2c0a 2020 2020  s["hashq"],.    
-00018580: 2020 2020 2020 2020 7461 6771 3d76 735b          tagq=vs[
-00018590: 2274 6167 7122 5d2c 0a20 2020 2020 2020  "tagq"],.       
-000185a0: 2020 2020 206d 7470 713d 7673 5b22 6d74       mtpq=vs["mt
-000185b0: 7071 225d 2c0a 2020 2020 2020 2020 2020  pq"],.          
-000185c0: 2020 6462 7774 3d76 735b 2264 6277 7422    dbwt=vs["dbwt"
-000185d0: 5d2c 0a20 2020 2020 2020 2020 2020 2075  ],.            u
-000185e0: 726c 5f73 7566 3d73 7566 2c0a 2020 2020  rl_suf=suf,.    
-000185f0: 2020 2020 2020 2020 6b33 3034 3d73 656c          k304=sel
-00018600: 662e 6b33 3034 2829 2c0a 2020 2020 2020  f.k304(),.      
-00018610: 2020 2020 2020 7665 723d 535f 5645 5253        ver=S_VERS
-00018620: 494f 4e20 6966 2073 656c 662e 6172 6773  ION if self.args
-00018630: 2e76 6572 2065 6c73 6520 2222 2c0a 2020  .ver else "",.  
-00018640: 2020 2020 2020 2020 2020 6168 7474 7073            ahttps
-00018650: 3d22 2220 6966 2073 656c 662e 6973 5f68  ="" if self.is_h
-00018660: 7474 7073 2065 6c73 6520 2268 7474 7073  ttps else "https
-00018670: 3a2f 2f22 202b 2073 656c 662e 686f 7374  ://" + self.host
-00018680: 202b 2073 656c 662e 7265 712c 0a20 2020   + self.req,.   
-00018690: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-000186a0: 656c 662e 7265 706c 7928 6874 6d6c 2e65  elf.reply(html.e
-000186b0: 6e63 6f64 6528 2275 7466 2d38 2229 290a  ncode("utf-8")).
-000186c0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-000186d0: 7275 650a 0a20 2020 2064 6566 2073 6574  rue..    def set
-000186e0: 5f6b 3330 3428 7365 6c66 2920 203a 0a20  _k304(self)  :. 
-000186f0: 2020 2020 2020 2063 6b20 3d20 6765 6e63         ck = genc
-00018700: 6f6f 6b69 6528 226b 3330 3422 2c20 7365  ookie("k304", se
-00018710: 6c66 2e75 7061 7261 6d5b 226b 3330 3422  lf.uparam["k304"
-00018720: 5d2c 2073 656c 662e 6172 6773 2e52 2c20  ], self.args.R, 
-00018730: 4661 6c73 652c 2038 3634 3030 202a 2032  False, 86400 * 2
-00018740: 3939 290a 2020 2020 2020 2020 7365 6c66  99).        self
-00018750: 2e6f 7574 5f68 6561 6465 726c 6973 742e  .out_headerlist.
-00018760: 6170 7065 6e64 2828 2253 6574 2d43 6f6f  append(("Set-Coo
-00018770: 6b69 6522 2c20 636b 2929 0a20 2020 2020  kie", ck)).     
-00018780: 2020 2073 656c 662e 7265 6469 7265 6374     self.redirect
-00018790: 2822 222c 2022 3f68 2363 6322 290a 2020  ("", "?h#cc").  
-000187a0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-000187b0: 650a 0a20 2020 2064 6566 2073 6574 636b  e..    def setck
-000187c0: 2873 656c 6629 2020 3a0a 2020 2020 2020  (self)  :.      
-000187d0: 2020 6b2c 2076 203d 2073 656c 662e 7570    k, v = self.up
-000187e0: 6172 616d 5b22 7365 7463 6b22 5d2e 7370  aram["setck"].sp
-000187f0: 6c69 7428 223d 222c 2031 290a 2020 2020  lit("=", 1).    
-00018800: 2020 2020 7420 3d20 4e6f 6e65 2069 6620      t = None if 
-00018810: 7620 3d3d 2022 2220 656c 7365 2038 3634  v == "" else 864
-00018820: 3030 202a 2032 3939 0a20 2020 2020 2020  00 * 299.       
-00018830: 2063 6b20 3d20 6765 6e63 6f6f 6b69 6528   ck = gencookie(
-00018840: 6b2c 2076 2c20 7365 6c66 2e61 7267 732e  k, v, self.args.
-00018850: 522c 2046 616c 7365 2c20 7429 0a20 2020  R, False, t).   
-00018860: 2020 2020 2073 656c 662e 6f75 745f 6865       self.out_he
-00018870: 6164 6572 6c69 7374 2e61 7070 656e 6428  aderlist.append(
-00018880: 2822 5365 742d 436f 6f6b 6965 222c 2063  ("Set-Cookie", c
-00018890: 6b29 290a 2020 2020 2020 2020 7365 6c66  k)).        self
-000188a0: 2e72 6570 6c79 2862 226f 375c 6e22 290a  .reply(b"o7\n").
-000188b0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-000188c0: 7275 650a 0a20 2020 2064 6566 2073 6574  rue..    def set
-000188d0: 5f63 6667 5f72 6573 6574 2873 656c 6629  _cfg_reset(self)
-000188e0: 2020 3a0a 2020 2020 2020 2020 666f 7220    :.        for 
-000188f0: 6b20 696e 2028 226b 3330 3422 2c20 226a  k in ("k304", "j
-00018900: 7322 2c20 2269 6478 6822 2c20 2263 7070  s", "idxh", "cpp
-00018910: 7764 222c 2022 6370 7077 7322 293a 0a20  wd", "cppws"):. 
-00018920: 2020 2020 2020 2020 2020 2063 6f6f 6b69             cooki
-00018930: 6520 3d20 6765 6e63 6f6f 6b69 6528 6b2c  e = gencookie(k,
-00018940: 2022 7822 2c20 7365 6c66 2e61 7267 732e   "x", self.args.
-00018950: 522c 2046 616c 7365 2c20 4e6f 6e65 290a  R, False, None).
-00018960: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018970: 2e6f 7574 5f68 6561 6465 726c 6973 742e  .out_headerlist.
-00018980: 6170 7065 6e64 2828 2253 6574 2d43 6f6f  append(("Set-Coo
-00018990: 6b69 6522 2c20 636f 6f6b 6965 2929 0a0a  kie", cookie))..
-000189a0: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
-000189b0: 6972 6563 7428 2222 2c20 223f 6823 6363  irect("", "?h#cc
-000189c0: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-000189d0: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
-000189e0: 7478 5f34 3034 2873 656c 662c 2069 735f  tx_404(self, is_
-000189f0: 3430 3320 203d 2046 616c 7365 2920 203a  403  = False)  :
-00018a00: 0a20 2020 2020 2020 2072 6320 3d20 3430  .        rc = 40
-00018a10: 340a 2020 2020 2020 2020 6966 2073 656c  4.        if sel
-00018a20: 662e 6172 6773 2e76 6167 7565 5f34 3033  f.args.vague_403
-00018a30: 3a0a 2020 2020 2020 2020 2020 2020 7420  :.            t 
-00018a40: 3d20 273c 6831 2069 643d 226e 223e 3430  = '<h1 id="n">40
-00018a50: 3420 6e6f 7420 666f 756e 6420 266e 6273  4 not found &nbs
-00018a60: 703b e294 9028 20c2 b420 2d60 29e2 948c  p;...( .. -`)...
-00018a70: 3c2f 6831 3e3c 7020 6964 3d22 6f22 3e6f  </h1><p id="o">o
-00018a80: 7220 6d61 7962 6520 796f 7520 646f 6e5c  r maybe you don\
-00018a90: 2774 2068 6176 6520 6163 6365 7373 202d  't have access -
-00018aa0: 2d20 7472 7920 6c6f 6767 696e 6720 696e  - try logging in
-00018ab0: 206f 7220 3c61 2068 7265 663d 227b 7d2f   or <a href="{}/
-00018ac0: 3f68 223e 676f 2068 6f6d 653c 2f61 3e3c  ?h">go home</a><
-00018ad0: 2f70 3e27 0a20 2020 2020 2020 2065 6c69  /p>'.        eli
-00018ae0: 6620 6973 5f34 3033 3a0a 2020 2020 2020  f is_403:.      
-00018af0: 2020 2020 2020 7420 3d20 273c 6831 2069        t = '<h1 i
-00018b00: 643d 2270 223e 3430 3320 666f 7262 6964  d="p">403 forbid
-00018b10: 6465 6e61 2026 6e62 7370 3b7e e294 bbe2  dena &nbsp;~....
-00018b20: 9481 e294 bb3c 2f68 313e 3c70 2069 643d  .....</h1><p id=
-00018b30: 2271 223e 796f 755c 276c 6c20 6861 7665  "q">you\'ll have
-00018b40: 2074 6f20 6c6f 6720 696e 206f 7220 3c61   to log in or <a
-00018b50: 2068 7265 663d 227b 7d2f 3f68 223e 676f   href="{}/?h">go
-00018b60: 2068 6f6d 653c 2f61 3e3c 2f70 3e27 0a20   home</a></p>'. 
-00018b70: 2020 2020 2020 2020 2020 2072 6320 3d20             rc = 
-00018b80: 3430 330a 2020 2020 2020 2020 656c 7365  403.        else
-00018b90: 3a0a 2020 2020 2020 2020 2020 2020 7420  :.            t 
-00018ba0: 3d20 273c 6831 2069 643d 226e 223e 3430  = '<h1 id="n">40
-00018bb0: 3420 6e6f 7420 666f 756e 6420 266e 6273  4 not found &nbs
-00018bc0: 703b e294 9028 20c2 b420 2d60 29e2 948c  p;...( .. -`)...
-00018bd0: 3c2f 6831 3e3c 703e 3c61 2069 643d 2272  </h1><p><a id="r
-00018be0: 2220 6872 6566 3d22 7b7d 2f3f 6822 3e67  " href="{}/?h">g
-00018bf0: 6f20 686f 6d65 3c2f 613e 3c2f 703e 270a  o home</a></p>'.
-00018c00: 0a20 2020 2020 2020 2074 203d 2074 2e66  .        t = t.f
-00018c10: 6f72 6d61 7428 7365 6c66 2e61 7267 732e  ormat(self.args.
-00018c20: 5352 290a 2020 2020 2020 2020 6874 6d6c  SR).        html
-00018c30: 203d 2073 656c 662e 6a32 7328 2273 706c   = self.j2s("spl
-00018c40: 6173 6822 2c20 7468 6973 3d73 656c 662c  ash", this=self,
-00018c50: 2071 7670 6174 683d 7175 6f74 6570 2873   qvpath=quotep(s
-00018c60: 656c 662e 7670 6174 6829 2c20 6d73 673d  elf.vpath), msg=
-00018c70: 7429 0a20 2020 2020 2020 2073 656c 662e  t).        self.
-00018c80: 7265 706c 7928 6874 6d6c 2e65 6e63 6f64  reply(html.encod
-00018c90: 6528 2275 7466 2d38 2229 2c20 7374 6174  e("utf-8"), stat
-00018ca0: 7573 3d72 6329 0a20 2020 2020 2020 2072  us=rc).        r
-00018cb0: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
-00018cc0: 6465 6620 6f6e 3430 7828 7365 6c66 2c20  def on40x(self, 
-00018cd0: 6d6f 6473 202c 2076 6e20 2c20 7265 6d20  mods , vn , rem 
-00018ce0: 2920 203a 0a20 2020 2020 2020 2066 6f72  )  :.        for
-00018cf0: 206d 7061 7468 2069 6e20 6d6f 6473 3a0a   mpath in mods:.
-00018d00: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00018d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d20: 206d 6f64 203d 206c 6f61 6470 7928 6d70   mod = loadpy(mp
-00018d30: 6174 682c 2073 656c 662e 6172 6773 2e68  ath, self.args.h
-00018d40: 6f74 5f68 616e 646c 6572 7329 0a20 2020  ot_handlers).   
-00018d50: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00018d60: 4578 6365 7074 696f 6e20 6173 2065 783a  Exception as ex:
-00018d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018d80: 2073 656c 662e 6c6f 6728 2269 6d70 6f72   self.log("impor
-00018d90: 7420 6661 696c 6564 3a20 7b21 727d 222e  t failed: {!r}".
-00018da0: 666f 726d 6174 2865 7829 290a 2020 2020  format(ex)).    
-00018db0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00018dc0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-00018dd0: 2020 7265 7420 3d20 6d6f 642e 6d61 696e    ret = mod.main
-00018de0: 2873 656c 662c 2076 6e2c 2072 656d 290a  (self, vn, rem).
-00018df0: 2020 2020 2020 2020 2020 2020 6966 2072              if r
-00018e00: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
-00018e10: 2020 2020 7265 7475 726e 2072 6574 2e6c      return ret.l
-00018e20: 6f77 6572 2829 0a0a 2020 2020 2020 2020  ower()..        
-00018e30: 7265 7475 726e 2022 2220 2023 2075 6e68  return ""  # unh
-00018e40: 616e 646c 6564 202f 2066 616c 6c74 6872  andled / fallthr
-00018e50: 6f75 6768 0a0a 2020 2020 6465 6620 7363  ough..    def sc
-00018e60: 616e 766f 6c28 7365 6c66 2920 203a 0a20  anvol(self)  :. 
-00018e70: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00018e80: 6c66 2e63 616e 5f61 646d 696e 3a0a 2020  lf.can_admin:.  
-00018e90: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00018ea0: 5065 626b 6163 2834 3033 2c20 226e 6f74  Pebkac(403, "not
-00018eb0: 2061 6c6c 6f77 6564 2066 6f72 2075 7365   allowed for use
-00018ec0: 7220 2220 2b20 7365 6c66 2e75 6e61 6d65  r " + self.uname
-00018ed0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-00018ee0: 6c66 2e61 7267 732e 6e6f 5f72 6573 6361  lf.args.no_resca
-00018ef0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
-00018f00: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
-00018f10: 2022 7468 6520 7265 7363 616e 2066 6561   "the rescan fea
-00018f20: 7475 7265 2069 7320 6469 7361 626c 6564  ture is disabled
-00018f30: 2069 6e20 7365 7276 6572 2063 6f6e 6669   in server confi
-00018f40: 6722 290a 0a20 2020 2020 2020 2076 6e2c  g")..        vn,
-00018f50: 205f 203d 2073 656c 662e 6173 7276 2e76   _ = self.asrv.v
-00018f60: 6673 2e67 6574 2873 656c 662e 7670 6174  fs.get(self.vpat
-00018f70: 682c 2073 656c 662e 756e 616d 652c 2054  h, self.uname, T
-00018f80: 7275 652c 2054 7275 6529 0a0a 2020 2020  rue, True)..    
-00018f90: 2020 2020 6172 6773 203d 205b 7365 6c66      args = [self
-00018fa0: 2e61 7372 762e 7666 732e 616c 6c5f 766f  .asrv.vfs.all_vo
-00018fb0: 6c73 2c20 5b76 6e2e 7670 6174 685d 2c20  ls, [vn.vpath], 
-00018fc0: 4661 6c73 652c 2054 7275 655d 0a0a 2020  False, True]..  
-00018fd0: 2020 2020 2020 7820 3d20 7365 6c66 2e63        x = self.c
-00018fe0: 6f6e 6e2e 6873 7276 2e62 726f 6b65 722e  onn.hsrv.broker.
-00018ff0: 6173 6b28 2275 7032 6b2e 7265 7363 616e  ask("up2k.rescan
-00019000: 222c 202a 6172 6773 290a 2020 2020 2020  ", *args).      
-00019010: 2020 6572 7220 3d20 782e 6765 7428 290a    err = x.get().
-00019020: 2020 2020 2020 2020 6966 206e 6f74 2065          if not e
-00019030: 7272 3a0a 2020 2020 2020 2020 2020 2020  rr:.            
-00019040: 7365 6c66 2e72 6564 6972 6563 7428 2222  self.redirect(""
-00019050: 2c20 223f 6822 290a 2020 2020 2020 2020  , "?h").        
-00019060: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-00019070: 0a20 2020 2020 2020 2072 6169 7365 2050  .        raise P
-00019080: 6562 6b61 6328 3530 302c 2065 7272 290a  ebkac(500, err).
-00019090: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-000190a0: 7265 6c6f 6164 2873 656c 6629 2020 3a0a  reload(self)  :.
-000190b0: 2020 2020 2020 2020 6163 7420 3d20 7365          act = se
-000190c0: 6c66 2e75 7061 7261 6d2e 6765 7428 2272  lf.uparam.get("r
-000190d0: 656c 6f61 6422 290a 2020 2020 2020 2020  eload").        
-000190e0: 6966 2061 6374 2021 3d20 2263 6667 223a  if act != "cfg":
-000190f0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00019100: 7365 2050 6562 6b61 6328 3430 302c 2022  se Pebkac(400, "
-00019110: 6f6e 6c79 2063 6f6e 6669 6720 6669 6c65  only config file
-00019120: 7320 2827 6366 6727 2920 6361 6e20 6265  s ('cfg') can be
-00019130: 2072 656c 6f61 6465 6420 726e 2229 0a0a   reloaded rn")..
-00019140: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00019150: 656c 662e 6176 6f6c 3a0a 2020 2020 2020  elf.avol:.      
-00019160: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-00019170: 6163 2834 3033 2c20 226e 6f74 2061 6c6c  ac(403, "not all
-00019180: 6f77 6564 2066 6f72 2075 7365 7220 2220  owed for user " 
-00019190: 2b20 7365 6c66 2e75 6e61 6d65 290a 0a20  + self.uname).. 
-000191a0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-000191b0: 7267 732e 6e6f 5f72 656c 6f61 643a 0a20  rgs.no_reload:. 
-000191c0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-000191d0: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
-000191e0: 6520 7265 6c6f 6164 2066 6561 7475 7265  e reload feature
-000191f0: 2069 7320 6469 7361 626c 6564 2069 6e20   is disabled in 
-00019200: 7365 7276 6572 2063 6f6e 6669 6722 290a  server config").
-00019210: 0a20 2020 2020 2020 2078 203d 2073 656c  .        x = sel
-00019220: 662e 636f 6e6e 2e68 7372 762e 6272 6f6b  f.conn.hsrv.brok
-00019230: 6572 2e61 736b 2822 7265 6c6f 6164 2229  er.ask("reload")
-00019240: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00019250: 7365 6c66 2e72 6564 6972 6563 7428 2222  self.redirect(""
-00019260: 2c20 223f 6822 2c20 782e 6765 7428 292c  , "?h", x.get(),
-00019270: 2022 7265 7475 726e 2074 6f22 2c20 4661   "return to", Fa
-00019280: 6c73 6529 0a0a 2020 2020 6465 6620 7478  lse)..    def tx
-00019290: 5f73 7461 636b 2873 656c 6629 2020 3a0a  _stack(self)  :.
-000192a0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000192b0: 656c 662e 6176 6f6c 2061 6e64 206e 6f74  elf.avol and not
-000192c0: 205b 7820 666f 7220 7820 696e 2073 656c   [x for x in sel
-000192d0: 662e 7776 6f6c 2069 6620 7820 696e 2073  f.wvol if x in s
-000192e0: 656c 662e 7276 6f6c 5d3a 0a20 2020 2020  elf.rvol]:.     
-000192f0: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-00019300: 6b61 6328 3430 332c 2022 6e6f 7420 616c  kac(403, "not al
-00019310: 6c6f 7765 6420 666f 7220 7573 6572 2022  lowed for user "
-00019320: 202b 2073 656c 662e 756e 616d 6529 0a0a   + self.uname)..
-00019330: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00019340: 6172 6773 2e6e 6f5f 7374 6163 6b3a 0a20  args.no_stack:. 
-00019350: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00019360: 2050 6562 6b61 6328 3430 332c 2022 7468   Pebkac(403, "th
-00019370: 6520 7374 6163 6b64 756d 7020 6665 6174  e stackdump feat
-00019380: 7572 6520 6973 2064 6973 6162 6c65 6420  ure is disabled 
-00019390: 696e 2073 6572 7665 7220 636f 6e66 6967  in server config
-000193a0: 2229 0a0a 2020 2020 2020 2020 7265 7420  ")..        ret 
-000193b0: 3d20 223c 7072 653e 7b7d 5c6e 7b7d 222e  = "<pre>{}\n{}".
-000193c0: 666f 726d 6174 2874 696d 652e 7469 6d65  format(time.time
-000193d0: 2829 2c20 6874 6d6c 5f65 7363 6170 6528  (), html_escape(
-000193e0: 616c 6c74 7261 6365 2829 2929 0a20 2020  alltrace())).   
-000193f0: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
-00019400: 7265 742e 656e 636f 6465 2822 7574 662d  ret.encode("utf-
-00019410: 3822 2929 0a20 2020 2020 2020 2072 6574  8")).        ret
-00019420: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
-00019430: 6620 7478 5f74 7265 6528 7365 6c66 2920  f tx_tree(self) 
-00019440: 203a 0a20 2020 2020 2020 2074 6f70 203d   :.        top =
-00019450: 2073 656c 662e 7570 6172 616d 5b22 7472   self.uparam["tr
-00019460: 6565 225d 206f 7220 2222 0a20 2020 2020  ee"] or "".     
-00019470: 2020 2064 7374 203d 2073 656c 662e 7670     dst = self.vp
-00019480: 6174 680a 2020 2020 2020 2020 6966 2074  ath.        if t
-00019490: 6f70 2069 6e20 5b22 2e22 2c20 222e 2e22  op in [".", ".."
-000194a0: 5d3a 0a20 2020 2020 2020 2020 2020 2074  ]:.            t
-000194b0: 6f70 203d 2075 6e64 6f74 2873 656c 662e  op = undot(self.
-000194c0: 7670 6174 6820 2b20 222f 2220 2b20 746f  vpath + "/" + to
-000194d0: 7029 0a0a 2020 2020 2020 2020 6966 2074  p)..        if t
-000194e0: 6f70 203d 3d20 6473 743a 0a20 2020 2020  op == dst:.     
-000194f0: 2020 2020 2020 2064 7374 203d 2022 220a         dst = "".
-00019500: 2020 2020 2020 2020 656c 6966 2074 6f70          elif top
-00019510: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00019520: 206e 6f74 2064 7374 2e73 7461 7274 7377   not dst.startsw
-00019530: 6974 6828 746f 7020 2b20 222f 2229 3a0a  ith(top + "/"):.
-00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019550: 7261 6973 6520 5065 626b 6163 2834 3030  raise Pebkac(400
-00019560: 2c20 2261 7267 2066 756e 6b22 290a 0a20  , "arg funk").. 
-00019570: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
-00019580: 2064 7374 5b6c 656e 2874 6f70 2920 2b20   dst[len(top) + 
-00019590: 3120 3a5d 0a0a 2020 2020 2020 2020 7265  1 :]..        re
-000195a0: 7420 3d20 7365 6c66 2e67 656e 5f74 7265  t = self.gen_tre
-000195b0: 6528 746f 702c 2064 7374 290a 2020 2020  e(top, dst).    
-000195c0: 2020 2020 6966 2073 656c 662e 6973 5f76      if self.is_v
-000195d0: 7072 6f78 6965 643a 0a20 2020 2020 2020  proxied:.       
-000195e0: 2020 2020 2070 6172 656e 7473 203d 2073       parents = s
-000195f0: 656c 662e 6172 6773 2e52 2e73 706c 6974  elf.args.R.split
-00019600: 2822 2f22 290a 2020 2020 2020 2020 2020  ("/").          
-00019610: 2020 666f 7220 7061 7265 6e74 2069 6e20    for parent in 
-00019620: 7265 7665 7273 6564 2870 6172 656e 7473  reversed(parents
-00019630: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00019640: 2020 2072 6574 203d 207b 226b 2573 2220     ret = {"k%s" 
-00019650: 2520 2870 6172 656e 742c 293a 2072 6574  % (parent,): ret
-00019660: 2c20 2261 223a 205b 5d7d 0a0a 2020 2020  , "a": []}..    
-00019670: 2020 2020 7a73 203d 206a 736f 6e2e 6475      zs = json.du
-00019680: 6d70 7328 7265 7429 0a20 2020 2020 2020  mps(ret).       
-00019690: 2073 656c 662e 7265 706c 7928 7a73 2e65   self.reply(zs.e
-000196a0: 6e63 6f64 6528 2275 7466 2d38 2229 2c20  ncode("utf-8"), 
-000196b0: 6d69 6d65 3d22 6170 706c 6963 6174 696f  mime="applicatio
-000196c0: 6e2f 6a73 6f6e 2229 0a20 2020 2020 2020  n/json").       
-000196d0: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-000196e0: 2020 6465 6620 6765 6e5f 7472 6565 2873    def gen_tree(s
-000196f0: 656c 662c 2074 6f70 202c 2074 6172 6765  elf, top , targe
-00019700: 7420 2920 2020 3a0a 2020 2020 2020 2020  t )   :.        
-00019710: 7265 7420 2020 3d20 7b7d 0a20 2020 2020  ret   = {}.     
-00019720: 2020 2065 7863 6c20 3d20 4e6f 6e65 0a20     excl = None. 
-00019730: 2020 2020 2020 2069 6620 7461 7267 6574         if target
-00019740: 3a0a 2020 2020 2020 2020 2020 2020 6578  :.            ex
-00019750: 636c 2c20 7461 7267 6574 203d 2028 7461  cl, target = (ta
-00019760: 7267 6574 2e73 706c 6974 2822 2f22 2c20  rget.split("/", 
-00019770: 3129 202b 205b 2222 5d29 5b3a 325d 0a20  1) + [""])[:2]. 
-00019780: 2020 2020 2020 2020 2020 2073 7562 203d             sub =
-00019790: 2073 656c 662e 6765 6e5f 7472 6565 2822   self.gen_tree("
-000197a0: 2f22 2e6a 6f69 6e28 5b74 6f70 2c20 6578  /".join([top, ex
-000197b0: 636c 5d29 2e73 7472 6970 2822 2f22 292c  cl]).strip("/"),
-000197c0: 2074 6172 6765 7429 0a20 2020 2020 2020   target).       
-000197d0: 2020 2020 2072 6574 5b22 6b22 202b 2071       ret["k" + q
-000197e0: 756f 7465 7028 6578 636c 295d 203d 2073  uotep(excl)] = s
-000197f0: 7562 0a0a 2020 2020 2020 2020 7472 793a  ub..        try:
-00019800: 0a20 2020 2020 2020 2020 2020 2076 6e2c  .            vn,
-00019810: 2072 656d 203d 2073 656c 662e 6173 7276   rem = self.asrv
-00019820: 2e76 6673 2e67 6574 2874 6f70 2c20 7365  .vfs.get(top, se
-00019830: 6c66 2e75 6e61 6d65 2c20 5472 7565 2c20  lf.uname, True, 
-00019840: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-00019850: 2020 2066 7372 6f6f 742c 2076 6673 5f6c     fsroot, vfs_l
-00019860: 732c 2076 6673 5f76 6972 7420 3d20 766e  s, vfs_virt = vn
-00019870: 2e6c 7328 0a20 2020 2020 2020 2020 2020  .ls(.           
-00019880: 2020 2020 2072 656d 2c0a 2020 2020 2020       rem,.      
-00019890: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-000198a0: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-000198b0: 2020 2020 2020 6e6f 7420 7365 6c66 2e61        not self.a
-000198c0: 7267 732e 6e6f 5f73 6361 6e64 6972 2c0a  rgs.no_scandir,.
-000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198e0: 5b5b 5472 7565 2c20 4661 6c73 655d 2c20  [[True, False], 
-000198f0: 5b46 616c 7365 2c20 5472 7565 5d5d 2c0a  [False, True]],.
-00019900: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00019910: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00019920: 2020 2020 2020 2020 2020 7666 735f 6c73            vfs_ls
-00019930: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
-00019940: 2020 7666 735f 7669 7274 203d 207b 7d0a    vfs_virt = {}.
-00019950: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00019960: 7620 696e 2073 656c 662e 7276 6f6c 3a0a  v in self.rvol:.
-00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019980: 6431 2c20 6432 203d 2076 2e72 7370 6c69  d1, d2 = v.rspli
-00019990: 7428 222f 222c 2031 2920 6966 2022 2f22  t("/", 1) if "/"
-000199a0: 2069 6e20 7620 656c 7365 205b 2222 2c20   in v else ["", 
-000199b0: 765d 0a20 2020 2020 2020 2020 2020 2020  v].             
-000199c0: 2020 2069 6620 6431 203d 3d20 746f 703a     if d1 == top:
-000199d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000199e0: 2020 2020 2076 6673 5f76 6972 745b 6432       vfs_virt[d2
-000199f0: 5d20 3d20 7365 6c66 2e61 7372 762e 7666  ] = self.asrv.vf
-00019a00: 7320 2023 2074 7970 6563 686b 2c20 7661  s  # typechk, va
-00019a10: 6c75 6520 6e65 7665 7220 7265 6164 0a0a  lue never read..
-00019a20: 2020 2020 2020 2020 6469 7273 203d 205b          dirs = [
-00019a30: 5d0a 0a20 2020 2020 2020 2064 6972 6e61  ]..        dirna
-00019a40: 6d65 7320 3d20 5b78 5b30 5d20 666f 7220  mes = [x[0] for 
-00019a50: 7820 696e 2076 6673 5f6c 7320 6966 2073  x in vfs_ls if s
-00019a60: 7461 742e 535f 4953 4449 5228 785b 315d  tat.S_ISDIR(x[1]
-00019a70: 2e73 745f 6d6f 6465 295d 0a0a 2020 2020  .st_mode)]..    
-00019a80: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-00019a90: 6172 6773 2e65 6420 6f72 2022 646f 7473  args.ed or "dots
-00019aa0: 2220 6e6f 7420 696e 2073 656c 662e 7570  " not in self.up
-00019ab0: 6172 616d 3a0a 2020 2020 2020 2020 2020  aram:.          
-00019ac0: 2020 6469 726e 616d 6573 203d 2065 7863    dirnames = exc
-00019ad0: 6c75 6465 5f64 6f74 6669 6c65 7328 6469  lude_dotfiles(di
-00019ae0: 726e 616d 6573 290a 0a20 2020 2020 2020  rnames)..       
-00019af0: 2066 6f72 2066 6e20 696e 205b 7820 666f   for fn in [x fo
-00019b00: 7220 7820 696e 2064 6972 6e61 6d65 7320  r x in dirnames 
-00019b10: 6966 2078 2021 3d20 6578 636c 5d3a 0a20  if x != excl]:. 
-00019b20: 2020 2020 2020 2020 2020 2064 6972 732e             dirs.
-00019b30: 6170 7065 6e64 2871 756f 7465 7028 666e  append(quotep(fn
-00019b40: 2929 0a0a 2020 2020 2020 2020 666f 7220  ))..        for 
-00019b50: 7820 696e 2076 6673 5f76 6972 743a 0a20  x in vfs_virt:. 
-00019b60: 2020 2020 2020 2020 2020 2069 6620 7820             if x 
-00019b70: 213d 2065 7863 6c3a 0a20 2020 2020 2020  != excl:.       
-00019b80: 2020 2020 2020 2020 2064 6972 732e 6170           dirs.ap
-00019b90: 7065 6e64 2878 290a 0a20 2020 2020 2020  pend(x)..       
-00019ba0: 2072 6574 5b22 6122 5d20 3d20 6469 7273   ret["a"] = dirs
-00019bb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00019bc0: 7265 740a 0a20 2020 2064 6566 2074 785f  ret..    def tx_
-00019bd0: 7570 7328 7365 6c66 2920 203a 0a20 2020  ups(self)  :.   
-00019be0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00019bf0: 2e61 7267 732e 756e 706f 7374 3a0a 2020  .args.unpost:.  
-00019c00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00019c10: 5065 626b 6163 2834 3033 2c20 2274 6865  Pebkac(403, "the
-00019c20: 2075 6e70 6f73 7420 6665 6174 7572 6520   unpost feature 
-00019c30: 6973 2064 6973 6162 6c65 6420 696e 2073  is disabled in s
-00019c40: 6572 7665 7220 636f 6e66 6967 2229 0a0a  erver config")..
-00019c50: 2020 2020 2020 2020 6964 7820 3d20 7365          idx = se
-00019c60: 6c66 2e63 6f6e 6e2e 6765 745f 7532 6964  lf.conn.get_u2id
-00019c70: 7828 290a 2020 2020 2020 2020 6966 206e  x().        if n
-00019c80: 6f74 2069 6478 206f 7220 6e6f 7420 6861  ot idx or not ha
-00019c90: 7361 7474 7228 6964 782c 2022 705f 656e  sattr(idx, "p_en
-00019ca0: 6422 293a 0a20 2020 2020 2020 2020 2020  d"):.           
-00019cb0: 2072 6169 7365 2050 6562 6b61 6328 3530   raise Pebkac(50
-00019cc0: 302c 2022 7371 6c69 7465 3320 6973 206e  0, "sqlite3 is n
-00019cd0: 6f74 2061 7661 696c 6162 6c65 206f 6e20  ot available on 
-00019ce0: 7468 6520 7365 7276 6572 3b20 6361 6e6e  the server; cann
-00019cf0: 6f74 2075 6e70 6f73 7422 290a 0a20 2020  ot unpost")..   
-00019d00: 2020 2020 2066 696c 7420 3d20 7365 6c66       filt = self
-00019d10: 2e75 7061 7261 6d2e 6765 7428 2266 696c  .uparam.get("fil
-00019d20: 7465 7222 290a 2020 2020 2020 2020 6669  ter").        fi
-00019d30: 6c74 203d 2075 6e71 756f 7465 7028 6669  lt = unquotep(fi
-00019d40: 6c74 206f 7220 2222 290a 2020 2020 2020  lt or "").      
-00019d50: 2020 6c6d 203d 2022 7570 7320 5b7b 7d5d    lm = "ups [{}]
-00019d60: 222e 666f 726d 6174 2866 696c 7429 0a20  ".format(filt). 
-00019d70: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
-00019d80: 6c6d 290a 0a20 2020 2020 2020 2072 6574  lm)..        ret
-00019d90: 2020 203d 205b 5d0a 2020 2020 2020 2020     = [].        
-00019da0: 7430 203d 2074 696d 652e 7469 6d65 2829  t0 = time.time()
-00019db0: 0a20 2020 2020 2020 206c 696d 203d 2074  .        lim = t
-00019dc0: 696d 652e 7469 6d65 2829 202d 2073 656c  ime.time() - sel
-00019dd0: 662e 6172 6773 2e75 6e70 6f73 740a 2020  f.args.unpost.  
-00019de0: 2020 2020 2020 666b 5f76 6f6c 7320 3d20        fk_vols = 
-00019df0: 7b0a 2020 2020 2020 2020 2020 2020 766f  {.            vo
-00019e00: 6c3a 2076 6f6c 2e66 6c61 6773 5b22 666b  l: vol.flags["fk
-00019e10: 225d 0a20 2020 2020 2020 2020 2020 2066  "].            f
-00019e20: 6f72 2076 702c 2076 6f6c 2069 6e20 7365  or vp, vol in se
-00019e30: 6c66 2e61 7372 762e 7666 732e 616c 6c5f  lf.asrv.vfs.all_
-00019e40: 766f 6c73 2e69 7465 6d73 2829 0a20 2020  vols.items().   
-00019e50: 2020 2020 2020 2020 2069 6620 2266 6b22           if "fk"
-00019e60: 2069 6e20 766f 6c2e 666c 6167 7320 616e   in vol.flags an
-00019e70: 6420 2876 7020 696e 2073 656c 662e 7276  d (vp in self.rv
-00019e80: 6f6c 206f 7220 7670 2069 6e20 7365 6c66  ol or vp in self
-00019e90: 2e75 7076 6f6c 290a 2020 2020 2020 2020  .upvol).        
-00019ea0: 7d0a 2020 2020 2020 2020 666f 7220 766f  }.        for vo
-00019eb0: 6c20 696e 2073 656c 662e 6173 7276 2e76  l in self.asrv.v
-00019ec0: 6673 2e61 6c6c 5f76 6f6c 732e 7661 6c75  fs.all_vols.valu
-00019ed0: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
-00019ee0: 2020 6375 7220 3d20 6964 782e 6765 745f    cur = idx.get_
-00019ef0: 6375 7228 766f 6c2e 7265 616c 7061 7468  cur(vol.realpath
-00019f00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00019f10: 206e 6f74 2063 7572 3a0a 2020 2020 2020   not cur:.      
-00019f20: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-00019f30: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-00019f40: 6e66 6b20 3d20 666b 5f76 6f6c 732e 6765  nfk = fk_vols.ge
-00019f50: 7428 766f 6c2c 2030 290a 0a20 2020 2020  t(vol, 0)..     
-00019f60: 2020 2020 2020 2071 203d 2022 7365 6c65         q = "sele
-00019f70: 6374 2073 7a2c 2072 642c 2066 6e2c 2061  ct sz, rd, fn, a
-00019f80: 7420 6672 6f6d 2075 7020 7768 6572 6520  t from up where 
-00019f90: 6970 3d3f 2061 6e64 2061 743e 3f22 0a20  ip=? and at>?". 
-00019fa0: 2020 2020 2020 2020 2020 2066 6f72 2073             for s
-00019fb0: 7a2c 2072 642c 2066 6e2c 2061 7420 696e  z, rd, fn, at in
-00019fc0: 2063 7572 2e65 7865 6375 7465 2871 2c20   cur.execute(q, 
-00019fd0: 2873 656c 662e 6970 2c20 6c69 6d29 293a  (self.ip, lim)):
-00019fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019ff0: 2076 7020 3d20 222f 2220 2b20 222f 222e   vp = "/" + "/".
-0001a000: 6a6f 696e 2878 2066 6f72 2078 2069 6e20  join(x for x in 
-0001a010: 5b76 6f6c 2e76 7061 7468 2c20 7264 2c20  [vol.vpath, rd, 
-0001a020: 666e 5d20 6966 2078 290a 2020 2020 2020  fn] if x).      
-0001a030: 2020 2020 2020 2020 2020 6966 2066 696c            if fil
-0001a040: 7420 616e 6420 6669 6c74 206e 6f74 2069  t and filt not i
-0001a050: 6e20 7670 3a0a 2020 2020 2020 2020 2020  n vp:.          
-0001a060: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0001a070: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-0001a080: 2020 2020 7276 203d 207b 2276 7022 3a20      rv = {"vp": 
-0001a090: 7175 6f74 6570 2876 7029 2c20 2273 7a22  quotep(vp), "sz"
-0001a0a0: 3a20 737a 2c20 2261 7422 3a20 6174 2c20  : sz, "at": at, 
-0001a0b0: 226e 666b 223a 206e 666b 7d0a 2020 2020  "nfk": nfk}.    
-0001a0c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001a0d0: 666b 3a0a 2020 2020 2020 2020 2020 2020  fk:.            
-0001a0e0: 2020 2020 2020 2020 7276 5b22 6170 225d          rv["ap"]
-0001a0f0: 203d 2076 6f6c 2e63 616e 6f6e 6963 616c   = vol.canonical
-0001a100: 2876 6a6f 696e 2872 642c 2066 6e29 290a  (vjoin(rd, fn)).
-0001a110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a120: 2072 6574 2e61 7070 656e 6428 7276 290a   ret.append(rv).
-0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a140: 6966 206c 656e 2872 6574 2920 3e20 3330  if len(ret) > 30
-0001a150: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
-0001a160: 2020 2020 2020 2020 7265 742e 736f 7274          ret.sort
-0001a170: 286b 6579 3d6c 616d 6264 6120 783a 2078  (key=lambda x: x
-0001a180: 5b22 6174 225d 2c20 7265 7665 7273 653d  ["at"], reverse=
-0001a190: 5472 7565 2920 2023 2074 7970 653a 2069  True)  # type: i
-0001a1a0: 676e 6f72 650a 2020 2020 2020 2020 2020  gnore.          
-0001a1b0: 2020 2020 2020 2020 2020 7265 7420 3d20            ret = 
-0001a1c0: 7265 745b 3a32 3030 305d 0a0a 2020 2020  ret[:2000]..    
-0001a1d0: 2020 2020 7265 742e 736f 7274 286b 6579      ret.sort(key
-0001a1e0: 3d6c 616d 6264 6120 783a 2078 5b22 6174  =lambda x: x["at
-0001a1f0: 225d 2c20 7265 7665 7273 653d 5472 7565  "], reverse=True
-0001a200: 2920 2023 2074 7970 653a 2069 676e 6f72  )  # type: ignor
-0001a210: 650a 2020 2020 2020 2020 6e20 3d20 300a  e.        n = 0.
-0001a220: 2020 2020 2020 2020 666f 7220 7276 2069          for rv i
-0001a230: 6e20 7265 745b 3a31 3130 3030 5d3a 0a20  n ret[:11000]:. 
-0001a240: 2020 2020 2020 2020 2020 206e 666b 203d             nfk =
-0001a250: 2072 762e 706f 7028 226e 666b 2229 0a20   rv.pop("nfk"). 
-0001a260: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0001a270: 7420 6e66 6b3a 0a20 2020 2020 2020 2020  t nfk:.         
-0001a280: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-0001a290: 0a20 2020 2020 2020 2020 2020 2061 7020  .            ap 
-0001a2a0: 3d20 7276 2e70 6f70 2822 6170 2229 0a20  = rv.pop("ap"). 
-0001a2b0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0001a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2d0: 7374 203d 2062 6f73 2e73 7461 7428 6170  st = bos.stat(ap
-0001a2e0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
-0001a2f0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-0001a300: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-0001a310: 2020 2020 2020 2020 2020 2020 666b 203d              fk =
-0001a320: 2073 656c 662e 6765 6e5f 666b 280a 2020   self.gen_fk(.  
-0001a330: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001a340: 6c66 2e61 7267 732e 666b 5f73 616c 742c  lf.args.fk_salt,
-0001a350: 2061 702c 2073 742e 7374 5f73 697a 652c   ap, st.st_size,
-0001a360: 2030 2069 6620 414e 5957 494e 2065 6c73   0 if ANYWIN els
-0001a370: 6520 7374 2e73 745f 696e 6f0a 2020 2020  e st.st_ino.    
-0001a380: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0001a390: 2020 2020 2020 7276 5b22 7670 225d 202b        rv["vp"] +
-0001a3a0: 3d20 223f 6b3d 2220 2b20 666b 5b3a 6e66  = "?k=" + fk[:nf
-0001a3b0: 6b5d 0a0a 2020 2020 2020 2020 2020 2020  k]..            
-0001a3c0: 6e20 2b3d 2031 0a20 2020 2020 2020 2020  n += 1.         
-0001a3d0: 2020 2069 6620 6e20 3e20 3230 3030 3a0a     if n > 2000:.
-0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3f0: 6272 6561 6b0a 0a20 2020 2020 2020 2072  break..        r
-0001a400: 6574 203d 2072 6574 5b3a 3230 3030 5d0a  et = ret[:2000].
-0001a410: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0001a420: 2e69 735f 7670 726f 7869 6564 3a0a 2020  .is_vproxied:.  
-0001a430: 2020 2020 2020 2020 2020 666f 7220 7620            for v 
-0001a440: 696e 2072 6574 3a0a 2020 2020 2020 2020  in ret:.        
-0001a450: 2020 2020 2020 2020 765b 2276 7022 5d20          v["vp"] 
-0001a460: 3d20 7365 6c66 2e61 7267 732e 5352 202b  = self.args.SR +
-0001a470: 2076 5b22 7670 225d 0a0a 2020 2020 2020   v["vp"]..      
-0001a480: 2020 6a74 7874 203d 206a 736f 6e2e 6475    jtxt = json.du
-0001a490: 6d70 7328 7265 742c 2069 6e64 656e 743d  mps(ret, indent=
-0001a4a0: 322c 2073 6f72 745f 6b65 7973 3d54 7275  2, sort_keys=Tru
-0001a4b0: 6529 2e65 6e63 6f64 6528 2275 7466 2d38  e).encode("utf-8
-0001a4c0: 222c 2022 7265 706c 6163 6522 290a 2020  ", "replace").  
-0001a4d0: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
-0001a4e0: 7b7d 2023 7b7d 207b 3a2e 3266 7d73 6563  {} #{} {:.2f}sec
-0001a4f0: 222e 666f 726d 6174 286c 6d2c 206c 656e  ".format(lm, len
-0001a500: 2872 6574 292c 2074 696d 652e 7469 6d65  (ret), time.time
-0001a510: 2829 202d 2074 3029 290a 2020 2020 2020  () - t0)).      
-0001a520: 2020 7365 6c66 2e72 6570 6c79 286a 7478    self.reply(jtx
-0001a530: 742c 206d 696d 653d 2261 7070 6c69 6361  t, mime="applica
-0001a540: 7469 6f6e 2f6a 736f 6e22 290a 2020 2020  tion/json").    
-0001a550: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0001a560: 0a20 2020 2064 6566 2068 616e 646c 655f  .    def handle_
-0001a570: 726d 2873 656c 662c 2072 6571 2029 2020  rm(self, req )  
-0001a580: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
-0001a590: 2072 6571 2061 6e64 206e 6f74 2073 656c   req and not sel
-0001a5a0: 662e 6361 6e5f 6465 6c65 7465 3a0a 2020  f.can_delete:.  
-0001a5b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001a5c0: 5065 626b 6163 2834 3033 2c20 226e 6f74  Pebkac(403, "not
-0001a5d0: 2061 6c6c 6f77 6564 2066 6f72 2075 7365   allowed for use
-0001a5e0: 7220 2220 2b20 7365 6c66 2e75 6e61 6d65  r " + self.uname
-0001a5f0: 290a 0a20 2020 2020 2020 2069 6620 7365  )..        if se
-0001a600: 6c66 2e61 7267 732e 6e6f 5f64 656c 3a0a  lf.args.no_del:.
-0001a610: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0001a620: 6520 5065 626b 6163 2834 3033 2c20 2274  e Pebkac(403, "t
-0001a630: 6865 2064 656c 6574 6520 6665 6174 7572  he delete featur
-0001a640: 6520 6973 2064 6973 6162 6c65 6420 696e  e is disabled in
-0001a650: 2073 6572 7665 7220 636f 6e66 6967 2229   server config")
-0001a660: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0001a670: 2072 6571 3a0a 2020 2020 2020 2020 2020   req:.          
-0001a680: 2020 7265 7120 3d20 5b73 656c 662e 7670    req = [self.vp
-0001a690: 6174 685d 0a20 2020 2020 2020 2065 6c69  ath].        eli
-0001a6a0: 6620 7365 6c66 2e69 735f 7670 726f 7869  f self.is_vproxi
-0001a6b0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-0001a6c0: 7265 7120 3d20 5b78 5b6c 656e 2873 656c  req = [x[len(sel
-0001a6d0: 662e 6172 6773 2e53 5229 203a 5d20 666f  f.args.SR) :] fo
-0001a6e0: 7220 7820 696e 2072 6571 5d0a 0a20 2020  r x in req]..   
-0001a6f0: 2020 2020 206e 6c69 6d20 3d20 696e 7428       nlim = int(
-0001a700: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
-0001a710: 226c 696d 2229 206f 7220 3029 0a20 2020  "lim") or 0).   
-0001a720: 2020 2020 206c 696d 203d 205b 6e6c 696d       lim = [nlim
-0001a730: 2c20 6e6c 696d 5d20 6966 206e 6c69 6d20  , nlim] if nlim 
-0001a740: 656c 7365 205b 5d0a 0a20 2020 2020 2020  else []..       
-0001a750: 2078 203d 2073 656c 662e 636f 6e6e 2e68   x = self.conn.h
-0001a760: 7372 762e 6272 6f6b 6572 2e61 736b 280a  srv.broker.ask(.
-0001a770: 2020 2020 2020 2020 2020 2020 2275 7032              "up2
-0001a780: 6b2e 6861 6e64 6c65 5f72 6d22 2c20 7365  k.handle_rm", se
-0001a790: 6c66 2e75 6e61 6d65 2c20 7365 6c66 2e69  lf.uname, self.i
-0001a7a0: 702c 2072 6571 2c20 6c69 6d2c 2046 616c  p, req, lim, Fal
-0001a7b0: 7365 0a20 2020 2020 2020 2029 0a20 2020  se.        ).   
-0001a7c0: 2020 2020 2073 656c 662e 6c6f 7564 5f72       self.loud_r
-0001a7d0: 6570 6c79 2878 2e67 6574 2829 290a 2020  eply(x.get()).  
-0001a7e0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0001a7f0: 650a 0a20 2020 2064 6566 2068 616e 646c  e..    def handl
-0001a800: 655f 6d76 2873 656c 6629 2020 3a0a 2020  e_mv(self)  :.  
-0001a810: 2020 2020 2020 2320 6675 6c6c 2070 6174        # full pat
-0001a820: 6820 6f66 206e 6577 206c 6f63 2028 696e  h of new loc (in
-0001a830: 636c 2066 696c 656e 616d 6529 0a20 2020  cl filename).   
-0001a840: 2020 2020 2064 7374 203d 2073 656c 662e       dst = self.
-0001a850: 7570 6172 616d 2e67 6574 2822 6d6f 7665  uparam.get("move
-0001a860: 2229 0a0a 2020 2020 2020 2020 6966 2073  ")..        if s
-0001a870: 656c 662e 6973 5f76 7072 6f78 6965 6420  elf.is_vproxied 
-0001a880: 616e 6420 6473 7420 616e 6420 6473 742e  and dst and dst.
-0001a890: 7374 6172 7473 7769 7468 2873 656c 662e  startswith(self.
-0001a8a0: 6172 6773 2e53 5229 3a0a 2020 2020 2020  args.SR):.      
-0001a8b0: 2020 2020 2020 6473 7420 3d20 6473 745b        dst = dst[
-0001a8c0: 6c65 6e28 7365 6c66 2e61 7267 732e 5253  len(self.args.RS
-0001a8d0: 2920 3a5d 0a0a 2020 2020 2020 2020 6966  ) :]..        if
-0001a8e0: 206e 6f74 2064 7374 3a0a 2020 2020 2020   not dst:.      
-0001a8f0: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
-0001a900: 6163 2834 3030 2c20 226e 6565 6420 6473  ac(400, "need ds
-0001a910: 7420 7670 6174 6822 290a 0a20 2020 2020  t vpath")..     
-0001a920: 2020 2023 2078 2d77 7777 2d66 6f72 6d2d     # x-www-form-
-0001a930: 7572 6c65 6e63 6f64 6564 2028 7572 6c20  urlencoded (url 
-0001a940: 7175 6572 7920 7061 7274 2920 7573 6573  query part) uses
-0001a950: 0a20 2020 2020 2020 2023 2065 6974 6865  .        # eithe
-0001a960: 7220 2b20 6f72 2025 3230 2066 6f72 2030  r + or %20 for 0
-0001a970: 7832 3020 736f 2068 616e 646c 6520 626f  x20 so handle bo
-0001a980: 7468 0a20 2020 2020 2020 2064 7374 203d  th.        dst =
-0001a990: 2075 6e71 756f 7465 7028 6473 742e 7265   unquotep(dst.re
-0001a9a0: 706c 6163 6528 222b 222c 2022 2022 2929  place("+", " "))
-0001a9b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001a9c0: 7365 6c66 2e5f 6d76 2873 656c 662e 7670  self._mv(self.vp
-0001a9d0: 6174 682c 2064 7374 2e6c 7374 7269 7028  ath, dst.lstrip(
-0001a9e0: 222f 2229 290a 0a20 2020 2064 6566 205f  "/"))..    def _
-0001a9f0: 6d76 2873 656c 662c 2076 7372 6320 2c20  mv(self, vsrc , 
-0001aa00: 7664 7374 2029 2020 3a0a 2020 2020 2020  vdst )  :.      
-0001aa10: 2020 6966 206e 6f74 2073 656c 662e 6361    if not self.ca
-0001aa20: 6e5f 6d6f 7665 3a0a 2020 2020 2020 2020  n_move:.        
-0001aa30: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
-0001aa40: 2834 3033 2c20 226e 6f74 2061 6c6c 6f77  (403, "not allow
-0001aa50: 6564 2066 6f72 2075 7365 7220 2220 2b20  ed for user " + 
-0001aa60: 7365 6c66 2e75 6e61 6d65 290a 0a20 2020  self.uname)..   
-0001aa70: 2020 2020 2069 6620 7365 6c66 2e61 7267       if self.arg
-0001aa80: 732e 6e6f 5f6d 763a 0a20 2020 2020 2020  s.no_mv:.       
-0001aa90: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
-0001aaa0: 6328 3430 332c 2022 7468 6520 7265 6e61  c(403, "the rena
-0001aab0: 6d65 2f6d 6f76 6520 6665 6174 7572 6520  me/move feature 
-0001aac0: 6973 2064 6973 6162 6c65 6420 696e 2073  is disabled in s
-0001aad0: 6572 7665 7220 636f 6e66 6967 2229 0a0a  erver config")..
-0001aae0: 2020 2020 2020 2020 7820 3d20 7365 6c66          x = self
-0001aaf0: 2e63 6f6e 6e2e 6873 7276 2e62 726f 6b65  .conn.hsrv.broke
-0001ab00: 722e 6173 6b28 2275 7032 6b2e 6861 6e64  r.ask("up2k.hand
-0001ab10: 6c65 5f6d 7622 2c20 7365 6c66 2e75 6e61  le_mv", self.una
-0001ab20: 6d65 2c20 7673 7263 2c20 7664 7374 290a  me, vsrc, vdst).
-0001ab30: 2020 2020 2020 2020 7365 6c66 2e6c 6f75          self.lou
-0001ab40: 645f 7265 706c 7928 782e 6765 7428 292c  d_reply(x.get(),
-0001ab50: 2073 7461 7475 733d 3230 3129 0a20 2020   status=201).   
-0001ab60: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-0001ab70: 0a0a 2020 2020 6465 6620 7478 5f6c 7328  ..    def tx_ls(
-0001ab80: 7365 6c66 2c20 6c73 2020 2920 203a 0a20  self, ls  )  :. 
-0001ab90: 2020 2020 2020 2064 6972 7320 3d20 6c73         dirs = ls
-0001aba0: 5b22 6469 7273 225d 0a20 2020 2020 2020  ["dirs"].       
-0001abb0: 2066 696c 6573 203d 206c 735b 2266 696c   files = ls["fil
-0001abc0: 6573 225d 0a20 2020 2020 2020 2061 7267  es"].        arg
-0001abd0: 203d 2073 656c 662e 7570 6172 616d 5b22   = self.uparam["
-0001abe0: 6c73 225d 0a20 2020 2020 2020 2069 6620  ls"].        if 
-0001abf0: 6172 6720 696e 205b 2276 222c 2022 7422  arg in ["v", "t"
-0001ac00: 2c20 2274 7874 225d 3a0a 2020 2020 2020  , "txt"]:.      
-0001ac10: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0001ac20: 2020 2020 2020 2020 2020 2062 6967 6765             bigge
-0001ac30: 7374 203d 206d 6178 286c 735b 2266 696c  st = max(ls["fil
-0001ac40: 6573 225d 202b 206c 735b 2264 6972 7322  es"] + ls["dirs"
-0001ac50: 5d2c 206b 6579 3d69 7465 6d67 6574 7465  ], key=itemgette
-0001ac60: 7228 2273 7a22 2929 5b22 737a 225d 0a20  r("sz"))["sz"]. 
-0001ac70: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0001ac80: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0001ac90: 2020 2062 6967 6765 7374 203d 2030 0a0a     biggest = 0..
-0001aca0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-0001acb0: 7267 203d 3d20 2276 223a 0a20 2020 2020  rg == "v":.     
-0001acc0: 2020 2020 2020 2020 2020 2066 6d74 203d             fmt =
-0001acd0: 2022 5c30 3333 5b30 3b37 3b33 366d 7b7b   "\033[0;7;36m{{
-0001ace0: 7d7d 7b7b 3a3e 7b7d 7d7d 5c30 3333 5b30  }}{{:>{}}}\033[0
-0001acf0: 6d20 7b7b 7d7d 220a 2020 2020 2020 2020  m {{}}".        
-0001ad00: 2020 2020 2020 2020 6e66 6d74 203d 2022          nfmt = "
-0001ad10: 7b7d 220a 2020 2020 2020 2020 2020 2020  {}".            
-0001ad20: 2020 2020 6269 6767 6573 7420 3d20 300a      biggest = 0.
-0001ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad40: 6632 203d 2022 222e 6a6f 696e 280a 2020  f2 = "".join(.  
+00018340: 7478 7420 2b3d 2022 207b 7d28 7b7d 2922  txt += " {}({})"
+00018350: 2e66 6f72 6d61 7428 6b2c 2076 735b 6b5d  .format(k, vs[k]
+00018360: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00018370: 6620 7276 6f6c 3a0a 2020 2020 2020 2020  f rvol:.        
+00018380: 2020 2020 2020 2020 7478 7420 2b3d 2022          txt += "
+00018390: 5c6e 796f 7520 6361 6e20 6272 6f77 7365  \nyou can browse
+000183a0: 3a22 0a20 2020 2020 2020 2020 2020 2020  :".             
+000183b0: 2020 2066 6f72 2076 2069 6e20 7276 6f6c     for v in rvol
+000183c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000183d0: 2020 2020 2020 7478 7420 2b3d 2022 5c6e        txt += "\n
+000183e0: 2020 2220 2b20 760a 0a20 2020 2020 2020    " + v..       
+000183f0: 2020 2020 2069 6620 7776 6f6c 3a0a 2020       if wvol:.  
+00018400: 2020 2020 2020 2020 2020 2020 2020 7478                tx
+00018410: 7420 2b3d 2022 5c6e 796f 7520 6361 6e20  t += "\nyou can 
+00018420: 7570 6c6f 6164 2074 6f3a 220a 2020 2020  upload to:".    
+00018430: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00018440: 7620 696e 2077 766f 6c3a 0a20 2020 2020  v in wvol:.     
+00018450: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00018460: 7874 202b 3d20 225c 6e20 2022 202b 2076  xt += "\n  " + v
+00018470: 0a0a 2020 2020 2020 2020 2020 2020 7a62  ..            zb
+00018480: 203d 2074 7874 2e65 6e63 6f64 6528 2275   = txt.encode("u
+00018490: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
+000184a0: 2920 2b20 6222 5c6e 220a 2020 2020 2020  ) + b"\n".      
+000184b0: 2020 2020 2020 7365 6c66 2e72 6570 6c79        self.reply
+000184c0: 287a 622c 206d 696d 653d 2274 6578 742f  (zb, mime="text/
+000184d0: 706c 6169 6e3b 2063 6861 7273 6574 3d75  plain; charset=u
+000184e0: 7466 2d38 2229 0a20 2020 2020 2020 2020  tf-8").         
+000184f0: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
+00018500: 2020 2020 2020 2020 6874 6d6c 203d 2073          html = s
+00018510: 656c 662e 6a32 7328 0a20 2020 2020 2020  elf.j2s(.       
+00018520: 2020 2020 2022 7370 6c61 7368 222c 0a20       "splash",. 
+00018530: 2020 2020 2020 2020 2020 2074 6869 733d             this=
+00018540: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00018550: 2020 7176 7061 7468 3d71 756f 7465 7028    qvpath=quotep(
+00018560: 7365 6c66 2e76 7061 7468 292c 0a20 2020  self.vpath),.   
+00018570: 2020 2020 2020 2020 2072 766f 6c3d 7276           rvol=rv
+00018580: 6f6c 2c0a 2020 2020 2020 2020 2020 2020  ol,.            
+00018590: 7776 6f6c 3d77 766f 6c2c 0a20 2020 2020  wvol=wvol,.     
+000185a0: 2020 2020 2020 2061 766f 6c3d 6176 6f6c         avol=avol
+000185b0: 2c0a 2020 2020 2020 2020 2020 2020 7673  ,.            vs
+000185c0: 7461 7465 3d76 7374 6174 652c 0a20 2020  tate=vstate,.   
+000185d0: 2020 2020 2020 2020 2073 6361 6e6e 696e           scannin
+000185e0: 673d 7673 5b22 7363 616e 6e69 6e67 225d  g=vs["scanning"]
+000185f0: 2c0a 2020 2020 2020 2020 2020 2020 6861  ,.            ha
+00018600: 7368 713d 7673 5b22 6861 7368 7122 5d2c  shq=vs["hashq"],
+00018610: 0a20 2020 2020 2020 2020 2020 2074 6167  .            tag
+00018620: 713d 7673 5b22 7461 6771 225d 2c0a 2020  q=vs["tagq"],.  
+00018630: 2020 2020 2020 2020 2020 6d74 7071 3d76            mtpq=v
+00018640: 735b 226d 7470 7122 5d2c 0a20 2020 2020  s["mtpq"],.     
+00018650: 2020 2020 2020 2064 6277 743d 7673 5b22         dbwt=vs["
+00018660: 6462 7774 225d 2c0a 2020 2020 2020 2020  dbwt"],.        
+00018670: 2020 2020 7572 6c5f 7375 663d 7375 662c      url_suf=suf,
+00018680: 0a20 2020 2020 2020 2020 2020 206b 3330  .            k30
+00018690: 343d 7365 6c66 2e6b 3330 3428 292c 0a20  4=self.k304(),. 
+000186a0: 2020 2020 2020 2020 2020 2076 6572 3d53             ver=S
+000186b0: 5f56 4552 5349 4f4e 2069 6620 7365 6c66  _VERSION if self
+000186c0: 2e61 7267 732e 7665 7220 656c 7365 2022  .args.ver else "
+000186d0: 222c 0a20 2020 2020 2020 2020 2020 2061  ",.            a
+000186e0: 6874 7470 733d 2222 2069 6620 7365 6c66  https="" if self
+000186f0: 2e69 735f 6874 7470 7320 656c 7365 2022  .is_https else "
+00018700: 6874 7470 733a 2f2f 2220 2b20 7365 6c66  https://" + self
+00018710: 2e68 6f73 7420 2b20 7365 6c66 2e72 6571  .host + self.req
+00018720: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00018730: 2020 2020 7365 6c66 2e72 6570 6c79 2868      self.reply(h
+00018740: 746d 6c2e 656e 636f 6465 2822 7574 662d  tml.encode("utf-
+00018750: 3822 2929 0a20 2020 2020 2020 2072 6574  8")).        ret
+00018760: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+00018770: 6620 7365 745f 6b33 3034 2873 656c 6629  f set_k304(self)
+00018780: 2020 3a0a 2020 2020 2020 2020 636b 203d    :.        ck =
+00018790: 2067 656e 636f 6f6b 6965 2822 6b33 3034   gencookie("k304
+000187a0: 222c 2073 656c 662e 7570 6172 616d 5b22  ", self.uparam["
+000187b0: 6b33 3034 225d 2c20 7365 6c66 2e61 7267  k304"], self.arg
+000187c0: 732e 522c 2046 616c 7365 2c20 3836 3430  s.R, False, 8640
+000187d0: 3020 2a20 3239 3929 0a20 2020 2020 2020  0 * 299).       
+000187e0: 2073 656c 662e 6f75 745f 6865 6164 6572   self.out_header
+000187f0: 6c69 7374 2e61 7070 656e 6428 2822 5365  list.append(("Se
+00018800: 742d 436f 6f6b 6965 222c 2063 6b29 290a  t-Cookie", ck)).
+00018810: 2020 2020 2020 2020 7365 6c66 2e72 6564          self.red
+00018820: 6972 6563 7428 2222 2c20 223f 6823 6363  irect("", "?h#cc
+00018830: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+00018840: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
+00018850: 7365 7463 6b28 7365 6c66 2920 203a 0a20  setck(self)  :. 
+00018860: 2020 2020 2020 206b 2c20 7620 3d20 7365         k, v = se
+00018870: 6c66 2e75 7061 7261 6d5b 2273 6574 636b  lf.uparam["setck
+00018880: 225d 2e73 706c 6974 2822 3d22 2c20 3129  "].split("=", 1)
+00018890: 0a20 2020 2020 2020 2074 203d 204e 6f6e  .        t = Non
+000188a0: 6520 6966 2076 203d 3d20 2222 2065 6c73  e if v == "" els
+000188b0: 6520 3836 3430 3020 2a20 3239 390a 2020  e 86400 * 299.  
+000188c0: 2020 2020 2020 636b 203d 2067 656e 636f        ck = genco
+000188d0: 6f6b 6965 286b 2c20 762c 2073 656c 662e  okie(k, v, self.
+000188e0: 6172 6773 2e52 2c20 4661 6c73 652c 2074  args.R, False, t
+000188f0: 290a 2020 2020 2020 2020 7365 6c66 2e6f  ).        self.o
+00018900: 7574 5f68 6561 6465 726c 6973 742e 6170  ut_headerlist.ap
+00018910: 7065 6e64 2828 2253 6574 2d43 6f6f 6b69  pend(("Set-Cooki
+00018920: 6522 2c20 636b 2929 0a20 2020 2020 2020  e", ck)).       
+00018930: 2073 656c 662e 7265 706c 7928 6222 6f37   self.reply(b"o7
+00018940: 5c6e 2229 0a20 2020 2020 2020 2072 6574  \n").        ret
+00018950: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
+00018960: 6620 7365 745f 6366 675f 7265 7365 7428  f set_cfg_reset(
+00018970: 7365 6c66 2920 203a 0a20 2020 2020 2020  self)  :.       
+00018980: 2066 6f72 206b 2069 6e20 2822 6b33 3034   for k in ("k304
+00018990: 222c 2022 6a73 222c 2022 6964 7868 222c  ", "js", "idxh",
+000189a0: 2022 6370 7077 6422 2c20 2263 7070 7773   "cppwd", "cppws
+000189b0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+000189c0: 636f 6f6b 6965 203d 2067 656e 636f 6f6b  cookie = gencook
+000189d0: 6965 286b 2c20 2278 222c 2073 656c 662e  ie(k, "x", self.
+000189e0: 6172 6773 2e52 2c20 4661 6c73 652c 204e  args.R, False, N
+000189f0: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+00018a00: 2073 656c 662e 6f75 745f 6865 6164 6572   self.out_header
+00018a10: 6c69 7374 2e61 7070 656e 6428 2822 5365  list.append(("Se
+00018a20: 742d 436f 6f6b 6965 222c 2063 6f6f 6b69  t-Cookie", cooki
+00018a30: 6529 290a 0a20 2020 2020 2020 2073 656c  e))..        sel
+00018a40: 662e 7265 6469 7265 6374 2822 222c 2022  f.redirect("", "
+00018a50: 3f68 2363 6322 290a 2020 2020 2020 2020  ?h#cc").        
+00018a60: 7265 7475 726e 2054 7275 650a 0a20 2020  return True..   
+00018a70: 2064 6566 2074 785f 3430 3428 7365 6c66   def tx_404(self
+00018a80: 2c20 6973 5f34 3033 2020 3d20 4661 6c73  , is_403  = Fals
+00018a90: 6529 2020 3a0a 2020 2020 2020 2020 7263  e)  :.        rc
+00018aa0: 203d 2034 3034 0a20 2020 2020 2020 2069   = 404.        i
+00018ab0: 6620 7365 6c66 2e61 7267 732e 7661 6775  f self.args.vagu
+00018ac0: 655f 3430 333a 0a20 2020 2020 2020 2020  e_403:.         
+00018ad0: 2020 2074 203d 2027 3c68 3120 6964 3d22     t = '<h1 id="
+00018ae0: 6e22 3e34 3034 206e 6f74 2066 6f75 6e64  n">404 not found
+00018af0: 2026 6e62 7370 3be2 9490 2820 c2b4 202d   &nbsp;...( .. -
+00018b00: 6029 e294 8c3c 2f68 313e 3c70 2069 643d  `)...</h1><p id=
+00018b10: 226f 223e 6f72 206d 6179 6265 2079 6f75  "o">or maybe you
+00018b20: 2064 6f6e 5c27 7420 6861 7665 2061 6363   don\'t have acc
+00018b30: 6573 7320 2d2d 2074 7279 206c 6f67 6769  ess -- try loggi
+00018b40: 6e67 2069 6e20 6f72 203c 6120 6872 6566  ng in or <a href
+00018b50: 3d22 7b7d 2f3f 6822 3e67 6f20 686f 6d65  ="{}/?h">go home
+00018b60: 3c2f 613e 3c2f 703e 270a 2020 2020 2020  </a></p>'.      
+00018b70: 2020 656c 6966 2069 735f 3430 333a 0a20    elif is_403:. 
+00018b80: 2020 2020 2020 2020 2020 2074 203d 2027             t = '
+00018b90: 3c68 3120 6964 3d22 7022 3e34 3033 2066  <h1 id="p">403 f
+00018ba0: 6f72 6269 6464 656e 6120 266e 6273 703b  orbiddena &nbsp;
+00018bb0: 7ee2 94bb e294 81e2 94bb 3c2f 6831 3e3c  ~.........</h1><
+00018bc0: 7020 6964 3d22 7122 3e79 6f75 5c27 6c6c  p id="q">you\'ll
+00018bd0: 2068 6176 6520 746f 206c 6f67 2069 6e20   have to log in 
+00018be0: 6f72 203c 6120 6872 6566 3d22 7b7d 2f3f  or <a href="{}/?
+00018bf0: 6822 3e67 6f20 686f 6d65 3c2f 613e 3c2f  h">go home</a></
+00018c00: 703e 270a 2020 2020 2020 2020 2020 2020  p>'.            
+00018c10: 7263 203d 2034 3033 0a20 2020 2020 2020  rc = 403.       
+00018c20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00018c30: 2020 2074 203d 2027 3c68 3120 6964 3d22     t = '<h1 id="
+00018c40: 6e22 3e34 3034 206e 6f74 2066 6f75 6e64  n">404 not found
+00018c50: 2026 6e62 7370 3be2 9490 2820 c2b4 202d   &nbsp;...( .. -
+00018c60: 6029 e294 8c3c 2f68 313e 3c70 3e3c 6120  `)...</h1><p><a 
+00018c70: 6964 3d22 7222 2068 7265 663d 227b 7d2f  id="r" href="{}/
+00018c80: 3f68 223e 676f 2068 6f6d 653c 2f61 3e3c  ?h">go home</a><
+00018c90: 2f70 3e27 0a0a 2020 2020 2020 2020 7420  /p>'..        t 
+00018ca0: 3d20 742e 666f 726d 6174 2873 656c 662e  = t.format(self.
+00018cb0: 6172 6773 2e53 5229 0a20 2020 2020 2020  args.SR).       
+00018cc0: 2068 746d 6c20 3d20 7365 6c66 2e6a 3273   html = self.j2s
+00018cd0: 2822 7370 6c61 7368 222c 2074 6869 733d  ("splash", this=
+00018ce0: 7365 6c66 2c20 7176 7061 7468 3d71 756f  self, qvpath=quo
+00018cf0: 7465 7028 7365 6c66 2e76 7061 7468 292c  tep(self.vpath),
+00018d00: 206d 7367 3d74 290a 2020 2020 2020 2020   msg=t).        
+00018d10: 7365 6c66 2e72 6570 6c79 2868 746d 6c2e  self.reply(html.
+00018d20: 656e 636f 6465 2822 7574 662d 3822 292c  encode("utf-8"),
+00018d30: 2073 7461 7475 733d 7263 290a 2020 2020   status=rc).    
+00018d40: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00018d50: 0a20 2020 2064 6566 206f 6e34 3078 2873  .    def on40x(s
+00018d60: 656c 662c 206d 6f64 7320 2c20 766e 202c  elf, mods , vn ,
+00018d70: 2072 656d 2029 2020 3a0a 2020 2020 2020   rem )  :.      
+00018d80: 2020 666f 7220 6d70 6174 6820 696e 206d    for mpath in m
+00018d90: 6f64 733a 0a20 2020 2020 2020 2020 2020  ods:.           
+00018da0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00018db0: 2020 2020 2020 6d6f 6420 3d20 6c6f 6164        mod = load
+00018dc0: 7079 286d 7061 7468 2c20 7365 6c66 2e61  py(mpath, self.a
+00018dd0: 7267 732e 686f 745f 6861 6e64 6c65 7273  rgs.hot_handlers
+00018de0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+00018df0: 6365 7074 2045 7863 6570 7469 6f6e 2061  cept Exception a
+00018e00: 7320 6578 3a0a 2020 2020 2020 2020 2020  s ex:.          
+00018e10: 2020 2020 2020 7365 6c66 2e6c 6f67 2822        self.log("
+00018e20: 696d 706f 7274 2066 6169 6c65 643a 207b  import failed: {
+00018e30: 2172 7d22 2e66 6f72 6d61 7428 6578 2929  !r}".format(ex))
+00018e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018e50: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+00018e60: 2020 2020 2020 2072 6574 203d 206d 6f64         ret = mod
+00018e70: 2e6d 6169 6e28 7365 6c66 2c20 766e 2c20  .main(self, vn, 
+00018e80: 7265 6d29 0a20 2020 2020 2020 2020 2020  rem).           
+00018e90: 2069 6620 7265 743a 0a20 2020 2020 2020   if ret:.       
+00018ea0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00018eb0: 7265 742e 6c6f 7765 7228 290a 0a20 2020  ret.lower()..   
+00018ec0: 2020 2020 2072 6574 7572 6e20 2222 2020       return ""  
+00018ed0: 2320 756e 6861 6e64 6c65 6420 2f20 6661  # unhandled / fa
+00018ee0: 6c6c 7468 726f 7567 680a 0a20 2020 2064  llthrough..    d
+00018ef0: 6566 2073 6361 6e76 6f6c 2873 656c 6629  ef scanvol(self)
+00018f00: 2020 3a0a 2020 2020 2020 2020 6966 206e    :.        if n
+00018f10: 6f74 2073 656c 662e 6361 6e5f 6164 6d69  ot self.can_admi
+00018f20: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
+00018f30: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
+00018f40: 2022 6e6f 7420 616c 6c6f 7765 6420 666f   "not allowed fo
+00018f50: 7220 7573 6572 2022 202b 2073 656c 662e  r user " + self.
+00018f60: 756e 616d 6529 0a0a 2020 2020 2020 2020  uname)..        
+00018f70: 6966 2073 656c 662e 6172 6773 2e6e 6f5f  if self.args.no_
+00018f80: 7265 7363 616e 3a0a 2020 2020 2020 2020  rescan:.        
+00018f90: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
+00018fa0: 2834 3033 2c20 2274 6865 2072 6573 6361  (403, "the resca
+00018fb0: 6e20 6665 6174 7572 6520 6973 2064 6973  n feature is dis
+00018fc0: 6162 6c65 6420 696e 2073 6572 7665 7220  abled in server 
+00018fd0: 636f 6e66 6967 2229 0a0a 2020 2020 2020  config")..      
+00018fe0: 2020 766e 2c20 5f20 3d20 7365 6c66 2e61    vn, _ = self.a
+00018ff0: 7372 762e 7666 732e 6765 7428 7365 6c66  srv.vfs.get(self
+00019000: 2e76 7061 7468 2c20 7365 6c66 2e75 6e61  .vpath, self.una
+00019010: 6d65 2c20 5472 7565 2c20 5472 7565 290a  me, True, True).
+00019020: 0a20 2020 2020 2020 2061 7267 7320 3d20  .        args = 
+00019030: 5b73 656c 662e 6173 7276 2e76 6673 2e61  [self.asrv.vfs.a
+00019040: 6c6c 5f76 6f6c 732c 205b 766e 2e76 7061  ll_vols, [vn.vpa
+00019050: 7468 5d2c 2046 616c 7365 2c20 5472 7565  th], False, True
+00019060: 5d0a 0a20 2020 2020 2020 2078 203d 2073  ]..        x = s
+00019070: 656c 662e 636f 6e6e 2e68 7372 762e 6272  elf.conn.hsrv.br
+00019080: 6f6b 6572 2e61 736b 2822 7570 326b 2e72  oker.ask("up2k.r
+00019090: 6573 6361 6e22 2c20 2a61 7267 7329 0a20  escan", *args). 
+000190a0: 2020 2020 2020 2065 7272 203d 2078 2e67         err = x.g
+000190b0: 6574 2829 0a20 2020 2020 2020 2069 6620  et().        if 
+000190c0: 6e6f 7420 6572 723a 0a20 2020 2020 2020  not err:.       
+000190d0: 2020 2020 2073 656c 662e 7265 6469 7265       self.redire
+000190e0: 6374 2822 222c 2022 3f68 2229 0a20 2020  ct("", "?h").   
+000190f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00019100: 5472 7565 0a0a 2020 2020 2020 2020 7261  True..        ra
+00019110: 6973 6520 5065 626b 6163 2835 3030 2c20  ise Pebkac(500, 
+00019120: 6572 7229 0a0a 2020 2020 6465 6620 6861  err)..    def ha
+00019130: 6e64 6c65 5f72 656c 6f61 6428 7365 6c66  ndle_reload(self
+00019140: 2920 203a 0a20 2020 2020 2020 2061 6374  )  :.        act
+00019150: 203d 2073 656c 662e 7570 6172 616d 2e67   = self.uparam.g
+00019160: 6574 2822 7265 6c6f 6164 2229 0a20 2020  et("reload").   
+00019170: 2020 2020 2069 6620 6163 7420 213d 2022       if act != "
+00019180: 6366 6722 3a0a 2020 2020 2020 2020 2020  cfg":.          
+00019190: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
+000191a0: 3030 2c20 226f 6e6c 7920 636f 6e66 6967  00, "only config
+000191b0: 2066 696c 6573 2028 2763 6667 2729 2063   files ('cfg') c
+000191c0: 616e 2062 6520 7265 6c6f 6164 6564 2072  an be reloaded r
+000191d0: 6e22 290a 0a20 2020 2020 2020 2069 6620  n")..        if 
+000191e0: 6e6f 7420 7365 6c66 2e61 766f 6c3a 0a20  not self.avol:. 
+000191f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00019200: 2050 6562 6b61 6328 3430 332c 2022 6e6f   Pebkac(403, "no
+00019210: 7420 616c 6c6f 7765 6420 666f 7220 7573  t allowed for us
+00019220: 6572 2022 202b 2073 656c 662e 756e 616d  er " + self.unam
+00019230: 6529 0a0a 2020 2020 2020 2020 6966 2073  e)..        if s
+00019240: 656c 662e 6172 6773 2e6e 6f5f 7265 6c6f  elf.args.no_relo
+00019250: 6164 3a0a 2020 2020 2020 2020 2020 2020  ad:.            
+00019260: 7261 6973 6520 5065 626b 6163 2834 3033  raise Pebkac(403
+00019270: 2c20 2274 6865 2072 656c 6f61 6420 6665  , "the reload fe
+00019280: 6174 7572 6520 6973 2064 6973 6162 6c65  ature is disable
+00019290: 6420 696e 2073 6572 7665 7220 636f 6e66  d in server conf
+000192a0: 6967 2229 0a0a 2020 2020 2020 2020 7820  ig")..        x 
+000192b0: 3d20 7365 6c66 2e63 6f6e 6e2e 6873 7276  = self.conn.hsrv
+000192c0: 2e62 726f 6b65 722e 6173 6b28 2272 656c  .broker.ask("rel
+000192d0: 6f61 6422 290a 2020 2020 2020 2020 7265  oad").        re
+000192e0: 7475 726e 2073 656c 662e 7265 6469 7265  turn self.redire
+000192f0: 6374 2822 222c 2022 3f68 222c 2078 2e67  ct("", "?h", x.g
+00019300: 6574 2829 2c20 2272 6574 7572 6e20 746f  et(), "return to
+00019310: 222c 2046 616c 7365 290a 0a20 2020 2064  ", False)..    d
+00019320: 6566 2074 785f 7374 6163 6b28 7365 6c66  ef tx_stack(self
+00019330: 2920 203a 0a20 2020 2020 2020 2069 6620  )  :.        if 
+00019340: 6e6f 7420 7365 6c66 2e61 766f 6c20 616e  not self.avol an
+00019350: 6420 6e6f 7420 5b78 2066 6f72 2078 2069  d not [x for x i
+00019360: 6e20 7365 6c66 2e77 766f 6c20 6966 2078  n self.wvol if x
+00019370: 2069 6e20 7365 6c66 2e72 766f 6c5d 3a0a   in self.rvol]:.
+00019380: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00019390: 6520 5065 626b 6163 2834 3033 2c20 226e  e Pebkac(403, "n
+000193a0: 6f74 2061 6c6c 6f77 6564 2066 6f72 2075  ot allowed for u
+000193b0: 7365 7220 2220 2b20 7365 6c66 2e75 6e61  ser " + self.una
+000193c0: 6d65 290a 0a20 2020 2020 2020 2069 6620  me)..        if 
+000193d0: 7365 6c66 2e61 7267 732e 6e6f 5f73 7461  self.args.no_sta
+000193e0: 636b 3a0a 2020 2020 2020 2020 2020 2020  ck:.            
+000193f0: 7261 6973 6520 5065 626b 6163 2834 3033  raise Pebkac(403
+00019400: 2c20 2274 6865 2073 7461 636b 6475 6d70  , "the stackdump
+00019410: 2066 6561 7475 7265 2069 7320 6469 7361   feature is disa
+00019420: 626c 6564 2069 6e20 7365 7276 6572 2063  bled in server c
+00019430: 6f6e 6669 6722 290a 0a20 2020 2020 2020  onfig")..       
+00019440: 2072 6574 203d 2022 3c70 7265 3e7b 7d5c   ret = "<pre>{}\
+00019450: 6e7b 7d22 2e66 6f72 6d61 7428 7469 6d65  n{}".format(time
+00019460: 2e74 696d 6528 292c 2068 746d 6c5f 6573  .time(), html_es
+00019470: 6361 7065 2861 6c6c 7472 6163 6528 2929  cape(alltrace())
+00019480: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+00019490: 6570 6c79 2872 6574 2e65 6e63 6f64 6528  eply(ret.encode(
+000194a0: 2275 7466 2d38 2229 290a 2020 2020 2020  "utf-8")).      
+000194b0: 2020 7265 7475 726e 2054 7275 650a 0a20    return True.. 
+000194c0: 2020 2064 6566 2074 785f 7472 6565 2873     def tx_tree(s
+000194d0: 656c 6629 2020 3a0a 2020 2020 2020 2020  elf)  :.        
+000194e0: 746f 7020 3d20 7365 6c66 2e75 7061 7261  top = self.upara
+000194f0: 6d5b 2274 7265 6522 5d20 6f72 2022 220a  m["tree"] or "".
+00019500: 2020 2020 2020 2020 6473 7420 3d20 7365          dst = se
+00019510: 6c66 2e76 7061 7468 0a20 2020 2020 2020  lf.vpath.       
+00019520: 2069 6620 746f 7020 696e 205b 222e 222c   if top in [".",
+00019530: 2022 2e2e 225d 3a0a 2020 2020 2020 2020   ".."]:.        
+00019540: 2020 2020 746f 7020 3d20 756e 646f 7428      top = undot(
+00019550: 7365 6c66 2e76 7061 7468 202b 2022 2f22  self.vpath + "/"
+00019560: 202b 2074 6f70 290a 0a20 2020 2020 2020   + top)..       
+00019570: 2069 6620 746f 7020 3d3d 2064 7374 3a0a   if top == dst:.
+00019580: 2020 2020 2020 2020 2020 2020 6473 7420              dst 
+00019590: 3d20 2222 0a20 2020 2020 2020 2065 6c69  = "".        eli
+000195a0: 6620 746f 703a 0a20 2020 2020 2020 2020  f top:.         
+000195b0: 2020 2069 6620 6e6f 7420 6473 742e 7374     if not dst.st
+000195c0: 6172 7473 7769 7468 2874 6f70 202b 2022  artswith(top + "
+000195d0: 2f22 293a 0a20 2020 2020 2020 2020 2020  /"):.           
+000195e0: 2020 2020 2072 6169 7365 2050 6562 6b61       raise Pebka
+000195f0: 6328 3430 302c 2022 6172 6720 6675 6e6b  c(400, "arg funk
+00019600: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+00019610: 6473 7420 3d20 6473 745b 6c65 6e28 746f  dst = dst[len(to
+00019620: 7029 202b 2031 203a 5d0a 0a20 2020 2020  p) + 1 :]..     
+00019630: 2020 2072 6574 203d 2073 656c 662e 6765     ret = self.ge
+00019640: 6e5f 7472 6565 2874 6f70 2c20 6473 7429  n_tree(top, dst)
+00019650: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00019660: 2e69 735f 7670 726f 7869 6564 3a0a 2020  .is_vproxied:.  
+00019670: 2020 2020 2020 2020 2020 7061 7265 6e74            parent
+00019680: 7320 3d20 7365 6c66 2e61 7267 732e 522e  s = self.args.R.
+00019690: 7370 6c69 7428 222f 2229 0a20 2020 2020  split("/").     
+000196a0: 2020 2020 2020 2066 6f72 2070 6172 656e         for paren
+000196b0: 7420 696e 2072 6576 6572 7365 6428 7061  t in reversed(pa
+000196c0: 7265 6e74 7329 3a0a 2020 2020 2020 2020  rents):.        
+000196d0: 2020 2020 2020 2020 7265 7420 3d20 7b22          ret = {"
+000196e0: 6b25 7322 2025 2028 7061 7265 6e74 2c29  k%s" % (parent,)
+000196f0: 3a20 7265 742c 2022 6122 3a20 5b5d 7d0a  : ret, "a": []}.
+00019700: 0a20 2020 2020 2020 207a 7320 3d20 6a73  .        zs = js
+00019710: 6f6e 2e64 756d 7073 2872 6574 290a 2020  on.dumps(ret).  
+00019720: 2020 2020 2020 7365 6c66 2e72 6570 6c79        self.reply
+00019730: 287a 732e 656e 636f 6465 2822 7574 662d  (zs.encode("utf-
+00019740: 3822 292c 206d 696d 653d 2261 7070 6c69  8"), mime="appli
+00019750: 6361 7469 6f6e 2f6a 736f 6e22 290a 2020  cation/json").  
+00019760: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00019770: 650a 0a20 2020 2064 6566 2067 656e 5f74  e..    def gen_t
+00019780: 7265 6528 7365 6c66 2c20 746f 7020 2c20  ree(self, top , 
+00019790: 7461 7267 6574 2029 2020 203a 0a20 2020  target )   :.   
+000197a0: 2020 2020 2072 6574 2020 203d 207b 7d0a       ret   = {}.
+000197b0: 2020 2020 2020 2020 6578 636c 203d 204e          excl = N
+000197c0: 6f6e 650a 2020 2020 2020 2020 6966 2074  one.        if t
+000197d0: 6172 6765 743a 0a20 2020 2020 2020 2020  arget:.         
+000197e0: 2020 2065 7863 6c2c 2074 6172 6765 7420     excl, target 
+000197f0: 3d20 2874 6172 6765 742e 7370 6c69 7428  = (target.split(
+00019800: 222f 222c 2031 2920 2b20 5b22 225d 295b  "/", 1) + [""])[
+00019810: 3a32 5d0a 2020 2020 2020 2020 2020 2020  :2].            
+00019820: 7375 6220 3d20 7365 6c66 2e67 656e 5f74  sub = self.gen_t
+00019830: 7265 6528 222f 222e 6a6f 696e 285b 746f  ree("/".join([to
+00019840: 702c 2065 7863 6c5d 292e 7374 7269 7028  p, excl]).strip(
+00019850: 222f 2229 2c20 7461 7267 6574 290a 2020  "/"), target).  
+00019860: 2020 2020 2020 2020 2020 7265 745b 226b            ret["k
+00019870: 2220 2b20 7175 6f74 6570 2865 7863 6c29  " + quotep(excl)
+00019880: 5d20 3d20 7375 620a 0a20 2020 2020 2020  ] = sub..       
+00019890: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000198a0: 2020 766e 2c20 7265 6d20 3d20 7365 6c66    vn, rem = self
+000198b0: 2e61 7372 762e 7666 732e 6765 7428 746f  .asrv.vfs.get(to
+000198c0: 702c 2073 656c 662e 756e 616d 652c 2054  p, self.uname, T
+000198d0: 7275 652c 2046 616c 7365 290a 2020 2020  rue, False).    
+000198e0: 2020 2020 2020 2020 6673 726f 6f74 2c20          fsroot, 
+000198f0: 7666 735f 6c73 2c20 7666 735f 7669 7274  vfs_ls, vfs_virt
+00019900: 203d 2076 6e2e 6c73 280a 2020 2020 2020   = vn.ls(.      
+00019910: 2020 2020 2020 2020 2020 7265 6d2c 0a20            rem,. 
+00019920: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019930: 656c 662e 756e 616d 652c 0a20 2020 2020  elf.uname,.     
+00019940: 2020 2020 2020 2020 2020 206e 6f74 2073             not s
+00019950: 656c 662e 6172 6773 2e6e 6f5f 7363 616e  elf.args.no_scan
+00019960: 6469 722c 0a20 2020 2020 2020 2020 2020  dir,.           
+00019970: 2020 2020 205b 5b54 7275 652c 2046 616c       [[True, Fal
+00019980: 7365 5d2c 205b 4661 6c73 652c 2054 7275  se], [False, Tru
+00019990: 655d 5d2c 0a20 2020 2020 2020 2020 2020  e]],.           
+000199a0: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
+000199b0: 743a 0a20 2020 2020 2020 2020 2020 2076  t:.            v
+000199c0: 6673 5f6c 7320 3d20 5b5d 0a20 2020 2020  fs_ls = [].     
+000199d0: 2020 2020 2020 2076 6673 5f76 6972 7420         vfs_virt 
+000199e0: 3d20 7b7d 0a20 2020 2020 2020 2020 2020  = {}.           
+000199f0: 2066 6f72 2076 2069 6e20 7365 6c66 2e72   for v in self.r
+00019a00: 766f 6c3a 0a20 2020 2020 2020 2020 2020  vol:.           
+00019a10: 2020 2020 2064 312c 2064 3220 3d20 762e       d1, d2 = v.
+00019a20: 7273 706c 6974 2822 2f22 2c20 3129 2069  rsplit("/", 1) i
+00019a30: 6620 222f 2220 696e 2076 2065 6c73 6520  f "/" in v else 
+00019a40: 5b22 222c 2076 5d0a 2020 2020 2020 2020  ["", v].        
+00019a50: 2020 2020 2020 2020 6966 2064 3120 3d3d          if d1 ==
+00019a60: 2074 6f70 3a0a 2020 2020 2020 2020 2020   top:.          
+00019a70: 2020 2020 2020 2020 2020 7666 735f 7669            vfs_vi
+00019a80: 7274 5b64 325d 203d 2073 656c 662e 6173  rt[d2] = self.as
+00019a90: 7276 2e76 6673 2020 2320 7479 7065 6368  rv.vfs  # typech
+00019aa0: 6b2c 2076 616c 7565 206e 6576 6572 2072  k, value never r
+00019ab0: 6561 640a 0a20 2020 2020 2020 2064 6972  ead..        dir
+00019ac0: 7320 3d20 5b5d 0a0a 2020 2020 2020 2020  s = []..        
+00019ad0: 6469 726e 616d 6573 203d 205b 785b 305d  dirnames = [x[0]
+00019ae0: 2066 6f72 2078 2069 6e20 7666 735f 6c73   for x in vfs_ls
+00019af0: 2069 6620 7374 6174 2e53 5f49 5344 4952   if stat.S_ISDIR
+00019b00: 2878 5b31 5d2e 7374 5f6d 6f64 6529 5d0a  (x[1].st_mode)].
+00019b10: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00019b20: 7365 6c66 2e61 7267 732e 6564 206f 7220  self.args.ed or 
+00019b30: 2264 6f74 7322 206e 6f74 2069 6e20 7365  "dots" not in se
+00019b40: 6c66 2e75 7061 7261 6d3a 0a20 2020 2020  lf.uparam:.     
+00019b50: 2020 2020 2020 2064 6972 6e61 6d65 7320         dirnames 
+00019b60: 3d20 6578 636c 7564 655f 646f 7466 696c  = exclude_dotfil
+00019b70: 6573 2864 6972 6e61 6d65 7329 0a0a 2020  es(dirnames)..  
+00019b80: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+00019b90: 5b78 2066 6f72 2078 2069 6e20 6469 726e  [x for x in dirn
+00019ba0: 616d 6573 2069 6620 7820 213d 2065 7863  ames if x != exc
+00019bb0: 6c5d 3a0a 2020 2020 2020 2020 2020 2020  l]:.            
+00019bc0: 6469 7273 2e61 7070 656e 6428 7175 6f74  dirs.append(quot
+00019bd0: 6570 2866 6e29 290a 0a20 2020 2020 2020  ep(fn))..       
+00019be0: 2066 6f72 2078 2069 6e20 7666 735f 7669   for x in vfs_vi
+00019bf0: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
+00019c00: 6966 2078 2021 3d20 6578 636c 3a0a 2020  if x != excl:.  
+00019c10: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00019c20: 7273 2e61 7070 656e 6428 7829 0a0a 2020  rs.append(x)..  
+00019c30: 2020 2020 2020 7265 745b 2261 225d 203d        ret["a"] =
+00019c40: 2064 6972 730a 2020 2020 2020 2020 7265   dirs.        re
+00019c50: 7475 726e 2072 6574 0a0a 2020 2020 6465  turn ret..    de
+00019c60: 6620 7478 5f75 7073 2873 656c 6629 2020  f tx_ups(self)  
+00019c70: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00019c80: 2073 656c 662e 6172 6773 2e75 6e70 6f73   self.args.unpos
+00019c90: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00019ca0: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
+00019cb0: 2022 7468 6520 756e 706f 7374 2066 6561   "the unpost fea
+00019cc0: 7475 7265 2069 7320 6469 7361 626c 6564  ture is disabled
+00019cd0: 2069 6e20 7365 7276 6572 2063 6f6e 6669   in server confi
+00019ce0: 6722 290a 0a20 2020 2020 2020 2069 6478  g")..        idx
+00019cf0: 203d 2073 656c 662e 636f 6e6e 2e67 6574   = self.conn.get
+00019d00: 5f75 3269 6478 2829 0a20 2020 2020 2020  _u2idx().       
+00019d10: 2069 6620 6e6f 7420 6964 7820 6f72 206e   if not idx or n
+00019d20: 6f74 2068 6173 6174 7472 2869 6478 2c20  ot hasattr(idx, 
+00019d30: 2270 5f65 6e64 2229 3a0a 2020 2020 2020  "p_end"):.      
+00019d40: 2020 2020 2020 7261 6973 6520 5065 626b        raise Pebk
+00019d50: 6163 2835 3030 2c20 2273 716c 6974 6533  ac(500, "sqlite3
+00019d60: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
+00019d70: 6520 6f6e 2074 6865 2073 6572 7665 723b  e on the server;
+00019d80: 2063 616e 6e6f 7420 756e 706f 7374 2229   cannot unpost")
+00019d90: 0a0a 2020 2020 2020 2020 6669 6c74 203d  ..        filt =
+00019da0: 2073 656c 662e 7570 6172 616d 2e67 6574   self.uparam.get
+00019db0: 2822 6669 6c74 6572 2229 0a20 2020 2020  ("filter").     
+00019dc0: 2020 2066 696c 7420 3d20 756e 7175 6f74     filt = unquot
+00019dd0: 6570 2866 696c 7420 6f72 2022 2229 0a20  ep(filt or ""). 
+00019de0: 2020 2020 2020 206c 6d20 3d20 2275 7073         lm = "ups
+00019df0: 205b 7b7d 5d22 2e66 6f72 6d61 7428 6669   [{}]".format(fi
+00019e00: 6c74 290a 2020 2020 2020 2020 7365 6c66  lt).        self
+00019e10: 2e6c 6f67 286c 6d29 0a0a 2020 2020 2020  .log(lm)..      
+00019e20: 2020 7265 7420 2020 3d20 5b5d 0a20 2020    ret   = [].   
+00019e30: 2020 2020 2074 3020 3d20 7469 6d65 2e74       t0 = time.t
+00019e40: 696d 6528 290a 2020 2020 2020 2020 6c69  ime().        li
+00019e50: 6d20 3d20 7469 6d65 2e74 696d 6528 2920  m = time.time() 
+00019e60: 2d20 7365 6c66 2e61 7267 732e 756e 706f  - self.args.unpo
+00019e70: 7374 0a20 2020 2020 2020 2066 6b5f 766f  st.        fk_vo
+00019e80: 6c73 203d 207b 0a20 2020 2020 2020 2020  ls = {.         
+00019e90: 2020 2076 6f6c 3a20 766f 6c2e 666c 6167     vol: vol.flag
+00019ea0: 735b 2266 6b22 5d0a 2020 2020 2020 2020  s["fk"].        
+00019eb0: 2020 2020 666f 7220 7670 2c20 766f 6c20      for vp, vol 
+00019ec0: 696e 2073 656c 662e 6173 7276 2e76 6673  in self.asrv.vfs
+00019ed0: 2e61 6c6c 5f76 6f6c 732e 6974 656d 7328  .all_vols.items(
+00019ee0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00019ef0: 2022 666b 2220 696e 2076 6f6c 2e66 6c61   "fk" in vol.fla
+00019f00: 6773 2061 6e64 2028 7670 2069 6e20 7365  gs and (vp in se
+00019f10: 6c66 2e72 766f 6c20 6f72 2076 7020 696e  lf.rvol or vp in
+00019f20: 2073 656c 662e 7570 766f 6c29 0a20 2020   self.upvol).   
+00019f30: 2020 2020 207d 0a20 2020 2020 2020 2066       }.        f
+00019f40: 6f72 2076 6f6c 2069 6e20 7365 6c66 2e61  or vol in self.a
+00019f50: 7372 762e 7666 732e 616c 6c5f 766f 6c73  srv.vfs.all_vols
+00019f60: 2e76 616c 7565 7328 293a 0a20 2020 2020  .values():.     
+00019f70: 2020 2020 2020 2063 7572 203d 2069 6478         cur = idx
+00019f80: 2e67 6574 5f63 7572 2876 6f6c 2e72 6561  .get_cur(vol.rea
+00019f90: 6c70 6174 6829 0a20 2020 2020 2020 2020  lpath).         
+00019fa0: 2020 2069 6620 6e6f 7420 6375 723a 0a20     if not cur:. 
+00019fb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00019fc0: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+00019fd0: 2020 2020 206e 666b 203d 2066 6b5f 766f       nfk = fk_vo
+00019fe0: 6c73 2e67 6574 2876 6f6c 2c20 3029 0a0a  ls.get(vol, 0)..
+00019ff0: 2020 2020 2020 2020 2020 2020 7120 3d20              q = 
+0001a000: 2273 656c 6563 7420 737a 2c20 7264 2c20  "select sz, rd, 
+0001a010: 666e 2c20 6174 2066 726f 6d20 7570 2077  fn, at from up w
+0001a020: 6865 7265 2069 703d 3f20 616e 6420 6174  here ip=? and at
+0001a030: 3e3f 220a 2020 2020 2020 2020 2020 2020  >?".            
+0001a040: 666f 7220 737a 2c20 7264 2c20 666e 2c20  for sz, rd, fn, 
+0001a050: 6174 2069 6e20 6375 722e 6578 6563 7574  at in cur.execut
+0001a060: 6528 712c 2028 7365 6c66 2e69 702c 206c  e(q, (self.ip, l
+0001a070: 696d 2929 3a0a 2020 2020 2020 2020 2020  im)):.          
+0001a080: 2020 2020 2020 7670 203d 2022 2f22 202b        vp = "/" +
+0001a090: 2022 2f22 2e6a 6f69 6e28 7820 666f 7220   "/".join(x for 
+0001a0a0: 7820 696e 205b 766f 6c2e 7670 6174 682c  x in [vol.vpath,
+0001a0b0: 2072 642c 2066 6e5d 2069 6620 7829 0a20   rd, fn] if x). 
+0001a0c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a0d0: 6620 6669 6c74 2061 6e64 2066 696c 7420  f filt and filt 
+0001a0e0: 6e6f 7420 696e 2076 703a 0a20 2020 2020  not in vp:.     
+0001a0f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001a100: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+0001a110: 2020 2020 2020 2020 2072 7620 3d20 7b22           rv = {"
+0001a120: 7670 223a 2071 756f 7465 7028 7670 292c  vp": quotep(vp),
+0001a130: 2022 737a 223a 2073 7a2c 2022 6174 223a   "sz": sz, "at":
+0001a140: 2061 742c 2022 6e66 6b22 3a20 6e66 6b7d   at, "nfk": nfk}
+0001a150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a160: 2069 6620 6e66 6b3a 0a20 2020 2020 2020   if nfk:.       
+0001a170: 2020 2020 2020 2020 2020 2020 2072 765b               rv[
+0001a180: 2261 7022 5d20 3d20 766f 6c2e 6361 6e6f  "ap"] = vol.cano
+0001a190: 6e69 6361 6c28 766a 6f69 6e28 7264 2c20  nical(vjoin(rd, 
+0001a1a0: 666e 2929 0a0a 2020 2020 2020 2020 2020  fn))..          
+0001a1b0: 2020 2020 2020 7265 742e 6170 7065 6e64        ret.append
+0001a1c0: 2872 7629 0a20 2020 2020 2020 2020 2020  (rv).           
+0001a1d0: 2020 2020 2069 6620 6c65 6e28 7265 7429       if len(ret)
+0001a1e0: 203e 2033 3030 303a 0a20 2020 2020 2020   > 3000:.       
+0001a1f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0001a200: 2e73 6f72 7428 6b65 793d 6c61 6d62 6461  .sort(key=lambda
+0001a210: 2078 3a20 785b 2261 7422 5d2c 2072 6576   x: x["at"], rev
+0001a220: 6572 7365 3d54 7275 6529 2020 2320 7479  erse=True)  # ty
+0001a230: 7065 3a20 6967 6e6f 7265 0a20 2020 2020  pe: ignore.     
+0001a240: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001a250: 6574 203d 2072 6574 5b3a 3230 3030 5d0a  et = ret[:2000].
+0001a260: 0a20 2020 2020 2020 2072 6574 2e73 6f72  .        ret.sor
+0001a270: 7428 6b65 793d 6c61 6d62 6461 2078 3a20  t(key=lambda x: 
+0001a280: 785b 2261 7422 5d2c 2072 6576 6572 7365  x["at"], reverse
+0001a290: 3d54 7275 6529 2020 2320 7479 7065 3a20  =True)  # type: 
+0001a2a0: 6967 6e6f 7265 0a20 2020 2020 2020 206e  ignore.        n
+0001a2b0: 203d 2030 0a20 2020 2020 2020 2066 6f72   = 0.        for
+0001a2c0: 2072 7620 696e 2072 6574 5b3a 3131 3030   rv in ret[:1100
+0001a2d0: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
+0001a2e0: 6e66 6b20 3d20 7276 2e70 6f70 2822 6e66  nfk = rv.pop("nf
+0001a2f0: 6b22 290a 2020 2020 2020 2020 2020 2020  k").            
+0001a300: 6966 206e 6f74 206e 666b 3a0a 2020 2020  if not nfk:.    
+0001a310: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0001a320: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+0001a330: 2020 6170 203d 2072 762e 706f 7028 2261    ap = rv.pop("a
+0001a340: 7022 290a 2020 2020 2020 2020 2020 2020  p").            
+0001a350: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0001a360: 2020 2020 2073 7420 3d20 626f 732e 7374       st = bos.st
+0001a370: 6174 2861 7029 0a20 2020 2020 2020 2020  at(ap).         
+0001a380: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+0001a390: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0001a3a0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+0001a3b0: 2066 6b20 3d20 7365 6c66 2e67 656e 5f66   fk = self.gen_f
+0001a3c0: 6b28 0a20 2020 2020 2020 2020 2020 2020  k(.             
+0001a3d0: 2020 2073 656c 662e 6172 6773 2e66 6b5f     self.args.fk_
+0001a3e0: 7361 6c74 2c20 6170 2c20 7374 2e73 745f  salt, ap, st.st_
+0001a3f0: 7369 7a65 2c20 3020 6966 2041 4e59 5749  size, 0 if ANYWI
+0001a400: 4e20 656c 7365 2073 742e 7374 5f69 6e6f  N else st.st_ino
+0001a410: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0001a420: 2020 2020 2020 2020 2020 2072 765b 2276             rv["v
+0001a430: 7022 5d20 2b3d 2022 3f6b 3d22 202b 2066  p"] += "?k=" + f
+0001a440: 6b5b 3a6e 666b 5d0a 0a20 2020 2020 2020  k[:nfk]..       
+0001a450: 2020 2020 206e 202b 3d20 310a 2020 2020       n += 1.    
+0001a460: 2020 2020 2020 2020 6966 206e 203e 2032          if n > 2
+0001a470: 3030 303a 0a20 2020 2020 2020 2020 2020  000:.           
+0001a480: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+0001a490: 2020 2020 7265 7420 3d20 7265 745b 3a32      ret = ret[:2
+0001a4a0: 3030 305d 0a0a 2020 2020 2020 2020 6966  000]..        if
+0001a4b0: 2073 656c 662e 6973 5f76 7072 6f78 6965   self.is_vproxie
+0001a4c0: 643a 0a20 2020 2020 2020 2020 2020 2066  d:.            f
+0001a4d0: 6f72 2076 2069 6e20 7265 743a 0a20 2020  or v in ret:.   
+0001a4e0: 2020 2020 2020 2020 2020 2020 2076 5b22               v["
+0001a4f0: 7670 225d 203d 2073 656c 662e 6172 6773  vp"] = self.args
+0001a500: 2e53 5220 2b20 765b 2276 7022 5d0a 0a20  .SR + v["vp"].. 
+0001a510: 2020 2020 2020 206a 7478 7420 3d20 6a73         jtxt = js
+0001a520: 6f6e 2e64 756d 7073 2872 6574 2c20 696e  on.dumps(ret, in
+0001a530: 6465 6e74 3d32 2c20 736f 7274 5f6b 6579  dent=2, sort_key
+0001a540: 733d 5472 7565 292e 656e 636f 6465 2822  s=True).encode("
+0001a550: 7574 662d 3822 2c20 2272 6570 6c61 6365  utf-8", "replace
+0001a560: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+0001a570: 6c6f 6728 227b 7d20 237b 7d20 7b3a 2e32  log("{} #{} {:.2
+0001a580: 667d 7365 6322 2e66 6f72 6d61 7428 6c6d  f}sec".format(lm
+0001a590: 2c20 6c65 6e28 7265 7429 2c20 7469 6d65  , len(ret), time
+0001a5a0: 2e74 696d 6528 2920 2d20 7430 2929 0a20  .time() - t0)). 
+0001a5b0: 2020 2020 2020 2073 656c 662e 7265 706c         self.repl
+0001a5c0: 7928 6a74 7874 2c20 6d69 6d65 3d22 6170  y(jtxt, mime="ap
+0001a5d0: 706c 6963 6174 696f 6e2f 6a73 6f6e 2229  plication/json")
+0001a5e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0001a5f0: 5472 7565 0a0a 2020 2020 6465 6620 6861  True..    def ha
+0001a600: 6e64 6c65 5f72 6d28 7365 6c66 2c20 7265  ndle_rm(self, re
+0001a610: 7120 2920 203a 0a20 2020 2020 2020 2069  q )  :.        i
+0001a620: 6620 6e6f 7420 7265 7120 616e 6420 6e6f  f not req and no
+0001a630: 7420 7365 6c66 2e63 616e 5f64 656c 6574  t self.can_delet
+0001a640: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0001a650: 6169 7365 2050 6562 6b61 6328 3430 332c  aise Pebkac(403,
+0001a660: 2022 6e6f 7420 616c 6c6f 7765 6420 666f   "not allowed fo
+0001a670: 7220 7573 6572 2022 202b 2073 656c 662e  r user " + self.
+0001a680: 756e 616d 6529 0a0a 2020 2020 2020 2020  uname)..        
+0001a690: 6966 2073 656c 662e 6172 6773 2e6e 6f5f  if self.args.no_
+0001a6a0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
+0001a6b0: 2072 6169 7365 2050 6562 6b61 6328 3430   raise Pebkac(40
+0001a6c0: 332c 2022 7468 6520 6465 6c65 7465 2066  3, "the delete f
+0001a6d0: 6561 7475 7265 2069 7320 6469 7361 626c  eature is disabl
+0001a6e0: 6564 2069 6e20 7365 7276 6572 2063 6f6e  ed in server con
+0001a6f0: 6669 6722 290a 0a20 2020 2020 2020 2069  fig")..        i
+0001a700: 6620 6e6f 7420 7265 713a 0a20 2020 2020  f not req:.     
+0001a710: 2020 2020 2020 2072 6571 203d 205b 7365         req = [se
+0001a720: 6c66 2e76 7061 7468 5d0a 2020 2020 2020  lf.vpath].      
+0001a730: 2020 656c 6966 2073 656c 662e 6973 5f76    elif self.is_v
+0001a740: 7072 6f78 6965 643a 0a20 2020 2020 2020  proxied:.       
+0001a750: 2020 2020 2072 6571 203d 205b 785b 6c65       req = [x[le
+0001a760: 6e28 7365 6c66 2e61 7267 732e 5352 2920  n(self.args.SR) 
+0001a770: 3a5d 2066 6f72 2078 2069 6e20 7265 715d  :] for x in req]
+0001a780: 0a0a 2020 2020 2020 2020 6e6c 696d 203d  ..        nlim =
+0001a790: 2069 6e74 2873 656c 662e 7570 6172 616d   int(self.uparam
+0001a7a0: 2e67 6574 2822 6c69 6d22 2920 6f72 2030  .get("lim") or 0
+0001a7b0: 290a 2020 2020 2020 2020 6c69 6d20 3d20  ).        lim = 
+0001a7c0: 5b6e 6c69 6d2c 206e 6c69 6d5d 2069 6620  [nlim, nlim] if 
+0001a7d0: 6e6c 696d 2065 6c73 6520 5b5d 0a0a 2020  nlim else []..  
+0001a7e0: 2020 2020 2020 7820 3d20 7365 6c66 2e63        x = self.c
+0001a7f0: 6f6e 6e2e 6873 7276 2e62 726f 6b65 722e  onn.hsrv.broker.
+0001a800: 6173 6b28 0a20 2020 2020 2020 2020 2020  ask(.           
+0001a810: 2022 7570 326b 2e68 616e 646c 655f 726d   "up2k.handle_rm
+0001a820: 222c 2073 656c 662e 756e 616d 652c 2073  ", self.uname, s
+0001a830: 656c 662e 6970 2c20 7265 712c 206c 696d  elf.ip, req, lim
+0001a840: 2c20 4661 6c73 650a 2020 2020 2020 2020  , False.        
+0001a850: 290a 2020 2020 2020 2020 7365 6c66 2e6c  ).        self.l
+0001a860: 6f75 645f 7265 706c 7928 782e 6765 7428  oud_reply(x.get(
+0001a870: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+0001a880: 6e20 5472 7565 0a0a 2020 2020 6465 6620  n True..    def 
+0001a890: 6861 6e64 6c65 5f6d 7628 7365 6c66 2920  handle_mv(self) 
+0001a8a0: 203a 0a20 2020 2020 2020 2023 2066 756c   :.        # ful
+0001a8b0: 6c20 7061 7468 206f 6620 6e65 7720 6c6f  l path of new lo
+0001a8c0: 6320 2869 6e63 6c20 6669 6c65 6e61 6d65  c (incl filename
+0001a8d0: 290a 2020 2020 2020 2020 6473 7420 3d20  ).        dst = 
+0001a8e0: 7365 6c66 2e75 7061 7261 6d2e 6765 7428  self.uparam.get(
+0001a8f0: 226d 6f76 6522 290a 0a20 2020 2020 2020  "move")..       
+0001a900: 2069 6620 7365 6c66 2e69 735f 7670 726f   if self.is_vpro
+0001a910: 7869 6564 2061 6e64 2064 7374 2061 6e64  xied and dst and
+0001a920: 2064 7374 2e73 7461 7274 7377 6974 6828   dst.startswith(
+0001a930: 7365 6c66 2e61 7267 732e 5352 293a 0a20  self.args.SR):. 
+0001a940: 2020 2020 2020 2020 2020 2064 7374 203d             dst =
+0001a950: 2064 7374 5b6c 656e 2873 656c 662e 6172   dst[len(self.ar
+0001a960: 6773 2e52 5329 203a 5d0a 0a20 2020 2020  gs.RS) :]..     
+0001a970: 2020 2069 6620 6e6f 7420 6473 743a 0a20     if not dst:. 
+0001a980: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0001a990: 2050 6562 6b61 6328 3430 302c 2022 6e65   Pebkac(400, "ne
+0001a9a0: 6564 2064 7374 2076 7061 7468 2229 0a0a  ed dst vpath")..
+0001a9b0: 2020 2020 2020 2020 2320 782d 7777 772d          # x-www-
+0001a9c0: 666f 726d 2d75 726c 656e 636f 6465 6420  form-urlencoded 
+0001a9d0: 2875 726c 2071 7565 7279 2070 6172 7429  (url query part)
+0001a9e0: 2075 7365 730a 2020 2020 2020 2020 2320   uses.        # 
+0001a9f0: 6569 7468 6572 202b 206f 7220 2532 3020  either + or %20 
+0001aa00: 666f 7220 3078 3230 2073 6f20 6861 6e64  for 0x20 so hand
+0001aa10: 6c65 2062 6f74 680a 2020 2020 2020 2020  le both.        
+0001aa20: 6473 7420 3d20 756e 7175 6f74 6570 2864  dst = unquotep(d
+0001aa30: 7374 2e72 6570 6c61 6365 2822 2b22 2c20  st.replace("+", 
+0001aa40: 2220 2229 290a 2020 2020 2020 2020 7265  " ")).        re
+0001aa50: 7475 726e 2073 656c 662e 5f6d 7628 7365  turn self._mv(se
+0001aa60: 6c66 2e76 7061 7468 2c20 6473 742e 6c73  lf.vpath, dst.ls
+0001aa70: 7472 6970 2822 2f22 2929 0a0a 2020 2020  trip("/"))..    
+0001aa80: 6465 6620 5f6d 7628 7365 6c66 2c20 7673  def _mv(self, vs
+0001aa90: 7263 202c 2076 6473 7420 2920 203a 0a20  rc , vdst )  :. 
+0001aaa0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0001aab0: 6c66 2e63 616e 5f6d 6f76 653a 0a20 2020  lf.can_move:.   
+0001aac0: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+0001aad0: 6562 6b61 6328 3430 332c 2022 6e6f 7420  ebkac(403, "not 
+0001aae0: 616c 6c6f 7765 6420 666f 7220 7573 6572  allowed for user
+0001aaf0: 2022 202b 2073 656c 662e 756e 616d 6529   " + self.uname)
+0001ab00: 0a0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0001ab10: 662e 6172 6773 2e6e 6f5f 6d76 3a0a 2020  f.args.no_mv:.  
+0001ab20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0001ab30: 5065 626b 6163 2834 3033 2c20 2274 6865  Pebkac(403, "the
+0001ab40: 2072 656e 616d 652f 6d6f 7665 2066 6561   rename/move fea
+0001ab50: 7475 7265 2069 7320 6469 7361 626c 6564  ture is disabled
+0001ab60: 2069 6e20 7365 7276 6572 2063 6f6e 6669   in server confi
+0001ab70: 6722 290a 0a20 2020 2020 2020 2078 203d  g")..        x =
+0001ab80: 2073 656c 662e 636f 6e6e 2e68 7372 762e   self.conn.hsrv.
+0001ab90: 6272 6f6b 6572 2e61 736b 2822 7570 326b  broker.ask("up2k
+0001aba0: 2e68 616e 646c 655f 6d76 222c 2073 656c  .handle_mv", sel
+0001abb0: 662e 756e 616d 652c 2076 7372 632c 2076  f.uname, vsrc, v
+0001abc0: 6473 7429 0a20 2020 2020 2020 2073 656c  dst).        sel
+0001abd0: 662e 6c6f 7564 5f72 6570 6c79 2878 2e67  f.loud_reply(x.g
+0001abe0: 6574 2829 2c20 7374 6174 7573 3d32 3031  et(), status=201
+0001abf0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001ac00: 2054 7275 650a 0a20 2020 2064 6566 2074   True..    def t
+0001ac10: 785f 6c73 2873 656c 662c 206c 7320 2029  x_ls(self, ls  )
+0001ac20: 2020 3a0a 2020 2020 2020 2020 6469 7273    :.        dirs
+0001ac30: 203d 206c 735b 2264 6972 7322 5d0a 2020   = ls["dirs"].  
+0001ac40: 2020 2020 2020 6669 6c65 7320 3d20 6c73        files = ls
+0001ac50: 5b22 6669 6c65 7322 5d0a 2020 2020 2020  ["files"].      
+0001ac60: 2020 6172 6720 3d20 7365 6c66 2e75 7061    arg = self.upa
+0001ac70: 7261 6d5b 226c 7322 5d0a 2020 2020 2020  ram["ls"].      
+0001ac80: 2020 6966 2061 7267 2069 6e20 5b22 7622    if arg in ["v"
+0001ac90: 2c20 2274 222c 2022 7478 7422 5d3a 0a20  , "t", "txt"]:. 
+0001aca0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+0001acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acc0: 6269 6767 6573 7420 3d20 6d61 7828 6c73  biggest = max(ls
+0001acd0: 5b22 6669 6c65 7322 5d20 2b20 6c73 5b22  ["files"] + ls["
+0001ace0: 6469 7273 225d 2c20 6b65 793d 6974 656d  dirs"], key=item
+0001acf0: 6765 7474 6572 2822 737a 2229 295b 2273  getter("sz"))["s
+0001ad00: 7a22 5d0a 2020 2020 2020 2020 2020 2020  z"].            
+0001ad10: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+0001ad20: 2020 2020 2020 2020 6269 6767 6573 7420          biggest 
+0001ad30: 3d20 300a 0a20 2020 2020 2020 2020 2020  = 0..           
+0001ad40: 2069 6620 6172 6720 3d3d 2022 7622 3a0a   if arg == "v":.
 0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad60: 2020 227b 7d7b 7b7d 7d22 2e66 6f72 6d61    "{}{{}}".forma
-0001ad70: 7428 7829 0a20 2020 2020 2020 2020 2020  t(x).           
-0001ad80: 2020 2020 2020 2020 2066 6f72 2078 2069           for x i
-0001ad90: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
-0001ada0: 2020 2020 2020 2020 2020 2020 225c 3033              "\03
-0001adb0: 335b 376d 222c 0a20 2020 2020 2020 2020  3[7m",.         
-0001adc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001add0: 5c30 3333 5b32 376d 222c 0a20 2020 2020  \033[27m",.     
-0001ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adf0: 2020 2022 222c 0a20 2020 2020 2020 2020     "",.         
-0001ae00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001ae10: 5c30 3333 5b30 3b31 6d22 2c0a 2020 2020  \033[0;1m",.    
-0001ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae30: 2020 2020 225c 3033 335b 303b 3336 6d22      "\033[0;36m"
-0001ae40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001ae50: 2020 2020 2020 2020 2020 225c 3033 335b            "\033[
-0001ae60: 306d 222c 0a20 2020 2020 2020 2020 2020  0m",.           
-0001ae70: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-0001ae80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0001ae90: 2020 2020 2020 2020 2020 2020 2063 7461               cta
-0001aea0: 6220 3d20 7b22 4222 3a20 362c 2022 4b22  b = {"B": 6, "K"
-0001aeb0: 3a20 352c 2022 4d22 3a20 312c 2022 4722  : 5, "M": 1, "G"
-0001aec0: 3a20 337d 0a20 2020 2020 2020 2020 2020  : 3}.           
-0001aed0: 2020 2020 2066 6f72 206c 7374 2069 6e20       for lst in 
-0001aee0: 5b64 6972 732c 2066 696c 6573 5d3a 0a20  [dirs, files]:. 
-0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af00: 2020 2066 6f72 2078 2069 6e20 6c73 743a     for x in lst:
-0001af10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001af20: 2020 2020 2020 2020 2061 203d 2078 5b22           a = x["
-0001af30: 6474 225d 2e72 6570 6c61 6365 2822 2d22  dt"].replace("-"
-0001af40: 2c20 2220 2229 2e72 6570 6c61 6365 2822  , " ").replace("
-0001af50: 3a22 2c20 2220 2229 2e73 706c 6974 2822  :", " ").split("
-0001af60: 2022 290a 2020 2020 2020 2020 2020 2020   ").            
-0001af70: 2020 2020 2020 2020 2020 2020 785b 2264              x["d
-0001af80: 7422 5d20 3d20 6632 2e66 6f72 6d61 7428  t"] = f2.format(
-0001af90: 2a6c 6973 7428 6129 290a 2020 2020 2020  *list(a)).      
-0001afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afb0: 2020 737a 203d 2068 756d 616e 7369 7a65    sz = humansize
-0001afc0: 2878 5b22 737a 225d 2c20 5472 7565 290a  (x["sz"], True).
-0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afe0: 2020 2020 2020 2020 785b 2273 7a22 5d20          x["sz"] 
-0001aff0: 3d20 225c 3033 335b 303b 337b 7d6d 207b  = "\033[0;3{}m {
-0001b000: 3a3e 357d 222e 666f 726d 6174 2863 7461  :>5}".format(cta
-0001b010: 622e 6765 7428 737a 5b2d 313a 5d2c 2030  b.get(sz[-1:], 0
-0001b020: 292c 2073 7a29 0a20 2020 2020 2020 2020  ), sz).         
-0001b030: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0001b040: 2020 2020 2020 2020 2066 6d74 203d 2022           fmt = "
-0001b050: 7b7b 7d7d 2020 7b7b 3a7b 7d2c 7d7d 2020  {{}}  {{:{},}}  
-0001b060: 7b7b 7d7d 220a 2020 2020 2020 2020 2020  {{}}".          
-0001b070: 2020 2020 2020 6e66 6d74 203d 2022 7b3a        nfmt = "{:
-0001b080: 2c7d 220a 0a20 2020 2020 2020 2020 2020  ,}"..           
-0001b090: 2066 6f72 2078 2069 6e20 6469 7273 3a0a   for x in dirs:.
-0001b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b0b0: 6e20 3d20 785b 226e 616d 6522 5d20 2b20  n = x["name"] + 
-0001b0c0: 222f 220a 2020 2020 2020 2020 2020 2020  "/".            
-0001b0d0: 2020 2020 6966 2061 7267 203d 3d20 2276      if arg == "v
-0001b0e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0001b0f0: 2020 2020 2020 206e 203d 2022 5c30 3333         n = "\033
-0001b100: 5b39 346d 2220 2b20 6e0a 0a20 2020 2020  [94m" + n..     
-0001b110: 2020 2020 2020 2020 2020 2078 5b22 6e61             x["na
-0001b120: 6d65 225d 203d 206e 0a0a 2020 2020 2020  me"] = n..      
-0001b130: 2020 2020 2020 666d 7420 3d20 666d 742e        fmt = fmt.
-0001b140: 666f 726d 6174 286c 656e 286e 666d 742e  format(len(nfmt.
-0001b150: 666f 726d 6174 2862 6967 6765 7374 2929  format(biggest))
-0001b160: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-0001b170: 746c 203d 205b 0a20 2020 2020 2020 2020  tl = [.         
-0001b180: 2020 2020 2020 2022 2320 7b7d 3a20 7b7d         "# {}: {}
-0001b190: 222e 666f 726d 6174 2878 2c20 6c73 5b78  ".format(x, ls[x
-0001b1a0: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
-0001b1b0: 2020 2066 6f72 2078 2069 6e20 5b22 6163     for x in ["ac
-0001b1c0: 6374 222c 2022 7065 726d 7322 2c20 2273  ct", "perms", "s
-0001b1d0: 7276 696e 6622 5d0a 2020 2020 2020 2020  rvinf"].        
-0001b1e0: 2020 2020 2020 2020 6966 2078 2069 6e20          if x in 
-0001b1f0: 6c73 0a20 2020 2020 2020 2020 2020 205d  ls.            ]
-0001b200: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0001b210: 6c20 2b3d 205b 0a20 2020 2020 2020 2020  l += [.         
-0001b220: 2020 2020 2020 2066 6d74 2e66 6f72 6d61         fmt.forma
-0001b230: 7428 785b 2264 7422 5d2c 2078 5b22 737a  t(x["dt"], x["sz
-0001b240: 225d 2c20 785b 226e 616d 6522 5d29 0a20  "], x["name"]). 
-0001b250: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001b260: 6f72 2079 2069 6e20 5b64 6972 732c 2066  or y in [dirs, f
-0001b270: 696c 6573 5d0a 2020 2020 2020 2020 2020  iles].          
-0001b280: 2020 2020 2020 666f 7220 7820 696e 2079        for x in y
-0001b290: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-0001b2a0: 2020 2020 2020 2020 2020 2072 6574 203d             ret =
-0001b2b0: 2022 5c6e 222e 6a6f 696e 2872 6574 6c29   "\n".join(retl)
-0001b2c0: 0a20 2020 2020 2020 2020 2020 206d 696d  .            mim
-0001b2d0: 6520 3d20 2274 6578 742f 706c 6169 6e3b  e = "text/plain;
-0001b2e0: 2063 6861 7273 6574 3d75 7466 2d38 220a   charset=utf-8".
-0001b2f0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001b300: 2020 2020 2020 2020 2020 5b78 2e70 6f70            [x.pop
-0001b310: 286b 2920 666f 7220 6b20 696e 205b 226e  (k) for k in ["n
-0001b320: 616d 6522 2c20 2264 7422 5d20 666f 7220  ame", "dt"] for 
-0001b330: 7920 696e 205b 6469 7273 2c20 6669 6c65  y in [dirs, file
-0001b340: 735d 2066 6f72 2078 2069 6e20 795d 0a0a  s] for x in y]..
-0001b350: 2020 2020 2020 2020 2020 2020 7265 7420              ret 
-0001b360: 3d20 6a73 6f6e 2e64 756d 7073 286c 7329  = json.dumps(ls)
-0001b370: 0a20 2020 2020 2020 2020 2020 206d 696d  .            mim
-0001b380: 6520 3d20 2261 7070 6c69 6361 7469 6f6e  e = "application
-0001b390: 2f6a 736f 6e22 0a0a 2020 2020 2020 2020  /json"..        
-0001b3a0: 7265 7420 2b3d 2022 5c6e 5c30 3333 5b30  ret += "\n\033[0
-0001b3b0: 6d22 2069 6620 6172 6720 3d3d 2022 7622  m" if arg == "v"
-0001b3c0: 2065 6c73 6520 225c 6e22 0a20 2020 2020   else "\n".     
-0001b3d0: 2020 2073 656c 662e 7265 706c 7928 7265     self.reply(re
-0001b3e0: 742e 656e 636f 6465 2822 7574 662d 3822  t.encode("utf-8"
-0001b3f0: 2c20 2272 6570 6c61 6365 2229 2c20 6d69  , "replace"), mi
-0001b400: 6d65 3d6d 696d 6529 0a20 2020 2020 2020  me=mime).       
-0001b410: 2072 6574 7572 6e20 5472 7565 0a0a 2020   return True..  
-0001b420: 2020 6465 6620 7478 5f62 726f 7773 6572    def tx_browser
-0001b430: 2873 656c 6629 2020 3a0a 2020 2020 2020  (self)  :.      
-0001b440: 2020 7670 6174 6820 3d20 2222 0a20 2020    vpath = "".   
-0001b450: 2020 2020 2076 706e 6f64 6573 203d 205b       vpnodes = [
-0001b460: 5b22 222c 2022 2f22 5d5d 0a20 2020 2020  ["", "/"]].     
-0001b470: 2020 2069 6620 7365 6c66 2e76 7061 7468     if self.vpath
-0001b480: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0001b490: 7220 6e6f 6465 2069 6e20 7365 6c66 2e76  r node in self.v
-0001b4a0: 7061 7468 2e73 706c 6974 2822 2f22 293a  path.split("/"):
-0001b4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b4c0: 2069 6620 6e6f 7420 7670 6174 683a 0a20   if not vpath:. 
-0001b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b4e0: 2020 2076 7061 7468 203d 206e 6f64 650a     vpath = node.
-0001b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b500: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001b510: 2020 2020 2020 2020 2020 7670 6174 6820            vpath 
-0001b520: 2b3d 2022 2f22 202b 206e 6f64 650a 0a20  += "/" + node.. 
-0001b530: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0001b540: 706e 6f64 6573 2e61 7070 656e 6428 5b71  pnodes.append([q
-0001b550: 756f 7465 7028 7670 6174 6829 202b 2022  uotep(vpath) + "
-0001b560: 2f22 2c20 6874 6d6c 5f65 7363 6170 6528  /", html_escape(
-0001b570: 6e6f 6465 2c20 6372 6c66 3d54 7275 6529  node, crlf=True)
-0001b580: 5d29 0a0a 2020 2020 2020 2020 766e 203d  ])..        vn =
-0001b590: 2073 656c 662e 766e 0a20 2020 2020 2020   self.vn.       
-0001b5a0: 2072 656d 203d 2073 656c 662e 7265 6d0a   rem = self.rem.
-0001b5b0: 2020 2020 2020 2020 6162 7370 6174 6820          abspath 
-0001b5c0: 3d20 766e 2e64 6361 6e6f 6e69 6361 6c28  = vn.dcanonical(
-0001b5d0: 7265 6d29 0a20 2020 2020 2020 2064 6276  rem).        dbv
-0001b5e0: 2c20 7672 656d 203d 2076 6e2e 6765 745f  , vrem = vn.get_
-0001b5f0: 6462 7628 7265 6d29 0a0a 2020 2020 2020  dbv(rem)..      
-0001b600: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0001b610: 2020 2073 7420 3d20 626f 732e 7374 6174     st = bos.stat
-0001b620: 2861 6273 7061 7468 290a 2020 2020 2020  (abspath).      
-0001b630: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-0001b640: 2020 2020 2020 6966 2022 6f6e 3430 3422        if "on404"
-0001b650: 206e 6f74 2069 6e20 766e 2e66 6c61 6773   not in vn.flags
-0001b660: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b670: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
-0001b680: 5f34 3034 2829 0a0a 2020 2020 2020 2020  _404()..        
-0001b690: 2020 2020 7265 7420 3d20 7365 6c66 2e6f      ret = self.o
-0001b6a0: 6e34 3078 2876 6e2e 666c 6167 735b 226f  n40x(vn.flags["o
-0001b6b0: 6e34 3034 225d 2c20 766e 2c20 7265 6d29  n404"], vn, rem)
-0001b6c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001b6d0: 7265 7420 3d3d 2022 7472 7565 223a 0a20  ret == "true":. 
-0001b6e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0001b6f0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-0001b700: 2020 2020 2020 2065 6c69 6620 7265 7420         elif ret 
-0001b710: 3d3d 2022 6661 6c73 6522 3a0a 2020 2020  == "false":.    
-0001b720: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001b730: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-0001b740: 2020 2020 2065 6c69 6620 7265 7420 3d3d       elif ret ==
-0001b750: 2022 7265 7472 7922 3a0a 2020 2020 2020   "retry":.      
-0001b760: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-0001b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b780: 2020 2073 7420 3d20 626f 732e 7374 6174     st = bos.stat
-0001b790: 2861 6273 7061 7468 290a 2020 2020 2020  (abspath).      
-0001b7a0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0001b7b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001b7c0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001b7d0: 662e 7478 5f34 3034 2829 0a20 2020 2020  f.tx_404().     
-0001b7e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001b7f0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001b800: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
-0001b810: 290a 0a20 2020 2020 2020 2069 6620 7265  )..        if re
-0001b820: 6d2e 7374 6172 7473 7769 7468 2822 2e68  m.startswith(".h
-0001b830: 6973 742f 7570 326b 2e22 2920 6f72 2028  ist/up2k.") or (
-0001b840: 0a20 2020 2020 2020 2020 2020 2072 656d  .            rem
-0001b850: 2e65 6e64 7377 6974 6828 222f 6469 722e  .endswith("/dir.
-0001b860: 7478 7422 2920 616e 6420 7265 6d2e 7374  txt") and rem.st
-0001b870: 6172 7473 7769 7468 2822 2e68 6973 742f  artswith(".hist/
-0001b880: 7468 2f22 290a 2020 2020 2020 2020 293a  th/").        ):
-0001b890: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-0001b8a0: 7365 2050 6562 6b61 6328 3430 3329 0a0a  se Pebkac(403)..
-0001b8b0: 2020 2020 2020 2020 6532 6420 3d20 2265          e2d = "e
-0001b8c0: 3264 2220 696e 2076 6e2e 666c 6167 730a  2d" in vn.flags.
-0001b8d0: 2020 2020 2020 2020 6532 7420 3d20 2265          e2t = "e
-0001b8e0: 3274 2220 696e 2076 6e2e 666c 6167 730a  2t" in vn.flags.
-0001b8f0: 0a20 2020 2020 2020 2073 656c 662e 6874  .        self.ht
-0001b900: 6d6c 5f68 6561 6420 3d20 766e 2e66 6c61  ml_head = vn.fla
-0001b910: 6773 2e67 6574 2822 6874 6d6c 5f68 6561  gs.get("html_hea
-0001b920: 6422 2c20 2222 290a 2020 2020 2020 2020  d", "").        
-0001b930: 6966 2076 6e2e 666c 6167 732e 6765 7428  if vn.flags.get(
-0001b940: 226e 6f72 6f62 6f74 7322 2920 6f72 2022  "norobots") or "
-0001b950: 6222 2069 6e20 7365 6c66 2e75 7061 7261  b" in self.upara
-0001b960: 6d3a 0a20 2020 2020 2020 2020 2020 2073  m:.            s
-0001b970: 656c 662e 6f75 745f 6865 6164 6572 735b  elf.out_headers[
-0001b980: 2258 2d52 6f62 6f74 732d 5461 6722 5d20  "X-Robots-Tag"] 
-0001b990: 3d20 226e 6f69 6e64 6578 2c20 6e6f 666f  = "noindex, nofo
-0001b9a0: 6c6c 6f77 220a 2020 2020 2020 2020 656c  llow".        el
-0001b9b0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0001b9c0: 7365 6c66 2e6f 7574 5f68 6561 6465 7273  self.out_headers
-0001b9d0: 2e70 6f70 2822 582d 526f 626f 7473 2d54  .pop("X-Robots-T
-0001b9e0: 6167 222c 204e 6f6e 6529 0a0a 2020 2020  ag", None)..    
-0001b9f0: 2020 2020 6973 5f64 6972 203d 2073 7461      is_dir = sta
-0001ba00: 742e 535f 4953 4449 5228 7374 2e73 745f  t.S_ISDIR(st.st_
-0001ba10: 6d6f 6465 290a 2020 2020 2020 2020 6963  mode).        ic
-0001ba20: 7572 203d 204e 6f6e 650a 2020 2020 2020  ur = None.      
-0001ba30: 2020 6966 2069 735f 6469 7220 616e 6420    if is_dir and 
-0001ba40: 2865 3274 206f 7220 6532 6429 3a0a 2020  (e2t or e2d):.  
-0001ba50: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
-0001ba60: 7365 6c66 2e63 6f6e 6e2e 6765 745f 7532  self.conn.get_u2
-0001ba70: 6964 7828 290a 2020 2020 2020 2020 2020  idx().          
-0001ba80: 2020 6966 2069 6478 2061 6e64 2068 6173    if idx and has
-0001ba90: 6174 7472 2869 6478 2c20 2270 5f65 6e64  attr(idx, "p_end
-0001baa0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0001bab0: 2020 2020 6963 7572 203d 2069 6478 2e67      icur = idx.g
-0001bac0: 6574 5f63 7572 2864 6276 2e72 6561 6c70  et_cur(dbv.realp
-0001bad0: 6174 6829 0a0a 2020 2020 2020 2020 6966  ath)..        if
-0001bae0: 2073 656c 662e 6361 6e5f 7265 6164 3a0a   self.can_read:.
-0001baf0: 2020 2020 2020 2020 2020 2020 7468 5f66              th_f
-0001bb00: 6d74 203d 2073 656c 662e 7570 6172 616d  mt = self.uparam
-0001bb10: 2e67 6574 2822 7468 2229 0a20 2020 2020  .get("th").     
-0001bb20: 2020 2020 2020 2069 6620 7468 5f66 6d74         if th_fmt
-0001bb30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0001bb40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001bb50: 2069 735f 6469 723a 0a20 2020 2020 2020   is_dir:.       
-0001bb60: 2020 2020 2020 2020 2020 2020 2076 7265               vre
-0001bb70: 6d20 3d20 7672 656d 2e72 7374 7269 7028  m = vrem.rstrip(
-0001bb80: 222f 2229 0a20 2020 2020 2020 2020 2020  "/").           
-0001bb90: 2020 2020 2020 2020 2069 6620 6963 7572           if icur
-0001bba0: 2061 6e64 2076 7265 6d3a 0a20 2020 2020   and vrem:.     
-0001bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bbc0: 2020 2071 203d 2022 7365 6c65 6374 2066     q = "select f
-0001bbd0: 6e20 6672 6f6d 2063 7620 7768 6572 6520  n from cv where 
-0001bbe0: 7264 3d3f 2061 6e64 2064 6e3d 3f22 0a20  rd=? and dn=?". 
+0001ad60: 666d 7420 3d20 225c 3033 335b 303b 373b  fmt = "\033[0;7;
+0001ad70: 3336 6d7b 7b7d 7d7b 7b3a 3e7b 7d7d 7d5c  36m{{}}{{:>{}}}\
+0001ad80: 3033 335b 306d 207b 7b7d 7d22 0a20 2020  033[0m {{}}".   
+0001ad90: 2020 2020 2020 2020 2020 2020 206e 666d               nfm
+0001ada0: 7420 3d20 227b 7d22 0a20 2020 2020 2020  t = "{}".       
+0001adb0: 2020 2020 2020 2020 2062 6967 6765 7374           biggest
+0001adc0: 203d 2030 0a20 2020 2020 2020 2020 2020   = 0.           
+0001add0: 2020 2020 2066 3220 3d20 2222 2e6a 6f69       f2 = "".joi
+0001ade0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0001adf0: 2020 2020 2020 2022 7b7d 7b7b 7d7d 222e         "{}{{}}".
+0001ae00: 666f 726d 6174 2878 290a 2020 2020 2020  format(x).      
+0001ae10: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0001ae20: 7220 7820 696e 205b 0a20 2020 2020 2020  r x in [.       
+0001ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae40: 2022 5c30 3333 5b37 6d22 2c0a 2020 2020   "\033[7m",.    
+0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae60: 2020 2020 225c 3033 335b 3237 6d22 2c0a      "\033[27m",.
+0001ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae80: 2020 2020 2020 2020 2222 2c0a 2020 2020          "",.    
+0001ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aea0: 2020 2020 225c 3033 335b 303b 316d 222c      "\033[0;1m",
+0001aeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aec0: 2020 2020 2020 2020 2022 5c30 3333 5b30           "\033[0
+0001aed0: 3b33 366d 222c 0a20 2020 2020 2020 2020  ;36m",.         
+0001aee0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001aef0: 5c30 3333 5b30 6d22 2c0a 2020 2020 2020  \033[0m",.      
+0001af00: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+0001af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001af30: 2020 6374 6162 203d 207b 2242 223a 2036    ctab = {"B": 6
+0001af40: 2c20 224b 223a 2035 2c20 224d 223a 2031  , "K": 5, "M": 1
+0001af50: 2c20 2247 223a 2033 7d0a 2020 2020 2020  , "G": 3}.      
+0001af60: 2020 2020 2020 2020 2020 666f 7220 6c73            for ls
+0001af70: 7420 696e 205b 6469 7273 2c20 6669 6c65  t in [dirs, file
+0001af80: 735d 3a0a 2020 2020 2020 2020 2020 2020  s]:.            
+0001af90: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
+0001afa0: 206c 7374 3a0a 2020 2020 2020 2020 2020   lst:.          
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 6120                a 
+0001afc0: 3d20 785b 2264 7422 5d2e 7265 706c 6163  = x["dt"].replac
+0001afd0: 6528 222d 222c 2022 2022 292e 7265 706c  e("-", " ").repl
+0001afe0: 6163 6528 223a 222c 2022 2022 292e 7370  ace(":", " ").sp
+0001aff0: 6c69 7428 2220 2229 0a20 2020 2020 2020  lit(" ").       
+0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b010: 2078 5b22 6474 225d 203d 2066 322e 666f   x["dt"] = f2.fo
+0001b020: 726d 6174 282a 6c69 7374 2861 2929 0a20  rmat(*list(a)). 
+0001b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b040: 2020 2020 2020 2073 7a20 3d20 6875 6d61         sz = huma
+0001b050: 6e73 697a 6528 785b 2273 7a22 5d2c 2054  nsize(x["sz"], T
+0001b060: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+0001b070: 2020 2020 2020 2020 2020 2020 2078 5b22               x["
+0001b080: 737a 225d 203d 2022 5c30 3333 5b30 3b33  sz"] = "\033[0;3
+0001b090: 7b7d 6d20 7b3a 3e35 7d22 2e66 6f72 6d61  {}m {:>5}".forma
+0001b0a0: 7428 6374 6162 2e67 6574 2873 7a5b 2d31  t(ctab.get(sz[-1
+0001b0b0: 3a5d 2c20 3029 2c20 737a 290a 2020 2020  :], 0), sz).    
+0001b0c0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001b0d0: 2020 2020 2020 2020 2020 2020 2020 666d                fm
+0001b0e0: 7420 3d20 227b 7b7d 7d20 207b 7b3a 7b7d  t = "{{}}  {{:{}
+0001b0f0: 2c7d 7d20 207b 7b7d 7d22 0a20 2020 2020  ,}}  {{}}".     
+0001b100: 2020 2020 2020 2020 2020 206e 666d 7420             nfmt 
+0001b110: 3d20 227b 3a2c 7d22 0a0a 2020 2020 2020  = "{:,}"..      
+0001b120: 2020 2020 2020 666f 7220 7820 696e 2064        for x in d
+0001b130: 6972 733a 0a20 2020 2020 2020 2020 2020  irs:.           
+0001b140: 2020 2020 206e 203d 2078 5b22 6e61 6d65       n = x["name
+0001b150: 225d 202b 2022 2f22 0a20 2020 2020 2020  "] + "/".       
+0001b160: 2020 2020 2020 2020 2069 6620 6172 6720           if arg 
+0001b170: 3d3d 2022 7622 3a0a 2020 2020 2020 2020  == "v":.        
+0001b180: 2020 2020 2020 2020 2020 2020 6e20 3d20              n = 
+0001b190: 225c 3033 335b 3934 6d22 202b 206e 0a0a  "\033[94m" + n..
+0001b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1b0: 785b 226e 616d 6522 5d20 3d20 6e0a 0a20  x["name"] = n.. 
+0001b1c0: 2020 2020 2020 2020 2020 2066 6d74 203d             fmt =
+0001b1d0: 2066 6d74 2e66 6f72 6d61 7428 6c65 6e28   fmt.format(len(
+0001b1e0: 6e66 6d74 2e66 6f72 6d61 7428 6269 6767  nfmt.format(bigg
+0001b1f0: 6573 7429 2929 0a20 2020 2020 2020 2020  est))).         
+0001b200: 2020 2072 6574 6c20 3d20 5b0a 2020 2020     retl = [.    
+0001b210: 2020 2020 2020 2020 2020 2020 2223 207b              "# {
+0001b220: 7d3a 207b 7d22 2e66 6f72 6d61 7428 782c  }: {}".format(x,
+0001b230: 206c 735b 785d 290a 2020 2020 2020 2020   ls[x]).        
+0001b240: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
+0001b250: 205b 2261 6363 7422 2c20 2270 6572 6d73   ["acct", "perms
+0001b260: 222c 2022 7372 7669 6e66 225d 0a20 2020  ", "srvinf"].   
+0001b270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001b280: 7820 696e 206c 730a 2020 2020 2020 2020  x in ls.        
+0001b290: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+0001b2a0: 2020 7265 746c 202b 3d20 5b0a 2020 2020    retl += [.    
+0001b2b0: 2020 2020 2020 2020 2020 2020 666d 742e              fmt.
+0001b2c0: 666f 726d 6174 2878 5b22 6474 225d 2c20  format(x["dt"], 
+0001b2d0: 785b 2273 7a22 5d2c 2078 5b22 6e61 6d65  x["sz"], x["name
+0001b2e0: 225d 290a 2020 2020 2020 2020 2020 2020  "]).            
+0001b2f0: 2020 2020 666f 7220 7920 696e 205b 6469      for y in [di
+0001b300: 7273 2c20 6669 6c65 735d 0a20 2020 2020  rs, files].     
+0001b310: 2020 2020 2020 2020 2020 2066 6f72 2078             for x
+0001b320: 2069 6e20 790a 2020 2020 2020 2020 2020   in y.          
+0001b330: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0001b340: 7265 7420 3d20 225c 6e22 2e6a 6f69 6e28  ret = "\n".join(
+0001b350: 7265 746c 290a 2020 2020 2020 2020 2020  retl).          
+0001b360: 2020 6d69 6d65 203d 2022 7465 7874 2f70    mime = "text/p
+0001b370: 6c61 696e 3b20 6368 6172 7365 743d 7574  lain; charset=ut
+0001b380: 662d 3822 0a20 2020 2020 2020 2065 6c73  f-8".        els
+0001b390: 653a 0a20 2020 2020 2020 2020 2020 205b  e:.            [
+0001b3a0: 782e 706f 7028 6b29 2066 6f72 206b 2069  x.pop(k) for k i
+0001b3b0: 6e20 5b22 6e61 6d65 222c 2022 6474 225d  n ["name", "dt"]
+0001b3c0: 2066 6f72 2079 2069 6e20 5b64 6972 732c   for y in [dirs,
+0001b3d0: 2066 696c 6573 5d20 666f 7220 7820 696e   files] for x in
+0001b3e0: 2079 5d0a 0a20 2020 2020 2020 2020 2020   y]..           
+0001b3f0: 2072 6574 203d 206a 736f 6e2e 6475 6d70   ret = json.dump
+0001b400: 7328 6c73 290a 2020 2020 2020 2020 2020  s(ls).          
+0001b410: 2020 6d69 6d65 203d 2022 6170 706c 6963    mime = "applic
+0001b420: 6174 696f 6e2f 6a73 6f6e 220a 0a20 2020  ation/json"..   
+0001b430: 2020 2020 2072 6574 202b 3d20 225c 6e5c       ret += "\n\
+0001b440: 3033 335b 306d 2220 6966 2061 7267 203d  033[0m" if arg =
+0001b450: 3d20 2276 2220 656c 7365 2022 5c6e 220a  = "v" else "\n".
+0001b460: 2020 2020 2020 2020 7365 6c66 2e72 6570          self.rep
+0001b470: 6c79 2872 6574 2e65 6e63 6f64 6528 2275  ly(ret.encode("u
+0001b480: 7466 2d38 222c 2022 7265 706c 6163 6522  tf-8", "replace"
+0001b490: 292c 206d 696d 653d 6d69 6d65 290a 2020  ), mime=mime).  
+0001b4a0: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0001b4b0: 650a 0a20 2020 2064 6566 2074 785f 6272  e..    def tx_br
+0001b4c0: 6f77 7365 7228 7365 6c66 2920 203a 0a20  owser(self)  :. 
+0001b4d0: 2020 2020 2020 2076 7061 7468 203d 2022         vpath = "
+0001b4e0: 220a 2020 2020 2020 2020 7670 6e6f 6465  ".        vpnode
+0001b4f0: 7320 3d20 5b5b 2222 2c20 222f 225d 5d0a  s = [["", "/"]].
+0001b500: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001b510: 7670 6174 683a 0a20 2020 2020 2020 2020  vpath:.         
+0001b520: 2020 2066 6f72 206e 6f64 6520 696e 2073     for node in s
+0001b530: 656c 662e 7670 6174 682e 7370 6c69 7428  elf.vpath.split(
+0001b540: 222f 2229 3a0a 2020 2020 2020 2020 2020  "/"):.          
+0001b550: 2020 2020 2020 6966 206e 6f74 2076 7061        if not vpa
+0001b560: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
+0001b570: 2020 2020 2020 2020 7670 6174 6820 3d20          vpath = 
+0001b580: 6e6f 6465 0a20 2020 2020 2020 2020 2020  node.           
+0001b590: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001b5a0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0001b5b0: 7061 7468 202b 3d20 222f 2220 2b20 6e6f  path += "/" + no
+0001b5c0: 6465 0a0a 2020 2020 2020 2020 2020 2020  de..            
+0001b5d0: 2020 2020 7670 6e6f 6465 732e 6170 7065      vpnodes.appe
+0001b5e0: 6e64 285b 7175 6f74 6570 2876 7061 7468  nd([quotep(vpath
+0001b5f0: 2920 2b20 222f 222c 2068 746d 6c5f 6573  ) + "/", html_es
+0001b600: 6361 7065 286e 6f64 652c 2063 726c 663d  cape(node, crlf=
+0001b610: 5472 7565 295d 290a 0a20 2020 2020 2020  True)])..       
+0001b620: 2076 6e20 3d20 7365 6c66 2e76 6e0a 2020   vn = self.vn.  
+0001b630: 2020 2020 2020 7265 6d20 3d20 7365 6c66        rem = self
+0001b640: 2e72 656d 0a20 2020 2020 2020 2061 6273  .rem.        abs
+0001b650: 7061 7468 203d 2076 6e2e 6463 616e 6f6e  path = vn.dcanon
+0001b660: 6963 616c 2872 656d 290a 2020 2020 2020  ical(rem).      
+0001b670: 2020 6462 762c 2076 7265 6d20 3d20 766e    dbv, vrem = vn
+0001b680: 2e67 6574 5f64 6276 2872 656d 290a 0a20  .get_dbv(rem).. 
+0001b690: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001b6a0: 2020 2020 2020 2020 7374 203d 2062 6f73          st = bos
+0001b6b0: 2e73 7461 7428 6162 7370 6174 6829 0a20  .stat(abspath). 
+0001b6c0: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+0001b6d0: 2020 2020 2020 2020 2020 2069 6620 226f             if "o
+0001b6e0: 6e34 3034 2220 6e6f 7420 696e 2076 6e2e  n404" not in vn.
+0001b6f0: 666c 6167 733a 0a20 2020 2020 2020 2020  flags:.         
+0001b700: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001b710: 6c66 2e74 785f 3430 3428 290a 0a20 2020  lf.tx_404()..   
+0001b720: 2020 2020 2020 2020 2072 6574 203d 2073           ret = s
+0001b730: 656c 662e 6f6e 3430 7828 766e 2e66 6c61  elf.on40x(vn.fla
+0001b740: 6773 5b22 6f6e 3430 3422 5d2c 2076 6e2c  gs["on404"], vn,
+0001b750: 2072 656d 290a 2020 2020 2020 2020 2020   rem).          
+0001b760: 2020 6966 2072 6574 203d 3d20 2274 7275    if ret == "tru
+0001b770: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
+0001b780: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0001b790: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0001b7a0: 2072 6574 203d 3d20 2266 616c 7365 223a   ret == "false":
+0001b7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b7c0: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0001b7d0: 2020 2020 2020 2020 2020 656c 6966 2072            elif r
+0001b7e0: 6574 203d 3d20 2272 6574 7279 223a 0a20  et == "retry":. 
+0001b7f0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001b800: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0001b810: 2020 2020 2020 2020 7374 203d 2062 6f73          st = bos
+0001b820: 2e73 7461 7428 6162 7370 6174 6829 0a20  .stat(abspath). 
+0001b830: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001b840: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+0001b850: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001b860: 6e20 7365 6c66 2e74 785f 3430 3428 290a  n self.tx_404().
+0001b870: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0001b880: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001b890: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+0001b8a0: 5f34 3034 2829 0a0a 2020 2020 2020 2020  _404()..        
+0001b8b0: 6966 2072 656d 2e73 7461 7274 7377 6974  if rem.startswit
+0001b8c0: 6828 222e 6869 7374 2f75 7032 6b2e 2229  h(".hist/up2k.")
+0001b8d0: 206f 7220 280a 2020 2020 2020 2020 2020   or (.          
+0001b8e0: 2020 7265 6d2e 656e 6473 7769 7468 2822    rem.endswith("
+0001b8f0: 2f64 6972 2e74 7874 2229 2061 6e64 2072  /dir.txt") and r
+0001b900: 656d 2e73 7461 7274 7377 6974 6828 222e  em.startswith(".
+0001b910: 6869 7374 2f74 682f 2229 0a20 2020 2020  hist/th/").     
+0001b920: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0001b930: 2020 7261 6973 6520 5065 626b 6163 2834    raise Pebkac(4
+0001b940: 3033 290a 0a20 2020 2020 2020 2065 3264  03)..        e2d
+0001b950: 203d 2022 6532 6422 2069 6e20 766e 2e66   = "e2d" in vn.f
+0001b960: 6c61 6773 0a20 2020 2020 2020 2065 3274  lags.        e2t
+0001b970: 203d 2022 6532 7422 2069 6e20 766e 2e66   = "e2t" in vn.f
+0001b980: 6c61 6773 0a0a 2020 2020 2020 2020 7365  lags..        se
+0001b990: 6c66 2e68 746d 6c5f 6865 6164 203d 2076  lf.html_head = v
+0001b9a0: 6e2e 666c 6167 732e 6765 7428 2268 746d  n.flags.get("htm
+0001b9b0: 6c5f 6865 6164 222c 2022 2229 0a20 2020  l_head", "").   
+0001b9c0: 2020 2020 2069 6620 766e 2e66 6c61 6773       if vn.flags
+0001b9d0: 2e67 6574 2822 6e6f 726f 626f 7473 2229  .get("norobots")
+0001b9e0: 206f 7220 2262 2220 696e 2073 656c 662e   or "b" in self.
+0001b9f0: 7570 6172 616d 3a0a 2020 2020 2020 2020  uparam:.        
+0001ba00: 2020 2020 7365 6c66 2e6f 7574 5f68 6561      self.out_hea
+0001ba10: 6465 7273 5b22 582d 526f 626f 7473 2d54  ders["X-Robots-T
+0001ba20: 6167 225d 203d 2022 6e6f 696e 6465 782c  ag"] = "noindex,
+0001ba30: 206e 6f66 6f6c 6c6f 7722 0a20 2020 2020   nofollow".     
+0001ba40: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001ba50: 2020 2020 2073 656c 662e 6f75 745f 6865       self.out_he
+0001ba60: 6164 6572 732e 706f 7028 2258 2d52 6f62  aders.pop("X-Rob
+0001ba70: 6f74 732d 5461 6722 2c20 4e6f 6e65 290a  ots-Tag", None).
+0001ba80: 0a20 2020 2020 2020 2069 735f 6469 7220  .        is_dir 
+0001ba90: 3d20 7374 6174 2e53 5f49 5344 4952 2873  = stat.S_ISDIR(s
+0001baa0: 742e 7374 5f6d 6f64 6529 0a20 2020 2020  t.st_mode).     
+0001bab0: 2020 2069 6375 7220 3d20 4e6f 6e65 0a20     icur = None. 
+0001bac0: 2020 2020 2020 2069 6620 6973 5f64 6972         if is_dir
+0001bad0: 2061 6e64 2028 6532 7420 6f72 2065 3264   and (e2t or e2d
+0001bae0: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0001baf0: 6478 203d 2073 656c 662e 636f 6e6e 2e67  dx = self.conn.g
+0001bb00: 6574 5f75 3269 6478 2829 0a20 2020 2020  et_u2idx().     
+0001bb10: 2020 2020 2020 2069 6620 6964 7820 616e         if idx an
+0001bb20: 6420 6861 7361 7474 7228 6964 782c 2022  d hasattr(idx, "
+0001bb30: 705f 656e 6422 293a 0a20 2020 2020 2020  p_end"):.       
+0001bb40: 2020 2020 2020 2020 2069 6375 7220 3d20           icur = 
+0001bb50: 6964 782e 6765 745f 6375 7228 6462 762e  idx.get_cur(dbv.
+0001bb60: 7265 616c 7061 7468 290a 0a20 2020 2020  realpath)..     
+0001bb70: 2020 2069 6620 7365 6c66 2e63 616e 5f72     if self.can_r
+0001bb80: 6561 643a 0a20 2020 2020 2020 2020 2020  ead:.           
+0001bb90: 2074 685f 666d 7420 3d20 7365 6c66 2e75   th_fmt = self.u
+0001bba0: 7061 7261 6d2e 6765 7428 2274 6822 290a  param.get("th").
+0001bbb0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
+0001bbc0: 685f 666d 7420 6973 206e 6f74 204e 6f6e  h_fmt is not Non
+0001bbd0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001bbe0: 2020 2069 6620 6973 5f64 6972 3a0a 2020     if is_dir:.  
 0001bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc00: 2020 2020 2020 2063 7264 2c20 6364 6e20         crd, cdn 
-0001bc10: 3d20 7672 656d 2e72 7370 6c69 7428 222f  = vrem.rsplit("/
-0001bc20: 222c 2031 2920 6966 2022 2f22 2069 6e20  ", 1) if "/" in 
-0001bc30: 7672 656d 2065 6c73 6520 2822 222c 2076  vrem else ("", v
-0001bc40: 7265 6d29 0a20 2020 2020 2020 2020 2020  rem).           
-0001bc50: 2020 2020 2020 2020 2020 2020 2023 206e               # n
-0001bc60: 6f20 6d6f 6a69 6261 6b65 2073 7570 706f  o mojibake suppo
-0001bc70: 7274 3a0a 2020 2020 2020 2020 2020 2020  rt:.            
-0001bc80: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-0001bc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bca0: 2020 2020 2020 2020 2020 2020 2063 666e               cfn
-0001bcb0: 203d 2069 6375 722e 6578 6563 7574 6528   = icur.execute(
-0001bcc0: 712c 2028 6372 642c 2063 646e 2929 2e66  q, (crd, cdn)).f
-0001bcd0: 6574 6368 6f6e 6528 290a 2020 2020 2020  etchone().      
+0001bc00: 2020 7672 656d 203d 2076 7265 6d2e 7273    vrem = vrem.rs
+0001bc10: 7472 6970 2822 2f22 290a 2020 2020 2020  trip("/").      
+0001bc20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001bc30: 2069 6375 7220 616e 6420 7672 656d 3a0a   icur and vrem:.
+0001bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bc50: 2020 2020 2020 2020 7120 3d20 2273 656c          q = "sel
+0001bc60: 6563 7420 666e 2066 726f 6d20 6376 2077  ect fn from cv w
+0001bc70: 6865 7265 2072 643d 3f20 616e 6420 646e  here rd=? and dn
+0001bc80: 3d3f 220a 2020 2020 2020 2020 2020 2020  =?".            
+0001bc90: 2020 2020 2020 2020 2020 2020 6372 642c              crd,
+0001bca0: 2063 646e 203d 2076 7265 6d2e 7273 706c   cdn = vrem.rspl
+0001bcb0: 6974 2822 2f22 2c20 3129 2069 6620 222f  it("/", 1) if "/
+0001bcc0: 2220 696e 2076 7265 6d20 656c 7365 2028  " in vrem else (
+0001bcd0: 2222 2c20 7672 656d 290a 2020 2020 2020  "", vrem).      
 0001bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcf0: 2020 2020 2020 6966 2063 666e 3a0a 2020        if cfn:.  
-0001bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd10: 2020 2020 2020 2020 2020 2020 2020 666e                fn
-0001bd20: 203d 2063 666e 5b30 5d0a 2020 2020 2020   = cfn[0].      
+0001bcf0: 2020 2320 6e6f 206d 6f6a 6962 616b 6520    # no mojibake 
+0001bd00: 7375 7070 6f72 743a 0a20 2020 2020 2020  support:.       
+0001bd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd20: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
 0001bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd40: 2020 2020 2020 2020 2020 6670 203d 206f            fp = o
-0001bd50: 732e 7061 7468 2e6a 6f69 6e28 6162 7370  s.path.join(absp
-0001bd60: 6174 682c 2066 6e29 0a20 2020 2020 2020  ath, fn).       
+0001bd40: 2020 6366 6e20 3d20 6963 7572 2e65 7865    cfn = icur.exe
+0001bd50: 6375 7465 2871 2c20 2863 7264 2c20 6364  cute(q, (crd, cd
+0001bd60: 6e29 292e 6665 7463 686f 6e65 2829 0a20  n)).fetchone(). 
 0001bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd80: 2020 2020 2020 2020 2069 6620 626f 732e           if bos.
-0001bd90: 7061 7468 2e65 7869 7374 7328 6670 293a  path.exists(fp):
-0001bda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bdc0: 2020 2020 2076 7265 6d20 3d20 227b 7d2f       vrem = "{}/
-0001bdd0: 7b7d 222e 666f 726d 6174 2876 7265 6d2c  {}".format(vrem,
-0001bde0: 2066 6e29 2e73 7472 6970 2822 2f22 290a   fn).strip("/").
-0001bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bd80: 2020 2020 2020 2020 2020 2069 6620 6366             if cf
+0001bd90: 6e3a 0a20 2020 2020 2020 2020 2020 2020  n:.             
+0001bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bdb0: 2020 2066 6e20 3d20 6366 6e5b 305d 0a20     fn = cfn[0]. 
+0001bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001bde0: 7020 3d20 6f73 2e70 6174 682e 6a6f 696e  p = os.path.join
+0001bdf0: 2861 6273 7061 7468 2c20 666e 290a 2020  (abspath, fn).  
 0001be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be10: 2020 2020 6973 5f64 6972 203d 2046 616c      is_dir = Fal
-0001be20: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-0001be30: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0001be40: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0001be50: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001be60: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-0001be70: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001be90: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
-0001bea0: 7365 6c66 2e61 7267 732e 7468 5f63 6f76  self.args.th_cov
-0001beb0: 6572 733a 0a20 2020 2020 2020 2020 2020  ers:.           
+0001be10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001be20: 2062 6f73 2e70 6174 682e 6578 6973 7473   bos.path.exists
+0001be30: 2866 7029 3a0a 2020 2020 2020 2020 2020  (fp):.          
+0001be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001be50: 2020 2020 2020 2020 2020 7672 656d 203d            vrem =
+0001be60: 2022 7b7d 2f7b 7d22 2e66 6f72 6d61 7428   "{}/{}".format(
+0001be70: 7672 656d 2c20 666e 292e 7374 7269 7028  vrem, fn).strip(
+0001be80: 222f 2229 0a20 2020 2020 2020 2020 2020  "/").           
+0001be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bea0: 2020 2020 2020 2020 2069 735f 6469 7220           is_dir 
+0001beb0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
 0001bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bed0: 2066 7020 3d20 6f73 2e70 6174 682e 6a6f   fp = os.path.jo
-0001bee0: 696e 2861 6273 7061 7468 2c20 666e 290a  in(abspath, fn).
-0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf00: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0001bf10: 6f73 2e70 6174 682e 6578 6973 7473 2866  os.path.exists(f
-0001bf20: 7029 3a0a 2020 2020 2020 2020 2020 2020  p):.            
-0001bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf40: 2020 2020 7672 656d 203d 2022 7b7d 2f7b      vrem = "{}/{
-0001bf50: 7d22 2e66 6f72 6d61 7428 7672 656d 2c20  }".format(vrem, 
-0001bf60: 666e 292e 7374 7269 7028 222f 2229 0a20  fn).strip("/"). 
-0001bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bf80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001bf90: 735f 6469 7220 3d20 4661 6c73 650a 2020  s_dir = False.  
-0001bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bfb0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-0001bfc0: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
-0001bfd0: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
-0001bfe0: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-0001bff0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0001c000: 726e 2073 656c 662e 7478 5f69 636f 2822  rn self.tx_ico("
-0001c010: 612e 666f 6c64 6572 2229 0a0a 2020 2020  a.folder")..    
-0001c020: 2020 2020 2020 2020 2020 2020 7468 7020              thp 
-0001c030: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-0001c040: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-0001c050: 6875 6d62 636c 693a 0a20 2020 2020 2020  humbcli:.       
-0001c060: 2020 2020 2020 2020 2020 2020 2074 6870               thp
-0001c070: 203d 2073 656c 662e 7468 756d 6263 6c69   = self.thumbcli
-0001c080: 2e67 6574 2864 6276 2c20 7672 656d 2c20  .get(dbv, vrem, 
-0001c090: 696e 7428 7374 2e73 745f 6d74 696d 6529  int(st.st_mtime)
-0001c0a0: 2c20 7468 5f66 6d74 290a 0a20 2020 2020  , th_fmt)..     
-0001c0b0: 2020 2020 2020 2020 2020 2069 6620 7468             if th
-0001c0c0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-0001c0d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0001c0e0: 6c66 2e74 785f 6669 6c65 2874 6870 290a  lf.tx_file(thp).
-0001c0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c100: 2069 6620 7468 5f66 6d74 203d 3d20 2270   if th_fmt == "p
-0001c110: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0001c120: 2020 2020 2020 2072 6169 7365 2050 6562         raise Peb
-0001c130: 6b61 6328 3430 3429 0a0a 2020 2020 2020  kac(404)..      
-0001c140: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001c150: 2073 656c 662e 7478 5f69 636f 2872 656d   self.tx_ico(rem
-0001c160: 290a 0a20 2020 2020 2020 2069 6620 6e6f  )..        if no
-0001c170: 7420 6973 5f64 6972 2061 6e64 2028 7365  t is_dir and (se
-0001c180: 6c66 2e63 616e 5f72 6561 6420 6f72 2073  lf.can_read or s
-0001c190: 656c 662e 6361 6e5f 6765 7429 3a0a 2020  elf.can_get):.  
-0001c1a0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0001c1b0: 2073 656c 662e 6361 6e5f 7265 6164 2061   self.can_read a
-0001c1c0: 6e64 2022 666b 2220 696e 2076 6e2e 666c  nd "fk" in vn.fl
-0001c1d0: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
-0001c1e0: 2020 2020 2063 6f72 7265 6374 203d 2073       correct = s
-0001c1f0: 656c 662e 6765 6e5f 666b 280a 2020 2020  elf.gen_fk(.    
-0001c200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c210: 7365 6c66 2e61 7267 732e 666b 5f73 616c  self.args.fk_sal
-0001c220: 742c 2061 6273 7061 7468 2c20 7374 2e73  t, abspath, st.s
-0001c230: 745f 7369 7a65 2c20 3020 6966 2041 4e59  t_size, 0 if ANY
-0001c240: 5749 4e20 656c 7365 2073 742e 7374 5f69  WIN else st.st_i
-0001c250: 6e6f 0a20 2020 2020 2020 2020 2020 2020  no.             
-0001c260: 2020 2029 5b3a 2076 6e2e 666c 6167 735b     )[: vn.flags[
-0001c270: 2266 6b22 5d5d 0a20 2020 2020 2020 2020  "fk"]].         
-0001c280: 2020 2020 2020 2067 6f74 203d 2073 656c         got = sel
-0001c290: 662e 7570 6172 616d 2e67 6574 2822 6b22  f.uparam.get("k"
-0001c2a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001c2b0: 2020 6966 2067 6f74 2021 3d20 636f 7272    if got != corr
-0001c2c0: 6563 743a 0a20 2020 2020 2020 2020 2020  ect:.           
-0001c2d0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0001c2e0: 6728 2277 726f 6e67 2066 696c 656b 6579  g("wrong filekey
-0001c2f0: 2c20 7761 6e74 207b 7d2c 2067 6f74 207b  , want {}, got {
-0001c300: 7d22 2e66 6f72 6d61 7428 636f 7272 6563  }".format(correc
-0001c310: 742c 2067 6f74 2929 0a20 2020 2020 2020  t, got)).       
-0001c320: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001c330: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
-0001c340: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0001c350: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
-0001c360: 2020 2020 6162 7370 6174 682e 656e 6473      abspath.ends
-0001c370: 7769 7468 2822 2e6d 6422 290a 2020 2020  with(".md").    
-0001c380: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0001c390: 226e 6f68 746d 6c22 206e 6f74 2069 6e20  "nohtml" not in 
-0001c3a0: 766e 2e66 6c61 6773 0a20 2020 2020 2020  vn.flags.       
-0001c3b0: 2020 2020 2020 2020 2061 6e64 2028 0a20           and (. 
-0001c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c3d0: 2020 2022 7622 2069 6e20 7365 6c66 2e75     "v" in self.u
-0001c3e0: 7061 7261 6d0a 2020 2020 2020 2020 2020  param.          
-0001c3f0: 2020 2020 2020 2020 2020 6f72 2022 6564            or "ed
-0001c400: 6974 2220 696e 2073 656c 662e 7570 6172  it" in self.upar
-0001c410: 616d 0a20 2020 2020 2020 2020 2020 2020  am.             
-0001c420: 2020 2020 2020 206f 7220 2265 6469 7432         or "edit2
-0001c430: 2220 696e 2073 656c 662e 7570 6172 616d  " in self.uparam
-0001c440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c450: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-0001c460: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001c470: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
-0001c480: 5f6d 6428 6162 7370 6174 6829 0a0a 2020  _md(abspath)..  
-0001c490: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001c4a0: 2073 656c 662e 7478 5f66 696c 6528 6162   self.tx_file(ab
-0001c4b0: 7370 6174 6829 0a0a 2020 2020 2020 2020  spath)..        
-0001c4c0: 656c 6966 2069 735f 6469 7220 616e 6420  elif is_dir and 
-0001c4d0: 6e6f 7420 7365 6c66 2e63 616e 5f72 6561  not self.can_rea
-0001c4e0: 6420 616e 6420 6e6f 7420 7365 6c66 2e63  d and not self.c
-0001c4f0: 616e 5f77 7269 7465 3a0a 2020 2020 2020  an_write:.      
-0001c500: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001c510: 662e 7478 5f34 3034 2854 7275 6529 0a0a  f.tx_404(True)..
-0001c520: 2020 2020 2020 2020 7372 765f 696e 666f          srv_info
-0001c530: 203d 205b 5d0a 0a20 2020 2020 2020 2074   = []..        t
-0001c540: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0001c550: 6966 206e 6f74 2073 656c 662e 6172 6773  if not self.args
-0001c560: 2e6e 6968 3a0a 2020 2020 2020 2020 2020  .nih:.          
-0001c570: 2020 2020 2020 7372 765f 696e 666f 2e61        srv_info.a
-0001c580: 7070 656e 6428 7365 6c66 2e61 7267 732e  ppend(self.args.
-0001c590: 6e61 6d65 290a 2020 2020 2020 2020 6578  name).        ex
-0001c5a0: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-0001c5b0: 2020 7365 6c66 2e6c 6f67 2822 2377 6f77    self.log("#wow
-0001c5c0: 2023 7768 6f61 2229 0a0a 2020 2020 2020   #whoa")..      
-0001c5d0: 2020 6966 206e 6f74 2073 656c 662e 6172    if not self.ar
-0001c5e0: 6773 2e6e 6964 3a0a 2020 2020 2020 2020  gs.nid:.        
-0001c5f0: 2020 2020 6672 6565 2c20 746f 7461 6c20      free, total 
-0001c600: 3d20 6765 745f 6466 2861 6273 7061 7468  = get_df(abspath
-0001c610: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0001c620: 2074 6f74 616c 2069 7320 6e6f 7420 4e6f   total is not No
-0001c630: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0001c640: 2020 2020 6831 203d 2068 756d 616e 7369      h1 = humansi
-0001c650: 7a65 2866 7265 6520 6f72 2030 290a 2020  ze(free or 0).  
-0001c660: 2020 2020 2020 2020 2020 2020 2020 6832                h2
-0001c670: 203d 2068 756d 616e 7369 7a65 2874 6f74   = humansize(tot
-0001c680: 616c 290a 2020 2020 2020 2020 2020 2020  al).            
-0001c690: 2020 2020 7372 765f 696e 666f 2e61 7070      srv_info.app
-0001c6a0: 656e 6428 227b 7d20 6672 6565 206f 6620  end("{} free of 
-0001c6b0: 7b7d 222e 666f 726d 6174 2868 312c 2068  {}".format(h1, h
-0001c6c0: 3229 290a 2020 2020 2020 2020 2020 2020  2)).            
-0001c6d0: 656c 6966 2066 7265 6520 6973 206e 6f74  elif free is not
-0001c6e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0001c6f0: 2020 2020 2020 2073 7276 5f69 6e66 6f2e         srv_info.
-0001c700: 6170 7065 6e64 2868 756d 616e 7369 7a65  append(humansize
-0001c710: 2866 7265 652c 2054 7275 6529 202b 2022  (free, True) + "
-0001c720: 2066 7265 6522 290a 0a20 2020 2020 2020   free")..       
-0001c730: 2073 7276 5f69 6e66 6f74 203d 2022 3c2f   srv_infot = "</
-0001c740: 7370 616e 3e20 2f2f 203c 7370 616e 3e22  span> // <span>"
-0001c750: 2e6a 6f69 6e28 7372 765f 696e 666f 290a  .join(srv_info).
-0001c760: 0a20 2020 2020 2020 2070 6572 6d73 203d  .        perms =
-0001c770: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
-0001c780: 656c 662e 6361 6e5f 7265 6164 3a0a 2020  elf.can_read:.  
-0001c790: 2020 2020 2020 2020 2020 7065 726d 732e            perms.
-0001c7a0: 6170 7065 6e64 2822 7265 6164 2229 0a20  append("read"). 
-0001c7b0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0001c7c0: 616e 5f77 7269 7465 3a0a 2020 2020 2020  an_write:.      
-0001c7d0: 2020 2020 2020 7065 726d 732e 6170 7065        perms.appe
-0001c7e0: 6e64 2822 7772 6974 6522 290a 2020 2020  nd("write").    
-0001c7f0: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
-0001c800: 6d6f 7665 3a0a 2020 2020 2020 2020 2020  move:.          
-0001c810: 2020 7065 726d 732e 6170 7065 6e64 2822    perms.append("
-0001c820: 6d6f 7665 2229 0a20 2020 2020 2020 2069  move").        i
-0001c830: 6620 7365 6c66 2e63 616e 5f64 656c 6574  f self.can_delet
-0001c840: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
-0001c850: 6572 6d73 2e61 7070 656e 6428 2264 656c  erms.append("del
-0001c860: 6574 6522 290a 2020 2020 2020 2020 6966  ete").        if
-0001c870: 2073 656c 662e 6361 6e5f 6765 743a 0a20   self.can_get:. 
-0001c880: 2020 2020 2020 2020 2020 2070 6572 6d73             perms
-0001c890: 2e61 7070 656e 6428 2267 6574 2229 0a20  .append("get"). 
-0001c8a0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-0001c8b0: 616e 5f75 7067 6574 3a0a 2020 2020 2020  an_upget:.      
-0001c8c0: 2020 2020 2020 7065 726d 732e 6170 7065        perms.appe
-0001c8d0: 6e64 2822 7570 6765 7422 290a 2020 2020  nd("upget").    
-0001c8e0: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
-0001c8f0: 6164 6d69 6e3a 0a20 2020 2020 2020 2020  admin:.         
-0001c900: 2020 2070 6572 6d73 2e61 7070 656e 6428     perms.append(
-0001c910: 2261 646d 696e 2229 0a0a 2020 2020 2020  "admin")..      
-0001c920: 2020 7572 6c5f 7375 6620 3d20 7365 6c66    url_suf = self
-0001c930: 2e75 726c 7128 7b7d 2c20 5b22 6b22 5d29  .urlq({}, ["k"])
-0001c940: 0a20 2020 2020 2020 2069 735f 6c73 203d  .        is_ls =
-0001c950: 2022 6c73 2220 696e 2073 656c 662e 7570   "ls" in self.up
-0001c960: 6172 616d 0a20 2020 2020 2020 2069 735f  aram.        is_
-0001c970: 6a73 203d 2073 656c 662e 6172 6773 2e66  js = self.args.f
-0001c980: 6f72 6365 5f6a 7320 6f72 2073 656c 662e  orce_js or self.
-0001c990: 636f 6f6b 6965 732e 6765 7428 226a 7322  cookies.get("js"
-0001c9a0: 2920 3d3d 2022 7922 0a0a 2020 2020 2020  ) == "y"..      
-0001c9b0: 2020 6966 206e 6f74 2069 735f 6c73 2061    if not is_ls a
-0001c9c0: 6e64 2028 7365 6c66 2e75 612e 7374 6172  nd (self.ua.star
-0001c9d0: 7473 7769 7468 2822 6375 726c 2f22 2920  tswith("curl/") 
-0001c9e0: 6f72 2073 656c 662e 7561 2e73 7461 7274  or self.ua.start
-0001c9f0: 7377 6974 6828 2266 6574 6368 2229 293a  swith("fetch")):
-0001ca00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001ca10: 662e 7570 6172 616d 5b22 6c73 225d 203d  f.uparam["ls"] =
-0001ca20: 2022 7622 0a20 2020 2020 2020 2020 2020   "v".           
-0001ca30: 2069 735f 6c73 203d 2054 7275 650a 0a20   is_ls = True.. 
-0001ca40: 2020 2020 2020 2074 706c 203d 2022 6272         tpl = "br
-0001ca50: 6f77 7365 7222 0a20 2020 2020 2020 2069  owser".        i
-0001ca60: 6620 2262 2220 696e 2073 656c 662e 7570  f "b" in self.up
-0001ca70: 6172 616d 3a0a 2020 2020 2020 2020 2020  aram:.          
-0001ca80: 2020 7470 6c20 3d20 2262 726f 7773 6572    tpl = "browser
-0001ca90: 3222 0a20 2020 2020 2020 2020 2020 2069  2".            i
-0001caa0: 735f 6a73 203d 2046 616c 7365 0a0a 2020  s_js = False..  
-0001cab0: 2020 2020 2020 6c6f 6775 6573 203d 205b        logues = [
-0001cac0: 2222 2c20 2222 5d0a 2020 2020 2020 2020  "", ""].        
-0001cad0: 6966 206e 6f74 2073 656c 662e 6172 6773  if not self.args
-0001cae0: 2e6e 6f5f 6c6f 6775 6573 3a0a 2020 2020  .no_logues:.    
-0001caf0: 2020 2020 2020 2020 666f 7220 6e2c 2066          for n, f
-0001cb00: 6e20 696e 2065 6e75 6d65 7261 7465 285b  n in enumerate([
-0001cb10: 222e 7072 6f6c 6f67 7565 2e68 746d 6c22  ".prologue.html"
-0001cb20: 2c20 222e 6570 696c 6f67 7565 2e68 746d  , ".epilogue.htm
-0001cb30: 6c22 5d29 3a0a 2020 2020 2020 2020 2020  l"]):.          
-0001cb40: 2020 2020 2020 666e 203d 206f 732e 7061        fn = os.pa
-0001cb50: 7468 2e6a 6f69 6e28 6162 7370 6174 682c  th.join(abspath,
-0001cb60: 2066 6e29 0a20 2020 2020 2020 2020 2020   fn).           
-0001cb70: 2020 2020 2069 6620 626f 732e 7061 7468       if bos.path
-0001cb80: 2e65 7869 7374 7328 666e 293a 0a20 2020  .exists(fn):.   
-0001cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cba0: 2077 6974 6820 6f70 656e 2866 7365 6e63   with open(fsenc
-0001cbb0: 2866 6e29 2c20 2272 6222 2920 6173 2066  (fn), "rb") as f
-0001cbc0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001cbd0: 2020 2020 2020 2020 2020 6c6f 6775 6573            logues
-0001cbe0: 5b6e 5d20 3d20 662e 7265 6164 2829 2e64  [n] = f.read().d
-0001cbf0: 6563 6f64 6528 2275 7466 2d38 2229 0a0a  ecode("utf-8")..
-0001cc00: 2020 2020 2020 2020 7265 6164 6d65 203d          readme =
-0001cc10: 2022 220a 2020 2020 2020 2020 6966 206e   "".        if n
-0001cc20: 6f74 2073 656c 662e 6172 6773 2e6e 6f5f  ot self.args.no_
-0001cc30: 7265 6164 6d65 2061 6e64 206e 6f74 206c  readme and not l
-0001cc40: 6f67 7565 735b 315d 3a0a 2020 2020 2020  ogues[1]:.      
-0001cc50: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
-0001cc60: 5b22 5245 4144 4d45 2e6d 6422 2c20 2272  ["README.md", "r
-0001cc70: 6561 646d 652e 6d64 225d 3a0a 2020 2020  eadme.md"]:.    
-0001cc80: 2020 2020 2020 2020 2020 2020 666e 203d              fn =
-0001cc90: 206f 732e 7061 7468 2e6a 6f69 6e28 6162   os.path.join(ab
-0001cca0: 7370 6174 682c 2066 6e29 0a20 2020 2020  spath, fn).     
-0001ccb0: 2020 2020 2020 2020 2020 2069 6620 626f             if bo
-0001ccc0: 732e 7061 7468 2e69 7366 696c 6528 666e  s.path.isfile(fn
-0001ccd0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0001cce0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-0001ccf0: 2866 7365 6e63 2866 6e29 2c20 2272 6222  (fsenc(fn), "rb"
-0001cd00: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-0001cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cd20: 7265 6164 6d65 203d 2066 2e72 6561 6428  readme = f.read(
-0001cd30: 292e 6465 636f 6465 2822 7574 662d 3822  ).decode("utf-8"
-0001cd40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001cd50: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-0001cd60: 0a20 2020 2020 2020 2076 6620 3d20 766e  .        vf = vn
-0001cd70: 2e66 6c61 6773 0a20 2020 2020 2020 2075  .flags.        u
-0001cd80: 6e6c 6973 7420 3d20 7666 2e67 6574 2822  nlist = vf.get("
-0001cd90: 756e 6c69 7374 222c 2022 2229 0a20 2020  unlist", "").   
-0001cda0: 2020 2020 206c 735f 7265 7420 3d20 7b0a       ls_ret = {.
-0001cdb0: 2020 2020 2020 2020 2020 2020 2264 6972              "dir
-0001cdc0: 7322 3a20 5b5d 2c0a 2020 2020 2020 2020  s": [],.        
-0001cdd0: 2020 2020 2266 696c 6573 223a 205b 5d2c      "files": [],
-0001cde0: 0a20 2020 2020 2020 2020 2020 2022 7461  .            "ta
-0001cdf0: 676c 6973 7422 3a20 5b5d 2c0a 2020 2020  glist": [],.    
-0001ce00: 2020 2020 2020 2020 2273 7276 696e 6622          "srvinf"
-0001ce10: 3a20 7372 765f 696e 666f 742c 0a20 2020  : srv_infot,.   
-0001ce20: 2020 2020 2020 2020 2022 6163 6374 223a           "acct":
-0001ce30: 2073 656c 662e 756e 616d 652c 0a20 2020   self.uname,.   
-0001ce40: 2020 2020 2020 2020 2022 6964 7822 3a20           "idx": 
-0001ce50: 6532 642c 0a20 2020 2020 2020 2020 2020  e2d,.           
-0001ce60: 2022 6974 6167 223a 2065 3274 2c0a 2020   "itag": e2t,.  
-0001ce70: 2020 2020 2020 2020 2020 226c 6966 6574            "lifet
-0001ce80: 696d 6522 3a20 766e 2e66 6c61 6773 2e67  ime": vn.flags.g
-0001ce90: 6574 2822 6c69 6665 7469 6d65 2229 206f  et("lifetime") o
-0001cea0: 7220 302c 0a20 2020 2020 2020 2020 2020  r 0,.           
-0001ceb0: 2022 6672 616e 6422 3a20 626f 6f6c 2876   "frand": bool(v
-0001cec0: 6e2e 666c 6167 732e 6765 7428 2272 616e  n.flags.get("ran
-0001ced0: 6422 2929 2c0a 2020 2020 2020 2020 2020  d")),.          
-0001cee0: 2020 2275 6e6c 6973 7422 3a20 756e 6c69    "unlist": unli
-0001cef0: 7374 2c0a 2020 2020 2020 2020 2020 2020  st,.            
-0001cf00: 2270 6572 6d73 223a 2070 6572 6d73 2c0a  "perms": perms,.
-0001cf10: 2020 2020 2020 2020 2020 2020 226c 6f67              "log
-0001cf20: 7565 7322 3a20 6c6f 6775 6573 2c0a 2020  ues": logues,.  
-0001cf30: 2020 2020 2020 2020 2020 2272 6561 646d            "readm
-0001cf40: 6522 3a20 7265 6164 6d65 2c0a 2020 2020  e": readme,.    
-0001cf50: 2020 2020 7d0a 2020 2020 2020 2020 6a32      }.        j2
-0001cf60: 6120 3d20 7b0a 2020 2020 2020 2020 2020  a = {.          
-0001cf70: 2020 2276 6469 7222 3a20 7175 6f74 6570    "vdir": quotep
-0001cf80: 2873 656c 662e 7670 6174 6829 2c0a 2020  (self.vpath),.  
-0001cf90: 2020 2020 2020 2020 2020 2276 706e 6f64            "vpnod
-0001cfa0: 6573 223a 2076 706e 6f64 6573 2c0a 2020  es": vpnodes,.  
-0001cfb0: 2020 2020 2020 2020 2020 2266 696c 6573            "files
-0001cfc0: 223a 205b 5d2c 0a20 2020 2020 2020 2020  ": [],.         
-0001cfd0: 2020 2022 6c73 3022 3a20 4e6f 6e65 2c0a     "ls0": None,.
-0001cfe0: 2020 2020 2020 2020 2020 2020 2261 6363              "acc
-0001cff0: 7422 3a20 7365 6c66 2e75 6e61 6d65 2c0a  t": self.uname,.
-0001d000: 2020 2020 2020 2020 2020 2020 2270 6572              "per
-0001d010: 6d73 223a 206a 736f 6e2e 6475 6d70 7328  ms": json.dumps(
-0001d020: 7065 726d 7329 2c0a 2020 2020 2020 2020  perms),.        
-0001d030: 2020 2020 226c 6966 6574 696d 6522 3a20      "lifetime": 
-0001d040: 6c73 5f72 6574 5b22 6c69 6665 7469 6d65  ls_ret["lifetime
-0001d050: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-0001d060: 2266 7261 6e64 223a 2062 6f6f 6c28 766e  "frand": bool(vn
-0001d070: 2e66 6c61 6773 2e67 6574 2822 7261 6e64  .flags.get("rand
-0001d080: 2229 292c 0a20 2020 2020 2020 2020 2020  ")),.           
-0001d090: 2022 7461 676c 6973 7422 3a20 5b5d 2c0a   "taglist": [],.
-0001d0a0: 2020 2020 2020 2020 2020 2020 2264 6566              "def
-0001d0b0: 5f68 636f 6c73 223a 205b 5d2c 0a20 2020  _hcols": [],.   
-0001d0c0: 2020 2020 2020 2020 2022 6861 7665 5f65           "have_e
-0001d0d0: 6d70 223a 2073 656c 662e 6172 6773 2e65  mp": self.args.e
-0001d0e0: 6d70 2c0a 2020 2020 2020 2020 2020 2020  mp,.            
-0001d0f0: 2268 6176 655f 7570 326b 5f69 6478 223a  "have_up2k_idx":
-0001d100: 2065 3264 2c0a 2020 2020 2020 2020 2020   e2d,.          
-0001d110: 2020 2268 6176 655f 7461 6773 5f69 6478    "have_tags_idx
-0001d120: 223a 2065 3274 2c0a 2020 2020 2020 2020  ": e2t,.        
-0001d130: 2020 2020 2268 6176 655f 6163 6f64 6522      "have_acode"
-0001d140: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
-0001d150: 2e6e 6f5f 6163 6f64 6529 2c0a 2020 2020  .no_acode),.    
-0001d160: 2020 2020 2020 2020 2268 6176 655f 6d76          "have_mv
-0001d170: 223a 2028 6e6f 7420 7365 6c66 2e61 7267  ": (not self.arg
-0001d180: 732e 6e6f 5f6d 7629 2c0a 2020 2020 2020  s.no_mv),.      
-0001d190: 2020 2020 2020 2268 6176 655f 6465 6c22        "have_del"
-0001d1a0: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
-0001d1b0: 2e6e 6f5f 6465 6c29 2c0a 2020 2020 2020  .no_del),.      
-0001d1c0: 2020 2020 2020 2268 6176 655f 7a69 7022        "have_zip"
-0001d1d0: 3a20 286e 6f74 2073 656c 662e 6172 6773  : (not self.args
-0001d1e0: 2e6e 6f5f 7a69 7029 2c0a 2020 2020 2020  .no_zip),.      
-0001d1f0: 2020 2020 2020 2268 6176 655f 756e 706f        "have_unpo
-0001d200: 7374 223a 2069 6e74 2873 656c 662e 6172  st": int(self.ar
-0001d210: 6773 2e75 6e70 6f73 7429 2c0a 2020 2020  gs.unpost),.    
-0001d220: 2020 2020 2020 2020 2268 6176 655f 625f          "have_b_
-0001d230: 7522 3a20 2873 656c 662e 6361 6e5f 7772  u": (self.can_wr
-0001d240: 6974 6520 616e 6420 7365 6c66 2e75 7061  ite and self.upa
-0001d250: 7261 6d2e 6765 7428 2262 2229 203d 3d20  ram.get("b") == 
-0001d260: 2275 2229 2c0a 2020 2020 2020 2020 2020  "u"),.          
-0001d270: 2020 2273 625f 6d64 223a 2022 2220 6966    "sb_md": "" if
-0001d280: 2022 6e6f 5f73 625f 6d64 2220 696e 2076   "no_sb_md" in v
-0001d290: 6620 656c 7365 2028 7666 2e67 6574 2822  f else (vf.get("
-0001d2a0: 6d64 5f73 6266 2229 206f 7220 2279 2229  md_sbf") or "y")
-0001d2b0: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
-0001d2c0: 625f 6c67 223a 2022 2220 6966 2022 6e6f  b_lg": "" if "no
-0001d2d0: 5f73 625f 6c67 2220 696e 2076 6620 656c  _sb_lg" in vf el
-0001d2e0: 7365 2028 7666 2e67 6574 2822 6c67 5f73  se (vf.get("lg_s
-0001d2f0: 6266 2229 206f 7220 2279 2229 2c0a 2020  bf") or "y"),.  
-0001d300: 2020 2020 2020 2020 2020 2275 726c 5f73            "url_s
-0001d310: 7566 223a 2075 726c 5f73 7566 2c0a 2020  uf": url_suf,.  
-0001d320: 2020 2020 2020 2020 2020 226c 6f67 7565            "logue
-0001d330: 7322 3a20 6c6f 6775 6573 2c0a 2020 2020  s": logues,.    
-0001d340: 2020 2020 2020 2020 2272 6561 646d 6522          "readme"
-0001d350: 3a20 7265 6164 6d65 2c0a 2020 2020 2020  : readme,.      
-0001d360: 2020 2020 2020 2274 6974 6c65 223a 2068        "title": h
-0001d370: 746d 6c5f 6573 6361 7065 2873 656c 662e  tml_escape(self.
-0001d380: 7670 6174 682c 2063 726c 663d 5472 7565  vpath, crlf=True
-0001d390: 2920 6f72 2022 f09f 92be f09f 8e89 222c  ) or "........",
-0001d3a0: 0a20 2020 2020 2020 2020 2020 2022 7372  .            "sr
-0001d3b0: 765f 696e 666f 223a 2073 7276 5f69 6e66  v_info": srv_inf
-0001d3c0: 6f74 2c0a 2020 2020 2020 2020 2020 2020  ot,.            
-0001d3d0: 2264 6772 6964 223a 2022 6772 6964 2220  "dgrid": "grid" 
-0001d3e0: 696e 2076 662c 0a20 2020 2020 2020 2020  in vf,.         
-0001d3f0: 2020 2022 756e 6c69 7374 223a 2075 6e6c     "unlist": unl
-0001d400: 6973 742c 0a20 2020 2020 2020 2020 2020  ist,.           
-0001d410: 2022 6474 6865 6d65 223a 2073 656c 662e   "dtheme": self.
-0001d420: 6172 6773 2e74 6865 6d65 2c0a 2020 2020  args.theme,.    
-0001d430: 2020 2020 2020 2020 2274 6865 6d65 7322          "themes"
-0001d440: 3a20 7365 6c66 2e61 7267 732e 7468 656d  : self.args.them
-0001d450: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-0001d460: 2274 7572 626f 6c76 6c22 3a20 7365 6c66  "turbolvl": self
-0001d470: 2e61 7267 732e 7475 7262 6f2c 0a20 2020  .args.turbo,.   
-0001d480: 2020 2020 2020 2020 2022 6964 7868 223a           "idxh":
-0001d490: 2069 6e74 2873 656c 662e 6172 6773 2e69   int(self.args.i
-0001d4a0: 6829 2c0a 2020 2020 2020 2020 2020 2020  h),.            
-0001d4b0: 2275 3273 6f72 7422 3a20 7365 6c66 2e61  "u2sort": self.a
-0001d4c0: 7267 732e 7532 736f 7274 2c0a 2020 2020  rgs.u2sort,.    
-0001d4d0: 2020 2020 7d0a 0a20 2020 2020 2020 2069      }..        i
-0001d4e0: 6620 7365 6c66 2e61 7267 732e 6a73 5f62  f self.args.js_b
-0001d4f0: 726f 7773 6572 3a0a 2020 2020 2020 2020  rowser:.        
-0001d500: 2020 2020 6a32 615b 226a 7322 5d20 3d20      j2a["js"] = 
-0001d510: 7365 6c66 2e61 7267 732e 6a73 5f62 726f  self.args.js_bro
-0001d520: 7773 6572 0a0a 2020 2020 2020 2020 6966  wser..        if
-0001d530: 2073 656c 662e 6172 6773 2e63 7373 5f62   self.args.css_b
-0001d540: 726f 7773 6572 3a0a 2020 2020 2020 2020  rowser:.        
-0001d550: 2020 2020 6a32 615b 2263 7373 225d 203d      j2a["css"] =
-0001d560: 2073 656c 662e 6172 6773 2e63 7373 5f62   self.args.css_b
-0001d570: 726f 7773 6572 0a0a 2020 2020 2020 2020  rowser..        
-0001d580: 6966 206e 6f74 2073 656c 662e 636f 6e6e  if not self.conn
-0001d590: 2e68 7372 762e 7072 6973 6d3a 0a20 2020  .hsrv.prism:.   
-0001d5a0: 2020 2020 2020 2020 206a 3261 5b22 6e6f           j2a["no
-0001d5b0: 5f70 7269 736d 225d 203d 2054 7275 650a  _prism"] = True.
-0001d5c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0001d5d0: 7365 6c66 2e63 616e 5f72 6561 643a 0a20  self.can_read:. 
-0001d5e0: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0001d5f0: 5f6c 733a 0a20 2020 2020 2020 2020 2020  _ls:.           
-0001d600: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001d610: 2e74 785f 6c73 286c 735f 7265 7429 0a0a  .tx_ls(ls_ret)..
-0001d620: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001d630: 6f74 2073 7461 742e 535f 4953 4449 5228  ot stat.S_ISDIR(
-0001d640: 7374 2e73 745f 6d6f 6465 293a 0a20 2020  st.st_mode):.   
-0001d650: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0001d660: 7572 6e20 7365 6c66 2e74 785f 3430 3428  urn self.tx_404(
-0001d670: 5472 7565 290a 0a20 2020 2020 2020 2020  True)..         
-0001d680: 2020 2069 6620 227a 6970 2220 696e 2073     if "zip" in s
-0001d690: 656c 662e 7570 6172 616d 206f 7220 2274  elf.uparam or "t
-0001d6a0: 6172 2220 696e 2073 656c 662e 7570 6172  ar" in self.upar
-0001d6b0: 616d 3a0a 2020 2020 2020 2020 2020 2020  am:.            
-0001d6c0: 2020 2020 7261 6973 6520 5065 626b 6163      raise Pebkac
-0001d6d0: 2834 3033 290a 0a20 2020 2020 2020 2020  (403)..         
-0001d6e0: 2020 2068 746d 6c20 3d20 7365 6c66 2e6a     html = self.j
-0001d6f0: 3273 2874 706c 2c20 2a2a 6a32 6129 0a20  2s(tpl, **j2a). 
-0001d700: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001d710: 7265 706c 7928 6874 6d6c 2e65 6e63 6f64  reply(html.encod
-0001d720: 6528 2275 7466 2d38 222c 2022 7265 706c  e("utf-8", "repl
-0001d730: 6163 6522 2929 0a20 2020 2020 2020 2020  ace")).         
-0001d740: 2020 2072 6574 7572 6e20 5472 7565 0a0a     return True..
-0001d750: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-0001d760: 205b 227a 6970 222c 2022 7461 7222 5d3a   ["zip", "tar"]:
-0001d770: 0a20 2020 2020 2020 2020 2020 2076 203d  .            v =
-0001d780: 2073 656c 662e 7570 6172 616d 2e67 6574   self.uparam.get
-0001d790: 286b 290a 2020 2020 2020 2020 2020 2020  (k).            
-0001d7a0: 6966 2076 2069 7320 6e6f 7420 4e6f 6e65  if v is not None
-0001d7b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001d7c0: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
-0001d7d0: 5f7a 6970 286b 2c20 762c 2073 656c 662e  _zip(k, v, self.
-0001d7e0: 7670 6174 682c 2076 6e2c 2072 656d 2c20  vpath, vn, rem, 
-0001d7f0: 5b5d 2c20 7365 6c66 2e61 7267 732e 6564  [], self.args.ed
-0001d800: 290a 0a20 2020 2020 2020 2066 7372 6f6f  )..        fsroo
-0001d810: 742c 2076 6673 5f6c 732c 2076 6673 5f76  t, vfs_ls, vfs_v
-0001d820: 6972 7420 3d20 766e 2e6c 7328 0a20 2020  irt = vn.ls(.   
-0001d830: 2020 2020 2020 2020 2072 656d 2c0a 2020           rem,.  
-0001d840: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-0001d850: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0001d860: 2020 6e6f 7420 7365 6c66 2e61 7267 732e    not self.args.
-0001d870: 6e6f 5f73 6361 6e64 6972 2c0a 2020 2020  no_scandir,.    
-0001d880: 2020 2020 2020 2020 5b5b 5472 7565 2c20          [[True, 
-0001d890: 4661 6c73 655d 2c20 5b46 616c 7365 2c20  False], [False, 
-0001d8a0: 5472 7565 5d5d 2c0a 2020 2020 2020 2020  True]],.        
-0001d8b0: 2020 2020 6c73 7461 743d 226c 7422 2069      lstat="lt" i
-0001d8c0: 6e20 7365 6c66 2e75 7061 7261 6d2c 0a20  n self.uparam,. 
-0001d8d0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0001d8e0: 2073 7461 7473 203d 207b 6b3a 2076 2066   stats = {k: v f
-0001d8f0: 6f72 206b 2c20 7620 696e 2076 6673 5f6c  or k, v in vfs_l
-0001d900: 737d 0a20 2020 2020 2020 206c 735f 6e61  s}.        ls_na
-0001d910: 6d65 7320 3d20 5b78 5b30 5d20 666f 7220  mes = [x[0] for 
-0001d920: 7820 696e 2076 6673 5f6c 735d 0a20 2020  x in vfs_ls].   
-0001d930: 2020 2020 206c 735f 6e61 6d65 732e 6578       ls_names.ex
-0001d940: 7465 6e64 286c 6973 7428 7666 735f 7669  tend(list(vfs_vi
-0001d950: 7274 2e6b 6579 7328 2929 290a 0a20 2020  rt.keys()))..   
-0001d960: 2020 2020 2023 2063 6865 636b 2066 6f72       # check for
-0001d970: 206f 6c64 2076 6572 7369 6f6e 7320 6f66   old versions of
-0001d980: 2066 696c 6573 2c0a 2020 2020 2020 2020   files,.        
-0001d990: 2320 5b6e 756d 2d62 6163 6b75 7073 2c20  # [num-backups, 
-0001d9a0: 6d6f 7374 2d72 6563 656e 742c 2068 6973  most-recent, his
-0001d9b0: 742d 7061 7468 5d0a 2020 2020 2020 2020  t-path].        
-0001d9c0: 6869 7374 2020 2020 203d 207b 7d0a 2020  hist     = {}.  
-0001d9d0: 2020 2020 2020 6869 7374 6469 7220 3d20        histdir = 
-0001d9e0: 6f73 2e70 6174 682e 6a6f 696e 2866 7372  os.path.join(fsr
-0001d9f0: 6f6f 742c 2022 2e68 6973 7422 290a 2020  oot, ".hist").  
-0001da00: 2020 2020 2020 7074 6e20 3d20 7265 2e63        ptn = re.c
-0001da10: 6f6d 7069 6c65 2872 2228 2e2a 295c 2e28  ompile(r"(.*)\.(
-0001da20: 5b30 2d39 5d2b 5c2e 5b30 2d39 5d7b 337d  [0-9]+\.[0-9]{3}
-0001da30: 2928 5c2e 5b5e 5c2e 5d2b 2924 2229 0a20  )(\.[^\.]+)$"). 
-0001da40: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-0001da50: 2020 2020 2020 2020 666f 7220 6866 6e20          for hfn 
-0001da60: 696e 2062 6f73 2e6c 6973 7464 6972 2868  in bos.listdir(h
-0001da70: 6973 7464 6972 293a 0a20 2020 2020 2020  istdir):.       
-0001da80: 2020 2020 2020 2020 206d 203d 2070 746e           m = ptn
-0001da90: 2e6d 6174 6368 2868 666e 290a 2020 2020  .match(hfn).    
-0001daa0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0001dab0: 6f74 206d 3a0a 2020 2020 2020 2020 2020  ot m:.          
-0001dac0: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0001dad0: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-0001dae0: 2020 2020 666e 203d 206d 2e67 726f 7570      fn = m.group
-0001daf0: 2831 2920 2b20 6d2e 6772 6f75 7028 3329  (1) + m.group(3)
-0001db00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001db10: 206e 2c20 7473 2c20 5f20 3d20 6869 7374   n, ts, _ = hist
-0001db20: 2e67 6574 2866 6e2c 2028 302c 2030 2c20  .get(fn, (0, 0, 
-0001db30: 2222 2929 0a20 2020 2020 2020 2020 2020  "")).           
-0001db40: 2020 2020 2068 6973 745b 666e 5d20 3d20       hist[fn] = 
-0001db50: 286e 202b 2031 2c20 6d61 7828 7473 2c20  (n + 1, max(ts, 
-0001db60: 666c 6f61 7428 6d2e 6772 6f75 7028 3229  float(m.group(2)
-0001db70: 2929 2c20 6866 6e29 0a20 2020 2020 2020  )), hfn).       
-0001db80: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-0001db90: 2020 2020 2070 6173 730a 0a20 2020 2020       pass..     
-0001dba0: 2020 2023 2073 686f 7720 646f 7466 696c     # show dotfil
-0001dbb0: 6573 2069 6620 7065 726d 6974 7465 6420  es if permitted 
-0001dbc0: 616e 6420 7265 7175 6573 7465 640a 2020  and requested.  
-0001dbd0: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-0001dbe0: 662e 6172 6773 2e65 6420 6f72 2022 646f  f.args.ed or "do
-0001dbf0: 7473 2220 6e6f 7420 696e 2073 656c 662e  ts" not in self.
-0001dc00: 7570 6172 616d 3a0a 2020 2020 2020 2020  uparam:.        
-0001dc10: 2020 2020 6c73 5f6e 616d 6573 203d 2065      ls_names = e
-0001dc20: 7863 6c75 6465 5f64 6f74 6669 6c65 7328  xclude_dotfiles(
-0001dc30: 6c73 5f6e 616d 6573 290a 0a20 2020 2020  ls_names)..     
-0001dc40: 2020 2061 6464 5f66 6b20 3d20 766e 2e66     add_fk = vn.f
-0001dc50: 6c61 6773 2e67 6574 2822 666b 2229 0a0a  lags.get("fk")..
-0001dc60: 2020 2020 2020 2020 6469 7273 203d 205b          dirs = [
-0001dc70: 5d0a 2020 2020 2020 2020 6669 6c65 7320  ].        files 
-0001dc80: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-0001dc90: 2066 6e20 696e 206c 735f 6e61 6d65 733a   fn in ls_names:
-0001dca0: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-0001dcb0: 6520 3d20 2222 0a20 2020 2020 2020 2020  e = "".         
-0001dcc0: 2020 2068 7265 6620 3d20 666e 0a20 2020     href = fn.   
-0001dcd0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0001dce0: 6973 5f6c 7320 616e 6420 6e6f 7420 6973  is_ls and not is
-0001dcf0: 5f6a 7320 616e 6420 6e6f 7420 7365 6c66  _js and not self
-0001dd00: 2e74 7261 696c 696e 675f 736c 6173 6820  .trailing_slash 
-0001dd10: 616e 6420 7670 6174 683a 0a20 2020 2020  and vpath:.     
-0001dd20: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0001dd30: 3d20 222f 2220 2b20 7670 6174 6820 2b20  = "/" + vpath + 
-0001dd40: 222f 220a 2020 2020 2020 2020 2020 2020  "/".            
-0001dd50: 2020 2020 6872 6566 203d 2062 6173 6520      href = base 
-0001dd60: 2b20 666e 0a0a 2020 2020 2020 2020 2020  + fn..          
-0001dd70: 2020 6966 2066 6e20 696e 2076 6673 5f76    if fn in vfs_v
-0001dd80: 6972 743a 0a20 2020 2020 2020 2020 2020  irt:.           
-0001dd90: 2020 2020 2066 7370 6174 6820 3d20 7666       fspath = vf
-0001dda0: 735f 7669 7274 5b66 6e5d 2e72 6561 6c70  s_virt[fn].realp
-0001ddb0: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
-0001ddc0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001ddd0: 2020 2020 2020 6673 7061 7468 203d 2066        fspath = f
-0001dde0: 7372 6f6f 7420 2b20 222f 2220 2b20 666e  sroot + "/" + fn
-0001ddf0: 0a0a 2020 2020 2020 2020 2020 2020 7472  ..            tr
-0001de00: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0001de10: 2020 206c 696e 6620 3d20 7374 6174 732e     linf = stats.
-0001de20: 6765 7428 666e 2920 6f72 2062 6f73 2e6c  get(fn) or bos.l
-0001de30: 7374 6174 2866 7370 6174 6829 0a20 2020  stat(fspath).   
-0001de40: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-0001de50: 203d 2062 6f73 2e73 7461 7428 6673 7061   = bos.stat(fspa
-0001de60: 7468 2920 6966 2073 7461 742e 535f 4953  th) if stat.S_IS
-0001de70: 4c4e 4b28 6c69 6e66 2e73 745f 6d6f 6465  LNK(linf.st_mode
-0001de80: 2920 656c 7365 206c 696e 660a 2020 2020  ) else linf.    
-0001de90: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-0001dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001deb0: 7365 6c66 2e6c 6f67 2822 6272 6f6b 656e  self.log("broken
-0001dec0: 2073 796d 6c69 6e6b 3a20 7b7d 222e 666f   symlink: {}".fo
-0001ded0: 726d 6174 2872 6570 7228 6673 7061 7468  rmat(repr(fspath
-0001dee0: 2929 290a 2020 2020 2020 2020 2020 2020  ))).            
-0001def0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-0001df00: 2020 2020 2020 2020 2020 6973 5f64 6972            is_dir
-0001df10: 203d 2073 7461 742e 535f 4953 4449 5228   = stat.S_ISDIR(
-0001df20: 696e 662e 7374 5f6d 6f64 6529 0a20 2020  inf.st_mode).   
-0001df30: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
-0001df40: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-0001df50: 2020 2020 6872 6566 202b 3d20 222f 220a      href += "/".
-0001df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df70: 6966 2073 656c 662e 6172 6773 2e6e 6f5f  if self.args.no_
-0001df80: 7a69 703a 0a20 2020 2020 2020 2020 2020  zip:.           
-0001df90: 2020 2020 2020 2020 206d 6172 6769 6e20           margin 
-0001dfa0: 3d20 2244 4952 220a 2020 2020 2020 2020  = "DIR".        
-0001dfb0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfd0: 2020 6d61 7267 696e 203d 2027 3c61 2068    margin = '<a h
-0001dfe0: 7265 663d 2225 733f 7a69 7022 2072 656c  ref="%s?zip" rel
-0001dff0: 3d22 6e6f 666f 6c6c 6f77 223e 7a69 703c  ="nofollow">zip<
-0001e000: 2f61 3e27 2025 2028 7175 6f74 6570 2868  /a>' % (quotep(h
-0001e010: 7265 6629 2c29 0a20 2020 2020 2020 2020  ref),).         
-0001e020: 2020 2065 6c69 6620 666e 2069 6e20 6869     elif fn in hi
-0001e030: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
-0001e040: 2020 2020 6d61 7267 696e 203d 2027 3c61      margin = '<a
-0001e050: 2068 7265 663d 2225 732e 6869 7374 2f25   href="%s.hist/%
-0001e060: 7322 3e23 2573 3c2f 613e 2720 2520 280a  s">#%s</a>' % (.
-0001e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e080: 2020 2020 6261 7365 2c0a 2020 2020 2020      base,.      
-0001e090: 2020 2020 2020 2020 2020 2020 2020 6874                ht
-0001e0a0: 6d6c 5f65 7363 6170 6528 6869 7374 5b66  ml_escape(hist[f
-0001e0b0: 6e5d 5b32 5d2c 2071 756f 743d 5472 7565  n][2], quot=True
-0001e0c0: 2c20 6372 6c66 3d54 7275 6529 2c0a 2020  , crlf=True),.  
-0001e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0e0: 2020 6869 7374 5b66 6e5d 5b30 5d2c 0a20    hist[fn][0],. 
-0001e0f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001e100: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001e110: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0001e120: 2020 206d 6172 6769 6e20 3d20 222d 220a     margin = "-".
-0001e130: 0a20 2020 2020 2020 2020 2020 2073 7a20  .            sz 
-0001e140: 3d20 696e 662e 7374 5f73 697a 650a 2020  = inf.st_size.  
-0001e150: 2020 2020 2020 2020 2020 7a64 203d 2064            zd = d
-0001e160: 6174 6574 696d 652e 7574 6366 726f 6d74  atetime.utcfromt
-0001e170: 696d 6573 7461 6d70 286c 696e 662e 7374  imestamp(linf.st
-0001e180: 5f6d 7469 6d65 290a 2020 2020 2020 2020  _mtime).        
-0001e190: 2020 2020 6474 203d 2022 2530 3464 2d25      dt = "%04d-%
-0001e1a0: 3032 642d 2530 3264 2025 3032 643a 2530  02d-%02d %02d:%0
-0001e1b0: 3264 3a25 3032 6422 2025 2028 0a20 2020  2d:%02d" % (.   
-0001e1c0: 2020 2020 2020 2020 2020 2020 207a 642e               zd.
-0001e1d0: 7965 6172 2c0a 2020 2020 2020 2020 2020  year,.          
-0001e1e0: 2020 2020 2020 7a64 2e6d 6f6e 7468 2c0a        zd.month,.
-0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e200: 7a64 2e64 6179 2c0a 2020 2020 2020 2020  zd.day,.        
-0001e210: 2020 2020 2020 2020 7a64 2e68 6f75 722c          zd.hour,
-0001e220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e230: 207a 642e 6d69 6e75 7465 2c0a 2020 2020   zd.minute,.    
-0001e240: 2020 2020 2020 2020 2020 2020 7a64 2e73              zd.s
-0001e250: 6563 6f6e 642c 0a20 2020 2020 2020 2020  econd,.         
-0001e260: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-0001e270: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0001e280: 2020 2020 2020 2065 7874 203d 2022 2d2d         ext = "--
-0001e290: 2d22 2069 6620 6973 5f64 6972 2065 6c73  -" if is_dir els
-0001e2a0: 6520 666e 2e72 7370 6c69 7428 222e 222c  e fn.rsplit(".",
-0001e2b0: 2031 295b 315d 0a20 2020 2020 2020 2020   1)[1].         
-0001e2c0: 2020 2020 2020 2069 6620 6c65 6e28 6578         if len(ex
-0001e2d0: 7429 203e 2031 363a 0a20 2020 2020 2020  t) > 16:.       
-0001e2e0: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-0001e2f0: 203d 2065 7874 5b3a 3136 5d0a 2020 2020   = ext[:16].    
-0001e300: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
-0001e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e320: 6578 7420 3d20 2225 220a 0a20 2020 2020  ext = "%"..     
-0001e330: 2020 2020 2020 2069 6620 6164 645f 666b         if add_fk
-0001e340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001e350: 2020 6872 6566 203d 2022 2573 3f6b 3d25    href = "%s?k=%
-0001e360: 7322 2025 2028 0a20 2020 2020 2020 2020  s" % (.         
-0001e370: 2020 2020 2020 2020 2020 2071 756f 7465             quote
-0001e380: 7028 6872 6566 292c 0a20 2020 2020 2020  p(href),.       
-0001e390: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001e3a0: 662e 6765 6e5f 666b 280a 2020 2020 2020  f.gen_fk(.      
-0001e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3c0: 2020 7365 6c66 2e61 7267 732e 666b 5f73    self.args.fk_s
-0001e3d0: 616c 742c 2066 7370 6174 682c 2073 7a2c  alt, fspath, sz,
-0001e3e0: 2030 2069 6620 414e 5957 494e 2065 6c73   0 if ANYWIN els
-0001e3f0: 6520 696e 662e 7374 5f69 6e6f 0a20 2020  e inf.st_ino.   
+0001bed0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
+0001bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bef0: 2020 2020 7061 7373 0a20 2020 2020 2020      pass.       
+0001bf00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0001bf10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001bf20: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0001bf30: 6e20 696e 2073 656c 662e 6172 6773 2e74  n in self.args.t
+0001bf40: 685f 636f 7665 7273 3a0a 2020 2020 2020  h_covers:.      
+0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf60: 2020 2020 2020 6670 203d 206f 732e 7061        fp = os.pa
+0001bf70: 7468 2e6a 6f69 6e28 6162 7370 6174 682c  th.join(abspath,
+0001bf80: 2066 6e29 0a20 2020 2020 2020 2020 2020   fn).           
+0001bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bfa0: 2069 6620 626f 732e 7061 7468 2e65 7869   if bos.path.exi
+0001bfb0: 7374 7328 6670 293a 0a20 2020 2020 2020  sts(fp):.       
+0001bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bfd0: 2020 2020 2020 2020 2076 7265 6d20 3d20           vrem = 
+0001bfe0: 227b 7d2f 7b7d 222e 666f 726d 6174 2876  "{}/{}".format(v
+0001bff0: 7265 6d2c 2066 6e29 2e73 7472 6970 2822  rem, fn).strip("
+0001c000: 2f22 290a 2020 2020 2020 2020 2020 2020  /").            
+0001c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c020: 2020 2020 6973 5f64 6972 203d 2046 616c      is_dir = Fal
+0001c030: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+0001c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c050: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+0001c060: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001c070: 2069 735f 6469 723a 0a20 2020 2020 2020   is_dir:.       
+0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c090: 2072 6574 7572 6e20 7365 6c66 2e74 785f   return self.tx_
+0001c0a0: 6963 6f28 2261 2e66 6f6c 6465 7222 290a  ico("a.folder").
+0001c0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c0c0: 2074 6870 203d 204e 6f6e 650a 2020 2020   thp = None.    
+0001c0d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001c0e0: 656c 662e 7468 756d 6263 6c69 3a0a 2020  elf.thumbcli:.  
+0001c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c100: 2020 7468 7020 3d20 7365 6c66 2e74 6875    thp = self.thu
+0001c110: 6d62 636c 692e 6765 7428 6462 762c 2076  mbcli.get(dbv, v
+0001c120: 7265 6d2c 2069 6e74 2873 742e 7374 5f6d  rem, int(st.st_m
+0001c130: 7469 6d65 292c 2074 685f 666d 7429 0a0a  time), th_fmt)..
+0001c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c150: 6966 2074 6870 3a0a 2020 2020 2020 2020  if thp:.        
+0001c160: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0001c170: 726e 2073 656c 662e 7478 5f66 696c 6528  rn self.tx_file(
+0001c180: 7468 7029 0a0a 2020 2020 2020 2020 2020  thp)..          
+0001c190: 2020 2020 2020 6966 2074 685f 666d 7420        if th_fmt 
+0001c1a0: 3d3d 2022 7022 3a0a 2020 2020 2020 2020  == "p":.        
+0001c1b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+0001c1c0: 6520 5065 626b 6163 2834 3034 290a 0a20  e Pebkac(404).. 
+0001c1d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001c1e0: 6574 7572 6e20 7365 6c66 2e74 785f 6963  eturn self.tx_ic
+0001c1f0: 6f28 7265 6d29 0a0a 2020 2020 2020 2020  o(rem)..        
+0001c200: 6966 206e 6f74 2069 735f 6469 7220 616e  if not is_dir an
+0001c210: 6420 2873 656c 662e 6361 6e5f 7265 6164  d (self.can_read
+0001c220: 206f 7220 7365 6c66 2e63 616e 5f67 6574   or self.can_get
+0001c230: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+0001c240: 6620 6e6f 7420 7365 6c66 2e63 616e 5f72  f not self.can_r
+0001c250: 6561 6420 616e 6420 2266 6b22 2069 6e20  ead and "fk" in 
+0001c260: 766e 2e66 6c61 6773 3a0a 2020 2020 2020  vn.flags:.      
+0001c270: 2020 2020 2020 2020 2020 636f 7272 6563            correc
+0001c280: 7420 3d20 7365 6c66 2e67 656e 5f66 6b28  t = self.gen_fk(
+0001c290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c2a0: 2020 2020 2073 656c 662e 6172 6773 2e66       self.args.f
+0001c2b0: 6b5f 7361 6c74 2c20 6162 7370 6174 682c  k_salt, abspath,
+0001c2c0: 2073 742e 7374 5f73 697a 652c 2030 2069   st.st_size, 0 i
+0001c2d0: 6620 414e 5957 494e 2065 6c73 6520 7374  f ANYWIN else st
+0001c2e0: 2e73 745f 696e 6f0a 2020 2020 2020 2020  .st_ino.        
+0001c2f0: 2020 2020 2020 2020 295b 3a20 766e 2e66          )[: vn.f
+0001c300: 6c61 6773 5b22 666b 225d 5d0a 2020 2020  lags["fk"]].    
+0001c310: 2020 2020 2020 2020 2020 2020 676f 7420              got 
+0001c320: 3d20 7365 6c66 2e75 7061 7261 6d2e 6765  = self.uparam.ge
+0001c330: 7428 226b 2229 0a20 2020 2020 2020 2020  t("k").         
+0001c340: 2020 2020 2020 2069 6620 676f 7420 213d         if got !=
+0001c350: 2063 6f72 7265 6374 3a0a 2020 2020 2020   correct:.      
+0001c360: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001c370: 6c66 2e6c 6f67 2822 7772 6f6e 6720 6669  lf.log("wrong fi
+0001c380: 6c65 6b65 792c 2077 616e 7420 7b7d 2c20  lekey, want {}, 
+0001c390: 676f 7420 7b7d 222e 666f 726d 6174 2863  got {}".format(c
+0001c3a0: 6f72 7265 6374 2c20 676f 7429 290a 2020  orrect, got)).  
+0001c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3c0: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+0001c3d0: 5f34 3034 2829 0a0a 2020 2020 2020 2020  _404()..        
+0001c3e0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+0001c3f0: 2020 2020 2020 2020 2061 6273 7061 7468           abspath
+0001c400: 2e65 6e64 7377 6974 6828 222e 6d64 2229  .endswith(".md")
+0001c410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c420: 2061 6e64 2022 6e6f 6874 6d6c 2220 6e6f   and "nohtml" no
+0001c430: 7420 696e 2076 6e2e 666c 6167 730a 2020  t in vn.flags.  
+0001c440: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0001c450: 6420 280a 2020 2020 2020 2020 2020 2020  d (.            
+0001c460: 2020 2020 2020 2020 2276 2220 696e 2073          "v" in s
+0001c470: 656c 662e 7570 6172 616d 0a20 2020 2020  elf.uparam.     
+0001c480: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001c490: 7220 2265 6469 7422 2069 6e20 7365 6c66  r "edit" in self
+0001c4a0: 2e75 7061 7261 6d0a 2020 2020 2020 2020  .uparam.        
+0001c4b0: 2020 2020 2020 2020 2020 2020 6f72 2022              or "
+0001c4c0: 6564 6974 3222 2069 6e20 7365 6c66 2e75  edit2" in self.u
+0001c4d0: 7061 7261 6d0a 2020 2020 2020 2020 2020  param.          
+0001c4e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0001c4f0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0001c500: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001c510: 6c66 2e74 785f 6d64 2861 6273 7061 7468  lf.tx_md(abspath
+0001c520: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
+0001c530: 6574 7572 6e20 7365 6c66 2e74 785f 6669  eturn self.tx_fi
+0001c540: 6c65 2861 6273 7061 7468 290a 0a20 2020  le(abspath)..   
+0001c550: 2020 2020 2065 6c69 6620 6973 5f64 6972       elif is_dir
+0001c560: 2061 6e64 206e 6f74 2073 656c 662e 6361   and not self.ca
+0001c570: 6e5f 7265 6164 2061 6e64 206e 6f74 2073  n_read and not s
+0001c580: 656c 662e 6361 6e5f 7772 6974 653a 0a20  elf.can_write:. 
+0001c590: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001c5a0: 6e20 7365 6c66 2e74 785f 3430 3428 5472  n self.tx_404(Tr
+0001c5b0: 7565 290a 0a20 2020 2020 2020 2073 7276  ue)..        srv
+0001c5c0: 5f69 6e66 6f20 3d20 5b5d 0a0a 2020 2020  _info = []..    
+0001c5d0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0001c5e0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0001c5f0: 2e61 7267 732e 6e69 683a 0a20 2020 2020  .args.nih:.     
+0001c600: 2020 2020 2020 2020 2020 2073 7276 5f69             srv_i
+0001c610: 6e66 6f2e 6170 7065 6e64 2873 656c 662e  nfo.append(self.
+0001c620: 6172 6773 2e6e 616d 6529 0a20 2020 2020  args.name).     
+0001c630: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+0001c640: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
+0001c650: 2223 776f 7720 2377 686f 6122 290a 0a20  "#wow #whoa").. 
+0001c660: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0001c670: 6c66 2e61 7267 732e 6e69 643a 0a20 2020  lf.args.nid:.   
+0001c680: 2020 2020 2020 2020 2066 7265 652c 2074           free, t
+0001c690: 6f74 616c 203d 2067 6574 5f64 6628 6162  otal = get_df(ab
+0001c6a0: 7370 6174 6829 0a20 2020 2020 2020 2020  spath).         
+0001c6b0: 2020 2069 6620 746f 7461 6c20 6973 206e     if total is n
+0001c6c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0001c6d0: 2020 2020 2020 2020 2068 3120 3d20 6875           h1 = hu
+0001c6e0: 6d61 6e73 697a 6528 6672 6565 206f 7220  mansize(free or 
+0001c6f0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+0001c700: 2020 2068 3220 3d20 6875 6d61 6e73 697a     h2 = humansiz
+0001c710: 6528 746f 7461 6c29 0a20 2020 2020 2020  e(total).       
+0001c720: 2020 2020 2020 2020 2073 7276 5f69 6e66           srv_inf
+0001c730: 6f2e 6170 7065 6e64 2822 7b7d 2066 7265  o.append("{} fre
+0001c740: 6520 6f66 207b 7d22 2e66 6f72 6d61 7428  e of {}".format(
+0001c750: 6831 2c20 6832 2929 0a20 2020 2020 2020  h1, h2)).       
+0001c760: 2020 2020 2065 6c69 6620 6672 6565 2069       elif free i
+0001c770: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0001c780: 2020 2020 2020 2020 2020 2020 7372 765f              srv_
+0001c790: 696e 666f 2e61 7070 656e 6428 6875 6d61  info.append(huma
+0001c7a0: 6e73 697a 6528 6672 6565 2c20 5472 7565  nsize(free, True
+0001c7b0: 2920 2b20 2220 6672 6565 2229 0a0a 2020  ) + " free")..  
+0001c7c0: 2020 2020 2020 7372 765f 696e 666f 7420        srv_infot 
+0001c7d0: 3d20 223c 2f73 7061 6e3e 202f 2f20 3c73  = "</span> // <s
+0001c7e0: 7061 6e3e 222e 6a6f 696e 2873 7276 5f69  pan>".join(srv_i
+0001c7f0: 6e66 6f29 0a0a 2020 2020 2020 2020 7065  nfo)..        pe
+0001c800: 726d 7320 3d20 5b5d 0a20 2020 2020 2020  rms = [].       
+0001c810: 2069 6620 7365 6c66 2e63 616e 5f72 6561   if self.can_rea
+0001c820: 643a 0a20 2020 2020 2020 2020 2020 2070  d:.            p
+0001c830: 6572 6d73 2e61 7070 656e 6428 2272 6561  erms.append("rea
+0001c840: 6422 290a 2020 2020 2020 2020 6966 2073  d").        if s
+0001c850: 656c 662e 6361 6e5f 7772 6974 653a 0a20  elf.can_write:. 
+0001c860: 2020 2020 2020 2020 2020 2070 6572 6d73             perms
+0001c870: 2e61 7070 656e 6428 2277 7269 7465 2229  .append("write")
+0001c880: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001c890: 2e63 616e 5f6d 6f76 653a 0a20 2020 2020  .can_move:.     
+0001c8a0: 2020 2020 2020 2070 6572 6d73 2e61 7070         perms.app
+0001c8b0: 656e 6428 226d 6f76 6522 290a 2020 2020  end("move").    
+0001c8c0: 2020 2020 6966 2073 656c 662e 6361 6e5f      if self.can_
+0001c8d0: 6465 6c65 7465 3a0a 2020 2020 2020 2020  delete:.        
+0001c8e0: 2020 2020 7065 726d 732e 6170 7065 6e64      perms.append
+0001c8f0: 2822 6465 6c65 7465 2229 0a20 2020 2020  ("delete").     
+0001c900: 2020 2069 6620 7365 6c66 2e63 616e 5f67     if self.can_g
+0001c910: 6574 3a0a 2020 2020 2020 2020 2020 2020  et:.            
+0001c920: 7065 726d 732e 6170 7065 6e64 2822 6765  perms.append("ge
+0001c930: 7422 290a 2020 2020 2020 2020 6966 2073  t").        if s
+0001c940: 656c 662e 6361 6e5f 7570 6765 743a 0a20  elf.can_upget:. 
+0001c950: 2020 2020 2020 2020 2020 2070 6572 6d73             perms
+0001c960: 2e61 7070 656e 6428 2275 7067 6574 2229  .append("upget")
+0001c970: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001c980: 2e63 616e 5f61 646d 696e 3a0a 2020 2020  .can_admin:.    
+0001c990: 2020 2020 2020 2020 7065 726d 732e 6170          perms.ap
+0001c9a0: 7065 6e64 2822 6164 6d69 6e22 290a 0a20  pend("admin").. 
+0001c9b0: 2020 2020 2020 2075 726c 5f73 7566 203d         url_suf =
+0001c9c0: 2073 656c 662e 7572 6c71 287b 7d2c 205b   self.urlq({}, [
+0001c9d0: 226b 225d 290a 2020 2020 2020 2020 6973  "k"]).        is
+0001c9e0: 5f6c 7320 3d20 226c 7322 2069 6e20 7365  _ls = "ls" in se
+0001c9f0: 6c66 2e75 7061 7261 6d0a 2020 2020 2020  lf.uparam.      
+0001ca00: 2020 6973 5f6a 7320 3d20 7365 6c66 2e61    is_js = self.a
+0001ca10: 7267 732e 666f 7263 655f 6a73 206f 7220  rgs.force_js or 
+0001ca20: 7365 6c66 2e63 6f6f 6b69 6573 2e67 6574  self.cookies.get
+0001ca30: 2822 6a73 2229 203d 3d20 2279 220a 0a20  ("js") == "y".. 
+0001ca40: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
+0001ca50: 5f6c 7320 616e 6420 2873 656c 662e 7561  _ls and (self.ua
+0001ca60: 2e73 7461 7274 7377 6974 6828 2263 7572  .startswith("cur
+0001ca70: 6c2f 2229 206f 7220 7365 6c66 2e75 612e  l/") or self.ua.
+0001ca80: 7374 6172 7473 7769 7468 2822 6665 7463  startswith("fetc
+0001ca90: 6822 2929 3a0a 2020 2020 2020 2020 2020  h")):.          
+0001caa0: 2020 7365 6c66 2e75 7061 7261 6d5b 226c    self.uparam["l
+0001cab0: 7322 5d20 3d20 2276 220a 2020 2020 2020  s"] = "v".      
+0001cac0: 2020 2020 2020 6973 5f6c 7320 3d20 5472        is_ls = Tr
+0001cad0: 7565 0a0a 2020 2020 2020 2020 7470 6c20  ue..        tpl 
+0001cae0: 3d20 2262 726f 7773 6572 220a 2020 2020  = "browser".    
+0001caf0: 2020 2020 6966 2022 6222 2069 6e20 7365      if "b" in se
+0001cb00: 6c66 2e75 7061 7261 6d3a 0a20 2020 2020  lf.uparam:.     
+0001cb10: 2020 2020 2020 2074 706c 203d 2022 6272         tpl = "br
+0001cb20: 6f77 7365 7232 220a 2020 2020 2020 2020  owser2".        
+0001cb30: 2020 2020 6973 5f6a 7320 3d20 4661 6c73      is_js = Fals
+0001cb40: 650a 0a20 2020 2020 2020 206c 6f67 7565  e..        logue
+0001cb50: 7320 3d20 5b22 222c 2022 225d 0a20 2020  s = ["", ""].   
+0001cb60: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0001cb70: 2e61 7267 732e 6e6f 5f6c 6f67 7565 733a  .args.no_logues:
+0001cb80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0001cb90: 206e 2c20 666e 2069 6e20 656e 756d 6572   n, fn in enumer
+0001cba0: 6174 6528 5b22 2e70 726f 6c6f 6775 652e  ate([".prologue.
+0001cbb0: 6874 6d6c 222c 2022 2e65 7069 6c6f 6775  html", ".epilogu
+0001cbc0: 652e 6874 6d6c 225d 293a 0a20 2020 2020  e.html"]):.     
+0001cbd0: 2020 2020 2020 2020 2020 2066 6e20 3d20             fn = 
+0001cbe0: 6f73 2e70 6174 682e 6a6f 696e 2861 6273  os.path.join(abs
+0001cbf0: 7061 7468 2c20 666e 290a 2020 2020 2020  path, fn).      
+0001cc00: 2020 2020 2020 2020 2020 6966 2062 6f73            if bos
+0001cc10: 2e70 6174 682e 6578 6973 7473 2866 6e29  .path.exists(fn)
+0001cc20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001cc30: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+0001cc40: 6673 656e 6328 666e 292c 2022 7262 2229  fsenc(fn), "rb")
+0001cc50: 2061 7320 663a 0a20 2020 2020 2020 2020   as f:.         
+0001cc60: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0001cc70: 6f67 7565 735b 6e5d 203d 2066 2e72 6561  ogues[n] = f.rea
+0001cc80: 6428 292e 6465 636f 6465 2822 7574 662d  d().decode("utf-
+0001cc90: 3822 290a 0a20 2020 2020 2020 2072 6561  8")..        rea
+0001cca0: 646d 6520 3d20 2222 0a20 2020 2020 2020  dme = "".       
+0001ccb0: 2069 6620 6e6f 7420 7365 6c66 2e61 7267   if not self.arg
+0001ccc0: 732e 6e6f 5f72 6561 646d 6520 616e 6420  s.no_readme and 
+0001ccd0: 6e6f 7420 6c6f 6775 6573 5b31 5d3a 0a20  not logues[1]:. 
+0001cce0: 2020 2020 2020 2020 2020 2066 6f72 2066             for f
+0001ccf0: 6e20 696e 205b 2252 4541 444d 452e 6d64  n in ["README.md
+0001cd00: 222c 2022 7265 6164 6d65 2e6d 6422 5d3a  ", "readme.md"]:
+0001cd10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001cd20: 2066 6e20 3d20 6f73 2e70 6174 682e 6a6f   fn = os.path.jo
+0001cd30: 696e 2861 6273 7061 7468 2c20 666e 290a  in(abspath, fn).
+0001cd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cd50: 6966 2062 6f73 2e70 6174 682e 6973 6669  if bos.path.isfi
+0001cd60: 6c65 2866 6e29 3a0a 2020 2020 2020 2020  le(fn):.        
+0001cd70: 2020 2020 2020 2020 2020 2020 7769 7468              with
+0001cd80: 206f 7065 6e28 6673 656e 6328 666e 292c   open(fsenc(fn),
+0001cd90: 2022 7262 2229 2061 7320 663a 0a20 2020   "rb") as f:.   
+0001cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cdb0: 2020 2020 2072 6561 646d 6520 3d20 662e       readme = f.
+0001cdc0: 7265 6164 2829 2e64 6563 6f64 6528 2275  read().decode("u
+0001cdd0: 7466 2d38 2229 0a20 2020 2020 2020 2020  tf-8").         
+0001cde0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0001cdf0: 7265 616b 0a0a 2020 2020 2020 2020 7666  reak..        vf
+0001ce00: 203d 2076 6e2e 666c 6167 730a 2020 2020   = vn.flags.    
+0001ce10: 2020 2020 756e 6c69 7374 203d 2076 662e      unlist = vf.
+0001ce20: 6765 7428 2275 6e6c 6973 7422 2c20 2222  get("unlist", ""
+0001ce30: 290a 2020 2020 2020 2020 6c73 5f72 6574  ).        ls_ret
+0001ce40: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
+0001ce50: 2022 6469 7273 223a 205b 5d2c 0a20 2020   "dirs": [],.   
+0001ce60: 2020 2020 2020 2020 2022 6669 6c65 7322           "files"
+0001ce70: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+0001ce80: 2020 2274 6167 6c69 7374 223a 205b 5d2c    "taglist": [],
+0001ce90: 0a20 2020 2020 2020 2020 2020 2022 7372  .            "sr
+0001cea0: 7669 6e66 223a 2073 7276 5f69 6e66 6f74  vinf": srv_infot
+0001ceb0: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
+0001cec0: 6363 7422 3a20 7365 6c66 2e75 6e61 6d65  cct": self.uname
+0001ced0: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
+0001cee0: 6478 223a 2065 3264 2c0a 2020 2020 2020  dx": e2d,.      
+0001cef0: 2020 2020 2020 2269 7461 6722 3a20 6532        "itag": e2
+0001cf00: 742c 0a20 2020 2020 2020 2020 2020 2022  t,.            "
+0001cf10: 6c69 6665 7469 6d65 223a 2076 6e2e 666c  lifetime": vn.fl
+0001cf20: 6167 732e 6765 7428 226c 6966 6574 696d  ags.get("lifetim
+0001cf30: 6522 2920 6f72 2030 2c0a 2020 2020 2020  e") or 0,.      
+0001cf40: 2020 2020 2020 2266 7261 6e64 223a 2062        "frand": b
+0001cf50: 6f6f 6c28 766e 2e66 6c61 6773 2e67 6574  ool(vn.flags.get
+0001cf60: 2822 7261 6e64 2229 292c 0a20 2020 2020  ("rand")),.     
+0001cf70: 2020 2020 2020 2022 756e 6c69 7374 223a         "unlist":
+0001cf80: 2075 6e6c 6973 742c 0a20 2020 2020 2020   unlist,.       
+0001cf90: 2020 2020 2022 7065 726d 7322 3a20 7065       "perms": pe
+0001cfa0: 726d 732c 0a20 2020 2020 2020 2020 2020  rms,.           
+0001cfb0: 2022 6c6f 6775 6573 223a 206c 6f67 7565   "logues": logue
+0001cfc0: 732c 0a20 2020 2020 2020 2020 2020 2022  s,.            "
+0001cfd0: 7265 6164 6d65 223a 2072 6561 646d 652c  readme": readme,
+0001cfe0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+0001cff0: 2020 206a 3261 203d 207b 0a20 2020 2020     j2a = {.     
+0001d000: 2020 2020 2020 2022 7664 6972 223a 2071         "vdir": q
+0001d010: 756f 7465 7028 7365 6c66 2e76 7061 7468  uotep(self.vpath
+0001d020: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
+0001d030: 7670 6e6f 6465 7322 3a20 7670 6e6f 6465  vpnodes": vpnode
+0001d040: 732c 0a20 2020 2020 2020 2020 2020 2022  s,.            "
+0001d050: 6669 6c65 7322 3a20 5b5d 2c0a 2020 2020  files": [],.    
+0001d060: 2020 2020 2020 2020 226c 7330 223a 204e          "ls0": N
+0001d070: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0001d080: 2022 6163 6374 223a 2073 656c 662e 756e   "acct": self.un
+0001d090: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0001d0a0: 2022 7065 726d 7322 3a20 6a73 6f6e 2e64   "perms": json.d
+0001d0b0: 756d 7073 2870 6572 6d73 292c 0a20 2020  umps(perms),.   
+0001d0c0: 2020 2020 2020 2020 2022 6c69 6665 7469           "lifeti
+0001d0d0: 6d65 223a 206c 735f 7265 745b 226c 6966  me": ls_ret["lif
+0001d0e0: 6574 696d 6522 5d2c 0a20 2020 2020 2020  etime"],.       
+0001d0f0: 2020 2020 2022 6672 616e 6422 3a20 626f       "frand": bo
+0001d100: 6f6c 2876 6e2e 666c 6167 732e 6765 7428  ol(vn.flags.get(
+0001d110: 2272 616e 6422 2929 2c0a 2020 2020 2020  "rand")),.      
+0001d120: 2020 2020 2020 2274 6167 6c69 7374 223a        "taglist":
+0001d130: 205b 5d2c 0a20 2020 2020 2020 2020 2020   [],.           
+0001d140: 2022 6465 665f 6863 6f6c 7322 3a20 5b5d   "def_hcols": []
+0001d150: 2c0a 2020 2020 2020 2020 2020 2020 2268  ,.            "h
+0001d160: 6176 655f 656d 7022 3a20 7365 6c66 2e61  ave_emp": self.a
+0001d170: 7267 732e 656d 702c 0a20 2020 2020 2020  rgs.emp,.       
+0001d180: 2020 2020 2022 6861 7665 5f75 7032 6b5f       "have_up2k_
+0001d190: 6964 7822 3a20 6532 642c 0a20 2020 2020  idx": e2d,.     
+0001d1a0: 2020 2020 2020 2022 6861 7665 5f74 6167         "have_tag
+0001d1b0: 735f 6964 7822 3a20 6532 742c 0a20 2020  s_idx": e2t,.   
+0001d1c0: 2020 2020 2020 2020 2022 6861 7665 5f61           "have_a
+0001d1d0: 636f 6465 223a 2028 6e6f 7420 7365 6c66  code": (not self
+0001d1e0: 2e61 7267 732e 6e6f 5f61 636f 6465 292c  .args.no_acode),
+0001d1f0: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
+0001d200: 7665 5f6d 7622 3a20 286e 6f74 2073 656c  ve_mv": (not sel
+0001d210: 662e 6172 6773 2e6e 6f5f 6d76 292c 0a20  f.args.no_mv),. 
+0001d220: 2020 2020 2020 2020 2020 2022 6861 7665             "have
+0001d230: 5f64 656c 223a 2028 6e6f 7420 7365 6c66  _del": (not self
+0001d240: 2e61 7267 732e 6e6f 5f64 656c 292c 0a20  .args.no_del),. 
+0001d250: 2020 2020 2020 2020 2020 2022 6861 7665             "have
+0001d260: 5f7a 6970 223a 2028 6e6f 7420 7365 6c66  _zip": (not self
+0001d270: 2e61 7267 732e 6e6f 5f7a 6970 292c 0a20  .args.no_zip),. 
+0001d280: 2020 2020 2020 2020 2020 2022 6861 7665             "have
+0001d290: 5f75 6e70 6f73 7422 3a20 696e 7428 7365  _unpost": int(se
+0001d2a0: 6c66 2e61 7267 732e 756e 706f 7374 292c  lf.args.unpost),
+0001d2b0: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
+0001d2c0: 7665 5f62 5f75 223a 2028 7365 6c66 2e63  ve_b_u": (self.c
+0001d2d0: 616e 5f77 7269 7465 2061 6e64 2073 656c  an_write and sel
+0001d2e0: 662e 7570 6172 616d 2e67 6574 2822 6222  f.uparam.get("b"
+0001d2f0: 2920 3d3d 2022 7522 292c 0a20 2020 2020  ) == "u"),.     
+0001d300: 2020 2020 2020 2022 7362 5f6d 6422 3a20         "sb_md": 
+0001d310: 2222 2069 6620 226e 6f5f 7362 5f6d 6422  "" if "no_sb_md"
+0001d320: 2069 6e20 7666 2065 6c73 6520 2876 662e   in vf else (vf.
+0001d330: 6765 7428 226d 645f 7362 6622 2920 6f72  get("md_sbf") or
+0001d340: 2022 7922 292c 0a20 2020 2020 2020 2020   "y"),.         
+0001d350: 2020 2022 7362 5f6c 6722 3a20 2222 2069     "sb_lg": "" i
+0001d360: 6620 226e 6f5f 7362 5f6c 6722 2069 6e20  f "no_sb_lg" in 
+0001d370: 7666 2065 6c73 6520 2876 662e 6765 7428  vf else (vf.get(
+0001d380: 226c 675f 7362 6622 2920 6f72 2022 7922  "lg_sbf") or "y"
+0001d390: 292c 0a20 2020 2020 2020 2020 2020 2022  ),.            "
+0001d3a0: 7572 6c5f 7375 6622 3a20 7572 6c5f 7375  url_suf": url_su
+0001d3b0: 662c 0a20 2020 2020 2020 2020 2020 2022  f,.            "
+0001d3c0: 6c6f 6775 6573 223a 206c 6f67 7565 732c  logues": logues,
+0001d3d0: 0a20 2020 2020 2020 2020 2020 2022 7265  .            "re
+0001d3e0: 6164 6d65 223a 2072 6561 646d 652c 0a20  adme": readme,. 
+0001d3f0: 2020 2020 2020 2020 2020 2022 7469 746c             "titl
+0001d400: 6522 3a20 6874 6d6c 5f65 7363 6170 6528  e": html_escape(
+0001d410: 7365 6c66 2e76 7061 7468 2c20 6372 6c66  self.vpath, crlf
+0001d420: 3d54 7275 6529 206f 7220 22f0 9f92 bef0  =True) or ".....
+0001d430: 9f8e 8922 2c0a 2020 2020 2020 2020 2020  ...",.          
+0001d440: 2020 2273 7276 5f69 6e66 6f22 3a20 7372    "srv_info": sr
+0001d450: 765f 696e 666f 742c 0a20 2020 2020 2020  v_infot,.       
+0001d460: 2020 2020 2022 6467 7269 6422 3a20 2267       "dgrid": "g
+0001d470: 7269 6422 2069 6e20 7666 2c0a 2020 2020  rid" in vf,.    
+0001d480: 2020 2020 2020 2020 2275 6e6c 6973 7422          "unlist"
+0001d490: 3a20 756e 6c69 7374 2c0a 2020 2020 2020  : unlist,.      
+0001d4a0: 2020 2020 2020 2264 7468 656d 6522 3a20        "dtheme": 
+0001d4b0: 7365 6c66 2e61 7267 732e 7468 656d 652c  self.args.theme,
+0001d4c0: 0a20 2020 2020 2020 2020 2020 2022 7468  .            "th
+0001d4d0: 656d 6573 223a 2073 656c 662e 6172 6773  emes": self.args
+0001d4e0: 2e74 6865 6d65 732c 0a20 2020 2020 2020  .themes,.       
+0001d4f0: 2020 2020 2022 7475 7262 6f6c 766c 223a       "turbolvl":
+0001d500: 2073 656c 662e 6172 6773 2e74 7572 626f   self.args.turbo
+0001d510: 2c0a 2020 2020 2020 2020 2020 2020 2269  ,.            "i
+0001d520: 6478 6822 3a20 696e 7428 7365 6c66 2e61  dxh": int(self.a
+0001d530: 7267 732e 6968 292c 0a20 2020 2020 2020  rgs.ih),.       
+0001d540: 2020 2020 2022 7532 736f 7274 223a 2073       "u2sort": s
+0001d550: 656c 662e 6172 6773 2e75 3273 6f72 742c  elf.args.u2sort,
+0001d560: 0a20 2020 2020 2020 207d 0a0a 2020 2020  .        }..    
+0001d570: 2020 2020 6966 2073 656c 662e 6172 6773      if self.args
+0001d580: 2e6a 735f 6272 6f77 7365 723a 0a20 2020  .js_browser:.   
+0001d590: 2020 2020 2020 2020 206a 3261 5b22 6a73           j2a["js
+0001d5a0: 225d 203d 2073 656c 662e 6172 6773 2e6a  "] = self.args.j
+0001d5b0: 735f 6272 6f77 7365 720a 0a20 2020 2020  s_browser..     
+0001d5c0: 2020 2069 6620 7365 6c66 2e61 7267 732e     if self.args.
+0001d5d0: 6373 735f 6272 6f77 7365 723a 0a20 2020  css_browser:.   
+0001d5e0: 2020 2020 2020 2020 206a 3261 5b22 6373           j2a["cs
+0001d5f0: 7322 5d20 3d20 7365 6c66 2e61 7267 732e  s"] = self.args.
+0001d600: 6373 735f 6272 6f77 7365 720a 0a20 2020  css_browser..   
+0001d610: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+0001d620: 2e63 6f6e 6e2e 6873 7276 2e70 7269 736d  .conn.hsrv.prism
+0001d630: 3a0a 2020 2020 2020 2020 2020 2020 6a32  :.            j2
+0001d640: 615b 226e 6f5f 7072 6973 6d22 5d20 3d20  a["no_prism"] = 
+0001d650: 5472 7565 0a0a 2020 2020 2020 2020 6966  True..        if
+0001d660: 206e 6f74 2073 656c 662e 6361 6e5f 7265   not self.can_re
+0001d670: 6164 3a0a 2020 2020 2020 2020 2020 2020  ad:.            
+0001d680: 6966 2069 735f 6c73 3a0a 2020 2020 2020  if is_ls:.      
+0001d690: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001d6a0: 2073 656c 662e 7478 5f6c 7328 6c73 5f72   self.tx_ls(ls_r
+0001d6b0: 6574 290a 0a20 2020 2020 2020 2020 2020  et)..           
+0001d6c0: 2069 6620 6e6f 7420 7374 6174 2e53 5f49   if not stat.S_I
+0001d6d0: 5344 4952 2873 742e 7374 5f6d 6f64 6529  SDIR(st.st_mode)
+0001d6e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001d6f0: 2020 7265 7475 726e 2073 656c 662e 7478    return self.tx
+0001d700: 5f34 3034 2854 7275 6529 0a0a 2020 2020  _404(True)..    
+0001d710: 2020 2020 2020 2020 6966 2022 7a69 7022          if "zip"
+0001d720: 2069 6e20 7365 6c66 2e75 7061 7261 6d20   in self.uparam 
+0001d730: 6f72 2022 7461 7222 2069 6e20 7365 6c66  or "tar" in self
+0001d740: 2e75 7061 7261 6d3a 0a20 2020 2020 2020  .uparam:.       
+0001d750: 2020 2020 2020 2020 2072 6169 7365 2050           raise P
+0001d760: 6562 6b61 6328 3430 3329 0a0a 2020 2020  ebkac(403)..    
+0001d770: 2020 2020 2020 2020 6874 6d6c 203d 2073          html = s
+0001d780: 656c 662e 6a32 7328 7470 6c2c 202a 2a6a  elf.j2s(tpl, **j
+0001d790: 3261 290a 2020 2020 2020 2020 2020 2020  2a).            
+0001d7a0: 7365 6c66 2e72 6570 6c79 2868 746d 6c2e  self.reply(html.
+0001d7b0: 656e 636f 6465 2822 7574 662d 3822 2c20  encode("utf-8", 
+0001d7c0: 2272 6570 6c61 6365 2229 290a 2020 2020  "replace")).    
+0001d7d0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0001d7e0: 7275 650a 0a20 2020 2020 2020 2066 6f72  rue..        for
+0001d7f0: 206b 2069 6e20 5b22 7a69 7022 2c20 2274   k in ["zip", "t
+0001d800: 6172 225d 3a0a 2020 2020 2020 2020 2020  ar"]:.          
+0001d810: 2020 7620 3d20 7365 6c66 2e75 7061 7261    v = self.upara
+0001d820: 6d2e 6765 7428 6b29 0a20 2020 2020 2020  m.get(k).       
+0001d830: 2020 2020 2069 6620 7620 6973 206e 6f74       if v is not
+0001d840: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0001d850: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0001d860: 6c66 2e74 785f 7a69 7028 6b2c 2076 2c20  lf.tx_zip(k, v, 
+0001d870: 7365 6c66 2e76 7061 7468 2c20 766e 2c20  self.vpath, vn, 
+0001d880: 7265 6d2c 205b 5d2c 2073 656c 662e 6172  rem, [], self.ar
+0001d890: 6773 2e65 6429 0a0a 2020 2020 2020 2020  gs.ed)..        
+0001d8a0: 6673 726f 6f74 2c20 7666 735f 6c73 2c20  fsroot, vfs_ls, 
+0001d8b0: 7666 735f 7669 7274 203d 2076 6e2e 6c73  vfs_virt = vn.ls
+0001d8c0: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+0001d8d0: 6d2c 0a20 2020 2020 2020 2020 2020 2073  m,.            s
+0001d8e0: 656c 662e 756e 616d 652c 0a20 2020 2020  elf.uname,.     
+0001d8f0: 2020 2020 2020 206e 6f74 2073 656c 662e         not self.
+0001d900: 6172 6773 2e6e 6f5f 7363 616e 6469 722c  args.no_scandir,
+0001d910: 0a20 2020 2020 2020 2020 2020 205b 5b54  .            [[T
+0001d920: 7275 652c 2046 616c 7365 5d2c 205b 4661  rue, False], [Fa
+0001d930: 6c73 652c 2054 7275 655d 5d2c 0a20 2020  lse, True]],.   
+0001d940: 2020 2020 2020 2020 206c 7374 6174 3d22           lstat="
+0001d950: 6c74 2220 696e 2073 656c 662e 7570 6172  lt" in self.upar
+0001d960: 616d 2c0a 2020 2020 2020 2020 290a 2020  am,.        ).  
+0001d970: 2020 2020 2020 7374 6174 7320 3d20 7b6b        stats = {k
+0001d980: 3a20 7620 666f 7220 6b2c 2076 2069 6e20  : v for k, v in 
+0001d990: 7666 735f 6c73 7d0a 2020 2020 2020 2020  vfs_ls}.        
+0001d9a0: 6c73 5f6e 616d 6573 203d 205b 785b 305d  ls_names = [x[0]
+0001d9b0: 2066 6f72 2078 2069 6e20 7666 735f 6c73   for x in vfs_ls
+0001d9c0: 5d0a 2020 2020 2020 2020 6c73 5f6e 616d  ].        ls_nam
+0001d9d0: 6573 2e65 7874 656e 6428 6c69 7374 2876  es.extend(list(v
+0001d9e0: 6673 5f76 6972 742e 6b65 7973 2829 2929  fs_virt.keys()))
+0001d9f0: 0a0a 2020 2020 2020 2020 2320 6368 6563  ..        # chec
+0001da00: 6b20 666f 7220 6f6c 6420 7665 7273 696f  k for old versio
+0001da10: 6e73 206f 6620 6669 6c65 732c 0a20 2020  ns of files,.   
+0001da20: 2020 2020 2023 205b 6e75 6d2d 6261 636b       # [num-back
+0001da30: 7570 732c 206d 6f73 742d 7265 6365 6e74  ups, most-recent
+0001da40: 2c20 6869 7374 2d70 6174 685d 0a20 2020  , hist-path].   
+0001da50: 2020 2020 2068 6973 7420 2020 2020 3d20       hist     = 
+0001da60: 7b7d 0a20 2020 2020 2020 2068 6973 7464  {}.        histd
+0001da70: 6972 203d 206f 732e 7061 7468 2e6a 6f69  ir = os.path.joi
+0001da80: 6e28 6673 726f 6f74 2c20 222e 6869 7374  n(fsroot, ".hist
+0001da90: 2229 0a20 2020 2020 2020 2070 746e 203d  ").        ptn =
+0001daa0: 2072 652e 636f 6d70 696c 6528 7222 282e   re.compile(r"(.
+0001dab0: 2a29 5c2e 285b 302d 395d 2b5c 2e5b 302d  *)\.([0-9]+\.[0-
+0001dac0: 395d 7b33 7d29 285c 2e5b 5e5c 2e5d 2b29  9]{3})(\.[^\.]+)
+0001dad0: 2422 290a 2020 2020 2020 2020 7472 793a  $").        try:
+0001dae0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0001daf0: 2068 666e 2069 6e20 626f 732e 6c69 7374   hfn in bos.list
+0001db00: 6469 7228 6869 7374 6469 7229 3a0a 2020  dir(histdir):.  
+0001db10: 2020 2020 2020 2020 2020 2020 2020 6d20                m 
+0001db20: 3d20 7074 6e2e 6d61 7463 6828 6866 6e29  = ptn.match(hfn)
+0001db30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001db40: 2069 6620 6e6f 7420 6d3a 0a20 2020 2020   if not m:.     
+0001db50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001db60: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+0001db70: 2020 2020 2020 2020 2066 6e20 3d20 6d2e           fn = m.
+0001db80: 6772 6f75 7028 3129 202b 206d 2e67 726f  group(1) + m.gro
+0001db90: 7570 2833 290a 2020 2020 2020 2020 2020  up(3).          
+0001dba0: 2020 2020 2020 6e2c 2074 732c 205f 203d        n, ts, _ =
+0001dbb0: 2068 6973 742e 6765 7428 666e 2c20 2830   hist.get(fn, (0
+0001dbc0: 2c20 302c 2022 2229 290a 2020 2020 2020  , 0, "")).      
+0001dbd0: 2020 2020 2020 2020 2020 6869 7374 5b66            hist[f
+0001dbe0: 6e5d 203d 2028 6e20 2b20 312c 206d 6178  n] = (n + 1, max
+0001dbf0: 2874 732c 2066 6c6f 6174 286d 2e67 726f  (ts, float(m.gro
+0001dc00: 7570 2832 2929 292c 2068 666e 290a 2020  up(2))), hfn).  
+0001dc10: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+0001dc20: 2020 2020 2020 2020 2020 7061 7373 0a0a            pass..
+0001dc30: 2020 2020 2020 2020 2320 7368 6f77 2064          # show d
+0001dc40: 6f74 6669 6c65 7320 6966 2070 6572 6d69  otfiles if permi
+0001dc50: 7474 6564 2061 6e64 2072 6571 7565 7374  tted and request
+0001dc60: 6564 0a20 2020 2020 2020 2069 6620 6e6f  ed.        if no
+0001dc70: 7420 7365 6c66 2e61 7267 732e 6564 206f  t self.args.ed o
+0001dc80: 7220 2264 6f74 7322 206e 6f74 2069 6e20  r "dots" not in 
+0001dc90: 7365 6c66 2e75 7061 7261 6d3a 0a20 2020  self.uparam:.   
+0001dca0: 2020 2020 2020 2020 206c 735f 6e61 6d65           ls_name
+0001dcb0: 7320 3d20 6578 636c 7564 655f 646f 7466  s = exclude_dotf
+0001dcc0: 696c 6573 286c 735f 6e61 6d65 7329 0a0a  iles(ls_names)..
+0001dcd0: 2020 2020 2020 2020 6164 645f 666b 203d          add_fk =
+0001dce0: 2076 6e2e 666c 6167 732e 6765 7428 2266   vn.flags.get("f
+0001dcf0: 6b22 290a 0a20 2020 2020 2020 2064 6972  k")..        dir
+0001dd00: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
+0001dd10: 696c 6573 203d 205b 5d0a 2020 2020 2020  iles = [].      
+0001dd20: 2020 666f 7220 666e 2069 6e20 6c73 5f6e    for fn in ls_n
+0001dd30: 616d 6573 3a0a 2020 2020 2020 2020 2020  ames:.          
+0001dd40: 2020 6261 7365 203d 2022 220a 2020 2020    base = "".    
+0001dd50: 2020 2020 2020 2020 6872 6566 203d 2066          href = f
+0001dd60: 6e0a 2020 2020 2020 2020 2020 2020 6966  n.            if
+0001dd70: 206e 6f74 2069 735f 6c73 2061 6e64 206e   not is_ls and n
+0001dd80: 6f74 2069 735f 6a73 2061 6e64 206e 6f74  ot is_js and not
+0001dd90: 2073 656c 662e 7472 6169 6c69 6e67 5f73   self.trailing_s
+0001dda0: 6c61 7368 2061 6e64 2076 7061 7468 3a0a  lash and vpath:.
+0001ddb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddc0: 6261 7365 203d 2022 2f22 202b 2076 7061  base = "/" + vpa
+0001ddd0: 7468 202b 2022 2f22 0a20 2020 2020 2020  th + "/".       
+0001dde0: 2020 2020 2020 2020 2068 7265 6620 3d20           href = 
+0001ddf0: 6261 7365 202b 2066 6e0a 0a20 2020 2020  base + fn..     
+0001de00: 2020 2020 2020 2069 6620 666e 2069 6e20         if fn in 
+0001de10: 7666 735f 7669 7274 3a0a 2020 2020 2020  vfs_virt:.      
+0001de20: 2020 2020 2020 2020 2020 6673 7061 7468            fspath
+0001de30: 203d 2076 6673 5f76 6972 745b 666e 5d2e   = vfs_virt[fn].
+0001de40: 7265 616c 7061 7468 0a20 2020 2020 2020  realpath.       
+0001de50: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001de60: 2020 2020 2020 2020 2020 2066 7370 6174             fspat
+0001de70: 6820 3d20 6673 726f 6f74 202b 2022 2f22  h = fsroot + "/"
+0001de80: 202b 2066 6e0a 0a20 2020 2020 2020 2020   + fn..         
+0001de90: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001dea0: 2020 2020 2020 2020 6c69 6e66 203d 2073          linf = s
+0001deb0: 7461 7473 2e67 6574 2866 6e29 206f 7220  tats.get(fn) or 
+0001dec0: 626f 732e 6c73 7461 7428 6673 7061 7468  bos.lstat(fspath
+0001ded0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001dee0: 2020 696e 6620 3d20 626f 732e 7374 6174    inf = bos.stat
+0001def0: 2866 7370 6174 6829 2069 6620 7374 6174  (fspath) if stat
+0001df00: 2e53 5f49 534c 4e4b 286c 696e 662e 7374  .S_ISLNK(linf.st
+0001df10: 5f6d 6f64 6529 2065 6c73 6520 6c69 6e66  _mode) else linf
+0001df20: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0001df30: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+0001df40: 2020 2020 2073 656c 662e 6c6f 6728 2262       self.log("b
+0001df50: 726f 6b65 6e20 7379 6d6c 696e 6b3a 207b  roken symlink: {
+0001df60: 7d22 2e66 6f72 6d61 7428 7265 7072 2866  }".format(repr(f
+0001df70: 7370 6174 6829 2929 0a20 2020 2020 2020  spath))).       
+0001df80: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0001df90: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
+0001dfa0: 735f 6469 7220 3d20 7374 6174 2e53 5f49  s_dir = stat.S_I
+0001dfb0: 5344 4952 2869 6e66 2e73 745f 6d6f 6465  SDIR(inf.st_mode
+0001dfc0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0001dfd0: 2069 735f 6469 723a 0a20 2020 2020 2020   is_dir:.       
+0001dfe0: 2020 2020 2020 2020 2068 7265 6620 2b3d           href +=
+0001dff0: 2022 2f22 0a20 2020 2020 2020 2020 2020   "/".           
+0001e000: 2020 2020 2069 6620 7365 6c66 2e61 7267       if self.arg
+0001e010: 732e 6e6f 5f7a 6970 3a0a 2020 2020 2020  s.no_zip:.      
+0001e020: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+0001e030: 7267 696e 203d 2022 4449 5222 0a20 2020  rgin = "DIR".   
+0001e040: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0001e050: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001e060: 2020 2020 2020 206d 6172 6769 6e20 3d20         margin = 
+0001e070: 273c 6120 6872 6566 3d22 2573 3f7a 6970  '<a href="%s?zip
+0001e080: 2220 7265 6c3d 226e 6f66 6f6c 6c6f 7722  " rel="nofollow"
+0001e090: 3e7a 6970 3c2f 613e 2720 2520 2871 756f  >zip</a>' % (quo
+0001e0a0: 7465 7028 6872 6566 292c 290a 2020 2020  tep(href),).    
+0001e0b0: 2020 2020 2020 2020 656c 6966 2066 6e20          elif fn 
+0001e0c0: 696e 2068 6973 743a 0a20 2020 2020 2020  in hist:.       
+0001e0d0: 2020 2020 2020 2020 206d 6172 6769 6e20           margin 
+0001e0e0: 3d20 273c 6120 6872 6566 3d22 2573 2e68  = '<a href="%s.h
+0001e0f0: 6973 742f 2573 223e 2325 733c 2f61 3e27  ist/%s">#%s</a>'
+0001e100: 2025 2028 0a20 2020 2020 2020 2020 2020   % (.           
+0001e110: 2020 2020 2020 2020 2062 6173 652c 0a20           base,. 
+0001e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e130: 2020 2068 746d 6c5f 6573 6361 7065 2868     html_escape(h
+0001e140: 6973 745b 666e 5d5b 325d 2c20 7175 6f74  ist[fn][2], quot
+0001e150: 3d54 7275 652c 2063 726c 663d 5472 7565  =True, crlf=True
+0001e160: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+0001e170: 2020 2020 2020 2068 6973 745b 666e 5d5b         hist[fn][
+0001e180: 305d 2c0a 2020 2020 2020 2020 2020 2020  0],.            
+0001e190: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0001e1a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0001e1b0: 2020 2020 2020 2020 6d61 7267 696e 203d          margin =
+0001e1c0: 2022 2d22 0a0a 2020 2020 2020 2020 2020   "-"..          
+0001e1d0: 2020 737a 203d 2069 6e66 2e73 745f 7369    sz = inf.st_si
+0001e1e0: 7a65 0a20 2020 2020 2020 2020 2020 207a  ze.            z
+0001e1f0: 6420 3d20 6461 7465 7469 6d65 2e75 7463  d = datetime.utc
+0001e200: 6672 6f6d 7469 6d65 7374 616d 7028 6c69  fromtimestamp(li
+0001e210: 6e66 2e73 745f 6d74 696d 6529 0a20 2020  nf.st_mtime).   
+0001e220: 2020 2020 2020 2020 2064 7420 3d20 2225           dt = "%
+0001e230: 3034 642d 2530 3264 2d25 3032 6420 2530  04d-%02d-%02d %0
+0001e240: 3264 3a25 3032 643a 2530 3264 2220 2520  2d:%02d:%02d" % 
+0001e250: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0001e260: 2020 7a64 2e79 6561 722c 0a20 2020 2020    zd.year,.     
+0001e270: 2020 2020 2020 2020 2020 207a 642e 6d6f             zd.mo
+0001e280: 6e74 682c 0a20 2020 2020 2020 2020 2020  nth,.           
+0001e290: 2020 2020 207a 642e 6461 792c 0a20 2020       zd.day,.   
+0001e2a0: 2020 2020 2020 2020 2020 2020 207a 642e               zd.
+0001e2b0: 686f 7572 2c0a 2020 2020 2020 2020 2020  hour,.          
+0001e2c0: 2020 2020 2020 7a64 2e6d 696e 7574 652c        zd.minute,
+0001e2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e2e0: 207a 642e 7365 636f 6e64 2c0a 2020 2020   zd.second,.    
+0001e2f0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0001e300: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0001e310: 2020 2020 2020 2020 2020 2020 6578 7420              ext 
+0001e320: 3d20 222d 2d2d 2220 6966 2069 735f 6469  = "---" if is_di
+0001e330: 7220 656c 7365 2066 6e2e 7273 706c 6974  r else fn.rsplit
+0001e340: 2822 2e22 2c20 3129 5b31 5d0a 2020 2020  (".", 1)[1].    
+0001e350: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+0001e360: 656e 2865 7874 2920 3e20 3136 3a0a 2020  en(ext) > 16:.  
+0001e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e380: 2020 6578 7420 3d20 6578 745b 3a31 365d    ext = ext[:16]
+0001e390: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+0001e3a0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+0001e3b0: 2020 2020 2065 7874 203d 2022 2522 0a0a       ext = "%"..
+0001e3c0: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0001e3d0: 6464 5f66 6b3a 0a20 2020 2020 2020 2020  dd_fk:.         
+0001e3e0: 2020 2020 2020 2068 7265 6620 3d20 2225         href = "%
+0001e3f0: 733f 6b3d 2573 2220 2520 280a 2020 2020  s?k=%s" % (.    
 0001e400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e410: 2029 5b3a 6164 645f 666b 5d2c 0a20 2020   )[:add_fk],.   
-0001e420: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0001e430: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001e440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e450: 2068 7265 6620 3d20 7175 6f74 6570 2868   href = quotep(h
-0001e460: 7265 6629 0a0a 2020 2020 2020 2020 2020  ref)..          
-0001e470: 2020 6974 656d 203d 207b 0a20 2020 2020    item = {.     
-0001e480: 2020 2020 2020 2020 2020 2022 6c65 6164             "lead
-0001e490: 223a 206d 6172 6769 6e2c 0a20 2020 2020  ": margin,.     
-0001e4a0: 2020 2020 2020 2020 2020 2022 6872 6566             "href
-0001e4b0: 223a 2068 7265 662c 0a20 2020 2020 2020  ": href,.       
-0001e4c0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-0001e4d0: 2066 6e2c 0a20 2020 2020 2020 2020 2020   fn,.           
-0001e4e0: 2020 2020 2022 737a 223a 2073 7a2c 0a20       "sz": sz,. 
-0001e4f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001e500: 6578 7422 3a20 6578 742c 0a20 2020 2020  ext": ext,.     
-0001e510: 2020 2020 2020 2020 2020 2022 6474 223a             "dt":
-0001e520: 2064 742c 0a20 2020 2020 2020 2020 2020   dt,.           
-0001e530: 2020 2020 2022 7473 223a 2069 6e74 286c       "ts": int(l
-0001e540: 696e 662e 7374 5f6d 7469 6d65 292c 0a20  inf.st_mtime),. 
-0001e550: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-0001e560: 2020 2020 2020 2020 2069 6620 6973 5f64           if is_d
-0001e570: 6972 3a0a 2020 2020 2020 2020 2020 2020  ir:.            
-0001e580: 2020 2020 6469 7273 2e61 7070 656e 6428      dirs.append(
-0001e590: 6974 656d 290a 2020 2020 2020 2020 2020  item).          
-0001e5a0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001e5b0: 2020 2020 2020 2020 6669 6c65 732e 6170          files.ap
-0001e5c0: 7065 6e64 2869 7465 6d29 0a20 2020 2020  pend(item).     
-0001e5d0: 2020 2020 2020 2020 2020 2069 7465 6d5b             item[
-0001e5e0: 2272 6422 5d20 3d20 7265 6d0a 0a20 2020  "rd"] = rem..   
-0001e5f0: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-0001e600: 2020 2020 2020 7365 6c66 2e63 6f6f 6b69        self.cooki
-0001e610: 6573 2e67 6574 2822 6964 7868 2229 203d  es.get("idxh") =
-0001e620: 3d20 2279 220a 2020 2020 2020 2020 2020  = "y".          
-0001e630: 2020 616e 6420 226c 7322 206e 6f74 2069    and "ls" not i
-0001e640: 6e20 7365 6c66 2e75 7061 7261 6d0a 2020  n self.uparam.  
-0001e650: 2020 2020 2020 2020 2020 616e 6420 2276            and "v
-0001e660: 2220 6e6f 7420 696e 2073 656c 662e 7570  " not in self.up
-0001e670: 6172 616d 0a20 2020 2020 2020 2029 3a0a  aram.        ):.
-0001e680: 2020 2020 2020 2020 2020 2020 6964 785f              idx_
-0001e690: 6874 6d6c 203d 2073 6574 285b 2269 6e64  html = set(["ind
-0001e6a0: 6578 2e68 746d 222c 2022 696e 6465 782e  ex.htm", "index.
-0001e6b0: 6874 6d6c 225d 290a 2020 2020 2020 2020  html"]).        
-0001e6c0: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
-0001e6d0: 6669 6c65 733a 0a20 2020 2020 2020 2020  files:.         
-0001e6e0: 2020 2020 2020 2069 6620 6974 656d 5b22         if item["
-0001e6f0: 6e61 6d65 225d 2069 6e20 6964 785f 6874  name"] in idx_ht
-0001e700: 6d6c 3a0a 2020 2020 2020 2020 2020 2020  ml:.            
-0001e710: 2020 2020 2020 2020 2320 646f 2066 756c          # do ful
-0001e720: 6c20 7265 736f 6c76 6520 696e 2063 6173  l resolve in cas
-0001e730: 6520 6f66 2073 6861 646f 7765 6420 6669  e of shadowed fi
-0001e740: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
-0001e750: 2020 2020 2020 2076 7020 3d20 766a 6f69         vp = vjoi
-0001e760: 6e28 7365 6c66 2e76 7061 7468 2e73 706c  n(self.vpath.spl
-0001e770: 6974 2822 3f22 295b 305d 2c20 6974 656d  it("?")[0], item
-0001e780: 5b22 6e61 6d65 225d 290a 2020 2020 2020  ["name"]).      
-0001e790: 2020 2020 2020 2020 2020 2020 2020 766e                vn
-0001e7a0: 2c20 7265 6d20 3d20 7365 6c66 2e61 7372  , rem = self.asr
-0001e7b0: 762e 7666 732e 6765 7428 7670 2c20 7365  v.vfs.get(vp, se
-0001e7c0: 6c66 2e75 6e61 6d65 2c20 5472 7565 2c20  lf.uname, True, 
-0001e7d0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
-0001e7e0: 2020 2020 2020 2020 2020 2061 7020 3d20             ap = 
-0001e7f0: 766e 2e63 616e 6f6e 6963 616c 2872 656d  vn.canonical(rem
-0001e800: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001e810: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0001e820: 662e 7478 5f66 696c 6528 6170 2920 2023  f.tx_file(ap)  #
-0001e830: 2069 7320 6e6f 2d63 6163 6865 0a0a 2020   is no-cache..  
-0001e840: 2020 2020 2020 7461 6773 6574 2020 3d20        tagset  = 
-0001e850: 7365 7428 290a 2020 2020 2020 2020 666f  set().        fo
-0001e860: 7220 6665 2069 6e20 6669 6c65 733a 0a20  r fe in files:. 
-0001e870: 2020 2020 2020 2020 2020 2066 6e20 3d20             fn = 
-0001e880: 6665 5b22 6e61 6d65 225d 0a20 2020 2020  fe["name"].     
-0001e890: 2020 2020 2020 2072 6420 3d20 6665 5b22         rd = fe["
-0001e8a0: 7264 225d 0a20 2020 2020 2020 2020 2020  rd"].           
-0001e8b0: 2064 656c 2066 655b 2272 6422 5d0a 2020   del fe["rd"].  
-0001e8c0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0001e8d0: 2069 6375 723a 0a20 2020 2020 2020 2020   icur:.         
-0001e8e0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-0001e8f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0001e900: 766e 2021 3d20 6462 763a 0a20 2020 2020  vn != dbv:.     
-0001e910: 2020 2020 2020 2020 2020 205f 2c20 7264             _, rd
-0001e920: 203d 2076 6e2e 6765 745f 6462 7628 7264   = vn.get_dbv(rd
-0001e930: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0001e940: 7264 5f65 666e 203d 2028 7264 2c20 666e  rd_efn = (rd, fn
-0001e950: 290a 2020 2020 2020 2020 2020 2020 7120  ).            q 
-0001e960: 3d20 2273 656c 6563 7420 6d74 2e6b 2c20  = "select mt.k, 
-0001e970: 6d74 2e76 2066 726f 6d20 7570 2069 6e6e  mt.v from up inn
-0001e980: 6572 206a 6f69 6e20 6d74 206f 6e20 6d74  er join mt on mt
-0001e990: 2e77 203d 2073 7562 7374 7228 7570 2e77  .w = substr(up.w
-0001e9a0: 2c31 2c31 3629 2077 6865 7265 2075 702e  ,1,16) where up.
-0001e9b0: 7264 203d 203f 2061 6e64 2075 702e 666e  rd = ? and up.fn
-0001e9c0: 203d 203f 2061 6e64 202b 6d74 2e6b 2021   = ? and +mt.k !
-0001e9d0: 3d20 2778 2722 0a20 2020 2020 2020 2020  = 'x'".         
-0001e9e0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-0001e9f0: 2020 2020 2020 2020 7220 3d20 6963 7572          r = icur
-0001ea00: 2e65 7865 6375 7465 2871 2c20 6572 645f  .execute(q, erd_
-0001ea10: 6566 6e29 0a20 2020 2020 2020 2020 2020  efn).           
-0001ea20: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0001ea30: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
-0001ea40: 2020 2020 2020 2020 2069 6620 2264 6174           if "dat
-0001ea50: 6162 6173 6520 6973 206c 6f63 6b65 6422  abase is locked"
-0001ea60: 2069 6e20 7374 7228 6578 293a 0a20 2020   in str(ex):.   
-0001ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea80: 2062 7265 616b 0a0a 2020 2020 2020 2020   break..        
-0001ea90: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0001eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eab0: 2065 7264 5f65 666e 203d 2073 3365 6e63   erd_efn = s3enc
-0001eac0: 2869 6478 2e6d 656d 5f63 7572 2c20 7264  (idx.mem_cur, rd
-0001ead0: 2c20 666e 290a 2020 2020 2020 2020 2020  , fn).          
-0001eae0: 2020 2020 2020 2020 2020 7220 3d20 6963            r = ic
-0001eaf0: 7572 2e65 7865 6375 7465 2871 2c20 6572  ur.execute(q, er
-0001eb00: 645f 6566 6e29 0a20 2020 2020 2020 2020  d_efn).         
-0001eb10: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
-0001eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb30: 2020 2074 203d 2022 7461 6720 7265 6164     t = "tag read
-0001eb40: 2065 7272 6f72 2c20 7b7d 2f7b 7d5c 6e7b   error, {}/{}\n{
-0001eb50: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-0001eb60: 2020 2020 2020 2073 656c 662e 6c6f 6728         self.log(
-0001eb70: 742e 666f 726d 6174 2872 642c 2066 6e2c  t.format(rd, fn,
-0001eb80: 206d 696e 5f65 7828 2929 290a 2020 2020   min_ex())).    
-0001eb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eba0: 6272 6561 6b0a 0a20 2020 2020 2020 2020  break..         
-0001ebb0: 2020 2066 655b 2274 6167 7322 5d20 3d20     fe["tags"] = 
-0001ebc0: 7b6b 3a20 7620 666f 7220 6b2c 2076 2069  {k: v for k, v i
-0001ebd0: 6e20 727d 0a0a 2020 2020 2020 2020 2020  n r}..          
-0001ebe0: 2020 6966 2073 656c 662e 6361 6e5f 6164    if self.can_ad
-0001ebf0: 6d69 6e3a 0a20 2020 2020 2020 2020 2020  min:.           
-0001ec00: 2020 2020 2071 203d 2022 7365 6c65 6374       q = "select
-0001ec10: 2069 702c 2061 7420 6672 6f6d 2075 7020   ip, at from up 
-0001ec20: 7768 6572 6520 7264 3d3f 2061 6e64 2066  where rd=? and f
-0001ec30: 6e3d 3f22 0a20 2020 2020 2020 2020 2020  n=?".           
-0001ec40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-0001ec50: 2020 2020 2020 2020 2020 2020 2020 7a73                zs
-0001ec60: 312c 207a 7332 203d 2069 6375 722e 6578  1, zs2 = icur.ex
-0001ec70: 6563 7574 6528 712c 2065 7264 5f65 666e  ecute(q, erd_efn
-0001ec80: 292e 6665 7463 686f 6e65 2829 0a20 2020  ).fetchone().   
-0001ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eca0: 2066 655b 2274 6167 7322 5d5b 2275 705f   fe["tags"]["up_
-0001ecb0: 6970 225d 203d 207a 7331 0a20 2020 2020  ip"] = zs1.     
-0001ecc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0001ecd0: 655b 2274 6167 7322 5d5b 222e 7570 5f61  e["tags"][".up_a
-0001ece0: 7422 5d20 3d20 7a73 320a 2020 2020 2020  t"] = zs2.      
-0001ecf0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-0001ed00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001ed10: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0001ed20: 2020 2020 2020 2020 5f20 3d20 5b74 6167          _ = [tag
-0001ed30: 7365 742e 6164 6428 6b29 2066 6f72 206b  set.add(k) for k
-0001ed40: 2069 6e20 6665 5b22 7461 6773 225d 5d0a   in fe["tags"]].
-0001ed50: 0a20 2020 2020 2020 2069 6620 6963 7572  .        if icur
-0001ed60: 3a0a 2020 2020 2020 2020 2020 2020 6d74  :.            mt
-0001ed70: 6520 3d20 766e 2e66 6c61 6773 2e67 6574  e = vn.flags.get
-0001ed80: 2822 6d74 6522 2920 6f72 2022 7570 5f69  ("mte") or "up_i
-0001ed90: 702c 2e75 705f 6174 220a 2020 2020 2020  p,.up_at".      
-0001eda0: 2020 2020 2020 7461 676c 6973 7420 3d20        taglist = 
-0001edb0: 5b6b 2066 6f72 206b 2069 6e20 6d74 652e  [k for k in mte.
-0001edc0: 7370 6c69 7428 222c 2229 2069 6620 6b20  split(",") if k 
-0001edd0: 696e 2074 6167 7365 745d 0a20 2020 2020  in tagset].     
-0001ede0: 2020 2020 2020 2066 6f72 2066 6520 696e         for fe in
-0001edf0: 2064 6972 733a 0a20 2020 2020 2020 2020   dirs:.         
-0001ee00: 2020 2020 2020 2066 655b 2274 6167 7322         fe["tags"
-0001ee10: 5d20 3d20 7b7d 0a20 2020 2020 2020 2065  ] = {}.        e
-0001ee20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001ee30: 2074 6167 6c69 7374 203d 206c 6973 7428   taglist = list(
-0001ee40: 7461 6773 6574 290a 0a20 2020 2020 2020  tagset)..       
-0001ee50: 2069 6620 6973 5f6c 733a 0a20 2020 2020   if is_ls:.     
-0001ee60: 2020 2020 2020 206c 735f 7265 745b 2264         ls_ret["d
-0001ee70: 6972 7322 5d20 3d20 6469 7273 0a20 2020  irs"] = dirs.   
-0001ee80: 2020 2020 2020 2020 206c 735f 7265 745b           ls_ret[
-0001ee90: 2266 696c 6573 225d 203d 2066 696c 6573  "files"] = files
-0001eea0: 0a20 2020 2020 2020 2020 2020 206c 735f  .            ls_
-0001eeb0: 7265 745b 2274 6167 6c69 7374 225d 203d  ret["taglist"] =
-0001eec0: 2074 6167 6c69 7374 0a20 2020 2020 2020   taglist.       
-0001eed0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0001eee0: 2e74 785f 6c73 286c 735f 7265 7429 0a0a  .tx_ls(ls_ret)..
-0001eef0: 2020 2020 2020 2020 646f 6320 3d20 7365          doc = se
-0001ef00: 6c66 2e75 7061 7261 6d2e 6765 7428 2264  lf.uparam.get("d
-0001ef10: 6f63 2229 2069 6620 7365 6c66 2e63 616e  oc") if self.can
-0001ef20: 5f72 6561 6420 656c 7365 204e 6f6e 650a  _read else None.
-0001ef30: 2020 2020 2020 2020 6966 2064 6f63 3a0a          if doc:.
-0001ef40: 2020 2020 2020 2020 2020 2020 646f 6320              doc 
-0001ef50: 3d20 756e 7175 6f74 6570 2864 6f63 2e72  = unquotep(doc.r
-0001ef60: 6570 6c61 6365 2822 2b22 2c20 2220 2229  eplace("+", " ")
-0001ef70: 2e73 706c 6974 2822 3f22 295b 305d 290a  .split("?")[0]).
-0001ef80: 2020 2020 2020 2020 2020 2020 6a32 615b              j2a[
-0001ef90: 2264 6f63 6e61 6d65 225d 203d 2064 6f63  "docname"] = doc
-0001efa0: 0a20 2020 2020 2020 2020 2020 2064 6f63  .            doc
-0001efb0: 7478 7420 3d20 4e6f 6e65 0a20 2020 2020  txt = None.     
-0001efc0: 2020 2020 2020 2069 6620 6e65 7874 2828         if next((
-0001efd0: 7820 666f 7220 7820 696e 2066 696c 6573  x for x in files
-0001efe0: 2069 6620 785b 226e 616d 6522 5d20 3d3d   if x["name"] ==
-0001eff0: 2064 6f63 292c 204e 6f6e 6529 3a0a 2020   doc), None):.  
-0001f000: 2020 2020 2020 2020 2020 2020 2020 646f                do
-0001f010: 6370 6174 6820 3d20 6f73 2e70 6174 682e  cpath = os.path.
-0001f020: 6a6f 696e 2861 6273 7061 7468 2c20 646f  join(abspath, do
-0001f030: 6329 0a20 2020 2020 2020 2020 2020 2020  c).             
-0001f040: 2020 2073 7a20 3d20 626f 732e 7061 7468     sz = bos.path
-0001f050: 2e67 6574 7369 7a65 2864 6f63 7061 7468  .getsize(docpath
-0001f060: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001f070: 2020 6966 2073 7a20 3c20 3130 3234 202a    if sz < 1024 *
-0001f080: 2073 656c 662e 6172 6773 2e74 7874 5f6d   self.args.txt_m
-0001f090: 6178 3a0a 2020 2020 2020 2020 2020 2020  ax:.            
-0001f0a0: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-0001f0b0: 6e28 6673 656e 6328 646f 6370 6174 6829  n(fsenc(docpath)
-0001f0c0: 2c20 2272 6222 2920 6173 2066 3a0a 2020  , "rb") as f:.  
-0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0e0: 2020 2020 2020 646f 6374 7874 203d 2066        doctxt = f
-0001f0f0: 2e72 6561 6428 292e 6465 636f 6465 2822  .read().decode("
-0001f100: 7574 662d 3822 2c20 2272 6570 6c61 6365  utf-8", "replace
-0001f110: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
-0001f120: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0001f130: 2020 2020 2073 656c 662e 6c6f 6728 2264       self.log("d
-0001f140: 6f63 2034 3034 3a20 5b7b 7d5d 222e 666f  oc 404: [{}]".fo
-0001f150: 726d 6174 2864 6f63 292c 2063 3d36 290a  rmat(doc), c=6).
-0001f160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f170: 646f 6374 7874 203d 2022 2820 7465 7874  doctxt = "( text
-0001f180: 6669 6c65 206e 6f74 2066 6f75 6e64 2029  file not found )
-0001f190: 220a 0a20 2020 2020 2020 2020 2020 2069  "..            i
-0001f1a0: 6620 646f 6374 7874 2069 7320 6e6f 7420  f doctxt is not 
-0001f1b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0001f1c0: 2020 2020 2020 6a32 615b 2264 6f63 225d        j2a["doc"]
-0001f1d0: 203d 2064 6f63 7478 740a 0a20 2020 2020   = doctxt..     
-0001f1e0: 2020 2066 6f72 2064 2069 6e20 6469 7273     for d in dirs
-0001f1f0: 3a0a 2020 2020 2020 2020 2020 2020 645b  :.            d[
-0001f200: 226e 616d 6522 5d20 2b3d 2022 2f22 0a0a  "name"] += "/"..
-0001f210: 2020 2020 2020 2020 6469 7273 2e73 6f72          dirs.sor
-0001f220: 7428 6b65 793d 6974 656d 6765 7474 6572  t(key=itemgetter
-0001f230: 2822 6e61 6d65 2229 290a 0a20 2020 2020  ("name"))..     
-0001f240: 2020 2069 6620 6973 5f6a 733a 0a20 2020     if is_js:.   
-0001f250: 2020 2020 2020 2020 206a 3261 5b22 6c73           j2a["ls
-0001f260: 3022 5d20 3d20 7b0a 2020 2020 2020 2020  0"] = {.        
-0001f270: 2020 2020 2020 2020 2264 6972 7322 3a20          "dirs": 
-0001f280: 6469 7273 2c0a 2020 2020 2020 2020 2020  dirs,.          
-0001f290: 2020 2020 2020 2266 696c 6573 223a 2066        "files": f
-0001f2a0: 696c 6573 2c0a 2020 2020 2020 2020 2020  iles,.          
-0001f2b0: 2020 2020 2020 2274 6167 6c69 7374 223a        "taglist":
-0001f2c0: 2074 6167 6c69 7374 2c0a 2020 2020 2020   taglist,.      
-0001f2d0: 2020 2020 2020 2020 2020 2275 6e6c 6973            "unlis
-0001f2e0: 7422 3a20 756e 6c69 7374 2c0a 2020 2020  t": unlist,.    
-0001f2f0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0001f300: 2020 2020 2020 6a32 615b 2266 696c 6573        j2a["files
-0001f310: 225d 203d 205b 5d0a 2020 2020 2020 2020  "] = [].        
-0001f320: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001f330: 2020 6a32 615b 2266 696c 6573 225d 203d    j2a["files"] =
-0001f340: 2064 6972 7320 2b20 6669 6c65 730a 0a20   dirs + files.. 
-0001f350: 2020 2020 2020 206a 3261 5b22 7461 676c         j2a["tagl
-0001f360: 6973 7422 5d20 3d20 7461 676c 6973 740a  ist"] = taglist.
-0001f370: 2020 2020 2020 2020 6a32 615b 2274 7874          j2a["txt
-0001f380: 5f65 7874 225d 203d 2073 656c 662e 6172  _ext"] = self.ar
-0001f390: 6773 2e74 6578 7466 696c 6573 2e72 6570  gs.textfiles.rep
-0001f3a0: 6c61 6365 2822 2c22 2c20 2220 2229 0a0a  lace(",", " ")..
-0001f3b0: 2020 2020 2020 2020 6966 2022 6d74 6822          if "mth"
-0001f3c0: 2069 6e20 766e 2e66 6c61 6773 3a0a 2020   in vn.flags:.  
-0001f3d0: 2020 2020 2020 2020 2020 6a32 615b 2264            j2a["d
-0001f3e0: 6566 5f68 636f 6c73 225d 203d 2076 6e2e  ef_hcols"] = vn.
-0001f3f0: 666c 6167 735b 226d 7468 225d 2e73 706c  flags["mth"].spl
-0001f400: 6974 2822 2c22 290a 0a20 2020 2020 2020  it(",")..       
-0001f410: 2068 746d 6c20 3d20 7365 6c66 2e6a 3273   html = self.j2s
-0001f420: 2874 706c 2c20 2a2a 6a32 6129 0a20 2020  (tpl, **j2a).   
-0001f430: 2020 2020 2073 656c 662e 7265 706c 7928       self.reply(
-0001f440: 6874 6d6c 2e65 6e63 6f64 6528 2275 7466  html.encode("utf
-0001f450: 2d38 222c 2022 7265 706c 6163 6522 2929  -8", "replace"))
-0001f460: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0001f470: 5472 7565 0a                             True.
+0001e410: 7175 6f74 6570 2868 7265 6629 2c0a 2020  quotep(href),.  
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 7365 6c66 2e67 656e 5f66 6b28 0a20    self.gen_fk(. 
+0001e440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e450: 2020 2020 2020 2073 656c 662e 6172 6773         self.args
+0001e460: 2e66 6b5f 7361 6c74 2c20 6673 7061 7468  .fk_salt, fspath
+0001e470: 2c20 737a 2c20 3020 6966 2041 4e59 5749  , sz, 0 if ANYWI
+0001e480: 4e20 656c 7365 2069 6e66 2e73 745f 696e  N else inf.st_in
+0001e490: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+0001e4a0: 2020 2020 2020 295b 3a61 6464 5f66 6b5d        )[:add_fk]
+0001e4b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001e4c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0001e4d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001e4e0: 2020 2020 2020 6872 6566 203d 2071 756f        href = quo
+0001e4f0: 7465 7028 6872 6566 290a 0a20 2020 2020  tep(href)..     
+0001e500: 2020 2020 2020 2069 7465 6d20 3d20 7b0a         item = {.
+0001e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e520: 226c 6561 6422 3a20 6d61 7267 696e 2c0a  "lead": margin,.
+0001e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e540: 2268 7265 6622 3a20 6872 6566 2c0a 2020  "href": href,.  
+0001e550: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+0001e560: 616d 6522 3a20 666e 2c0a 2020 2020 2020  ame": fn,.      
+0001e570: 2020 2020 2020 2020 2020 2273 7a22 3a20            "sz": 
+0001e580: 737a 2c0a 2020 2020 2020 2020 2020 2020  sz,.            
+0001e590: 2020 2020 2265 7874 223a 2065 7874 2c0a      "ext": ext,.
+0001e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5b0: 2264 7422 3a20 6474 2c0a 2020 2020 2020  "dt": dt,.      
+0001e5c0: 2020 2020 2020 2020 2020 2274 7322 3a20            "ts": 
+0001e5d0: 696e 7428 6c69 6e66 2e73 745f 6d74 696d  int(linf.st_mtim
+0001e5e0: 6529 2c0a 2020 2020 2020 2020 2020 2020  e),.            
+0001e5f0: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+0001e600: 2069 735f 6469 723a 0a20 2020 2020 2020   is_dir:.       
+0001e610: 2020 2020 2020 2020 2064 6972 732e 6170           dirs.ap
+0001e620: 7065 6e64 2869 7465 6d29 0a20 2020 2020  pend(item).     
+0001e630: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001e640: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+0001e650: 6573 2e61 7070 656e 6428 6974 656d 290a  es.append(item).
+0001e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e670: 6974 656d 5b22 7264 225d 203d 2072 656d  item["rd"] = rem
+0001e680: 0a0a 2020 2020 2020 2020 6966 2028 0a20  ..        if (. 
+0001e690: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001e6a0: 636f 6f6b 6965 732e 6765 7428 2269 6478  cookies.get("idx
+0001e6b0: 6822 2920 3d3d 2022 7922 0a20 2020 2020  h") == "y".     
+0001e6c0: 2020 2020 2020 2061 6e64 2022 6c73 2220         and "ls" 
+0001e6d0: 6e6f 7420 696e 2073 656c 662e 7570 6172  not in self.upar
+0001e6e0: 616d 0a20 2020 2020 2020 2020 2020 2061  am.            a
+0001e6f0: 6e64 2022 7622 206e 6f74 2069 6e20 7365  nd "v" not in se
+0001e700: 6c66 2e75 7061 7261 6d0a 2020 2020 2020  lf.uparam.      
+0001e710: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0001e720: 2069 6478 5f68 746d 6c20 3d20 7365 7428   idx_html = set(
+0001e730: 5b22 696e 6465 782e 6874 6d22 2c20 2269  ["index.htm", "i
+0001e740: 6e64 6578 2e68 746d 6c22 5d29 0a20 2020  ndex.html"]).   
+0001e750: 2020 2020 2020 2020 2066 6f72 2069 7465           for ite
+0001e760: 6d20 696e 2066 696c 6573 3a0a 2020 2020  m in files:.    
+0001e770: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0001e780: 7465 6d5b 226e 616d 6522 5d20 696e 2069  tem["name"] in i
+0001e790: 6478 5f68 746d 6c3a 0a20 2020 2020 2020  dx_html:.       
+0001e7a0: 2020 2020 2020 2020 2020 2020 2023 2064               # d
+0001e7b0: 6f20 6675 6c6c 2072 6573 6f6c 7665 2069  o full resolve i
+0001e7c0: 6e20 6361 7365 206f 6620 7368 6164 6f77  n case of shadow
+0001e7d0: 6564 2066 696c 650a 2020 2020 2020 2020  ed file.        
+0001e7e0: 2020 2020 2020 2020 2020 2020 7670 203d              vp =
+0001e7f0: 2076 6a6f 696e 2873 656c 662e 7670 6174   vjoin(self.vpat
+0001e800: 682e 7370 6c69 7428 223f 2229 5b30 5d2c  h.split("?")[0],
+0001e810: 2069 7465 6d5b 226e 616d 6522 5d29 0a20   item["name"]). 
+0001e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e830: 2020 2076 6e2c 2072 656d 203d 2073 656c     vn, rem = sel
+0001e840: 662e 6173 7276 2e76 6673 2e67 6574 2876  f.asrv.vfs.get(v
+0001e850: 702c 2073 656c 662e 756e 616d 652c 2054  p, self.uname, T
+0001e860: 7275 652c 2046 616c 7365 290a 2020 2020  rue, False).    
+0001e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e880: 6170 203d 2076 6e2e 6361 6e6f 6e69 6361  ap = vn.canonica
+0001e890: 6c28 7265 6d29 0a20 2020 2020 2020 2020  l(rem).         
+0001e8a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0001e8b0: 6e20 7365 6c66 2e74 785f 6669 6c65 2861  n self.tx_file(a
+0001e8c0: 7029 2020 2320 6973 206e 6f2d 6361 6368  p)  # is no-cach
+0001e8d0: 650a 0a20 2020 2020 2020 2074 6167 7365  e..        tagse
+0001e8e0: 7420 203d 2073 6574 2829 0a20 2020 2020  t  = set().     
+0001e8f0: 2020 2066 6f72 2066 6520 696e 2066 696c     for fe in fil
+0001e900: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
+0001e910: 666e 203d 2066 655b 226e 616d 6522 5d0a  fn = fe["name"].
+0001e920: 2020 2020 2020 2020 2020 2020 7264 203d              rd =
+0001e930: 2066 655b 2272 6422 5d0a 2020 2020 2020   fe["rd"].      
+0001e940: 2020 2020 2020 6465 6c20 6665 5b22 7264        del fe["rd
+0001e950: 225d 0a20 2020 2020 2020 2020 2020 2069  "].            i
+0001e960: 6620 6e6f 7420 6963 7572 3a0a 2020 2020  f not icur:.    
+0001e970: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0001e980: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
+0001e990: 2020 6966 2076 6e20 213d 2064 6276 3a0a    if vn != dbv:.
+0001e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9b0: 5f2c 2072 6420 3d20 766e 2e67 6574 5f64  _, rd = vn.get_d
+0001e9c0: 6276 2872 6429 0a0a 2020 2020 2020 2020  bv(rd)..        
+0001e9d0: 2020 2020 6572 645f 6566 6e20 3d20 2872      erd_efn = (r
+0001e9e0: 642c 2066 6e29 0a20 2020 2020 2020 2020  d, fn).         
+0001e9f0: 2020 2071 203d 2022 7365 6c65 6374 206d     q = "select m
+0001ea00: 742e 6b2c 206d 742e 7620 6672 6f6d 2075  t.k, mt.v from u
+0001ea10: 7020 696e 6e65 7220 6a6f 696e 206d 7420  p inner join mt 
+0001ea20: 6f6e 206d 742e 7720 3d20 7375 6273 7472  on mt.w = substr
+0001ea30: 2875 702e 772c 312c 3136 2920 7768 6572  (up.w,1,16) wher
+0001ea40: 6520 7570 2e72 6420 3d20 3f20 616e 6420  e up.rd = ? and 
+0001ea50: 7570 2e66 6e20 3d20 3f20 616e 6420 2b6d  up.fn = ? and +m
+0001ea60: 742e 6b20 213d 2027 7827 220a 2020 2020  t.k != 'x'".    
+0001ea70: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0001ea80: 2020 2020 2020 2020 2020 2020 2072 203d               r =
+0001ea90: 2069 6375 722e 6578 6563 7574 6528 712c   icur.execute(q,
+0001eaa0: 2065 7264 5f65 666e 290a 2020 2020 2020   erd_efn).      
+0001eab0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+0001eac0: 6570 7469 6f6e 2061 7320 6578 3a0a 2020  eption as ex:.  
+0001ead0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001eae0: 2022 6461 7461 6261 7365 2069 7320 6c6f   "database is lo
+0001eaf0: 636b 6564 2220 696e 2073 7472 2865 7829  cked" in str(ex)
+0001eb00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001eb10: 2020 2020 2020 6272 6561 6b0a 0a20 2020        break..   
+0001eb20: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0001eb30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001eb40: 2020 2020 2020 6572 645f 6566 6e20 3d20        erd_efn = 
+0001eb50: 7333 656e 6328 6964 782e 6d65 6d5f 6375  s3enc(idx.mem_cu
+0001eb60: 722c 2072 642c 2066 6e29 0a20 2020 2020  r, rd, fn).     
+0001eb70: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001eb80: 203d 2069 6375 722e 6578 6563 7574 6528   = icur.execute(
+0001eb90: 712c 2065 7264 5f65 666e 290a 2020 2020  q, erd_efn).    
+0001eba0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0001ebb0: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
+0001ebc0: 2020 2020 2020 2020 7420 3d20 2274 6167          t = "tag
+0001ebd0: 2072 6561 6420 6572 726f 722c 207b 7d2f   read error, {}/
+0001ebe0: 7b7d 5c6e 7b7d 220a 2020 2020 2020 2020  {}\n{}".        
+0001ebf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ec00: 2e6c 6f67 2874 2e66 6f72 6d61 7428 7264  .log(t.format(rd
+0001ec10: 2c20 666e 2c20 6d69 6e5f 6578 2829 2929  , fn, min_ex()))
+0001ec20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ec30: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+0001ec40: 2020 2020 2020 2020 6665 5b22 7461 6773          fe["tags
+0001ec50: 225d 203d 207b 6b3a 2076 2066 6f72 206b  "] = {k: v for k
+0001ec60: 2c20 7620 696e 2072 7d0a 0a20 2020 2020  , v in r}..     
+0001ec70: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
+0001ec80: 616e 5f61 646d 696e 3a0a 2020 2020 2020  an_admin:.      
+0001ec90: 2020 2020 2020 2020 2020 7120 3d20 2273            q = "s
+0001eca0: 656c 6563 7420 6970 2c20 6174 2066 726f  elect ip, at fro
+0001ecb0: 6d20 7570 2077 6865 7265 2072 643d 3f20  m up where rd=? 
+0001ecc0: 616e 6420 666e 3d3f 220a 2020 2020 2020  and fn=?".      
+0001ecd0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+0001ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecf0: 2020 207a 7331 2c20 7a73 3220 3d20 6963     zs1, zs2 = ic
+0001ed00: 7572 2e65 7865 6375 7465 2871 2c20 6572  ur.execute(q, er
+0001ed10: 645f 6566 6e29 2e66 6574 6368 6f6e 6528  d_efn).fetchone(
+0001ed20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001ed30: 2020 2020 2020 6665 5b22 7461 6773 225d        fe["tags"]
+0001ed40: 5b22 7570 5f69 7022 5d20 3d20 7a73 310a  ["up_ip"] = zs1.
+0001ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed60: 2020 2020 6665 5b22 7461 6773 225d 5b22      fe["tags"]["
+0001ed70: 2e75 705f 6174 225d 203d 207a 7332 0a20  .up_at"] = zs2. 
+0001ed80: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0001ed90: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+0001eda0: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+0001edb0: 0a20 2020 2020 2020 2020 2020 205f 203d  .            _ =
+0001edc0: 205b 7461 6773 6574 2e61 6464 286b 2920   [tagset.add(k) 
+0001edd0: 666f 7220 6b20 696e 2066 655b 2274 6167  for k in fe["tag
+0001ede0: 7322 5d5d 0a0a 2020 2020 2020 2020 6966  s"]]..        if
+0001edf0: 2069 6375 723a 0a20 2020 2020 2020 2020   icur:.         
+0001ee00: 2020 206d 7465 203d 2076 6e2e 666c 6167     mte = vn.flag
+0001ee10: 732e 6765 7428 226d 7465 2229 206f 7220  s.get("mte") or 
+0001ee20: 2275 705f 6970 2c2e 7570 5f61 7422 0a20  "up_ip,.up_at". 
+0001ee30: 2020 2020 2020 2020 2020 2074 6167 6c69             tagli
+0001ee40: 7374 203d 205b 6b20 666f 7220 6b20 696e  st = [k for k in
+0001ee50: 206d 7465 2e73 706c 6974 2822 2c22 2920   mte.split(",") 
+0001ee60: 6966 206b 2069 6e20 7461 6773 6574 5d0a  if k in tagset].
+0001ee70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0001ee80: 6665 2069 6e20 6469 7273 3a0a 2020 2020  fe in dirs:.    
+0001ee90: 2020 2020 2020 2020 2020 2020 6665 5b22              fe["
+0001eea0: 7461 6773 225d 203d 207b 7d0a 2020 2020  tags"] = {}.    
+0001eeb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001eec0: 2020 2020 2020 7461 676c 6973 7420 3d20        taglist = 
+0001eed0: 6c69 7374 2874 6167 7365 7429 0a0a 2020  list(tagset)..  
+0001eee0: 2020 2020 2020 6966 2069 735f 6c73 3a0a        if is_ls:.
+0001eef0: 2020 2020 2020 2020 2020 2020 6c73 5f72              ls_r
+0001ef00: 6574 5b22 6469 7273 225d 203d 2064 6972  et["dirs"] = dir
+0001ef10: 730a 2020 2020 2020 2020 2020 2020 6c73  s.            ls
+0001ef20: 5f72 6574 5b22 6669 6c65 7322 5d20 3d20  _ret["files"] = 
+0001ef30: 6669 6c65 730a 2020 2020 2020 2020 2020  files.          
+0001ef40: 2020 6c73 5f72 6574 5b22 7461 676c 6973    ls_ret["taglis
+0001ef50: 7422 5d20 3d20 7461 676c 6973 740a 2020  t"] = taglist.  
+0001ef60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001ef70: 2073 656c 662e 7478 5f6c 7328 6c73 5f72   self.tx_ls(ls_r
+0001ef80: 6574 290a 0a20 2020 2020 2020 2064 6f63  et)..        doc
+0001ef90: 203d 2073 656c 662e 7570 6172 616d 2e67   = self.uparam.g
+0001efa0: 6574 2822 646f 6322 2920 6966 2073 656c  et("doc") if sel
+0001efb0: 662e 6361 6e5f 7265 6164 2065 6c73 6520  f.can_read else 
+0001efc0: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+0001efd0: 646f 633a 0a20 2020 2020 2020 2020 2020  doc:.           
+0001efe0: 2064 6f63 203d 2075 6e71 756f 7465 7028   doc = unquotep(
+0001eff0: 646f 632e 7265 706c 6163 6528 222b 222c  doc.replace("+",
+0001f000: 2022 2022 292e 7370 6c69 7428 223f 2229   " ").split("?")
+0001f010: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0001f020: 206a 3261 5b22 646f 636e 616d 6522 5d20   j2a["docname"] 
+0001f030: 3d20 646f 630a 2020 2020 2020 2020 2020  = doc.          
+0001f040: 2020 646f 6374 7874 203d 204e 6f6e 650a    doctxt = None.
+0001f050: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+0001f060: 6578 7428 2878 2066 6f72 2078 2069 6e20  ext((x for x in 
+0001f070: 6669 6c65 7320 6966 2078 5b22 6e61 6d65  files if x["name
+0001f080: 225d 203d 3d20 646f 6329 2c20 4e6f 6e65  "] == doc), None
+0001f090: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001f0a0: 2020 2064 6f63 7061 7468 203d 206f 732e     docpath = os.
+0001f0b0: 7061 7468 2e6a 6f69 6e28 6162 7370 6174  path.join(abspat
+0001f0c0: 682c 2064 6f63 290a 2020 2020 2020 2020  h, doc).        
+0001f0d0: 2020 2020 2020 2020 737a 203d 2062 6f73          sz = bos
+0001f0e0: 2e70 6174 682e 6765 7473 697a 6528 646f  .path.getsize(do
+0001f0f0: 6370 6174 6829 0a20 2020 2020 2020 2020  cpath).         
+0001f100: 2020 2020 2020 2069 6620 737a 203c 2031         if sz < 1
+0001f110: 3032 3420 2a20 7365 6c66 2e61 7267 732e  024 * self.args.
+0001f120: 7478 745f 6d61 783a 0a20 2020 2020 2020  txt_max:.       
+0001f130: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0001f140: 6820 6f70 656e 2866 7365 6e63 2864 6f63  h open(fsenc(doc
+0001f150: 7061 7468 292c 2022 7262 2229 2061 7320  path), "rb") as 
+0001f160: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+0001f170: 2020 2020 2020 2020 2020 2064 6f63 7478             doctx
+0001f180: 7420 3d20 662e 7265 6164 2829 2e64 6563  t = f.read().dec
+0001f190: 6f64 6528 2275 7466 2d38 222c 2022 7265  ode("utf-8", "re
+0001f1a0: 706c 6163 6522 290a 2020 2020 2020 2020  place").        
+0001f1b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001f1c0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0001f1d0: 6f67 2822 646f 6320 3430 343a 205b 7b7d  og("doc 404: [{}
+0001f1e0: 5d22 2e66 6f72 6d61 7428 646f 6329 2c20  ]".format(doc), 
+0001f1f0: 633d 3629 0a20 2020 2020 2020 2020 2020  c=6).           
+0001f200: 2020 2020 2064 6f63 7478 7420 3d20 2228       doctxt = "(
+0001f210: 2074 6578 7466 696c 6520 6e6f 7420 666f   textfile not fo
+0001f220: 756e 6420 2922 0a0a 2020 2020 2020 2020  und )"..        
+0001f230: 2020 2020 6966 2064 6f63 7478 7420 6973      if doctxt is
+0001f240: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0001f250: 2020 2020 2020 2020 2020 206a 3261 5b22             j2a["
+0001f260: 646f 6322 5d20 3d20 646f 6374 7874 0a0a  doc"] = doctxt..
+0001f270: 2020 2020 2020 2020 666f 7220 6420 696e          for d in
+0001f280: 2064 6972 733a 0a20 2020 2020 2020 2020   dirs:.         
+0001f290: 2020 2064 5b22 6e61 6d65 225d 202b 3d20     d["name"] += 
+0001f2a0: 222f 220a 0a20 2020 2020 2020 2064 6972  "/"..        dir
+0001f2b0: 732e 736f 7274 286b 6579 3d69 7465 6d67  s.sort(key=itemg
+0001f2c0: 6574 7465 7228 226e 616d 6522 2929 0a0a  etter("name"))..
+0001f2d0: 2020 2020 2020 2020 6966 2069 735f 6a73          if is_js
+0001f2e0: 3a0a 2020 2020 2020 2020 2020 2020 6a32  :.            j2
+0001f2f0: 615b 226c 7330 225d 203d 207b 0a20 2020  a["ls0"] = {.   
+0001f300: 2020 2020 2020 2020 2020 2020 2022 6469               "di
+0001f310: 7273 223a 2064 6972 732c 0a20 2020 2020  rs": dirs,.     
+0001f320: 2020 2020 2020 2020 2020 2022 6669 6c65             "file
+0001f330: 7322 3a20 6669 6c65 732c 0a20 2020 2020  s": files,.     
+0001f340: 2020 2020 2020 2020 2020 2022 7461 676c             "tagl
+0001f350: 6973 7422 3a20 7461 676c 6973 742c 0a20  ist": taglist,. 
+0001f360: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001f370: 756e 6c69 7374 223a 2075 6e6c 6973 742c  unlist": unlist,
+0001f380: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+0001f390: 2020 2020 2020 2020 2020 206a 3261 5b22             j2a["
+0001f3a0: 6669 6c65 7322 5d20 3d20 5b5d 0a20 2020  files"] = [].   
+0001f3b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001f3c0: 2020 2020 2020 206a 3261 5b22 6669 6c65         j2a["file
+0001f3d0: 7322 5d20 3d20 6469 7273 202b 2066 696c  s"] = dirs + fil
+0001f3e0: 6573 0a0a 2020 2020 2020 2020 6a32 615b  es..        j2a[
+0001f3f0: 2274 6167 6c69 7374 225d 203d 2074 6167  "taglist"] = tag
+0001f400: 6c69 7374 0a20 2020 2020 2020 206a 3261  list.        j2a
+0001f410: 5b22 7478 745f 6578 7422 5d20 3d20 7365  ["txt_ext"] = se
+0001f420: 6c66 2e61 7267 732e 7465 7874 6669 6c65  lf.args.textfile
+0001f430: 732e 7265 706c 6163 6528 222c 222c 2022  s.replace(",", "
+0001f440: 2022 290a 0a20 2020 2020 2020 2069 6620   ")..        if 
+0001f450: 226d 7468 2220 696e 2076 6e2e 666c 6167  "mth" in vn.flag
+0001f460: 733a 0a20 2020 2020 2020 2020 2020 206a  s:.            j
+0001f470: 3261 5b22 6465 665f 6863 6f6c 7322 5d20  2a["def_hcols"] 
+0001f480: 3d20 766e 2e66 6c61 6773 5b22 6d74 6822  = vn.flags["mth"
+0001f490: 5d2e 7370 6c69 7428 222c 2229 0a0a 2020  ].split(",")..  
+0001f4a0: 2020 2020 2020 6874 6d6c 203d 2073 656c        html = sel
+0001f4b0: 662e 6a32 7328 7470 6c2c 202a 2a6a 3261  f.j2s(tpl, **j2a
+0001f4c0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+0001f4d0: 6570 6c79 2868 746d 6c2e 656e 636f 6465  eply(html.encode
+0001f4e0: 2822 7574 662d 3822 2c20 2272 6570 6c61  ("utf-8", "repla
+0001f4f0: 6365 2229 290a 2020 2020 2020 2020 7265  ce")).        re
+0001f500: 7475 726e 2054 7275 650a                 turn True.
```

### Comparing `copyparty-1.8.4/copyparty/httpconn.py` & `copyparty-1.8.6/copyparty/httpconn.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/httpsrv.py` & `copyparty-1.8.6/copyparty/httpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/ico.py` & `copyparty-1.8.6/copyparty/ico.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/mdns.py` & `copyparty-1.8.6/copyparty/mdns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/mtag.py` & `copyparty-1.8.6/copyparty/mtag.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/multicast.py` & `copyparty-1.8.6/copyparty/multicast.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/pwhash.py` & `copyparty-1.8.6/copyparty/pwhash.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/res/COPYING.txt` & `copyparty-1.8.6/copyparty/res/COPYING.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/res/insecure.pem` & `copyparty-1.8.6/copyparty/res/insecure.pem`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/smbd.py` & `copyparty-1.8.6/copyparty/smbd.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/ssdp.py` & `copyparty-1.8.6/copyparty/ssdp.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/star.py` & `copyparty-1.8.6/copyparty/star.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/dnslib/bimap.py` & `copyparty-1.8.6/copyparty/stolen/dnslib/bimap.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/dnslib/buffer.py` & `copyparty-1.8.6/copyparty/stolen/dnslib/buffer.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/dnslib/dns.py` & `copyparty-1.8.6/copyparty/stolen/dnslib/dns.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/dnslib/label.py` & `copyparty-1.8.6/copyparty/stolen/dnslib/label.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/dnslib/lex.py` & `copyparty-1.8.6/copyparty/stolen/dnslib/lex.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/dnslib/ranges.py` & `copyparty-1.8.6/copyparty/stolen/dnslib/ranges.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/ifaddr/_posix.py` & `copyparty-1.8.6/copyparty/stolen/ifaddr/_posix.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/ifaddr/_shared.py` & `copyparty-1.8.6/copyparty/stolen/ifaddr/_shared.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/ifaddr/_win32.py` & `copyparty-1.8.6/copyparty/stolen/ifaddr/_win32.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/qrcodegen.py` & `copyparty-1.8.6/copyparty/stolen/qrcodegen.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/stolen/surrogateescape.py` & `copyparty-1.8.6/copyparty/stolen/surrogateescape.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/sutil.py` & `copyparty-1.8.6/copyparty/sutil.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/svchub.py` & `copyparty-1.8.6/copyparty/svchub.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/szip.py` & `copyparty-1.8.6/copyparty/szip.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/tcpsrv.py` & `copyparty-1.8.6/copyparty/tcpsrv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/th_cli.py` & `copyparty-1.8.6/copyparty/th_cli.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/th_srv.py` & `copyparty-1.8.6/copyparty/th_srv.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/u2idx.py` & `copyparty-1.8.6/copyparty/u2idx.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/up2k.py` & `copyparty-1.8.6/copyparty/up2k.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/util.py` & `copyparty-1.8.6/copyparty/util.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/a/partyfuse.py` & `copyparty-1.8.6/copyparty/web/a/partyfuse.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/a/u2c.py` & `copyparty-1.8.6/copyparty/web/a/u2c.py`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/a/webdav-cfg.bat` & `copyparty-1.8.6/copyparty/web/a/webdav-cfg.bat`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/baguettebox.js.gz` & `copyparty-1.8.6/copyparty/web/baguettebox.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/browser.css.gz` & `copyparty-1.8.6/copyparty/web/browser.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/browser.html` & `copyparty-1.8.6/copyparty/web/browser.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/browser.js.gz` & `copyparty-1.8.6/copyparty/web/browser.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/browser2.html` & `copyparty-1.8.6/copyparty/web/browser2.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/cf.html` & `copyparty-1.8.6/copyparty/web/cf.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/dbg-audio.js.gz` & `copyparty-1.8.6/copyparty/web/dbg-audio.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/easymde.css.gz` & `copyparty-1.8.6/copyparty/web/deps/easymde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/easymde.js.gz` & `copyparty-1.8.6/copyparty/web/deps/easymde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/marked.js.gz` & `copyparty-1.8.6/copyparty/web/deps/marked.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/mini-fa.css.gz` & `copyparty-1.8.6/copyparty/web/deps/mini-fa.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/mini-fa.woff` & `copyparty-1.8.6/copyparty/web/deps/mini-fa.woff`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/prism.css.gz` & `copyparty-1.8.6/copyparty/web/deps/prism.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/prism.js.gz` & `copyparty-1.8.6/copyparty/web/deps/prism.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/prismd.css.gz` & `copyparty-1.8.6/copyparty/web/deps/prismd.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/scp.woff2` & `copyparty-1.8.6/copyparty/web/deps/scp.woff2`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/sha512.ac.js.gz` & `copyparty-1.8.6/copyparty/web/deps/sha512.ac.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/deps/sha512.hw.js.gz` & `copyparty-1.8.6/copyparty/web/deps/sha512.hw.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/md.css.gz` & `copyparty-1.8.6/copyparty/web/md.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/md.html` & `copyparty-1.8.6/copyparty/web/md.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/md.js.gz` & `copyparty-1.8.6/copyparty/web/md.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/md2.css.gz` & `copyparty-1.8.6/copyparty/web/md2.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/md2.js.gz` & `copyparty-1.8.6/copyparty/web/md2.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/mde.css.gz` & `copyparty-1.8.6/copyparty/web/mde.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/mde.html` & `copyparty-1.8.6/copyparty/web/mde.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/mde.js.gz` & `copyparty-1.8.6/copyparty/web/mde.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/msg.html` & `copyparty-1.8.6/copyparty/web/msg.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/splash.css.gz` & `copyparty-1.8.6/copyparty/web/splash.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/splash.html` & `copyparty-1.8.6/copyparty/web/splash.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/splash.js.gz` & `copyparty-1.8.6/copyparty/web/splash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/svcs.html` & `copyparty-1.8.6/copyparty/web/svcs.html`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/svcs.js.gz` & `copyparty-1.8.6/copyparty/web/svcs.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/ui.css.gz` & `copyparty-1.8.6/copyparty/web/ui.css.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/up2k.js.gz` & `copyparty-1.8.6/copyparty/web/up2k.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/util.js.gz` & `copyparty-1.8.6/copyparty/web/util.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty/web/w.hash.js.gz` & `copyparty-1.8.6/copyparty/web/w.hash.js.gz`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/copyparty.egg-info/PKG-INFO` & `copyparty-1.8.6/copyparty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyparty
-Version: 1.8.4
+Version: 1.8.6
 Summary:   Portable file server with accelerated resumable uploads, deduplication, WebDAV, FTP, zeroconf, media indexer, video thumbnails, audio transcoding, and write-only folders
 Author-email: ed <copyparty@ocv.me>
 License: MIT
 Project-URL: Source Code, https://github.com/9001/copyparty
 Project-URL: Bug Tracker, https://github.com/9001/copyparty/issues
 Project-URL: Demo Server, https://a.ocv.me/pub/demo/
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `copyparty-1.8.4/copyparty.egg-info/SOURCES.txt` & `copyparty-1.8.6/copyparty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copyparty-1.8.4/pyproject.toml` & `copyparty-1.8.6/pyproject.toml`

 * *Files identical despite different names*

