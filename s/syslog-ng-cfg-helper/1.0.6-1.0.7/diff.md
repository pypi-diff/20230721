# Comparing `tmp/syslog_ng_cfg_helper-1.0.6.tar.gz` & `tmp/syslog_ng_cfg_helper-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syslog_ng_cfg_helper-1.0.6.tar", max compression
+gzip compressed data, was "syslog_ng_cfg_helper-1.0.7.tar", max compression
```

## Comparing `syslog_ng_cfg_helper-1.0.6.tar` & `syslog_ng_cfg_helper-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35148 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/LICENSE
--rw-r--r--   0        0        0     2869 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/README.md
--rw-r--r--   0        0        0     1147 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/__init__.py
--rw-r--r--   0        0        0      941 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/build_db.py
--rw-r--r--   0        0        0     2486 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/console.py
--rw-r--r--   0        0        0      244 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/__init__.py
--rw-r--r--   0        0        0     3783 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/block.py
--rw-r--r--   0        0        0     1769 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/driver.py
--rw-r--r--   0        0        0     2263 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/driver_db.py
--rw-r--r--   0        0        0       42 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/exceptions.py
--rw-r--r--   0        0        0     2249 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/option.py
--rw-r--r--   0        0        0      479 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/utils.py
--rw-r--r--   0        0        0      893 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/globals.py
--rw-r--r--   0        0        0       75 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/module_loader/__init__.py
--rw-r--r--   0        0        0     6094 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/module_loader/load_modules.py
--rw-r--r--   0        0        0     4225 2023-05-13 21:40:08.791417 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/module_loader/parse_sentence.py
--rw-r--r--   0        0        0   215603 2023-05-13 21:41:15.576502 syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db
--rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 syslog_ng_cfg_helper-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-07-21 11:44:07.511030 syslog_ng_cfg_helper-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2869 2023-07-21 11:44:07.511030 syslog_ng_cfg_helper-1.0.7/README.md
+-rw-r--r--   0        0        0     1147 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/__init__.py
+-rw-r--r--   0        0        0      941 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/build_db.py
+-rw-r--r--   0        0        0     2486 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/console.py
+-rw-r--r--   0        0        0      244 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/__init__.py
+-rw-r--r--   0        0        0     3783 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/block.py
+-rw-r--r--   0        0        0     1769 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/driver.py
+-rw-r--r--   0        0        0     2263 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/driver_db.py
+-rw-r--r--   0        0        0       42 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/exceptions.py
+-rw-r--r--   0        0        0     2249 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/option.py
+-rw-r--r--   0        0        0      479 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/utils.py
+-rw-r--r--   0        0        0      893 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/globals.py
+-rw-r--r--   0        0        0       75 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/__init__.py
+-rw-r--r--   0        0        0     6094 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/load_modules.py
+-rw-r--r--   0        0        0     4225 2023-07-21 11:44:07.515035 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/parse_sentence.py
+-rw-r--r--   0        0        0   235140 2023-07-21 11:45:17.349223 syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db
+-rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 syslog_ng_cfg_helper-1.0.7/PKG-INFO
```

### Comparing `syslog_ng_cfg_helper-1.0.6/LICENSE` & `syslog_ng_cfg_helper-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/README.md` & `syslog_ng_cfg_helper-1.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # syslog-ng CFG Helper
 
 This tool makes configuring [syslog-ng](https://github.com/syslog-ng/syslog-ng) a bit easier by listing the options of each available driver.
 
-The options are generated from [syslog-ng v4.2.0](https://github.com/syslog-ng/syslog-ng/releases/tag/syslog-ng-4.2.0).
+The options are generated from [syslog-ng v4.3.0](https://github.com/syslog-ng/syslog-ng/releases/tag/syslog-ng-4.3.0).
 
 ## Quickstart
 
 ### Install with pipx
 ```
 pipx install syslog-ng-cfg-helper
 ```
```

### Comparing `syslog_ng_cfg_helper-1.0.6/pyproject.toml` & `syslog_ng_cfg_helper-1.0.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syslog-ng-cfg-helper"
-version = "1.0.6"
+version = "1.0.7"
 description = "Configuration helper for syslog-ng."
 authors = ["Attila Szakacs <szakacs.attila96@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/alltilla/syslog-ng-cfg-helper"
 repository = "https://github.com/alltilla/syslog-ng-cfg-helper"
 keywords = ["syslog-ng", "configuration", "cfg"]
```

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/build_db.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/build_db.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/console.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/console.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/block.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/block.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/driver.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/driver.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/driver_db.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/driver_db.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/driver_db/option.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/driver_db/option.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/globals.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/globals.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/module_loader/load_modules.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/load_modules.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/module_loader/parse_sentence.py` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/module_loader/parse_sentence.py`

 * *Files identical despite different names*

### Comparing `syslog_ng_cfg_helper-1.0.6/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db` & `syslog_ng_cfg_helper-1.0.7/syslog_ng_cfg_helper/syslog-ng-cfg-helper.db`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933317975779106%*

 * *Differences: {"'contexts'": "{'parser': {'syslog-parser': {'options': {'flags': {'params': {insert: [(2, "*

 * *               "['check-hostname'])], delete: [1]}}, 'default-facility': {'params': {insert: [(1, "*

 * *               "['KW_SYSLOG'])], delete: [0]}}}}, 'python': {'blocks': {'options': {'options': "*

 * *               "{'': {'params': {insert: [(0, ['<empty>']), (6, ['<string>', '=>', '<string>'])], "*

 * *               "delete: [3, 1]}}}}}}, 'db-parser': {'options': {'inject-mode': {'params': {insert: "*

 * *               "[(1, […]*

```diff
@@ -3,14 +3,22 @@
         "destination": {
             "amqp": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -27,14 +35,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -71,18 +103,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -180,38 +212,30 @@
                                                 "name": null,
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_LOWER": {
-                                                "name": "KW_LOWER",
+                                            "add-prefix": {
+                                                "name": "add-prefix",
                                                 "params": [
                                                     [
-                                                        "<empty>"
+                                                        "<string>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_UPPER": {
-                                                "name": "KW_UPPER",
+                                            "lower": {
+                                                "name": "lower",
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "add-prefix": {
-                                                "name": "add-prefix",
-                                                "params": [
-                                                    [
-                                                        "<string>"
-                                                    ]
-                                                ]
-                                            },
                                             "replace": {
                                                 "name": "replace",
                                                 "params": [
                                                     [
                                                         "<string>",
                                                         "<string>"
                                                     ]
@@ -237,28 +261,36 @@
                                             "shift-levels": {
                                                 "name": "shift-levels",
                                                 "params": [
                                                     [
                                                         "<positive-integer>"
                                                     ]
                                                 ]
+                                            },
+                                            "upper": {
+                                                "name": "upper",
+                                                "params": [
+                                                    [
+                                                        "<empty>"
+                                                    ]
+                                                ]
                                             }
                                         }
                                     }
                                 },
                                 "name": "key",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<string-list>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<string-list>"
                                             ]
                                         ]
                                     }
                                 }
                             },
                             "rekey": {
                                 "blocks": {},
@@ -268,38 +300,30 @@
                                         "name": null,
                                         "params": [
                                             [
                                                 "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_LOWER": {
-                                        "name": "KW_LOWER",
+                                    "add-prefix": {
+                                        "name": "add-prefix",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_UPPER": {
-                                        "name": "KW_UPPER",
+                                    "lower": {
+                                        "name": "lower",
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "add-prefix": {
-                                        "name": "add-prefix",
-                                        "params": [
-                                            [
-                                                "<string>"
-                                            ]
-                                        ]
-                                    },
                                     "replace": {
                                         "name": "replace",
                                         "params": [
                                             [
                                                 "<string>",
                                                 "<string>"
                                             ]
@@ -325,14 +349,22 @@
                                     "shift-levels": {
                                         "name": "shift-levels",
                                         "params": [
                                             [
                                                 "<positive-integer>"
                                             ]
                                         ]
+                                    },
+                                    "upper": {
+                                        "name": "upper",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
                                     }
                                 }
                             }
                         },
                         "name": "value-pairs",
                         "options": {
                             "": {
@@ -355,24 +387,32 @@
                                 "name": "exclude",
                                 "params": [
                                     [
                                         "<string-list>"
                                     ]
                                 ]
                             },
+                            "include-bytes": {
+                                "name": "include-bytes",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
@@ -642,14 +682,22 @@
             },
             "example-destination": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -666,14 +714,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -710,18 +782,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -825,14 +897,22 @@
             },
             "fifo": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -849,14 +929,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -893,18 +997,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -986,18 +1090,18 @@
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
@@ -1083,18 +1187,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -1121,18 +1225,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -1240,14 +1344,22 @@
             },
             "file": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -1264,14 +1376,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -1308,18 +1444,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -1506,18 +1642,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -1560,18 +1696,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -1774,14 +1910,22 @@
                             }
                         }
                     },
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -1798,14 +1942,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -1842,18 +2010,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -1913,45 +2081,45 @@
                                 "blocks": {},
                                 "name": "options",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<string>",
-                                                "=>",
-                                                "<float>"
+                                                "<empty>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
-                                                "<string>"
+                                                "<float>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
                                                 "[",
                                                 "<string-list>",
                                                 "]"
                                             ],
                                             [
-                                                "<empty>"
-                                            ],
-                                            [
                                                 "<string>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
                                                 "<python-yesno>"
                                             ],
                                             [
                                                 "<string>",
                                                 "=>",
                                                 "<number>"
+                                            ],
+                                            [
+                                                "<string>",
+                                                "=>",
+                                                "<string>"
                                             ]
                                         ]
                                     },
                                     "LogTemplate": {
                                         "name": "LogTemplate",
                                         "params": [
                                             [
@@ -2322,35 +2490,35 @@
                             ]
                         ]
                     },
                     "response-action": {
                         "name": "response-action",
                         "params": [
                             [
-                                "<positive-integer>",
-                                "=>",
-                                "retry"
+                                "<empty>"
                             ],
                             [
                                 "<positive-integer>",
                                 "=>",
-                                "drop"
+                                "success"
                             ],
                             [
                                 "<positive-integer>",
                                 "=>",
                                 "disconnect"
                             ],
                             [
-                                "<empty>"
+                                "<positive-integer>",
+                                "=>",
+                                "retry"
                             ],
                             [
                                 "<positive-integer>",
                                 "=>",
-                                "success"
+                                "drop"
                             ]
                         ]
                     },
                     "retries": {
                         "name": "retries",
                         "params": [
                             [
@@ -2458,14 +2626,22 @@
             },
             "java": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -2482,14 +2658,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -2526,18 +2726,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -2674,19 +2874,19 @@
                         "name": "options",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
                                 "<string>",
+                                "=>",
                                 "<string-or-number>"
                             ],
                             [
                                 "<string>",
-                                "=>",
                                 "<string-or-number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
@@ -2786,14 +2986,22 @@
                             }
                         }
                     },
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -2810,14 +3018,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -2854,18 +3086,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -3105,14 +3337,22 @@
             },
             "mongodb": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -3129,14 +3369,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -3173,18 +3437,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -3236,38 +3500,30 @@
                                                 "name": null,
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_LOWER": {
-                                                "name": "KW_LOWER",
+                                            "add-prefix": {
+                                                "name": "add-prefix",
                                                 "params": [
                                                     [
-                                                        "<empty>"
+                                                        "<string>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_UPPER": {
-                                                "name": "KW_UPPER",
+                                            "lower": {
+                                                "name": "lower",
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "add-prefix": {
-                                                "name": "add-prefix",
-                                                "params": [
-                                                    [
-                                                        "<string>"
-                                                    ]
-                                                ]
-                                            },
                                             "replace": {
                                                 "name": "replace",
                                                 "params": [
                                                     [
                                                         "<string>",
                                                         "<string>"
                                                     ]
@@ -3293,28 +3549,36 @@
                                             "shift-levels": {
                                                 "name": "shift-levels",
                                                 "params": [
                                                     [
                                                         "<positive-integer>"
                                                     ]
                                                 ]
+                                            },
+                                            "upper": {
+                                                "name": "upper",
+                                                "params": [
+                                                    [
+                                                        "<empty>"
+                                                    ]
+                                                ]
                                             }
                                         }
                                     }
                                 },
                                 "name": "key",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<string-list>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<string-list>"
                                             ]
                                         ]
                                     }
                                 }
                             },
                             "rekey": {
                                 "blocks": {},
@@ -3324,38 +3588,30 @@
                                         "name": null,
                                         "params": [
                                             [
                                                 "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_LOWER": {
-                                        "name": "KW_LOWER",
+                                    "add-prefix": {
+                                        "name": "add-prefix",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_UPPER": {
-                                        "name": "KW_UPPER",
+                                    "lower": {
+                                        "name": "lower",
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "add-prefix": {
-                                        "name": "add-prefix",
-                                        "params": [
-                                            [
-                                                "<string>"
-                                            ]
-                                        ]
-                                    },
                                     "replace": {
                                         "name": "replace",
                                         "params": [
                                             [
                                                 "<string>",
                                                 "<string>"
                                             ]
@@ -3381,14 +3637,22 @@
                                     "shift-levels": {
                                         "name": "shift-levels",
                                         "params": [
                                             [
                                                 "<positive-integer>"
                                             ]
                                         ]
+                                    },
+                                    "upper": {
+                                        "name": "upper",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
                                     }
                                 }
                             }
                         },
                         "name": "value-pairs",
                         "options": {
                             "": {
@@ -3411,24 +3675,32 @@
                                 "name": "exclude",
                                 "params": [
                                     [
                                         "<string-list>"
                                     ]
                                 ]
                             },
+                            "include-bytes": {
+                                "name": "include-bytes",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
@@ -3442,14 +3714,54 @@
                             }
                         }
                     }
                 },
                 "context": "destination",
                 "name": "mongodb",
                 "options": {
+                    "batch-lines": {
+                        "name": "batch-lines",
+                        "params": [
+                            [
+                                "<nonnegative-integer>"
+                            ]
+                        ]
+                    },
+                    "batch-timeout": {
+                        "name": "batch-timeout",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "bulk": {
+                        "name": "bulk",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "bulk-bypass-validation": {
+                        "name": "bulk-bypass-validation",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "bulk-unordered": {
+                        "name": "bulk-unordered",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
                     "collection": {
                         "name": "collection",
                         "params": [
                             [
                                 "<template-content>"
                             ]
                         ]
@@ -3561,23 +3873,48 @@
                     "workers": {
                         "name": "workers",
                         "params": [
                             [
                                 "<positive-integer>"
                             ]
                         ]
+                    },
+                    "write-concern": {
+                        "name": "write-concern",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ],
+                            [
+                                "acked"
+                            ],
+                            [
+                                "majority"
+                            ],
+                            [
+                                "unacked"
+                            ]
+                        ]
                     }
                 }
             },
             "mqtt": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -3594,14 +3931,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -3638,18 +3999,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -3969,14 +4330,22 @@
             },
             "network": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -3993,14 +4362,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -4037,18 +4430,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "failover": {
                         "blocks": {
@@ -4288,18 +4681,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -4538,18 +4931,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -4749,24 +5142,24 @@
                             ]
                         ]
                     },
                     "transport": {
                         "name": "transport",
                         "params": [
                             [
-                                "udp"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "tcp"
                             ],
                             [
                                 "tls"
+                            ],
+                            [
+                                "udp"
                             ]
                         ]
                     },
                     "truncate-size": {
                         "name": "truncate-size",
                         "params": [
                             [
@@ -4780,20 +5173,114 @@
                             [
                                 "<string>"
                             ]
                         ]
                     }
                 }
             },
-            "pipe": {
+            "opentelemetry": {
                 "blocks": {
+                    "auth": {
+                        "blocks": {
+                            "alts": {
+                                "blocks": {},
+                                "name": "alts",
+                                "options": {
+                                    "": {
+                                        "name": null,
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
+                                    },
+                                    "target-service-accounts": {
+                                        "name": "target-service-accounts",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ],
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    }
+                                }
+                            },
+                            "tls": {
+                                "blocks": {},
+                                "name": "tls",
+                                "options": {
+                                    "": {
+                                        "name": null,
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
+                                    },
+                                    "ca-file": {
+                                        "name": "ca-file",
+                                        "params": [
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    },
+                                    "cert-file": {
+                                        "name": "cert-file",
+                                        "params": [
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    },
+                                    "key-file": {
+                                        "name": "key-file",
+                                        "params": [
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    }
+                                }
+                            }
+                        },
+                        "name": "auth",
+                        "options": {
+                            "adc": {
+                                "name": "adc",
+                                "params": [
+                                    [
+                                        "<empty>"
+                                    ]
+                                ]
+                            },
+                            "insecure": {
+                                "name": "insecure",
+                                "params": [
+                                    [
+                                        "<empty>"
+                                    ]
+                                ]
+                            }
+                        }
+                    },
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -4810,14 +5297,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -4854,20 +5365,259 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
+                                        "<float>"
+                                    ]
+                                ]
+                            }
+                        }
+                    },
+                    "hook-commands": {
+                        "blocks": {},
+                        "name": "hook-commands",
+                        "options": {
+                            "setup": {
+                                "name": "setup",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "shutdown": {
+                                "name": "shutdown",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "startup": {
+                                "name": "startup",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "teardown": {
+                                "name": "teardown",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            }
+                        }
+                    }
+                },
+                "context": "destination",
+                "name": "opentelemetry",
+                "options": {
+                    "batch-lines": {
+                        "name": "batch-lines",
+                        "params": [
+                            [
+                                "<nonnegative-integer>"
+                            ]
+                        ]
+                    },
+                    "batch-timeout": {
+                        "name": "batch-timeout",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "internal": {
+                        "name": "internal",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "log-fifo-size": {
+                        "name": "log-fifo-size",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "persist-name": {
+                        "name": "persist-name",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "retries": {
+                        "name": "retries",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "throttle": {
+                        "name": "throttle",
+                        "params": [
+                            [
+                                "<nonnegative-integer>"
+                            ]
+                        ]
+                    },
+                    "time-reopen": {
+                        "name": "time-reopen",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "url": {
+                        "name": "url",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "workers": {
+                        "name": "workers",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    }
+                }
+            },
+            "pipe": {
+                "blocks": {
+                    "disk-buffer": {
+                        "blocks": {},
+                        "name": "disk-buffer",
+                        "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
+                            "compaction": {
+                                "name": "compaction",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
+                            "dir": {
+                                "name": "dir",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "disk-buf-size": {
+                                "name": "disk-buf-size",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "mem-buf-length": {
+                                "name": "mem-buf-length",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "mem-buf-size": {
+                                "name": "mem-buf-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "prealloc": {
+                                "name": "prealloc",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
+                            "qout-size": {
+                                "name": "qout-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "reliable": {
+                                "name": "reliable",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
+                            "truncate-size-ratio": {
+                                "name": "truncate-size-ratio",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ],
+                                    [
+                                        "<float>"
+                                    ]
+                                ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
                         "name": "hook-commands",
                         "options": {
@@ -4947,18 +5697,18 @@
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
@@ -5044,18 +5794,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -5082,18 +5832,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -5201,14 +5951,22 @@
             },
             "program": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -5225,14 +5983,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -5269,18 +6051,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -5423,18 +6205,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -5550,14 +6332,22 @@
             },
             "pseudofile": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -5574,14 +6364,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -5618,18 +6432,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -5781,14 +6595,22 @@
             },
             "python": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -5805,14 +6627,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -5849,18 +6695,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -5904,45 +6750,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<string>",
-                                        "=>",
-                                        "<float>"
+                                        "<empty>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<float>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<number>"
+                                    ],
+                                    [
+                                        "<string>",
+                                        "=>",
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -5964,38 +6810,30 @@
                                                 "name": null,
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_LOWER": {
-                                                "name": "KW_LOWER",
+                                            "add-prefix": {
+                                                "name": "add-prefix",
                                                 "params": [
                                                     [
-                                                        "<empty>"
+                                                        "<string>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_UPPER": {
-                                                "name": "KW_UPPER",
+                                            "lower": {
+                                                "name": "lower",
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "add-prefix": {
-                                                "name": "add-prefix",
-                                                "params": [
-                                                    [
-                                                        "<string>"
-                                                    ]
-                                                ]
-                                            },
                                             "replace": {
                                                 "name": "replace",
                                                 "params": [
                                                     [
                                                         "<string>",
                                                         "<string>"
                                                     ]
@@ -6021,28 +6859,36 @@
                                             "shift-levels": {
                                                 "name": "shift-levels",
                                                 "params": [
                                                     [
                                                         "<positive-integer>"
                                                     ]
                                                 ]
+                                            },
+                                            "upper": {
+                                                "name": "upper",
+                                                "params": [
+                                                    [
+                                                        "<empty>"
+                                                    ]
+                                                ]
                                             }
                                         }
                                     }
                                 },
                                 "name": "key",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<string-list>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<string-list>"
                                             ]
                                         ]
                                     }
                                 }
                             },
                             "rekey": {
                                 "blocks": {},
@@ -6052,38 +6898,30 @@
                                         "name": null,
                                         "params": [
                                             [
                                                 "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_LOWER": {
-                                        "name": "KW_LOWER",
+                                    "add-prefix": {
+                                        "name": "add-prefix",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_UPPER": {
-                                        "name": "KW_UPPER",
+                                    "lower": {
+                                        "name": "lower",
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "add-prefix": {
-                                        "name": "add-prefix",
-                                        "params": [
-                                            [
-                                                "<string>"
-                                            ]
-                                        ]
-                                    },
                                     "replace": {
                                         "name": "replace",
                                         "params": [
                                             [
                                                 "<string>",
                                                 "<string>"
                                             ]
@@ -6109,14 +6947,22 @@
                                     "shift-levels": {
                                         "name": "shift-levels",
                                         "params": [
                                             [
                                                 "<positive-integer>"
                                             ]
                                         ]
+                                    },
+                                    "upper": {
+                                        "name": "upper",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
                                     }
                                 }
                             }
                         },
                         "name": "value-pairs",
                         "options": {
                             "": {
@@ -6139,24 +6985,32 @@
                                 "name": "exclude",
                                 "params": [
                                     [
                                         "<string-list>"
                                     ]
                                 ]
                             },
+                            "include-bytes": {
+                                "name": "include-bytes",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
@@ -6314,14 +7168,22 @@
             },
             "redis": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -6338,14 +7200,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -6382,18 +7268,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -6461,19 +7347,19 @@
                             ]
                         ]
                     },
                     "command": {
                         "name": "command",
                         "params": [
                             [
-                                "<string>",
-                                "<template-content>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<string>",
+                                "<template-content>"
                             ]
                         ]
                     },
                     "frac-digits": {
                         "name": "frac-digits",
                         "params": [
                             [
@@ -6617,38 +7503,30 @@
                                                 "name": null,
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_LOWER": {
-                                                "name": "KW_LOWER",
+                                            "add-prefix": {
+                                                "name": "add-prefix",
                                                 "params": [
                                                     [
-                                                        "<empty>"
+                                                        "<string>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_UPPER": {
-                                                "name": "KW_UPPER",
+                                            "lower": {
+                                                "name": "lower",
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "add-prefix": {
-                                                "name": "add-prefix",
-                                                "params": [
-                                                    [
-                                                        "<string>"
-                                                    ]
-                                                ]
-                                            },
                                             "replace": {
                                                 "name": "replace",
                                                 "params": [
                                                     [
                                                         "<string>",
                                                         "<string>"
                                                     ]
@@ -6674,28 +7552,36 @@
                                             "shift-levels": {
                                                 "name": "shift-levels",
                                                 "params": [
                                                     [
                                                         "<positive-integer>"
                                                     ]
                                                 ]
+                                            },
+                                            "upper": {
+                                                "name": "upper",
+                                                "params": [
+                                                    [
+                                                        "<empty>"
+                                                    ]
+                                                ]
                                             }
                                         }
                                     }
                                 },
                                 "name": "key",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<string-list>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<string-list>"
                                             ]
                                         ]
                                     }
                                 }
                             },
                             "rekey": {
                                 "blocks": {},
@@ -6705,38 +7591,30 @@
                                         "name": null,
                                         "params": [
                                             [
                                                 "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_LOWER": {
-                                        "name": "KW_LOWER",
+                                    "add-prefix": {
+                                        "name": "add-prefix",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_UPPER": {
-                                        "name": "KW_UPPER",
+                                    "lower": {
+                                        "name": "lower",
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "add-prefix": {
-                                        "name": "add-prefix",
-                                        "params": [
-                                            [
-                                                "<string>"
-                                            ]
-                                        ]
-                                    },
                                     "replace": {
                                         "name": "replace",
                                         "params": [
                                             [
                                                 "<string>",
                                                 "<string>"
                                             ]
@@ -6762,14 +7640,22 @@
                                     "shift-levels": {
                                         "name": "shift-levels",
                                         "params": [
                                             [
                                                 "<positive-integer>"
                                             ]
                                         ]
+                                    },
+                                    "upper": {
+                                        "name": "upper",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
                                     }
                                 }
                             }
                         },
                         "name": "attributes",
                         "options": {
                             "": {
@@ -6800,24 +7686,32 @@
                                 "name": "exclude",
                                 "params": [
                                     [
                                         "<string-list>"
                                     ]
                                 ]
                             },
+                            "include-bytes": {
+                                "name": "include-bytes",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
@@ -6831,14 +7725,22 @@
                             }
                         }
                     },
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -6855,14 +7757,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -6899,18 +7825,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -7298,14 +8224,22 @@
             },
             "smtp": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -7322,14 +8256,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -7366,18 +8324,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -7634,14 +8592,22 @@
             },
             "snmp": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -7658,14 +8624,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -7702,18 +8692,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -7909,14 +8899,22 @@
             },
             "sql": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -7933,14 +8931,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -7977,18 +8999,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -8081,14 +9103,22 @@
                             ],
                             [
                                 "<string>",
                                 "<string>"
                             ]
                         ]
                     },
+                    "dbi-driver-dir": {
+                        "name": "dbi-driver-dir",
+                        "params": [
+                            [
+                                "<path>"
+                            ]
+                        ]
+                    },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
@@ -8204,14 +9234,22 @@
                         "name": "port",
                         "params": [
                             [
                                 "<string-or-number>"
                             ]
                         ]
                     },
+                    "quote-char": {
+                        "name": "quote-char",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
                     "retries": {
                         "name": "retries",
                         "params": [
                             [
                                 "<positive-integer>"
                             ]
                         ]
@@ -8296,32 +9334,40 @@
                             ]
                         ]
                     },
                     "values": {
                         "name": "values",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "<template-content>"
                             ],
                             [
                                 "default"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     }
                 }
             },
             "stomp": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -8338,14 +9384,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -8382,18 +9452,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -8445,38 +9515,30 @@
                                                 "name": null,
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_LOWER": {
-                                                "name": "KW_LOWER",
+                                            "add-prefix": {
+                                                "name": "add-prefix",
                                                 "params": [
                                                     [
-                                                        "<empty>"
+                                                        "<string>"
                                                     ]
                                                 ]
                                             },
-                                            "KW_UPPER": {
-                                                "name": "KW_UPPER",
+                                            "lower": {
+                                                "name": "lower",
                                                 "params": [
                                                     [
                                                         "<empty>"
                                                     ]
                                                 ]
                                             },
-                                            "add-prefix": {
-                                                "name": "add-prefix",
-                                                "params": [
-                                                    [
-                                                        "<string>"
-                                                    ]
-                                                ]
-                                            },
                                             "replace": {
                                                 "name": "replace",
                                                 "params": [
                                                     [
                                                         "<string>",
                                                         "<string>"
                                                     ]
@@ -8502,28 +9564,36 @@
                                             "shift-levels": {
                                                 "name": "shift-levels",
                                                 "params": [
                                                     [
                                                         "<positive-integer>"
                                                     ]
                                                 ]
+                                            },
+                                            "upper": {
+                                                "name": "upper",
+                                                "params": [
+                                                    [
+                                                        "<empty>"
+                                                    ]
+                                                ]
                                             }
                                         }
                                     }
                                 },
                                 "name": "key",
                                 "options": {
                                     "": {
                                         "name": null,
                                         "params": [
                                             [
-                                                "<string-list>"
+                                                "<string>"
                                             ],
                                             [
-                                                "<string>"
+                                                "<string-list>"
                                             ]
                                         ]
                                     }
                                 }
                             },
                             "rekey": {
                                 "blocks": {},
@@ -8533,38 +9603,30 @@
                                         "name": null,
                                         "params": [
                                             [
                                                 "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_LOWER": {
-                                        "name": "KW_LOWER",
+                                    "add-prefix": {
+                                        "name": "add-prefix",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_UPPER": {
-                                        "name": "KW_UPPER",
+                                    "lower": {
+                                        "name": "lower",
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "add-prefix": {
-                                        "name": "add-prefix",
-                                        "params": [
-                                            [
-                                                "<string>"
-                                            ]
-                                        ]
-                                    },
                                     "replace": {
                                         "name": "replace",
                                         "params": [
                                             [
                                                 "<string>",
                                                 "<string>"
                                             ]
@@ -8590,14 +9652,22 @@
                                     "shift-levels": {
                                         "name": "shift-levels",
                                         "params": [
                                             [
                                                 "<positive-integer>"
                                             ]
                                         ]
+                                    },
+                                    "upper": {
+                                        "name": "upper",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
                                     }
                                 }
                             }
                         },
                         "name": "value-pairs",
                         "options": {
                             "": {
@@ -8620,24 +9690,32 @@
                                 "name": "exclude",
                                 "params": [
                                     [
                                         "<string-list>"
                                     ]
                                 ]
                             },
+                            "include-bytes": {
+                                "name": "include-bytes",
+                                "params": [
+                                    [
+                                        "<yesno>"
+                                    ]
+                                ]
+                            },
                             "pair": {
                                 "name": "pair",
                                 "params": [
                                     [
                                         "<string>",
+                                        ":",
                                         "<template-content>"
                                     ],
                                     [
                                         "<string>",
-                                        ":",
                                         "<template-content>"
                                     ]
                                 ]
                             },
                             "scope": {
                                 "name": "scope",
                                 "params": [
@@ -8819,14 +9897,22 @@
             },
             "syslog": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -8843,14 +9929,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -8887,18 +9997,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "failover": {
                         "blocks": {
@@ -9138,18 +10248,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -9388,18 +10498,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -9599,24 +10709,24 @@
                             ]
                         ]
                     },
                     "transport": {
                         "name": "transport",
                         "params": [
                             [
-                                "tcp"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
-                                "udp"
+                                "tcp"
                             ],
                             [
                                 "tls"
+                            ],
+                            [
+                                "udp"
                             ]
                         ]
                     },
                     "truncate-size": {
                         "name": "truncate-size",
                         "params": [
                             [
@@ -9636,14 +10746,22 @@
             },
             "tcp": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -9660,14 +10778,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -9704,18 +10846,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "failover": {
                         "blocks": {
@@ -9955,18 +11097,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -10197,18 +11339,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -10412,14 +11554,22 @@
             },
             "tcp6": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -10436,14 +11586,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -10480,18 +11654,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "failover": {
                         "blocks": {
@@ -10731,18 +11905,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -10973,18 +12147,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -11188,14 +12362,22 @@
             },
             "udp": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -11212,14 +12394,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -11256,18 +12462,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "failover": {
                         "blocks": {
@@ -11519,18 +12725,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -11750,14 +12956,22 @@
             },
             "udp6": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -11774,14 +12988,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -11818,18 +13056,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "failover": {
                         "blocks": {
@@ -12081,18 +13319,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -12312,14 +13550,22 @@
             },
             "unix-dgram": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -12336,14 +13582,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -12380,18 +13650,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -12534,18 +13804,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -12717,14 +13987,22 @@
             },
             "unix-stream": {
                 "blocks": {
                     "disk-buffer": {
                         "blocks": {},
                         "name": "disk-buffer",
                         "options": {
+                            "capacity-bytes": {
+                                "name": "capacity-bytes",
+                                "params": [
+                                    [
+                                        "<number>"
+                                    ]
+                                ]
+                            },
                             "compaction": {
                                 "name": "compaction",
                                 "params": [
                                     [
                                         "<yesno>"
                                     ]
                                 ]
@@ -12741,14 +14019,38 @@
                                 "name": "disk-buf-size",
                                 "params": [
                                     [
                                         "<number>"
                                     ]
                                 ]
                             },
+                            "flow-control-window-bytes": {
+                                "name": "flow-control-window-bytes",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "flow-control-window-size": {
+                                "name": "flow-control-window-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
+                            "front-cache-size": {
+                                "name": "front-cache-size",
+                                "params": [
+                                    [
+                                        "<nonnegative-integer>"
+                                    ]
+                                ]
+                            },
                             "mem-buf-length": {
                                 "name": "mem-buf-length",
                                 "params": [
                                     [
                                         "<nonnegative-integer>"
                                     ]
                                 ]
@@ -12785,18 +14087,18 @@
                                     ]
                                 ]
                             },
                             "truncate-size-ratio": {
                                 "name": "truncate-size-ratio",
                                 "params": [
                                     [
-                                        "<float>"
+                                        "<nonnegative-integer>"
                                     ],
                                     [
-                                        "<nonnegative-integer>"
+                                        "<float>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "hook-commands": {
                         "blocks": {},
@@ -12939,18 +14241,18 @@
                             ]
                         ]
                     },
                     "mark-mode": {
                         "name": "mark-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "on-error": {
                         "name": "on-error",
                         "params": [
                             [
@@ -13229,18 +14531,18 @@
                             ]
                         ]
                     },
                     "truncate-size-ratio": {
                         "name": "truncate-size-ratio",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     }
                 }
             },
             "jvm-options": {
                 "blocks": {},
@@ -13559,18 +14861,18 @@
                             ]
                         ]
                     },
                     "inject-mode": {
                         "name": "inject-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -13815,18 +15117,18 @@
                             ]
                         ]
                     },
                     "inject-mode": {
                         "name": "inject-mode",
                         "params": [
                             [
-                                "internal"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "internal"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -14101,38 +15403,30 @@
                                         "name": null,
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "KW_LOWER": {
-                                        "name": "KW_LOWER",
+                                    "add-prefix": {
+                                        "name": "add-prefix",
                                         "params": [
                                             [
-                                                "<empty>"
+                                                "<string>"
                                             ]
                                         ]
                                     },
-                                    "KW_UPPER": {
-                                        "name": "KW_UPPER",
+                                    "lower": {
+                                        "name": "lower",
                                         "params": [
                                             [
                                                 "<empty>"
                                             ]
                                         ]
                                     },
-                                    "add-prefix": {
-                                        "name": "add-prefix",
-                                        "params": [
-                                            [
-                                                "<string>"
-                                            ]
-                                        ]
-                                    },
                                     "replace": {
                                         "name": "replace",
                                         "params": [
                                             [
                                                 "<string>",
                                                 "<string>"
                                             ]
@@ -14158,28 +15452,36 @@
                                     "shift-levels": {
                                         "name": "shift-levels",
                                         "params": [
                                             [
                                                 "<positive-integer>"
                                             ]
                                         ]
+                                    },
+                                    "upper": {
+                                        "name": "upper",
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
                                     }
                                 }
                             }
                         },
                         "name": "key",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<string-list>"
+                                        "<string>"
                                     ],
                                     [
-                                        "<string>"
+                                        "<string-list>"
                                     ]
                                 ]
                             }
                         }
                     },
                     "rekey": {
                         "blocks": {},
@@ -14189,38 +15491,30 @@
                                 "name": null,
                                 "params": [
                                     [
                                         "<string>"
                                     ]
                                 ]
                             },
-                            "KW_LOWER": {
-                                "name": "KW_LOWER",
+                            "add-prefix": {
+                                "name": "add-prefix",
                                 "params": [
                                     [
-                                        "<empty>"
+                                        "<string>"
                                     ]
                                 ]
                             },
-                            "KW_UPPER": {
-                                "name": "KW_UPPER",
+                            "lower": {
+                                "name": "lower",
                                 "params": [
                                     [
                                         "<empty>"
                                     ]
                                 ]
                             },
-                            "add-prefix": {
-                                "name": "add-prefix",
-                                "params": [
-                                    [
-                                        "<string>"
-                                    ]
-                                ]
-                            },
                             "replace": {
                                 "name": "replace",
                                 "params": [
                                     [
                                         "<string>",
                                         "<string>"
                                     ]
@@ -14246,14 +15540,22 @@
                             "shift-levels": {
                                 "name": "shift-levels",
                                 "params": [
                                     [
                                         "<positive-integer>"
                                     ]
                                 ]
+                            },
+                            "upper": {
+                                "name": "upper",
+                                "params": [
+                                    [
+                                        "<empty>"
+                                    ]
+                                ]
                             }
                         }
                     }
                 },
                 "context": "parser",
                 "name": "map-value-pairs",
                 "options": {
@@ -14269,24 +15571,32 @@
                         "name": "exclude",
                         "params": [
                             [
                                 "<string-list>"
                             ]
                         ]
                     },
+                    "include-bytes": {
+                        "name": "include-bytes",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
                     "pair": {
                         "name": "pair",
                         "params": [
                             [
                                 "<string>",
+                                ":",
                                 "<template-content>"
                             ],
                             [
                                 "<string>",
-                                ":",
                                 "<template-content>"
                             ]
                         ]
                     },
                     "scope": {
                         "name": "scope",
                         "params": [
@@ -14404,55 +15714,78 @@
                             [
                                 "<string>"
                             ]
                         ]
                     }
                 }
             },
+            "opentelemetry": {
+                "blocks": {},
+                "context": "parser",
+                "name": "opentelemetry",
+                "options": {
+                    "internal": {
+                        "name": "internal",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "template": {
+                        "name": "template",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    }
+                }
+            },
             "python": {
                 "blocks": {
                     "options": {
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<string>",
-                                        "=>",
-                                        "<float>"
+                                        "<empty>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<float>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<number>"
+                                    ],
+                                    [
+                                        "<string>",
+                                        "=>",
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -14641,18 +15974,18 @@
                 "context": "parser",
                 "name": "syslog-parser",
                 "options": {
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -14687,18 +16020,18 @@
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ]
                         ]
                     },
                     "internal": {
                         "name": "internal",
                         "params": [
                             [
@@ -14987,18 +16320,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -15030,18 +16363,18 @@
                             ]
                         ]
                     },
                     "fetch-no-data-delay": {
                         "name": "fetch-no-data-delay",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "file": {
                         "name": "file",
                         "params": [
                             [
@@ -15188,18 +16521,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -15305,18 +16638,18 @@
                             ]
                         ]
                     },
                     "freq": {
                         "name": "freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "host-override": {
                         "name": "host-override",
                         "params": [
                             [
@@ -15428,18 +16761,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -15558,18 +16891,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -15751,18 +17084,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -15884,18 +17217,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -15968,21 +17301,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "check-hostname"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -16207,18 +17540,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -16332,18 +17665,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -16389,18 +17722,18 @@
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "dns-cache": {
                         "name": "dns-cache",
                         "params": [
                             [
@@ -16419,29 +17752,29 @@
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ]
                         ]
                     },
                     "follow-freq": {
                         "name": "follow-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "force-directory-polling": {
                         "name": "force-directory-polling",
                         "params": [
                             [
@@ -16682,18 +18015,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -16911,18 +18244,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -17125,18 +18458,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -17377,18 +18710,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -17509,18 +18842,18 @@
                             ]
                         ]
                     },
                     "dynamic-window-stats-freq": {
                         "name": "dynamic-window-stats-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "encoding": {
                         "name": "encoding",
                         "params": [
                             [
@@ -17528,21 +18861,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "check-hostname"
                             ],
                             [
                                 "<string>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -17857,21 +19190,21 @@
                     "transport": {
                         "name": "transport",
                         "params": [
                             [
                                 "<string>"
                             ],
                             [
-                                "udp"
-                            ],
-                            [
                                 "tcp"
                             ],
                             [
                                 "tls"
+                            ],
+                            [
+                                "udp"
                             ]
                         ]
                     },
                     "trim-large-messages": {
                         "name": "trim-large-messages",
                         "params": [
                             [
@@ -17879,18 +19212,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -17994,14 +19327,383 @@
                             [
                                 "<string>"
                             ]
                         ]
                     }
                 }
             },
+            "opentelemetry": {
+                "blocks": {
+                    "auth": {
+                        "blocks": {
+                            "tls": {
+                                "blocks": {},
+                                "name": "tls",
+                                "options": {
+                                    "": {
+                                        "name": null,
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
+                                    },
+                                    "ca-file": {
+                                        "name": "ca-file",
+                                        "params": [
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    },
+                                    "cert-file": {
+                                        "name": "cert-file",
+                                        "params": [
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    },
+                                    "key-file": {
+                                        "name": "key-file",
+                                        "params": [
+                                            [
+                                                "<string>"
+                                            ]
+                                        ]
+                                    },
+                                    "peer-verify": {
+                                        "name": "peer-verify",
+                                        "params": [
+                                            [
+                                                "optional-trusted"
+                                            ],
+                                            [
+                                                "required-untrusted"
+                                            ],
+                                            [
+                                                "optional-untrusted"
+                                            ],
+                                            [
+                                                "required-trusted"
+                                            ]
+                                        ]
+                                    }
+                                }
+                            }
+                        },
+                        "name": "auth",
+                        "options": {
+                            "alts": {
+                                "name": "alts",
+                                "params": [
+                                    [
+                                        "<empty>"
+                                    ]
+                                ]
+                            },
+                            "insecure": {
+                                "name": "insecure",
+                                "params": [
+                                    [
+                                        "<empty>"
+                                    ]
+                                ]
+                            }
+                        }
+                    },
+                    "ebpf": {
+                        "blocks": {
+                            "reuseport": {
+                                "blocks": {},
+                                "name": "reuseport",
+                                "options": {
+                                    "": {
+                                        "name": null,
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
+                                    },
+                                    "sockets": {
+                                        "name": "sockets",
+                                        "params": [
+                                            [
+                                                "<positive-integer>"
+                                            ]
+                                        ]
+                                    }
+                                }
+                            }
+                        },
+                        "name": "ebpf",
+                        "options": {}
+                    },
+                    "hook-commands": {
+                        "blocks": {},
+                        "name": "hook-commands",
+                        "options": {
+                            "setup": {
+                                "name": "setup",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "shutdown": {
+                                "name": "shutdown",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "startup": {
+                                "name": "startup",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "teardown": {
+                                "name": "teardown",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            }
+                        }
+                    }
+                },
+                "context": "source",
+                "name": "opentelemetry",
+                "options": {
+                    "chain-hostnames": {
+                        "name": "chain-hostnames",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "default-facility": {
+                        "name": "default-facility",
+                        "params": [
+                            [
+                                "<string>"
+                            ],
+                            [
+                                "KW_SYSLOG"
+                            ]
+                        ]
+                    },
+                    "default-level": {
+                        "name": "default-level",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "default-priority": {
+                        "name": "default-priority",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "default-severity": {
+                        "name": "default-severity",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "dns-cache": {
+                        "name": "dns-cache",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "flags": {
+                        "name": "flags",
+                        "params": [
+                            [
+                                "<empty>"
+                            ],
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "format": {
+                        "name": "format",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "host-override": {
+                        "name": "host-override",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "internal": {
+                        "name": "internal",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "keep-hostname": {
+                        "name": "keep-hostname",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "keep-timestamp": {
+                        "name": "keep-timestamp",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "log-iw-size": {
+                        "name": "log-iw-size",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "log-prefix": {
+                        "name": "log-prefix",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "long-hostnames": {
+                        "name": "long-hostnames",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "normalize-hostnames": {
+                        "name": "normalize-hostnames",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "persist-name": {
+                        "name": "persist-name",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "port": {
+                        "name": "port",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "program-override": {
+                        "name": "program-override",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "read-old-records": {
+                        "name": "read-old-records",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "sdata-prefix": {
+                        "name": "sdata-prefix",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "tags": {
+                        "name": "tags",
+                        "params": [
+                            [
+                                "<string-list>"
+                            ]
+                        ]
+                    },
+                    "time-zone": {
+                        "name": "time-zone",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "use-dns": {
+                        "name": "use-dns",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ],
+                            [
+                                "persist-only"
+                            ]
+                        ]
+                    },
+                    "use-fqdn": {
+                        "name": "use-fqdn",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "use-syslogng-pid": {
+                        "name": "use-syslogng-pid",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    }
+                }
+            },
             "pipe": {
                 "blocks": {
                     "ebpf": {
                         "blocks": {
                             "reuseport": {
                                 "blocks": {},
                                 "name": "reuseport",
@@ -18102,18 +19804,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -18186,21 +19888,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "check-hostname"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -18358,18 +20060,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -18425,18 +20127,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -18550,18 +20252,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -18604,18 +20306,18 @@
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -18767,18 +20469,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -18868,45 +20570,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<string>",
-                                        "=>",
-                                        "<float>"
+                                        "<empty>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
-                                        "<string>"
+                                        "<float>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<number>"
+                                    ],
+                                    [
+                                        "<string>",
+                                        "=>",
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -18936,18 +20638,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -19118,18 +20820,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -19219,45 +20921,45 @@
                         "blocks": {},
                         "name": "options",
                         "options": {
                             "": {
                                 "name": null,
                                 "params": [
                                     [
-                                        "<string>",
-                                        "=>",
-                                        "<float>"
+                                        "<empty>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "[",
                                         "<string-list>",
                                         "]"
                                     ],
                                     [
-                                        "<empty>"
-                                    ],
-                                    [
                                         "<string>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<python-yesno>"
                                     ],
                                     [
                                         "<string>",
                                         "=>",
                                         "<number>"
+                                    ],
+                                    [
+                                        "<string>",
+                                        "=>",
+                                        "<float>"
                                     ]
                                 ]
                             },
                             "LogTemplate": {
                                 "name": "LogTemplate",
                                 "params": [
                                     [
@@ -19287,18 +20989,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -19330,18 +21032,18 @@
                             ]
                         ]
                     },
                     "fetch-no-data-delay": {
                         "name": "fetch-no-data-delay",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
@@ -19488,21 +21190,323 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
+                                "<yesno>"
+                            ],
+                            [
                                 "persist-only"
+                            ]
+                        ]
+                    },
+                    "use-fqdn": {
+                        "name": "use-fqdn",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "use-syslogng-pid": {
+                        "name": "use-syslogng-pid",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    }
+                }
+            },
+            "random-choice-generator": {
+                "blocks": {
+                    "ebpf": {
+                        "blocks": {
+                            "reuseport": {
+                                "blocks": {},
+                                "name": "reuseport",
+                                "options": {
+                                    "": {
+                                        "name": null,
+                                        "params": [
+                                            [
+                                                "<empty>"
+                                            ]
+                                        ]
+                                    },
+                                    "sockets": {
+                                        "name": "sockets",
+                                        "params": [
+                                            [
+                                                "<positive-integer>"
+                                            ]
+                                        ]
+                                    }
+                                }
+                            }
+                        },
+                        "name": "ebpf",
+                        "options": {}
+                    },
+                    "hook-commands": {
+                        "blocks": {},
+                        "name": "hook-commands",
+                        "options": {
+                            "setup": {
+                                "name": "setup",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "shutdown": {
+                                "name": "shutdown",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "startup": {
+                                "name": "startup",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            },
+                            "teardown": {
+                                "name": "teardown",
+                                "params": [
+                                    [
+                                        "<string>"
+                                    ]
+                                ]
+                            }
+                        }
+                    }
+                },
+                "context": "source",
+                "name": "random-choice-generator",
+                "options": {
+                    "chain-hostnames": {
+                        "name": "chain-hostnames",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "choices": {
+                        "name": "choices",
+                        "params": [
+                            [
+                                "<string-list>"
+                            ]
+                        ]
+                    },
+                    "default-facility": {
+                        "name": "default-facility",
+                        "params": [
+                            [
+                                "<string>"
+                            ],
+                            [
+                                "KW_SYSLOG"
+                            ]
+                        ]
+                    },
+                    "default-level": {
+                        "name": "default-level",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "default-priority": {
+                        "name": "default-priority",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "default-severity": {
+                        "name": "default-severity",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "dns-cache": {
+                        "name": "dns-cache",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "flags": {
+                        "name": "flags",
+                        "params": [
+                            [
+                                "<empty>"
                             ],
                             [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "format": {
+                        "name": "format",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "freq": {
+                        "name": "freq",
+                        "params": [
+                            [
+                                "<nonnegative-integer>"
+                            ],
+                            [
+                                "<float>"
+                            ]
+                        ]
+                    },
+                    "host-override": {
+                        "name": "host-override",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "internal": {
+                        "name": "internal",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "keep-hostname": {
+                        "name": "keep-hostname",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "keep-timestamp": {
+                        "name": "keep-timestamp",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "log-iw-size": {
+                        "name": "log-iw-size",
+                        "params": [
+                            [
+                                "<positive-integer>"
+                            ]
+                        ]
+                    },
+                    "log-prefix": {
+                        "name": "log-prefix",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "long-hostnames": {
+                        "name": "long-hostnames",
+                        "params": [
+                            [
                                 "<yesno>"
                             ]
                         ]
                     },
+                    "normalize-hostnames": {
+                        "name": "normalize-hostnames",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "persist-name": {
+                        "name": "persist-name",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "program-override": {
+                        "name": "program-override",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "read-old-records": {
+                        "name": "read-old-records",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ]
+                        ]
+                    },
+                    "sdata-prefix": {
+                        "name": "sdata-prefix",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "tags": {
+                        "name": "tags",
+                        "params": [
+                            [
+                                "<string-list>"
+                            ]
+                        ]
+                    },
+                    "time-zone": {
+                        "name": "time-zone",
+                        "params": [
+                            [
+                                "<string>"
+                            ]
+                        ]
+                    },
+                    "use-dns": {
+                        "name": "use-dns",
+                        "params": [
+                            [
+                                "<yesno>"
+                            ],
+                            [
+                                "persist-only"
+                            ]
+                        ]
+                    },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
                                 "<yesno>"
                             ]
                         ]
@@ -19605,18 +21609,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -19662,18 +21666,18 @@
                             ]
                         ]
                     },
                     "dir-perm": {
                         "name": "dir-perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "dns-cache": {
                         "name": "dns-cache",
                         "params": [
                             [
@@ -19689,32 +21693,32 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "check-hostname"
                             ],
                             [
                                 "<string>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "follow-freq": {
                         "name": "follow-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "force-directory-polling": {
                         "name": "force-directory-polling",
                         "params": [
                             [
@@ -19880,18 +21884,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -19955,18 +21959,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -20411,18 +22415,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -20543,18 +22547,18 @@
                             ]
                         ]
                     },
                     "dynamic-window-stats-freq": {
                         "name": "dynamic-window-stats-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "encoding": {
                         "name": "encoding",
                         "params": [
                             [
@@ -20562,18 +22566,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<string>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
                                 "check-hostname"
                             ]
                         ]
                     },
                     "format": {
@@ -20888,23 +22892,23 @@
                             ]
                         ]
                     },
                     "transport": {
                         "name": "transport",
                         "params": [
                             [
-                                "tls"
-                            ],
-                            [
                                 "<string>"
                             ],
                             [
                                 "tcp"
                             ],
                             [
+                                "tls"
+                            ],
+                            [
                                 "udp"
                             ]
                         ]
                     },
                     "trim-large-messages": {
                         "name": "trim-large-messages",
                         "params": [
@@ -20913,18 +22917,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -21022,18 +23026,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -21222,18 +23226,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -21390,21 +23394,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "check-hostname"
                             ],
                             [
                                 "<string>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -21604,18 +23608,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -21848,18 +23852,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -21980,18 +23984,18 @@
                             ]
                         ]
                     },
                     "dynamic-window-stats-freq": {
                         "name": "dynamic-window-stats-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "encoding": {
                         "name": "encoding",
                         "params": [
                             [
@@ -22002,18 +24006,18 @@
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -22325,18 +24329,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -22569,18 +24573,18 @@
                                     ]
                                 ]
                             },
                             "peer-verify": {
                                 "name": "peer-verify",
                                 "params": [
                                     [
-                                        "<string>"
+                                        "<yesno>"
                                     ],
                                     [
-                                        "<yesno>"
+                                        "<string>"
                                     ]
                                 ]
                             },
                             "pkcs12-file": {
                                 "name": "pkcs12-file",
                                 "params": [
                                     [
@@ -22701,18 +24705,18 @@
                             ]
                         ]
                     },
                     "dynamic-window-stats-freq": {
                         "name": "dynamic-window-stats-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "encoding": {
                         "name": "encoding",
                         "params": [
                             [
@@ -22720,18 +24724,18 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<string>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
                                 "check-hostname"
                             ]
                         ]
                     },
                     "format": {
@@ -23046,18 +25050,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -23217,18 +25221,18 @@
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "<empty>"
                             ],
                             [
-                                "check-hostname"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "check-hostname"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -23516,18 +25520,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -23684,21 +25688,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<empty>"
-                            ],
-                            [
                                 "check-hostname"
                             ],
                             [
                                 "<string>"
+                            ],
+                            [
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -23986,18 +25990,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -24211,18 +26215,18 @@
                             ]
                         ]
                     },
                     "dynamic-window-stats-freq": {
                         "name": "dynamic-window-stats-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "encoding": {
                         "name": "encoding",
                         "params": [
                             [
@@ -24230,21 +26234,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "<string>"
+                                "check-hostname"
                             ],
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "check-hostname"
+                                "<empty>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -24533,18 +26537,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -24758,18 +26762,18 @@
                             ]
                         ]
                     },
                     "dynamic-window-stats-freq": {
                         "name": "dynamic-window-stats-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "encoding": {
                         "name": "encoding",
                         "params": [
                             [
@@ -24777,21 +26781,21 @@
                             ]
                         ]
                     },
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
-                                "check-hostname"
-                            ],
-                            [
                                 "<empty>"
                             ],
                             [
                                 "<string>"
+                            ],
+                            [
+                                "check-hostname"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -24949,18 +26953,18 @@
                             ]
                         ]
                     },
                     "perm": {
                         "name": "perm",
                         "params": [
                             [
-                                "<number>"
+                                "<empty>"
                             ],
                             [
-                                "<empty>"
+                                "<number>"
                             ]
                         ]
                     },
                     "persist-name": {
                         "name": "persist-name",
                         "params": [
                             [
@@ -25080,18 +27084,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
@@ -25205,18 +27209,18 @@
                             ]
                         ]
                     },
                     "default-facility": {
                         "name": "default-facility",
                         "params": [
                             [
-                                "KW_SYSLOG"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "KW_SYSLOG"
                             ]
                         ]
                     },
                     "default-level": {
                         "name": "default-level",
                         "params": [
                             [
@@ -25300,29 +27304,29 @@
                     "flags": {
                         "name": "flags",
                         "params": [
                             [
                                 "check-hostname"
                             ],
                             [
-                                "<empty>"
+                                "<string>"
                             ],
                             [
-                                "<string>"
+                                "<empty>"
                             ]
                         ]
                     },
                     "follow-freq": {
                         "name": "follow-freq",
                         "params": [
                             [
-                                "<float>"
+                                "<nonnegative-integer>"
                             ],
                             [
-                                "<nonnegative-integer>"
+                                "<float>"
                             ]
                         ]
                     },
                     "format": {
                         "name": "format",
                         "params": [
                             [
@@ -25571,18 +27575,18 @@
                             ]
                         ]
                     },
                     "use-dns": {
                         "name": "use-dns",
                         "params": [
                             [
-                                "persist-only"
+                                "<yesno>"
                             ],
                             [
-                                "<yesno>"
+                                "persist-only"
                             ]
                         ]
                     },
                     "use-fqdn": {
                         "name": "use-fqdn",
                         "params": [
                             [
```

### Comparing `syslog_ng_cfg_helper-1.0.6/PKG-INFO` & `syslog_ng_cfg_helper-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syslog-ng-cfg-helper
-Version: 1.0.6
+Version: 1.0.7
 Summary: Configuration helper for syslog-ng.
 Home-page: https://github.com/alltilla/syslog-ng-cfg-helper
 License: GPL-3.0-only
 Keywords: syslog-ng,configuration,cfg
 Author: Attila Szakacs
 Author-email: szakacs.attila96@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -21,15 +21,15 @@
 Project-URL: Repository, https://github.com/alltilla/syslog-ng-cfg-helper
 Description-Content-Type: text/markdown
 
 # syslog-ng CFG Helper
 
 This tool makes configuring [syslog-ng](https://github.com/syslog-ng/syslog-ng) a bit easier by listing the options of each available driver.
 
-The options are generated from [syslog-ng v4.2.0](https://github.com/syslog-ng/syslog-ng/releases/tag/syslog-ng-4.2.0).
+The options are generated from [syslog-ng v4.3.0](https://github.com/syslog-ng/syslog-ng/releases/tag/syslog-ng-4.3.0).
 
 ## Quickstart
 
 ### Install with pipx
 ```
 pipx install syslog-ng-cfg-helper
 ```
```

