# Comparing `tmp/ralph-malph-3.8.0.tar.gz` & `tmp/ralph-malph-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralph-malph-3.8.0.tar", last modified: Wed Jun 21 14:01:33 2023, max compression
+gzip compressed data, was "ralph-malph-3.9.0.tar", last modified: Fri Jul 21 14:54:50 2023, max compression
```

## Comparing `ralph-malph-3.8.0.tar` & `ralph-malph-3.9.0.tar`

### file list

```diff
@@ -1,188 +1,189 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/LICENSE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/ralph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/__main__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/ralph/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.238829 ralph-malph-3.8.0/src/ralph/api/auth/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5871 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4882 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/oidc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/auth/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/forwarding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/models.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/api/routers/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/routers/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/routers/health.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16304 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/api/routers/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/database/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/base.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13603 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/clickhouse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9315 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9873 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/database/mongo.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/http/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/http/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3713 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/http/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10463 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/http/lrs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/mixins.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/storage/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/fs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/ldp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5310 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/s3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/storage/swift.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/backends/stream/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/stream/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/stream/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/backends/stream/ws.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21846 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12019 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/logger.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.242829 ralph-malph-3.8.0/src/ralph/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/converter.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2066 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/browser.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/converters/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3000 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/navigational.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7195 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/enrollment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/navigational/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/navigational/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10009 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8242 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.246829 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/edx/video/fields/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/fields/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/fields/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/edx/video/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/selector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/validator.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/xapi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/xapi/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2055 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/agents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/attachments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/common.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/groups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/ifi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1455 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4079 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/unnested_objects.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/base/verbs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.250829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/video.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1170 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/video.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4575 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/constants.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/navigation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/navigation/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/navigation/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/video/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9579 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5263 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7587 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/video/statements.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.254829 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7328 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/contexts.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/results.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/statements.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2919 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/src/ralph/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/src/ralph_malph.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5925 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1127 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-21 14:01:33.000000 ralph-malph-3.8.0/src/ralph_malph.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-21 14:01:33.258829 ralph-malph-3.8.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26259 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9962 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_cli_usage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_dependencies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_filters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_parsers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-06-21 14:01:32.000000 ralph-malph-3.8.0/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.616606 ralph-malph-3.9.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1094 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/LICENSE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-07-21 14:54:50.616606 ralph-malph-3.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5291 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2822 2023-07-21 14:54:50.616606 ralph-malph-3.9.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.596606 ralph-malph-3.9.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/api/auth/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      437 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/auth/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5871 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/auth/basic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4882 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/auth/oidc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/auth/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1892 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/forwarding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1658 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/models.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/api/routers/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/routers/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1009 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/routers/health.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17485 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/api/routers/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/backends/database/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      122 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/database/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/database/base.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13939 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/database/clickhouse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9315 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/database/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9992 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/database/mongo.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/backends/http/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/http/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14092 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/http/async_lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3734 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/http/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1369 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/http/lrs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/mixins.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.600606 ralph-malph-3.9.0/src/ralph/backends/storage/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/storage/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      685 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/storage/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4026 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/storage/fs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4995 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/storage/ldp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5310 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/storage/s3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6485 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/storage/swift.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/backends/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      304 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/stream/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1003 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/backends/stream/ws.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22490 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12089 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      940 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      384 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/logger.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9015 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/converter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2066 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/browser.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/converters/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/converters/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      333 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3000 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      913 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/navigational.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      887 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7195 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/fields/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      927 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/enrollment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/navigational/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/navigational/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/navigational/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/navigational/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/navigational/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3602 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/navigational/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10009 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8242 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.604606 ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13075 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10605 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1949 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10265 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13320 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/video/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/edx/video/fields/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/video/fields/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3031 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/video/fields/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8175 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/edx/video/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5215 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/selector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/validator.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/xapi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/xapi/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2055 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/attachments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/groups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/ifi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1455 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2343 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3067 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4079 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/unnested_objects.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      449 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/base/verbs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.608606 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.612606 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      900 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2893 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1236 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.612606 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      154 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      202 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/cmi5_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      222 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1689 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/video.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.612606 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      721 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1072 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1157 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2151 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1170 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1625 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/video.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4575 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/constants.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.612606 ralph-malph-3.9.0/src/ralph/models/xapi/navigation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/navigation/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1308 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/navigation/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.612606 ralph-malph-3.9.0/src/ralph/models/xapi/video/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/video/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9579 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/video/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5263 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/video/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7587 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/video/statements.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.612606 ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7328 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/contexts.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/results.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12787 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/statements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2731 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3714 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/src/ralph/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.616606 ralph-malph-3.9.0/src/ralph_malph.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6471 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5962 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1133 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 14:54:50.000000 ralph-malph-3.9.0/src/ralph_malph.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 14:54:50.616606 ralph-malph-3.9.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26350 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13861 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_cli_usage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6621 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1478 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_dependencies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      625 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_filters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2401 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4904 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_parsers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3919 2023-07-21 14:54:49.000000 ralph-malph-3.9.0/tests/test_utils.py
```

### Comparing `ralph-malph-3.8.0/LICENSE.md` & `ralph-malph-3.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/PKG-INFO` & `ralph-malph-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.8.0
+Version: 3.9.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ralph-malph-3.8.0/README.md` & `ralph-malph-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/setup.cfg` & `ralph-malph-3.9.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ralph-malph
-version = 3.8.0
+version = 3.9.0
 description = The ultimate toolbox for your learning analytics
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Open FUN (France Universite Numerique)
 author_email = fun.dev@fun-mooc.fr
 url = https://openfun.github.io/ralph/
 license = MIT
@@ -21,15 +21,15 @@
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 include_package_data = True
 install_requires = 
 	langcodes>=3.2.0
-	pydantic[dotenv,email]>=1.10.0
+	pydantic[dotenv,email]>=1.10.0, <2.0
 	rfc3987>=1.3.0
 package_dir = 
 	=src
 packages = find:
 zip_safe = True
 python_requires = >= 3.7
 
@@ -59,45 +59,45 @@
 cli = 
 	bcrypt>=4.0.0
 	click>=8.1.0
 	click-option-group>=0.5.0
 	sentry-sdk[fastapi]>=1.9.0
 dev = 
 	bandit==1.7.5
-	black==23.3.0
-	cryptography==41.0.1
+	black==23.7.0
+	cryptography==41.0.2
 	factory-boy==3.2.1
 	flake8==6.0.0
-	hypothesis==6.79.1
+	hypothesis==6.81.2
 	isort==5.12.0
 	logging-gelf==0.0.31
 	mkdocs==1.4.3
 	mkdocs-click==0.8.0
-	mkdocs-material==9.1.16
+	mkdocs-material==9.1.18
 	mkdocstrings[python-legacy]==0.22.0
-	moto==4.1.11
+	moto==4.1.13
 	pydocstyle==6.3.0
-	pyfakefs==5.2.2
+	pyfakefs==5.2.3
 	pylint==2.17.4
-	pytest==7.3.2
-	pytest-asyncio==0.21.0
+	pytest==7.4.0
+	pytest-asyncio==0.21.1
 	pytest-cov==4.1.0
 	pytest-httpx==0.22.0
 	responses==0.23.1
 ci = 
 	twine==4.0.2
 lrs = 
 	bcrypt==4.0.1
-	fastapi==0.97.0
+	fastapi==0.100.0
 	cachetools==5.3.1
 	h11>=0.11.0
 	httpx==0.24.1
-	sentry_sdk==1.25.1
+	sentry_sdk==1.28.1
 	python-jose==3.3.0
-	uvicorn[standard]==0.22.0
+	uvicorn[standard]==0.23.0
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	ralph = ralph.__main__:cli.cli
@@ -105,14 +105,15 @@
 [wheel]
 universal = 1
 
 [flake8]
 max-line-length = 88
 extend-ignore = E203
 exclude = 
+	.conda
 	.git,
 	.venv,
 	build,
 	venv,
 	__pycache__,
 	node_modules,
 	*/migrations/*
```

### Comparing `ralph-malph-3.8.0/src/ralph/__main__.py` & `ralph-malph-3.9.0/src/ralph/__main__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/__init__.py` & `ralph-malph-3.9.0/src/ralph/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/auth/basic.py` & `ralph-malph-3.9.0/src/ralph/api/auth/basic.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/auth/oidc.py` & `ralph-malph-3.9.0/src/ralph/api/auth/oidc.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/forwarding.py` & `ralph-malph-3.9.0/src/ralph/api/forwarding.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/models.py` & `ralph-malph-3.9.0/src/ralph/api/models.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/routers/health.py` & `ralph-malph-3.9.0/src/ralph/api/routers/health.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/api/routers/statements.py` & `ralph-malph-3.9.0/src/ralph/api/routers/statements.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from fastapi import (
     APIRouter,
     BackgroundTasks,
     Depends,
     HTTPException,
     Query,
     Request,
+    Response,
     status,
 )
 from pydantic import parse_raw_as
 from pydantic.types import Json
 
 from ralph.api.auth import get_authenticated_user
 from ralph.api.forwarding import forward_xapi_statements, get_active_xapi_forwardings
@@ -26,14 +27,15 @@
 from ralph.models.xapi.base.agents import (
     BaseXapiAgent,
     BaseXapiAgentWithAccount,
     BaseXapiAgentWithMbox,
     BaseXapiAgentWithMboxSha1Sum,
     BaseXapiAgentWithOpenId,
 )
+from ralph.models.xapi.base.common import IRI
 
 from ..models import ErrorDetail, LaxStatement
 
 logger = logging.getLogger(__name__)
 
 router = APIRouter(
     prefix="/xAPI/statements",
@@ -78,15 +80,15 @@
             "Agent or Group is the Actor or Object of the Statement"
         ),
     ),
     verb: Optional[str] = Query(
         None,
         description="Filter, only return Statements matching the specified Verb id",
     ),
-    activity: Optional[str] = Query(
+    activity: Optional[IRI] = Query(
         None,
         description=(
             "Filter, only return Statements for which the Object "
             "of the Statement is an Activity with the specified id"
         ),
     ),
     # pylint: disable=unused-argument
@@ -227,15 +229,15 @@
     # NB: bool(param) relies on all defaults being None, 0, or False
     if (statementId or voidedStatementId) and any(
         bool(param) for param in excluded_params
     ):
         raise HTTPException(
             status_code=status.HTTP_400_BAD_REQUEST,
             detail=(
-                "Querying by id only accepts `attachments` and `format` as extra"
+                "Querying by id only accepts `attachments` and `format` as extra "
                 "parameters"
             ),
         )
 
     # Parse the agent parameter (JSON) into multiple string parameters
     query_params = dict(request.query_params)
     if query_params.get("agent") is not None:
@@ -327,29 +329,32 @@
 
     if get_active_xapi_forwardings():
         background_tasks.add_task(
             forward_xapi_statements, list(statement_dict.values())
         )
 
     try:
-        statements_ids_result = DATABASE_CLIENT.query_statements_by_ids([statementId])
+        existing_statement = DATABASE_CLIENT.query_statements_by_ids([statementId])
     except BackendException as error:
         raise HTTPException(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
             detail="xAPI statements query failed",
         ) from error
 
-    if len(statements_ids_result) > 0:
-        # NB: LRS specification calls for performing a deep comparison of incoming
-        # statements and existing statements with the same ID.
-        # This seems too costly for performance and was not implemented for this POC.
-        raise HTTPException(
-            status_code=status.HTTP_409_CONFLICT,
-            detail="Statement already exists with the same ID",
-        )
+    if existing_statement:
+        # The LRS specification calls for deep comparison of duplicate statement ids.
+        # In the case that the current statement is not an exact duplicate of the one
+        # found in the database we return a 409, otherwise the usual 204.
+        for existing in existing_statement:
+            if statement_dict != existing["_source"]:
+                raise HTTPException(
+                    status_code=status.HTTP_409_CONFLICT,
+                    detail="A different statement already exists with the same ID",
+                )
+        return
 
     # For valid requests, perform the bulk indexing of all incoming statements
     try:
         success_count = DATABASE_CLIENT.put(
             statement_dict.values(), ignore_errors=False
         )
     except (BackendException, BadFormatException) as exc:
@@ -363,14 +368,15 @@
 
 
 @router.post("/", responses=POST_PUT_RESPONSES)
 @router.post("", responses=POST_PUT_RESPONSES)
 async def post(
     statements: Union[LaxStatement, List[LaxStatement]],
     background_tasks: BackgroundTasks,
+    response: Response,
 ):
     """Stores a set of statements (or a single statement as a single member of a set).
 
     NB: at this time, using POST to make a GET request, is not supported.
     LRS Specification:
     https://github.com/adlnet/xAPI-Spec/blob/1.0.3/xAPI-Communication.md#212-post-statements
     """
@@ -400,29 +406,52 @@
 
     if get_active_xapi_forwardings():
         background_tasks.add_task(
             forward_xapi_statements, list(statements_dict.values())
         )
 
     try:
-        statements_ids_result = DATABASE_CLIENT.query_statements_by_ids(statements_ids)
+        existing_statements = DATABASE_CLIENT.query_statements_by_ids(statements_ids)
     except BackendException as error:
         raise HTTPException(
             status_code=status.HTTP_500_INTERNAL_SERVER_ERROR,
             detail="xAPI statements query failed",
         ) from error
 
-    if len(statements_ids_result) > 0:
-        # NB: LRS specification calls for performing a deep comparison of incoming
-        # statements and existing statements with the same ID.
-        # This seems too costly for performance and was not implemented for this POC.
-        raise HTTPException(
-            status_code=status.HTTP_409_CONFLICT,
-            detail="Statements already exist with the same ID",
-        )
+    # If there are duplicate statements, remove them from our id list and
+    # dictionary for insertion. We will return the shortened list of ids below
+    # so that consumers can derive which statements were inserted and which
+    # were skipped for being duplicates.
+    # See: https://github.com/openfun/ralph/issues/345
+    if existing_statements:
+        existing_ids = []
+        for existing in existing_statements:
+            existing_ids.append(existing["_id"])
+
+            # The LRS specification calls for deep comparison of duplicates. This
+            # is done here. If they are not exactly the same, we raise an error.
+            if statements_dict[existing["_id"]] != existing["_source"]:
+                raise HTTPException(
+                    status_code=status.HTTP_409_CONFLICT,
+                    detail="Differing statements already exist with the same ID: "
+                    f"{existing['_id']}",
+                )
+
+        # Overwrite our statements and ids with the deduplicated ones.
+        statements_ids = [id for id in statements_ids if id not in existing_ids]
+
+        statements_dict = {
+            key: value
+            for key, value in statements_dict.items()
+            if key in statements_ids
+        }
+
+        if not statements_ids:
+            response.status_code = status.HTTP_204_NO_CONTENT
+            return
 
     # For valid requests, perform the bulk indexing of all incoming statements
     try:
         success_count = DATABASE_CLIENT.put(
             statements_dict.values(), ignore_errors=False
         )
     except (BackendException, BadFormatException) as exc:
```

### Comparing `ralph-malph-3.8.0/src/ralph/backends/database/base.py` & `ralph-malph-3.9.0/src/ralph/backends/database/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/database/clickhouse.py` & `ralph-malph-3.9.0/src/ralph/backends/database/clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,42 +234,49 @@
         if len(batch) > 0:
             rows_inserted += self.bulk_import(batch, ignore_errors=ignore_errors)
 
         logger.debug("Inserted a total of %s documents with success", rows_inserted)
 
         return rows_inserted
 
-    def query_statements_by_ids(self, ids: List[str]) -> List:
-        """Returns the list of matching statement IDs from the database."""
+    def query_statements_by_ids(self, ids: List[str]) -> List[dict]:
+        """Returns the list of matching statements from the database."""
 
         def chunk_id_list(chunk_size=10000):
             for i in range(0, len(ids), chunk_size):
                 yield ids[i : i + chunk_size]
 
         sql = """
-                SELECT event_id
+                SELECT event_id, event_str
                 FROM {table_name:Identifier}
                 WHERE event_id IN ({ids:Array(String)})
         """
 
         query_context = self.client.create_query_context(
             query=sql,
             parameters={"ids": ["1"], "table_name": self.event_table_name},
             column_oriented=True,
         )
 
-        found_ids = []
+        found_statements = []
 
         try:
             for chunk_ids in chunk_id_list():
                 query_context.set_parameter("ids", chunk_ids)
                 result = self.client.query(context=query_context).named_results()
-                found_ids.extend(result)
+                for row in result:
+                    # This is the format to match the other backends
+                    found_statements.append(
+                        {
+                            "_id": str(row["event_id"]),
+                            "_source": json.loads(row["event_str"]),
+                        }
+                    )
 
-            return found_ids
+            return found_statements
         except (ClickHouseError, IndexError, TypeError, ValueError) as error:
             msg = "Failed to execute ClickHouse query"
             logger.error("%s. %s", msg, error)
             raise BackendException(msg, *error.args) from error
 
     def query_statements(self, params: StatementParameters) -> StatementQueryResult:
         """Returns the results of a statements query using xAPI parameters."""
```

### Comparing `ralph-malph-3.8.0/src/ralph/backends/database/es.py` & `ralph-malph-3.9.0/src/ralph/backends/database/es.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/database/mongo.py` & `ralph-malph-3.9.0/src/ralph/backends/database/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,16 +250,19 @@
         return StatementQueryResult(
             statements=[document["_source"] for document in mongo_response],
             pit_id=None,
             search_after=search_after,
         )
 
     def query_statements_by_ids(self, ids: List[str]) -> List:
-        """Returns the list of matching statement IDs from the database."""
-        return self._find(filter={"_source.id": {"$in": ids}})
+        """Returns the list of matching statements from the database."""
+        return [
+            {"_id": statement["_source"]["id"], "_source": statement["_source"]}
+            for statement in self._find(filter={"_source.id": {"$in": ids}})
+        ]
 
     def _find(self, **kwargs):
         """Wraps the MongoClient.collection.find method.
 
         Raises:
             BackendException: raised for any failure.
         """
```

### Comparing `ralph-malph-3.8.0/src/ralph/backends/http/base.py` & `ralph-malph-3.9.0/src/ralph/backends/http/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,37 +95,37 @@
             )
 
         logger.debug("Query: %s", str(query))
 
         return query
 
     @abstractmethod
-    def list(
+    async def list(
         self, target: str = None, details: bool = False, new: bool = False
     ) -> Iterator[Union[str, dict]]:
-        """Lists containers in the data backend. E.g., collections, files, indexes."""
+        """List containers in the data backend. E.g., collections, files, indexes."""
 
     @abstractmethod
-    def status(self) -> HTTPBackendStatus:
-        """Implements HTTP backend check for server status."""
+    async def status(self) -> HTTPBackendStatus:
+        """Implement HTTP backend check for server status."""
 
     @abstractmethod
     @enforce_query_checks
-    def read(  # pylint: disable=too-many-arguments
+    async def read(  # pylint: disable=too-many-arguments
         self,
         query: Union[str, BaseQuery] = None,
         target: str = None,
         chunk_size: Union[None, int] = 500,
         raw_output: bool = False,
         ignore_errors: bool = False,
     ) -> Iterator[Union[bytes, dict]]:
-        """Yields records read from the HTTP response results."""
+        """Yield records read from the HTTP response results."""
 
     @abstractmethod
-    def write(  # pylint: disable=too-many-arguments
+    async def write(  # pylint: disable=too-many-arguments
         self,
         data: Union[List[bytes], List[dict]],
         target: Union[None, str] = None,
         chunk_size: Union[None, int] = 500,
         ignore_errors: bool = False,
         operation_type: Union[None, OperationType] = None,
     ) -> int:
```

### Comparing `ralph-malph-3.8.0/src/ralph/backends/http/lrs.py` & `ralph-malph-3.9.0/src/ralph/backends/http/async_lrs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-"""LRS HTTP backend for Ralph."""
+"""Async LRS HTTP backend for Ralph."""
 
+import asyncio
 import json
 import logging
 from itertools import chain
 from typing import Iterable, Iterator, List, Optional, Union
 from urllib.parse import ParseResult, parse_qs, urljoin, urlparse
 
-import httpx
-from httpx import Client, HTTPError, HTTPStatusError, RequestError
+from httpx import AsyncClient, HTTPError, HTTPStatusError, RequestError
 from more_itertools import chunked
 from pydantic import AnyHttpUrl, BaseModel, parse_obj_as
 
 from ralph.conf import LRSHeaders, settings
 from ralph.exceptions import BackendException, BackendParameterException
+from ralph.utils import gather_with_limited_concurrency
 
 from .base import (
     BaseHTTP,
     BaseQuery,
     HTTPBackendStatus,
     OperationType,
     enforce_query_checks,
@@ -35,31 +36,31 @@
 
 class LRSQuery(BaseQuery):
     """LRS body query model."""
 
     query: Optional[dict]
 
 
-class LRSHTTP(BaseHTTP):
-    """LRS HTTP backend."""
+class AsyncLRSHTTP(BaseHTTP):
+    """Asynchroneous LRS HTTP backend."""
 
-    name = "lrs"
+    name = "async_lrs"
     query = LRSQuery
     default_operation_type = OperationType.CREATE
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
         base_url: str = lrs_settings.BASE_URL,
         username: str = lrs_settings.USERNAME,
         password: str = lrs_settings.PASSWORD,
         headers: LRSHeaders = lrs_settings.HEADERS,
         status_endpoint: str = lrs_settings.STATUS_ENDPOINT,
         statements_endpoint: str = lrs_settings.STATEMENTS_ENDPOINT,
     ):
-        """Instantiates the LRS client.
+        """Instantiate the LRS client.
 
         Args:
             base_url (AnyHttpUrl): LRS server URL.
             username (str): Basic auth username for LRS authentication.
             password (str): Basic auth password for LRS authentication.
             headers (dict): Headers defined for the LRS server connection.
             status_endpoint (str): Endpoint used to check server status.
@@ -67,51 +68,51 @@
         """
         self.base_url = parse_obj_as(AnyHttpUrl, base_url)
         self.auth = (username, password)
         self.headers = headers
         self.status_endpoint = status_endpoint
         self.statements_endpoint = statements_endpoint
 
-    def status(self):
-        """Implements HTTP backend check for server status."""
+    async def status(self):
+        """HTTP backend check for server status."""
         status_url = urljoin(self.base_url, self.status_endpoint)
 
         try:
-            response = httpx.get(status_url)
+            async with AsyncClient() as client:
+                response = await client.get(status_url)
             response.raise_for_status()
         except RequestError:
             msg = "Unable to request the server"
             logger.error(msg)
             return HTTPBackendStatus.AWAY
         except HTTPStatusError:
             msg = "Response raised an HTTP status of 4xx or 5xx"
             logger.error(msg)
             return HTTPBackendStatus.ERROR
 
         return HTTPBackendStatus.OK
 
-    def list(
+    async def list(
         self, target: str = None, details: bool = False, new: bool = False
     ) -> Iterator[Union[str, dict]]:
-        # noqa: D205, D415
-        """LRS HTTP backend does not support `list` method,
-        calling this method will raise an error.
-        """
+        """Raise error for unsupported `list` method."""
         msg = "LRS HTTP backend does not support `list` method, cannot list from %s"
+
         logger.error(msg, target)
         raise NotImplementedError(msg % target)
 
     @enforce_query_checks
-    def read(  # pylint: disable=too-many-arguments
+    async def read(  # pylint: disable=too-many-arguments
         self,
         query: Union[str, LRSQuery] = None,
         target: str = None,
         chunk_size: Union[None, int] = 500,
         raw_output: bool = False,
         ignore_errors: bool = False,
+        greedy: bool = True,
     ) -> Iterator[Union[bytes, dict]]:
         """Get statements from LRS `target` endpoint.
 
         The `read` method defined in the LRS specification returns `statements` array
         and `more` IRL. The latter is required when the returned `statement` list has
         been limited.
 
@@ -125,14 +126,18 @@
                 If the records are dictionaries and `raw_output` is set to `True`, they
                 are encoded as JSON.
                 If the records are bytes and `raw_output` is set to `False`, they are
                 decoded as JSON by line.
             ignore_errors (bool): If `True`, errors during the read operation
                 are be ignored and logged. If `False` (default), a `BackendException`
                 is raised if an error occurs.
+            greedy: If set to True, the client will fetch all available pages even
+                before the statements yielded by the generator are consumed. Caution:
+                this might potentially lead to large amounts of API calls and to the
+                memory filling up.
         """
         if not target:
             target = self.statements_endpoint
 
         query_params = {}
         if query.query:
             query_params.update(query.query)
@@ -146,76 +151,68 @@
             netloc=urlparse(self.base_url).netloc,
             path=target,
             query="",
             params="",
             fragment="",
         ).geturl()
 
-        def fetch_statements(params: dict):
-            while True:
-                with Client(auth=self.auth, headers=self.headers) as client:
-                    response = client.get(target, params=params)
-                    response.raise_for_status()
-
-                    statements_response = StatementResponse.parse_obj(response.json())
-                    statements = statements_response.statements
-                    statements = (
-                        [statements] if not isinstance(statements, list) else statements
-                    )
-                    if raw_output:
-                        for statement in statements:
-                            yield bytes(json.dumps(statement), encoding="utf-8")
-                    else:
-                        for statement in statements:
-                            yield statement
-
-                    if not statements_response.more:
-                        break
-
-                    params.update(parse_qs(urlparse(statements_response.more).query))
-
         try:
-            yield from fetch_statements(params=query_params)
+            if greedy:
+                async for statement in self._greedy_fetch_statements(
+                    target, raw_output, query_params
+                ):
+                    yield statement
+            else:
+                async for statement in self._fetch_statements(
+                    target=target, raw_output=raw_output, query_params=query_params
+                ):
+                    yield statement
+
         except HTTPError as error:
             msg = "Failed to fetch statements."
             logger.error("%s. %s", msg, error)
             raise BackendException(msg, *error.args) from error
 
-    def write(  # pylint: disable=too-many-arguments
+    async def write(  # pylint: disable=too-many-arguments
         self,
         data: Union[Iterable[bytes], Iterable[dict]],
         target: Union[None, str] = None,
         chunk_size: Union[None, int] = 500,
         ignore_errors: bool = False,
         operation_type: Union[None, OperationType] = None,
+        simultaneous: bool = False,
+        max_num_simultaneous: Union[None, int] = None,
     ) -> int:
-        """Writes `data` records to the `target` endpoint and returns their count.
+        """Write `data` records to the `target` endpoint and return their count.
 
         Args:
             data: (Iterable): The data to write.
             target (str or None): Endpoint in which to write data (e.g. `/statements`).
                 If `target` is `None`, `/xAPI/statements` default endpoint is used.
             chunk_size (int or None): The number of records or bytes to write in one
                 batch, depending on whether `data` contains dictionaries or bytes.
                 If `chunk_size` is `None`, a default value is used instead.
             ignore_errors (bool): If `True`, errors during the write operation
                 are ignored and logged. If `False` (default), a `BackendException`
                 is raised if an error occurs.
             operation_type (OperationType or None): The mode of the write operation.
                 If `operation_type` is `None`, the `default_operation_type` is used
                 instead. See `OperationType`.
+            simultaneous (bool): If `True`, chunks requests will be made concurrently.
+                If `False` (default), chunks will be sent sequentially
+            max_num_simultaneous (int or None): If simultaneous is `True`, the maximum
+                number of chunks to POST concurrently. If `None` (default), no limit is
+                set.
         """
-        statements_count = 0
-
         data = iter(data)
         try:
             first_record = next(data)
         except StopIteration:
-            logger.debug("Data Iterator is empty; skipping write to target.")
-            return statements_count
+            logger.info("Data Iterator is empty; skipping write to target.")
+            return 0
 
         if not operation_type:
             operation_type = self.default_operation_type
 
         if operation_type in (
             OperationType.APPEND,
             OperationType.UPDATE,
@@ -233,43 +230,131 @@
             netloc=urlparse(self.base_url).netloc,
             path=target,
             query="",
             params="",
             fragment="",
         ).geturl()
 
+        if (max_num_simultaneous is not None) and max_num_simultaneous < 1:
+            msg = "max_num_simultaneous must be a stricly positive integer"
+            logger.error(msg)
+            raise BackendParameterException(msg)
+
+        if (not simultaneous) and (max_num_simultaneous is not None):
+            msg = "max_num_simultaneous can only be used with `simultaneous=True`"
+            logger.error(msg)
+            raise BackendParameterException(msg)
+
+        # Gather only one chunk at a time when not using the simultaneous option
+        if not simultaneous:
+            max_num_simultaneous = 1
+
         data = chain((first_record,), data)
-        if isinstance(first_record, dict):
-            data = self._parse_dict_to_bytes(data, ignore_errors)
 
         logger.debug(
-            "Start writing to the %s endpoint (chunk size: %d)", target, chunk_size
+            "Start writing to the %s endpoint (chunk size: %s)", target, chunk_size
         )
 
-        with Client(auth=self.auth, headers=self.headers) as client:
-            for chunk in chunked(data, chunk_size):
-                request = client.post(target, content=chunk)
-                try:
-                    request.raise_for_status()
-                except HTTPError as error:
-                    msg = "Failed to post statements"
-                    logger.error("%s. %s", msg, error)
-                    raise BackendException(msg, *error.args) from error
-                statements_count += len(chunk)
-                logger.info("Posted %d statements", statements_count)
+        # Create tasks
+        tasks = set()
+        for chunk in chunked(data, chunk_size):
+            tasks.add(self._post_and_raise_for_status(target, chunk, ignore_errors))
+
+        # Run POST tasks
+        result = await gather_with_limited_concurrency(max_num_simultaneous, *tasks)
+        statements_count = sum(result)
 
+        logger.debug("Posted %d statements", statements_count)
         return statements_count
 
-    @staticmethod
-    def _parse_dict_to_bytes(
-        statements: Iterable[dict], ignore_errors: bool
-    ) -> Iterator[bytes]:
-        """Reads the `statements` Iterable and yields dictionaries."""
-        for statement in statements:
+    async def _fetch_statements(self, target, raw_output, query_params: dict):
+        """Fetch statements from a LRS. Used in `read`."""
+        async with AsyncClient(
+            auth=self.auth, headers=self.headers.dict(by_alias=True)
+        ) as client:
+            while True:
+                response = await client.get(target, params=query_params)
+                response.raise_for_status()
+
+                statements_response = StatementResponse.parse_obj(response.json())
+                statements = statements_response.statements
+                statements = (
+                    [statements] if not isinstance(statements, list) else statements
+                )
+                if raw_output:
+                    for statement in statements:
+                        yield bytes(json.dumps(statement), encoding="utf-8")
+                else:
+                    for statement in statements:
+                        yield statement
+
+                if not statements_response.more:
+                    break
+
+                query_params.update(parse_qs(urlparse(statements_response.more).query))
+
+    async def _greedy_fetch_statements(self, target, raw_output, query_params):
+        """Fetch as many statements as possible and yield when they are available.
+
+        This may be used in the context of paginated results, to allow processing
+        of statements while the following page is being fetched. Implementation of
+        this function relies on the class method `_fetch_statements`, which must yield
+        statements.
+        """
+        queue = asyncio.Queue()
+
+        async def fetch_all_statements(queue):
+            """Fetch all statements and put them in a queue."""
             try:
-                yield bytes(json.dumps(statement), encoding="utf-8")
+                async for statement in self._fetch_statements(
+                    target=target, raw_output=raw_output, query_params=query_params
+                ):
+                    await queue.put(statement)
+
+            # Re-raising exceptions is necessary as create_task fails silently
+            except Exception as exception:
+                # None signals that the queue is done
+                await queue.put(None)
+                raise exception
+            await queue.put(None)
+
+        # Run fetch_all_statements in the backround
+        task = asyncio.create_task(fetch_all_statements(queue))
+
+        # Yield statements as they arrive
+        while True:
+            statement = await queue.get()
+            if statement is None:
+                # Check for exception in fetch_all_statements
+                if task.exception():
+                    raise task.exception()
+                break
+            yield statement
+
+    async def _post_and_raise_for_status(self, target, chunk, ignore_errors):
+        """POST chunk of statements to `target` and return the number of insertions.
+
+        For use in `write`.
+        """
+        async with AsyncClient(auth=self.auth, headers=self.headers) as client:
+            try:
+                request = await client.post(
+                    # Encode data to allow async post
+                    target,
+                    content=json.dumps(list(chunk)).encode("utf-8"),
+                )
             except TypeError as error:
-                msg = "Failed to encode JSON: %s, for document %s"
-                logger.error(msg, error, statement)
+                msg = f"Failed to encode JSON: {error}, for document {chunk}"
+                logger.error(msg)
+                if ignore_errors:
+                    return 0
+                raise BackendException(msg) from error
+
+            try:
+                request.raise_for_status()
+                return len(chunk)
+            except HTTPError as error:
+                msg = "Failed to post statements"
+                logger.error("%s. %s", msg, error)
                 if ignore_errors:
-                    continue
-                raise BackendException(msg % (error, statement)) from error
+                    return 0
+                raise BackendException(msg, *error.args) from error
```

### Comparing `ralph-malph-3.8.0/src/ralph/backends/mixins.py` & `ralph-malph-3.9.0/src/ralph/backends/mixins.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/storage/base.py` & `ralph-malph-3.9.0/src/ralph/backends/storage/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/storage/fs.py` & `ralph-malph-3.9.0/src/ralph/backends/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/storage/ldp.py` & `ralph-malph-3.9.0/src/ralph/backends/storage/ldp.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/storage/s3.py` & `ralph-malph-3.9.0/src/ralph/backends/storage/s3.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/storage/swift.py` & `ralph-malph-3.9.0/src/ralph/backends/storage/swift.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/backends/stream/ws.py` & `ralph-malph-3.9.0/src/ralph/backends/stream/ws.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/cli.py` & `ralph-malph-3.9.0/src/ralph/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -546,38 +546,70 @@
     "-I",
     "--ignore-errors",
     default=False,
     is_flag=True,
     help="Continue writing regardless of raised errors",
 )
 @click.option(
+    "-s",
+    "--simultaneous",
+    default=False,
+    is_flag=True,
+    help="With HTTP backend, POST all chunks simultaneously (instead of sequentially)",
+)
+@click.option(
+    "-m",
+    "--max-num-simultaneous",
+    type=int,
+    default=-1,
+    help=(
+        "The maximum number of chunks to send at once, when using `--simultaneous`. "
+        "Use `-1` to not set a limit."
+    ),
+)
+@click.option(
     "-t",
     "--target",
     type=str,
     default=None,
     help="Endpoint in which to push events (e.g. `statements`)",
 )
-def push(backend, archive, chunk_size, force, ignore_errors, target, **options):
+def push(
+    backend,
+    archive,
+    chunk_size,
+    force,
+    ignore_errors,
+    simultaneous,
+    max_num_simultaneous,
+    target,
+    **options,
+):
     """Push an archive to a configured backend."""
     logger.info("Pushing archive %s to the configured %s backend", archive, backend)
     logger.debug("Backend parameters: %s", options)
 
+    if max_num_simultaneous == 1:
+        max_num_simultaneous = None
+
     backend_type = get_backend_type(settings.BACKENDS, backend)
     backend = get_backend_instance(backend_type, backend, options)
 
     if backend_type == settings.BACKENDS.STORAGE:
         backend.write(sys.stdin.buffer, archive, overwrite=force)
     elif backend_type == settings.BACKENDS.DATABASE:
         backend.put(sys.stdin, chunk_size=chunk_size, ignore_errors=ignore_errors)
     elif backend_type == settings.BACKENDS.HTTP:
         backend.write(
             target=target,
             data=sys.stdin.buffer,
             chunk_size=chunk_size,
             ignore_errors=ignore_errors,
+            simultaneous=simultaneous,
+            max_num_simultaneous=max_num_simultaneous,
         )
     elif backend_type is None:
         msg = "Cannot find an implemented backend type for backend %s"
         logger.error(msg, backend)
         raise UnsupportedBackendException(msg, backend)
```

### Comparing `ralph-malph-3.8.0/src/ralph/conf.py` & `ralph-malph-3.9.0/src/ralph/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,16 +162,16 @@
     class Config:  # pylint: disable=missing-class-docstring # noqa: D106
         extra = Extra.allow
 
 
 class LRSHeaders(HeadersParameters):
     """Pydantic model for LRS headers."""
 
-    X_EXPERIENCE_API_VERSION: str = "1.0.3"
-    CONTENT_TYPE: str = "application/json"
+    X_EXPERIENCE_API_VERSION: str = Field("1.0.3", alias="X-Experience-API-Version")
+    CONTENT_TYPE: str = Field("application/json", alias="content-type")
 
 
 class LRSHTTPBackendSettings(InstantiableSettingsItem):
     """Pydantic model for LRS HTTP backend configuration settings."""
 
     _class_path: str = "ralph.backends.http.lrs.LRSHTTP"
```

### Comparing `ralph-malph-3.8.0/src/ralph/exceptions.py` & `ralph-malph-3.9.0/src/ralph/exceptions.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/filters.py` & `ralph-malph-3.9.0/src/ralph/filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/converter.py` & `ralph-malph-3.9.0/src/ralph/models/converter.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/__init__.py` & `ralph-malph-3.9.0/src/ralph/models/edx/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/base.py` & `ralph-malph-3.9.0/src/ralph/models/edx/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/browser.py` & `ralph-malph-3.9.0/src/ralph/models/edx/browser.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/base.py` & `ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/base.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/navigational.py` & `ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/navigational.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/server.py` & `ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/converters/xapi/video.py` & `ralph-malph-3.9.0/src/ralph/models/edx/converters/xapi/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/contexts.py` & `ralph-malph-3.9.0/src/ralph/models/edx/enrollment/fields/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/enrollment/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/enrollment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/enrollment/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/enrollment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/navigational/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/navigational/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/navigational/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/navigational/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/open_response_assessment/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/open_response_assessment/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/peer_instruction/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/peer_instruction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/problem_interaction/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/problem_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/server.py` & `ralph-malph-3.9.0/src/ralph/models/edx/server.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/textbook_interaction/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/textbook_interaction/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/video/fields/events.py` & `ralph-malph-3.9.0/src/ralph/models/edx/video/fields/events.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/edx/video/statements.py` & `ralph-malph-3.9.0/src/ralph/models/edx/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/selector.py` & `ralph-malph-3.9.0/src/ralph/models/selector.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/validator.py` & `ralph-malph-3.9.0/src/ralph/models/validator.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/__init__.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/agents.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/agents.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/attachments.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/attachments.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/common.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/common.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/contexts.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/groups.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/groups.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/ifi.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/ifi.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/objects.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/results.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/statements.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/base/unnested_objects.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/base/unnested_objects.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/acrossx_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/activity_streams_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/scorm_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/video.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/activity_types/virtual_classroom.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/constants/video.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/constants/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/acrossx_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/activity_streams_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/adl_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/scorm_profile.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/tincan_vocabulary.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/video.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/video.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/concepts/verbs/virtual_classroom.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/config.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/config.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/navigation/statements.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/navigation/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/video/contexts.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/video/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/video/results.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/video/results.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/video/statements.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/video/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/contexts.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/contexts.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/models/xapi/virtual_classroom/statements.py` & `ralph-malph-3.9.0/src/ralph/models/xapi/virtual_classroom/statements.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/parsers.py` & `ralph-malph-3.9.0/src/ralph/parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/src/ralph/utils.py` & `ralph-malph-3.9.0/src/ralph/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Utilities for Ralph."""
 
+import asyncio
 import datetime
 import logging
 import operator
 from functools import reduce
 from importlib import import_module
-from typing import List
+from typing import List, Union
 
 from pydantic import BaseModel
 
 
 # Taken from Django utilities
 # https://docs.djangoproject.com/en/3.1/_modules/django/utils/module_loading/#import_string
 def import_string(dotted_path):
@@ -88,7 +89,34 @@
         dict_ (dict): dictionnary where the given value is set
         path (List): array of keys representing the path to the value
         value: value to be set
     """
     for key in path[:-1]:
         dict_ = dict_.setdefault(key, {})
     dict_[path[-1]] = value
+
+
+async def gather_with_limited_concurrency(num_tasks: Union[None, int], *tasks):
+    """Gather no more than `num_tasks` tasks at time.
+
+    Args:
+        num_tasks: the maximum number of tasks to run concurrently, if None,
+            no maximum value is set
+        tasks: tasks to run concurrently
+    """
+    if num_tasks is not None:
+        semaphore = asyncio.Semaphore(num_tasks)
+
+        async def sem_task(task):
+            async with semaphore:
+                return await task
+
+        group = asyncio.gather(*(sem_task(task) for task in tasks))
+    else:
+        group = asyncio.gather(*tasks)
+
+    # Cancel background tasks on first error
+    try:
+        return await group
+    except Exception as exception:
+        group.cancel()
+        raise exception
```

### Comparing `ralph-malph-3.8.0/src/ralph_malph.egg-info/PKG-INFO` & `ralph-malph-3.9.0/src/ralph_malph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralph-malph
-Version: 3.8.0
+Version: 3.9.0
 Summary: The ultimate toolbox for your learning analytics
 Home-page: https://openfun.github.io/ralph/
 Author: Open FUN (France Universite Numerique)
 Author-email: fun.dev@fun-mooc.fr
 License: MIT
 Keywords: Open edX,Analytics,xAPI,LRS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ralph-malph-3.8.0/src/ralph_malph.egg-info/SOURCES.txt` & `ralph-malph-3.9.0/src/ralph_malph.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 src/ralph/backends/mixins.py
 src/ralph/backends/database/__init__.py
 src/ralph/backends/database/base.py
 src/ralph/backends/database/clickhouse.py
 src/ralph/backends/database/es.py
 src/ralph/backends/database/mongo.py
 src/ralph/backends/http/__init__.py
+src/ralph/backends/http/async_lrs.py
 src/ralph/backends/http/base.py
 src/ralph/backends/http/lrs.py
 src/ralph/backends/storage/__init__.py
 src/ralph/backends/storage/base.py
 src/ralph/backends/storage/fs.py
 src/ralph/backends/storage/ldp.py
 src/ralph/backends/storage/s3.py
```

### Comparing `ralph-malph-3.8.0/src/ralph_malph.egg-info/requires.txt` & `ralph-malph-3.9.0/src/ralph_malph.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 langcodes>=3.2.0
-pydantic[dotenv,email]>=1.10.0
+pydantic[dotenv,email]<2.0,>=1.10.0
 rfc3987>=1.3.0
 
 [backend-clickhouse]
 clickhouse-connect[numpy,pandas]<0.6
 python-dateutil>=2.8.2
 
 [backend-es]
@@ -39,37 +39,37 @@
 bcrypt>=4.0.0
 click>=8.1.0
 click-option-group>=0.5.0
 sentry-sdk[fastapi]>=1.9.0
 
 [dev]
 bandit==1.7.5
-black==23.3.0
-cryptography==41.0.1
+black==23.7.0
+cryptography==41.0.2
 factory-boy==3.2.1
 flake8==6.0.0
-hypothesis==6.79.1
+hypothesis==6.81.2
 isort==5.12.0
 logging-gelf==0.0.31
 mkdocs==1.4.3
 mkdocs-click==0.8.0
-mkdocs-material==9.1.16
+mkdocs-material==9.1.18
 mkdocstrings[python-legacy]==0.22.0
-moto==4.1.11
+moto==4.1.13
 pydocstyle==6.3.0
-pyfakefs==5.2.2
+pyfakefs==5.2.3
 pylint==2.17.4
-pytest==7.3.2
-pytest-asyncio==0.21.0
+pytest==7.4.0
+pytest-asyncio==0.21.1
 pytest-cov==4.1.0
 pytest-httpx==0.22.0
 responses==0.23.1
 
 [lrs]
 bcrypt==4.0.1
-fastapi==0.97.0
+fastapi==0.100.0
 cachetools==5.3.1
 h11>=0.11.0
 httpx==0.24.1
-sentry_sdk==1.25.1
+sentry_sdk==1.28.1
 python-jose==3.3.0
-uvicorn[standard]==0.22.0
+uvicorn[standard]==0.23.0
```

### Comparing `ralph-malph-3.8.0/tests/test_cli.py` & `ralph-malph-3.9.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import logging
 from pathlib import Path
 
 import pytest
 from click.exceptions import BadParameter
 from click.testing import CliRunner
 from elasticsearch.helpers import bulk, scan
+from hypothesis import settings as hypothesis_settings
 from pydantic import ValidationError
 
 from ralph.backends.storage.fs import FSStorage
 from ralph.backends.storage.ldp import LDPStorage
 from ralph.cli import (
     CommaSeparatedKeyValueParamType,
     CommaSeparatedTupleParamType,
@@ -314,14 +315,15 @@
     """Tests the validate command using the edx format."""
     event_str = event.json()
     runner = CliRunner()
     result = runner.invoke(cli, ["validate", "-f", "edx"], input=event_str)
     assert event_str in result.output
 
 
+@hypothesis_settings(deadline=None)
 @custom_given(UIPageClose)
 @pytest.mark.parametrize("valid_uuid", ["ee241f8b-174f-5bdb-bae9-c09de5fe017f"])
 def test_cli_convert_command_from_edx_to_xapi_format(valid_uuid, event):
     """Tests the convert command from edx to xapi format."""
     event_str = event.json()
     runner = CliRunner()
     command = f"-v ERROR convert -f edx -t xapi -u {valid_uuid} -p https://fun-mooc.fr"
```

### Comparing `ralph-malph-3.8.0/tests/test_cli_usage.py` & `ralph-malph-3.9.0/tests/test_cli_usage.py`

 * *Files 13% similar despite different names*

```diff
@@ -79,30 +79,31 @@
     assert result.exit_code == 0
     assert (
         "Options:\n"
         "  From edX to xAPI converter options: \n"
         "    -u, --uuid-namespace TEXT     The UUID namespace to use for the `ID` "
         "field\n"
         "                                  generation\n"
-        "    -p, --platform-url TEXT       The `actor.account.homePage` to use in the\n"
+        "    -p, --platform-url TEXT       The `actor.account.homePage` to use in"
+        " the\n"
         "                                  xAPI statements  [required]\n"
         "  -f, --from [edx]                Input events format to convert  [required]\n"
         "  -t, --to [xapi]                 Output events format  [required]\n"
         "  -I, --ignore-errors             Continue writing regardless of raised "
         "errors\n"
         "  -F, --fail-on-unknown           Stop converting at first unknown event\n"
     ) in result.output
 
     result = runner.invoke(cli, ["convert"])
     assert result.exit_code > 0
     assert "Error: Missing option '-p' / '--platform-url'" in result.output
 
 
 def test_cli_fetch_command_usage():
-    """Tests ralph fetch command usage."""
+    """Test ralph fetch command usage."""
     runner = CliRunner()
     result = runner.invoke(cli, ["fetch", "--help"])
 
     assert result.exit_code == 0
     assert (
         "Options:\n"
         "  -b, --backend [es|mongo|clickhouse|lrs|ldp|fs|swift|s3|ws]\n"
@@ -176,15 +177,15 @@
         "Error: Missing option '-b' / '--backend'. "
         "Choose from:\n\tes,\n\tmongo,\n\tclickhouse,\n\tlrs,\n\tldp,\n\tfs,\n\tswift,"
         "\n\ts3,\n\tws\n"
     ) in result.output
 
 
 def test_cli_list_command_usage():
-    """Tests ralph list command usage."""
+    """Test ralph list command usage."""
     runner = CliRunner()
     result = runner.invoke(cli, ["list", "--help"])
 
     assert result.exit_code == 0
     assert (
         "Options:\n"
         "  -b, --backend [ldp|fs|swift|s3]\n"
@@ -224,16 +225,109 @@
     assert result.exit_code > 0
     assert (
         "Error: Missing option '-b' / '--backend'. Choose from:\n\tldp,\n\tfs,\n\t"
         "swift,\n\ts3\n"
     ) in result.output
 
 
+def test_cli_push_command_usage():
+    """Test ralph push command usage."""
+    runner = CliRunner()
+    result = runner.invoke(cli, ["push", "--help"])
+
+    assert result.exit_code == 0
+
+    expected_output = (
+        "Usage: ralph push [OPTIONS] [ARCHIVE]\n"
+        "\n"
+        "  Push an archive to a configured backend.\n"
+        "\n"
+        "Options:\n"
+        "  -b, --backend [es|mongo|clickhouse|ldp|fs|swift|s3|lrs]\n"
+        "                                  Backend  [required]\n"
+        "  lrs backend: \n"
+        "    --lrs-statements-endpoint TEXT\n"
+        "    --lrs-status-endpoint TEXT\n"
+        "    --lrs-headers KEY=VALUE,KEY=VALUE\n"
+        "    --lrs-password TEXT\n"
+        "    --lrs-username TEXT\n"
+        "    --lrs-base-url TEXT\n"
+        "  s3 backend: \n"
+        "    --s3-endpoint-url TEXT\n"
+        "    --s3-bucket-name TEXT\n"
+        "    --s3-default-region TEXT\n"
+        "    --s3-session-token TEXT\n"
+        "    --s3-secret-access-key TEXT\n"
+        "    --s3-access-key-id TEXT\n"
+        "  swift backend: \n"
+        "    --swift-os-identity-api-version TEXT\n"
+        "    --swift-os-auth-url TEXT\n"
+        "    --swift-os-project-domain-name TEXT\n"
+        "    --swift-os-user-domain-name TEXT\n"
+        "    --swift-os-storage-url TEXT\n"
+        "    --swift-os-region-name TEXT\n"
+        "    --swift-os-password TEXT\n"
+        "    --swift-os-username TEXT\n"
+        "    --swift-os-tenant-name TEXT\n"
+        "    --swift-os-tenant-id TEXT\n"
+        "  fs backend: \n"
+        "    --fs-path TEXT\n"
+        "  ldp backend: \n"
+        "    --ldp-stream-id TEXT\n"
+        "    --ldp-service-name TEXT\n"
+        "    --ldp-consumer-key TEXT\n"
+        "    --ldp-application-secret TEXT\n"
+        "    --ldp-application-key TEXT\n"
+        "    --ldp-endpoint TEXT\n"
+        "  clickhouse backend: \n"
+        "    --clickhouse-client-options KEY=VALUE,KEY=VALUE\n"
+        "    --clickhouse-password TEXT\n"
+        "    --clickhouse-username TEXT\n"
+        "    --clickhouse-event-table-name TEXT\n"
+        "    --clickhouse-database TEXT\n"
+        "    --clickhouse-port INTEGER\n"
+        "    --clickhouse-host TEXT\n"
+        "  mongo backend: \n"
+        "    --mongo-client-options KEY=VALUE,KEY=VALUE\n"
+        "    --mongo-collection TEXT\n"
+        "    --mongo-database TEXT\n"
+        "    --mongo-connection-uri TEXT\n"
+        "  es backend: \n"
+        "    --es-op-type TEXT\n"
+        "    --es-client-options KEY=VALUE,KEY=VALUE\n"
+        "    --es-index TEXT\n"
+        "    --es-hosts VALUE1,VALUE2,VALUE3\n"
+        "  -c, --chunk-size INTEGER        Get events by chunks of size #\n"
+        "  -f, --force                     Overwrite existing archives or records\n"
+        "  -I, --ignore-errors             Continue writing regardless of raised "
+        "errors\n"
+        "  -s, --simultaneous              With HTTP backend, POST all chunks\n"
+        "                                  simultaneously (instead of sequentially)\n"
+        "  -m, --max-num-simultaneous INTEGER\n"
+        "                                  The maximum number of chunks to send at "
+        "once,\n"
+        "                                  when using `--simultaneous`. Use `-1` to "
+        "not\n"
+        "                                  set a limit.\n"
+        "  -t, --target TEXT               Endpoint in which to push events (e.g.\n"
+        "                                  `statements`)\n"
+        "  --help                          Show this message and exit.\n"
+    )
+    assert expected_output in result.output
+
+    result = runner.invoke(cli, ["push"])
+    assert result.exit_code > 0
+    assert (
+        "Missing option '-b' / '--backend'. Choose from:\n\tes,\n\tmongo,"
+        "\n\tclickhouse,\n\tldp,\n\tfs,\n\tswift,\n\ts3,\n\tlrs\n"
+    ) in result.output
+
+
 def test_cli_runserver_command_usage():
-    """Tests ralph runserver command usage."""
+    """Test ralph runserver command usage."""
     runner = CliRunner()
     result = runner.invoke(cli, ["runserver", "--help"])
 
     expected_output = (
         "Options:\n"
         "  -b, --backend [es|mongo|clickhouse]\n"
         "                                  Backend  [required]\n"
```

### Comparing `ralph-malph-3.8.0/tests/test_conf.py` & `ralph-malph-3.9.0/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/tests/test_dependencies.py` & `ralph-malph-3.9.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/tests/test_filters.py` & `ralph-malph-3.9.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/tests/test_logger.py` & `ralph-malph-3.9.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/tests/test_parsers.py` & `ralph-malph-3.9.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `ralph-malph-3.8.0/tests/test_utils.py` & `ralph-malph-3.9.0/tests/test_utils.py`

 * *Files identical despite different names*

