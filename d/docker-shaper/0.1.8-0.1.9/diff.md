# Comparing `tmp/docker_shaper-0.1.8.tar.gz` & `tmp/docker_shaper-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.8.tar", max compression
+gzip compressed data, was "docker_shaper-0.1.9.tar", max compression
```

## Comparing `docker_shaper-0.1.8.tar` & `docker_shaper-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0     3006 2023-07-05 08:01:08.591249 docker_shaper-0.1.8/Readme.md
--rw-r--r--   0        0        0        0 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/cli.py
--rw-r--r--   0        0        0    31566 2023-07-07 15:54:26.006882 docker_shaper-0.1.8/docker_shaper/dynamic.py
--rw-r--r--   0        0        0     8739 2023-07-07 15:54:25.814886 docker_shaper-0.1.8/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   155631 2023-07-05 08:01:08.599249 docker_shaper-0.1.8/docker_shaper/static/bootstrap.css
--rw-r--r--   0        0        0        0 2023-07-05 08:01:08.579249 docker_shaper-0.1.8/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0     1333 2023-07-07 06:45:33.419474 docker_shaper-0.1.8/docker_shaper/templates/base.html
--rw-r--r--   0        0        0      321 2023-07-05 08:01:08.595249 docker_shaper-0.1.8/docker_shaper/templates/containers.html
--rw-r--r--   0        0        0      956 2023-07-05 08:01:08.595249 docker_shaper-0.1.8/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0      309 2023-07-05 08:01:08.595249 docker_shaper-0.1.8/docker_shaper/templates/images.html
--rw-r--r--   0        0        0     5474 2023-07-06 14:45:56.181912 docker_shaper-0.1.8/docker_shaper/utils.py
--rw-r--r--   0        0        0     2259 2023-07-07 15:54:16.227094 docker_shaper-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3810 1970-01-01 00:00:00.000000 docker_shaper-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3084 2023-07-21 09:44:02.034044 docker_shaper-0.1.9/Readme.md
+-rw-r--r--   0        0        0        0 2023-07-21 09:44:02.034044 docker_shaper-0.1.9/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1459 2023-07-21 09:44:02.034044 docker_shaper-0.1.9/docker_shaper/cli.py
+-rw-r--r--   0        0        0    41373 2023-07-21 19:30:35.081819 docker_shaper-0.1.9/docker_shaper/dynamic.py
+-rw-r--r--   0        0        0    12075 2023-07-21 19:35:11.395918 docker_shaper-0.1.9/docker_shaper/server.py
+-rw-r--r--   0        0        0        0 2023-07-21 09:44:02.038044 docker_shaper-0.1.9/docker_shaper/static/__init__.py
+-rw-r--r--   0        0        0   232914 2023-07-21 15:40:59.051386 docker_shaper-0.1.9/docker_shaper/static/bootstrap.min.css
+-rw-r--r--   0        0        0   589307 2023-07-21 15:40:59.055386 docker_shaper-0.1.9/docker_shaper/static/bootstrap.min.css.map
+-rw-r--r--   0        0        0     1001 2023-07-21 15:40:59.059386 docker_shaper-0.1.9/docker_shaper/static/docker_shaper.js
+-rw-r--r--   0        0        0        0 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-21 15:40:59.059386 docker_shaper-0.1.9/docker_shaper/templates/base.html
+-rw-r--r--   0        0        0      312 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/containers.html
+-rw-r--r--   0        0        0     1362 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/dashboard.html
+-rw-r--r--   0        0        0      299 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/images.html
+-rw-r--r--   0        0        0      315 2023-07-21 09:44:02.066044 docker_shaper-0.1.9/docker_shaper/templates/messages.html
+-rw-r--r--   0        0        0      315 2023-07-21 09:44:02.066044 docker_shaper-0.1.9/docker_shaper/templates/rules.html
+-rw-r--r--   0        0        0      317 2023-07-21 09:44:02.066044 docker_shaper-0.1.9/docker_shaper/templates/volumes.html
+-rw-r--r--   0        0        0     9586 2023-07-21 17:39:57.663751 docker_shaper-0.1.9/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2296 2023-07-21 09:44:02.074044 docker_shaper-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 docker_shaper-0.1.9/PKG-INFO
```

### Comparing `docker_shaper-0.1.8/Readme.md` & `docker_shaper-0.1.9/Readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,29 @@
 - [x] bring in dockermon
 - [x] auto update
 - [x] outsource config
 - [x] bring in dgcd
 - [x] new: untag certain tags
 - [x] new: container cleanup
 - [x] Fix `none` image lookup
-- [ ] Exceptions to messages
-- [ ] Clip / persist messages
+- [x] Exceptions to messages
+- [x] Clip
+- [x] Increase/decrease logging via web / signal
+- [x] Link: cleanup (images/containers) now
+- [x] Add volumes list (with recent owners)
+- [ ] Bring in `list_volumes` (volume monitoring)
+- [ ] Containers: show total CPU usage
+- [ ] Containers: list volumes
+- [ ] Volumes: list usage
+- [ ] Persist messages
 - [ ] Instructions to readme
 - [ ] List unmatched / overmatched tags
-- [ ] bring in `list_volumes` (volume monitoring)
-- [ ] Add volumes list (with recent owners)
-- [ ] Increase/decrease logging via web / signal
 - [ ] Links to `delete` / `remove`
 - [ ] Links to jobs
-- [ ] Skipable `wait`
 - [ ] Link: inspect
-- [ ] Link: cleanup (images/containers) now
 - [ ] Graph: cpu / containers (idle/up)
 - [ ] Authenticate (at least if we can modify behavior, like stopping/removing images/containers)
 
 
 ### Setup
```

### Comparing `docker_shaper-0.1.8/docker_shaper/cli.py` & `docker_shaper-0.1.9/docker_shaper/cli.py`

 * *Files identical despite different names*

### Comparing `docker_shaper-0.1.8/docker_shaper/dynamic.py` & `docker_shaper-0.1.9/docker_shaper/dynamic.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,124 +2,124 @@
 
 """Functionality that might change during runtime
 """
 import asyncio
 import logging
 import os
 import re
-import signal
-import sys
 import time
-import traceback
 from collections import Counter
 from contextlib import suppress
 from dataclasses import dataclass
 from datetime import datetime
-from pathlib import Path
 from subprocess import CalledProcessError
-from typing import MutableMapping, MutableSequence, Optional, Tuple, Union
+from typing import MutableMapping, MutableSequence, Optional, Set, Tuple
 
 from aiodocker import Docker, DockerError
 from dateutil import tz
 from flask_table import Col, Table
-from quart import render_template, request, url_for
+from quart import redirect, render_template, request, url_for, websocket
 
-from docker_shaper.utils import impatient, process_output, watchdog
+from docker_shaper.utils import (
+    age_str,
+    date_from,
+    date_str,
+    dur_str,
+    impatient,
+    process_output,
+    setup_introspection_on_signal,
+)
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
-    return logging.getLogger("docker-shaper.dynamic")
+    return logging.getLogger("docker-shaper")
 
 
 @dataclass
 class GlobalState:
+    """The dirty globally shared state of docker-shaper"""
+
     intervals: MutableMapping[str, float]
     image_ids: MutableMapping[str, object]
     images: MutableMapping[str, object]
+    images_crawled: bool
     containers: MutableMapping[str, object]
+    containers_crawled: bool
+    volumes: MutableMapping[str, object]
+    volumes_crawled: bool
     event_horizon: int
     last_referenced: MutableMapping[str, MutableSequence[int]]
     tag_rules: MutableMapping[str, int]
     extra_links: MutableMapping[str, int]
     messages: MutableSequence[Tuple[int, str, str]]
     switches: MutableMapping[str, bool]
     hostname: str
     expiration_ages: MutableMapping[str, int]
+    update_mqueues: Set[asyncio.Queue]
 
     def __init__(self):
         self.intervals = {
             "state": 2,
             "image_stats": 2,
             "image_update": 2,
             "container_update": 2,
             "container_stats": 2,
             "cleanup": 3600,
         }
+        self.cleanup_fuse = 0
         self.image_ids = {}
         self.images = {}
+        self.images_crawled = False
         self.containers = {}
+        self.containers_crawled = False
+        self.volumes = {}
+        self.volumes_crawled = False
+
         self.event_horizon = int(time.time())
         self.last_referenced = {}
         self.tag_rules = {}
         self.counter = 0
         self.extra_links = {}
         self.switches = {}
         self.messages = []
         self.hostname = open("/etc/hostname").read().strip()
         self.expiration_ages = {}
+        self.update_mqueues = set()
+
+    def new_update_queue(self) -> asyncio.Queue:
+        """Creates and returns a new message queue"""
+        mqueue = asyncio.Queue()
+        self.update_mqueues.add(mqueue)
+        log().info("new connection (%d)", len(self.update_mqueues))
+        return mqueue
+
+    def remove_queue(self, mqueue: asyncio.Queue) -> None:
+        """Removes an existing queue from message queues"""
+        self.update_mqueues.remove(mqueue)
+        del mqueue
+        log().info("closed connection (%d)", len(self.update_mqueues))
+
+    async def inform(self, message: str) -> None:
+        """Send a message to all connected message queues"""
+        for mqueue in self.update_mqueues:
+            await mqueue.put(message)
 
 
 def short_id(docker_id: str) -> str:
     """Return the 10-digit variant of a long docker ID
     >>> short_id("sha256:abcdefghijklmnop")
     'abcdefghij'
     """
     if not docker_id:
         return docker_id
     assert is_uid(docker_id)
     return docker_id[7:17] if docker_id.startswith("sha256:") else docker_id[:10]
 
 
-def age_str(now: Union[int, datetime], age: Union[int, datetime, None]) -> str:
-    """Turn a number of seconds into something human readable"""
-    if age is None:
-        return "--"
-    tds = int(
-        (now.timestamp() if isinstance(now, datetime) else now)
-        - (age.timestamp() if isinstance(age, datetime) else age)
-    )
-    return f"{tds//86400:02d}d" f":{tds//3600%24:02d}h" f":{tds//60%60:02d}m"
-
-
-def date_str(date: datetime) -> str:
-    if not date:
-        return "--"
-    return (date if isinstance(date, datetime) else datetime.fromtimestamp(date)).strftime(
-        "%Y.%m.%d-%H:%M:%S"
-    )
-
-
-def date_from(timestamp: Union[int, float, str]) -> datetime:
-    try:
-        if isinstance(timestamp, (int, float)):
-            return datetime.fromtimestamp(timestamp)
-
-        if timestamp[-1] == "Z":
-            return (
-                datetime.strptime(timestamp[:19], "%Y-%m-%dT%H:%M:%S")
-                .replace(tzinfo=tz.tzutc())
-                .astimezone(tz.tzlocal())
-            )
-    except OverflowError:
-        return None
-    except Exception as exc:
-        raise ValueError(f"Could not parse datetime from <{timestamp!r}> ({exc})")
-
-
 @impatient
 def id_from(name: str) -> Optional[str]:
     """Looks up name using `docker inspect` and returns a 10 digit Docker ID"""
     with suppress(CalledProcessError):
         log().debug("resolve %s", name)
         return short_id(
             name
@@ -208,82 +208,152 @@
         operator,
         cmd,
         uid,
         dict(p.split("=") for p in params.split(", ")),
     )
 
 
-async def handle_docker_event_line(docker_client, global_state, line):
+async def handle_docker_event_line(global_state: GlobalState, line: str, docker_client) -> None:
     """Read a `docker events` line and maintain the last-used information"""
 
     tstamp, object_type, operator, _cmd, uid, params = event_from(line)
 
+    # print(f"{object_type} {operator} {uid} {params['name']}")
+    # print("XXXX", line)
+
     if (object_type, operator) in {
         ("image", "tag"),
         ("image", "pull"),
         ("container", "create"),
     }:
         ident = params.get("image") or params["name"]
         log().info(
             "docker event %s %s %s ident=%s _uid=%s",
             datetime.fromtimestamp(tstamp),
             object_type,
             operator,
             ident,
             uid,
         )
-    elif object_type in {"network", "builder"}:
-        return
-    elif (object_type, operator) in {
-        ("image", "untag"),
-        ("image", "prune"),
-        ("image", "push"),
-        ("image", "delete"),
-        ("container", "exec_create:"),
-        ("container", "exec_start:"),
-        ("container", "exec_die"),
-        ("container", "kill"),
-        ("container", "start"),
-        ("container", "attach"),
-        ("container", "die"),
-        ("container", "top"),
-        ("container", "destroy"),
-        ("container", "prune"),
-        ("container", "stop"),
-        ("container", "archive-path"),
-        ("network", "connect"),
-        ("network", "disconnect"),
-        ("volume", "create"),
-        ("volume", "mount"),
-        ("volume", "unmount"),
-        ("volume", "destroy"),
-    }:
-        return
-    else:
-        log().warning("unknown type/operator %s %s", object_type, operator)
-        return
+        global_state.event_horizon = min(global_state.event_horizon, tstamp)
+        register_reference(ident, tstamp, global_state)
+
+    if object_type == "container":
+        if operator in {
+            "create",
+        }:
+            container = await container_from(docker_client, uid)
+            assert container
+            await register_container(container, global_state)
+            return
+
+        if operator in {
+            "destroy",
+        }:
+            # not needed, since watch_container() already takes care..
+            # unregister_container(uid, global_state)
+
+            if await container_from(docker_client, uid):
+                report(global_state, "error", f"container {uid} still alive after {operator}")
+            return
+
+        if operator in {
+            "exec_create:",
+            "exec_start:",
+            "exec_die",
+            "kill",
+            "start",
+            "attach",
+            "top",
+            "prune",
+            "die",
+            "stop",
+            "resize",
+            "archive-path",
+        }:
+            if (
+                operator not in {"prune", "destroy"}
+                and not await container_from(docker_client, uid)
+                and global_state.containers_crawled
+            ):
+                report(
+                    global_state,
+                    "error",
+                    f"operator is {operator} but container {uid} does not exist",
+                )
+            return
+        # del global_state.images[ident]
+        # del global_state.volumes[ident]
+
+    elif object_type == "image":
+        if operator in {
+            "pull",
+        }:
+            await register_image(global_state, await image_from(docker_client, uid))
+            return
+
+        if operator in {
+            "tag",
+        }:
+            await update_image_registration(global_state, docker_client, params["name"])
+            return
+
+        if operator in {
+            "untag",
+            "prune",
+            "push",
+            "delete",
+        }:
+            await update_image_registration(global_state, docker_client, params["name"])
+            return
+
+    elif object_type == "network":
+        if operator in {
+            "connect",
+            "disconnect",
+        }:
+            return
+
+    elif object_type == "volume":
+        if operator in {
+            "create",
+            "mount",
+            "unmount",
+            "destroy",
+        }:
+            return
 
-    global_state.event_horizon = min(global_state.event_horizon, tstamp)
-    register_reference(ident, tstamp, global_state)
+    log().warning("unknown type/operator %s %s", object_type, operator)
 
 
 def is_uid(ident: str) -> bool:
     """
-    sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2
-    48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2
-    48a3535fe27f
+    >>> is_uid("sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2")
+    True
+    >>> is_uid("48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2")
+    True
+    >>> is_uid("48a3535fe2")
+    True
+    >>> is_uid("48a3535fe27f")
+    False
     """
-    return (
+    return bool(
         ident.startswith("sha256:")
-        or re.match("[0-9a-f]{64}", ident)
-        or re.match("[0-9a-f]{10}", ident)
+        or re.match("^[0-9a-f]{64}$", ident)
+        or re.match("^[0-9a-f]{10}$", ident)
     )
 
 
 def unique_ident(ident: str) -> str:
+    """Return a short Id if ident is a unique id and leave it as it is otherwise
+    >>> unique_ident("sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2")
+    '48a3535fe2'
+    >>> unique_ident("914463316976.dkr.ecr.eu-central-1.amazonaws.com/user_admin_panel:958")
+    '914463316976.dkr.ecr.eu-central-1.amazonaws.com/user_admin_panel:958'
+    """
     return short_id(ident) if is_uid(ident) else ident
 
 
 def register_reference(ident: str, timestamp: int, global_state) -> None:
     effective_ident = unique_ident(ident)
     if effective_ident not in global_state.last_referenced:
         global_state.last_referenced[effective_ident] = [
@@ -294,14 +364,15 @@
     # increase last reference date if applicable
     global_state.last_referenced[effective_ident][0] = max(
         global_state.last_referenced[effective_ident][0] or 0, timestamp
     )
 
 
 def expiration_age_from_ident(ident: str, global_state: GlobalState) -> int:
+    # TODO: distinguish between container, image and volume
     if is_uid(ident):
         return global_state.expiration_ages["tag_default"]
 
     effective_ident = unique_ident(ident)
 
     matching_rules = tuple(
         (regex, age)
@@ -320,15 +391,18 @@
 
     return global_state.expiration_ages["tag_unknown"]
 
 
 @impatient
 def expired(ident: str, global_state, now: int, extra_date: int = 0) -> bool:
     if ident not in global_state.last_referenced:
-        log().warn("no reference: %s", ident)
+        log().debug("expired(%s): no reference yet", ident)
+
+    if ident != unique_ident(ident):
+        log().error("expired() called with non-uniform identifier: %s", ident)
 
     # TODO
     last_referenced, expiration_age = global_state.last_referenced.setdefault(
         ident, [None, expiration_age_from_ident(ident, global_state)]
     )
 
     effective_age = now - max(
@@ -379,24 +453,29 @@
             "org.tribe29.cmk_version",
         )
         for w in l.split()
         if not (w.startswith("sha256") or len(w) == 64)
     )
 
 
-async def dump_global_state(global_state):
+async def dump_global_state(global_state: GlobalState):
     global_state.counter += 1
-    print(f"STATE: {', '.join('='.join(map(str, i)) for i in global_state.intervals.items())}")
+    print(f"STATE: ========================================================")
     print(f"STATE: frame counter: {global_state.counter}")
-    print(f"STATE: images: {len(global_state.images)}")
-    print(f"STATE: containers: {len(global_state.containers)}")
-    print(f"STATE: tag_rules: {len(global_state.tag_rules)}")
+    print(
+        f"STATE: intervals:     {', '.join('='.join(map(str, i)) for i in global_state.intervals.items())}"
+    )
+    print(f"STATE: images:        {len(global_state.images)}")
+    print(f"STATE: containers:    {len(global_state.containers)}")
+    print(f"STATE: tag_rules:     {len(global_state.tag_rules)}")
+    print(f"STATE: connections:   {len(global_state.update_mqueues)}")
     print(
         f"STATE: tasks: {', '.join('/'.join(map(str, i)) for i in Counter(t.get_coro().__name__ for t in asyncio.all_tasks()).items())}"
     )
+    print(f"STATE: ========================================================")
 
 
 class BaseTable(Table):
     allow_sort = True
     classes = ["table", "table-striped"]
 
     def __init__(self, endpoint, items):
@@ -427,30 +506,33 @@
 
     @staticmethod
     def html_from(endpoint, global_state, sort, reverse):
         now = datetime.now(tz=tz.tzutc())
 
         def dict_from(image):
             now_timestamp = now.timestamp()
+            # todo: no need for date_from
             created_timestamp = date_from(image["created_at"]).timestamp()
 
             def coloured_ident(ident):
                 is_expired, last_referenced, expiration_age = expired(
                     ident, global_state, now_timestamp, created_timestamp
                 )
                 return (
                     f"<div class='text-{'danger' if is_expired else 'success'}'>"
-                    f"{ident} ({age_str(now, last_referenced)}/{age_str(expiration_age, 0)})</div>"
+                    f"{ident} ({age_str(now, last_referenced)}/{age_str(expiration_age, 0)}) "
+                    f"<a href=remove_image_ident?ident={ident}>del</a>"
+                    f"</div>"
                 )
 
             return {
                 "short_id": coloured_ident(image["short_id"]),
                 "tags": "".join(map(coloured_ident, image["tags"] or [])),
                 "created_at": date_str(image["created_at"]),
-                "age": age_str(now, date_from(image["created_at"])),
+                "age": age_str(now, image["created_at"], fixed=True),
                 # "last_referenced": last_referenced_str(image["short_id"]),
                 # "class": "text-danger" if would_cleanup_image(image, now, global_state) else "text-success",
             }
 
         return ImageTable(
             endpoint,
             items=sorted(
@@ -485,41 +567,48 @@
             sort_key_containers=col_key,
             sort_direction_containers="desc" if reverse else "asc",
         )
 
     @staticmethod
     def html_from(endpoint, global_state, sort, reverse):
         now = datetime.now(tz=tz.tzutc())
+
+        def coloured_ident(cnt):
+            cnt_expired = would_cleanup_container(cnt, now.timestamp(), global_state)
+            return (
+                f"<div class='text-{'danger' if cnt_expired else 'success'}'>"
+                f"{cnt['short_id']} "
+                f"<a href=delete_container?ident={cnt['short_id']}>del</a>"
+                f"</div>"
+            )
+
         return ContainerTable(
             endpoint,
             items=sorted(
                 (
                     {
-                        "short_id": cnt["short_id"],
+                        "short_id": coloured_ident(cnt),
                         "name": cnt["name"],
                         "image": short_id(cnt["image"]) if is_uid(cnt["image"]) else cnt["image"],
                         "mem_usage": f"{(mem_stats.get('usage', 0)>>20)}MiB",
                         "cpu": f"{int(cpu_perc(cpu_stats, last_cpu_stats) * 1000) / 10}%",
                         "cmd": " ".join(cnt["show"]["Config"]["Cmd"])[:100],
                         "job": jobname_from(
                             cnt["show"]["HostConfig"]["Binds"]
                             or list(cnt["show"]["Config"]["Volumes"] or [])
                         ),
                         "created_at": date_str(date_from(cnt["show"]["Created"])),
                         "started_at": date_str(
                             started_at := date_from(cnt["show"]["State"]["StartedAt"])
                         ),
-                        "uptime": age_str(now, started_at),
+                        "uptime": age_str(now, started_at, fixed=True),
                         "status": cnt["show"]["State"]["Status"],
                         "hints": label_filter(cnt["show"]["Config"]["Labels"]),
                         "pid": int(cnt["show"]["State"]["Pid"]),
                         # https://getbootstrap.com/docs/4.0/utilities/colors/
-                        "class": "text-danger"
-                        if would_cleanup_container(cnt, now.timestamp(), global_state)
-                        else "text-success",
                     }
                     for cnt, mem_stats, cpu_stats, last_cpu_stats in (
                         (
                             c,
                             c["stats"].get("memory_stats", {}),
                             c["stats"]["cpu_stats"],
                             c["last_stats"].get("cpu_stats"),
@@ -530,58 +619,160 @@
                 ),
                 key=lambda e: e[sort],
                 reverse=reverse,
             ),
         ).__html__()
 
 
-def meta_info(global_state):
+class VolumeTable(BaseTable):
+    name = PlainCol("name")
+    labels = PlainCol("labels")
+    created_at = PlainCol("created_at")
+    age = PlainCol("age")
+    mountpoint = PlainCol("mountpoint")
+
+    def sort_url(self, col_key, reverse=False):
+        return url_for(
+            self.endpoint,
+            sort_key_volumes=col_key,
+            sort_direction_volumes="desc" if reverse else "asc",
+        )
+
+    @staticmethod
+    def html_from(endpoint, global_state, sort, reverse):
+        now = datetime.now(tz=tz.tzutc())
+
+        def dict_from(volume):
+            now_timestamp = now.timestamp()
+            created_timestamp = date_from(volume["CreatedAt"]).timestamp()
+
+            def coloured_ident(ident: str, formatter=lambda s: s) -> str:
+                is_expired, last_referenced, expiration_age = expired(
+                    ident, global_state, now_timestamp, created_timestamp
+                )
+                return (
+                    f"<div class='text-{'danger' if is_expired else 'success'}'>"
+                    f"{formatter(ident)} ({age_str(now, last_referenced)}/{age_str(expiration_age, 0)})"
+                    f"<a href=delete_volume?ident={ident}>del</a></div>"
+                )
+
+            return {
+                "name": coloured_ident(volume["Name"], formatter=lambda s: s[:12]),
+                "labels": "".join(map(coloured_ident, volume["Labels"] or [])),
+                "created_at": date_str(date_from(volume["CreatedAt"])),
+                "age": age_str(now, date_from(volume["CreatedAt"])),
+                "mountpoint": volume["Mountpoint"],
+            }
+
+        return VolumeTable(
+            endpoint,
+            items=sorted(
+                map(dict_from, global_state.volumes.values()),
+                key=lambda e: e[sort],
+                reverse=reverse,
+            ),
+        ).__html__()
+
+
+def meta_info(global_state: GlobalState):
     return {
         "refresh_interval": global_state.intervals.get("site_refresh", 10),
         "event_horizon": age_str(time.time(), global_state.event_horizon),
         "container_count": len(global_state.containers),
         "image_count": len(global_state.images),
+        "volume_count": len(global_state.volumes),
         "extra_links": global_state.extra_links,
-        "intervals": global_state.intervals,
+        "intervals": {key: dur_str(value) for key, value in global_state.intervals.items()},
+        "next_cleanup": dur_str(global_state.intervals["cleanup"] - global_state.cleanup_fuse),
         "hostname": global_state.hostname,
         "switches": global_state.switches,
-        "expiration_ages": global_state.expiration_ages,
+        "expiration_ages": {
+            key: dur_str(value) for key, value in global_state.expiration_ages.items()
+        },
         "self_pid": os.getpid(),
     }
 
 
-async def container_table_html(global_state):
+async def response_remove_image_ident(global_state: GlobalState):
+    docker = Docker()
+    try:
+        await remove_image_ident(global_state, docker, request.args.get("ident"))
+    except Exception as exc:
+        return f"Exception raised in remove_image_ident({request.args.get('ident')}): {exc}"
+    finally:
+        await docker.close()
+    return redirect(request.referrer or url_for("route_dashboard"))
+
+
+async def response_delete_container(global_state: GlobalState):
+    docker = Docker()
+    try:
+        await delete_container(global_state, docker, request.args.get("ident"))
+    except Exception as exc:
+        return f"Exception raised in remove_image_ident({request.args.get('ident')}): {exc}"
+    finally:
+        await docker.close()
+    return redirect(request.referrer or url_for("route_dashboard"))
+
+
+async def response_cleanup(global_state: GlobalState):
+    global_state.cleanup_fuse = global_state.intervals["cleanup"]
+    return redirect(request.referrer or url_for("route_dashboard"))
+
+
+async def response_rules(global_state):
+    return "no rules yet"
+
+
+async def response_messages(global_state):
+    return "no messages yet"
+
+
+async def response_volumes(global_state):
+    return await render_template(
+        "volumes.html",
+        meta=meta_info(global_state),
+        volumes_html=VolumeTable.html_from(
+            "route_volumes",
+            global_state,
+            sort=request.args.get("sort_key_volumes", "created_at"),
+            reverse=request.args.get("sort_direction_volumes", "desc") == "desc",
+        ),
+    )
+
+
+async def response_containers(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "containers.html",
         meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_containers",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
             reverse=request.args.get("sort_direction_containers", "desc") == "desc",
         ),
     )
 
 
-async def image_table_html(global_state):
+async def response_images(global_state):
     # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
     return await render_template(
         "images.html",
         meta=meta_info(global_state),
         images_html=ImageTable.html_from(
             "route_images",
             global_state,
             sort=request.args.get("sort_key_images", "created_at"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
     )
 
 
-async def dashboard(global_state):
+async def response_dashboard(global_state):
     return await render_template(
         "dashboard.html",
         meta=meta_info(global_state),
         containers_html=ContainerTable.html_from(
             "route_dashboard",
             global_state,
             sort=request.args.get("sort_key_containers", "cpu"),
@@ -593,17 +784,36 @@
             sort=request.args.get("sort_key_images", "created_at"),
             reverse=request.args.get("sort_direction_images", "asc") == "desc",
         ),
         messages=[(date_str(m[0]), m[1], m[2]) for m in global_state.messages],
     )
 
 
+async def container_table_html(global_state):
+    return await response_containers(global_state)
+
+
+async def image_table_html(global_state):
+    return await response_images(global_state)
+
+
+async def dashboard(global_state):
+    return await response_dashboard(global_state)
+
+
+# leftover - remove me after restarts
 async def generic_html(generic, global_state):
     if generic == "favicon.ico":
         return ""
+    if generic == "volumes":
+        return await response_volumes(global_state)
+    if generic == "rules":
+        return await response_rules(global_state)
+    if generic == "messages":
+        return await response_messages(global_state)
 
     raise RuntimeError(f"not found: {generic}")
 
 
 async def print_container_stats(global_state):
     hostname = open("/etc/hostname").read().strip()
     stats = [
@@ -684,15 +894,14 @@
         f" {''}"
         f" {'':>9}"
         f" {'':<60}"
         f" {''}"
     )
 
 
-@watchdog
 async def watch_container(container, global_state: GlobalState):
     name = "unknown"
     containers = global_state.containers
     try:
         container_info = containers[container.id]
         container_info["container"] = container
         container_info["short_id"] = (short_id_ := short_id(container.id))
@@ -708,51 +917,99 @@
         async for stats in container.stats():
             container_info["last_stats"] = container_info.get("stats", {})
             container_info["stats"] = stats
             container_info["show"] = await container.show()
 
     except DockerError as exc:
         log().error("DockerError: %s", exc)
+    except Exception:
+        log().exception("Unhandled exception in watch_container()")
     finally:
         log().info("<< container terminated: %s %s", short_id_, name)
-        del containers[container.id]
+        await unregister_container(container.id, global_state)
+
+
+async def unregister_image(global_state: GlobalState, image):
+    ident = image if isinstance(image, str) else image["Id"]
+    # todo? assert image_from() results None
+    if ident in global_state.images:
+        del global_state.images[ident]
+        await global_state.inform("refresh")
+
+
+async def register_image(global_state: GlobalState, image):
+    global_state.images[image["Id"]] = {
+        "short_id": short_id(image["Id"]),
+        "created_at": date_from(image["Created"]),
+        "tags": [tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"],
+        "size": image["Size"],
+        "parent": short_id(image.get("ParentId", "")),
+    }
+    await global_state.inform("refresh")
+
+
+async def update_image_registration(global_state: GlobalState, docker_client, image_id):
+    if image := await image_from(docker_client, image_id):
+        if image["Id"] in global_state.images:
+            global_state.images[image["Id"]]["tags"] = [
+                tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"
+            ]
+            await global_state.inform("refresh")
+        else:
+            await register_image(global_state, image)
+    else:
+        await unregister_image(global_state, image_id)
 
 
-async def watch_images(docker_client, global_state):
+async def watch_images(docker_client, global_state: GlobalState) -> None:
     # TODO: also use events to register
     log().info("crawl images..")
-    await asyncio.sleep(1)
-    # raise RuntimeError("XXX")
     for image in await docker_client.images.list(all=True):
-        # log().debug("  found image %s", image["Id"])
-        if True or image["Id"] not in global_state.images:
-            global_state.images.setdefault(image["Id"], {}).update(
-                {
-                    "short_id": short_id(image["Id"]),
-                    "created_at": image["Created"],
-                    "tags": [tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"],
-                    "size": image["Size"],
-                    "parent": short_id(image["ParentId"]),
-                }
-            )
+        if image["Id"] not in global_state.images:
+            log().warning("  found unregistered image %s", image["Id"])
+            await register_image(global_state, image)
+
+
+async def register_container(container, global_state: GlobalState) -> None:
+    log().debug("register container %s", container.id)
+    global_state.containers[container.id] = {}
+    asyncio.ensure_future(watch_container(container, global_state))
+    await global_state.inform("refresh")
 
 
-async def watch_containers(docker_client, global_state):
+async def unregister_container(ident, global_state: GlobalState) -> None:
+    try:
+        del global_state.containers[ident]
+        await global_state.inform("refresh")
+    except KeyError:
+        report(global_state, "error", f"tried to remove container {ident} unknown to registry")
+
+
+async def watch_containers(docker_client, global_state: GlobalState):
     # TODO: also use events to register
-    log().info("crawl containers..")
+    log().debug("crawl containers..")
     for container in await docker_client.containers.list(all=True):
-        log().debug("  found container %s", container.id)
         if container.id not in global_state.containers:
-            global_state.containers[container.id] = {}
+            log().debug("  found container %s", container.id)
+            if global_state.containers_crawled:
+                log().error("%s should have been registered automatically before!", container.id)
+            await register_container(container, global_state)
+    global_state.containers_crawled = True
 
-            asyncio.ensure_future(watch_container(container, global_state))
 
+async def watch_volumes(docker_client, global_state: GlobalState):
+    # TODO: also use events to register
+    log().info("crawl volumes..")
+    for volume in (await docker_client.volumes.list())["Volumes"]:
+        if volume["Name"] not in global_state.volumes:
+            log().debug("  found volume %s", volume)
+            global_state.volumes[volume["Name"]] = volume
 
-@impatient
-def would_cleanup_container(container, now: int, global_state):
+
+def would_cleanup_container(container, now: int, global_state: GlobalState):
     if "show" not in container:
         return False
     status = (show := container["show"])["State"]["Status"]
     if status == "exited":
         return (
             now - date_from(show["State"]["FinishedAt"]).timestamp()
             > global_state.expiration_ages["container_exited"]
@@ -768,152 +1025,180 @@
             > global_state.expiration_ages["container_running"]
         )
     return False
 
 
 def expired_idents(image, now, global_state: GlobalState):
     log().debug("check expiration for image %s, tags=%s", image["short_id"], image["tags"])
+
+    # todo: remove date_from
     created_timestamp = int(date_from(image["created_at"]).timestamp())
+
     for tag in image["tags"] or []:
         if expired(tag, global_state, now, created_timestamp)[0]:
             yield tag
-    if expired(image["short_id"], global_state, now, created_timestamp)[0]:
-        yield image["short_id"]
+
+    # only remove a container directly if there are no tags we could monitor
+    if not image["tags"]:
+        if expired(image["short_id"], global_state, now, created_timestamp)[0]:
+            yield image["short_id"]
 
 
 async def image_from(docker_client: Docker, ident: str) -> bool:
     with suppress(DockerError):
         return await docker_client.images.get(ident)
     return None
 
 
+async def container_from(docker_client: Docker, ident: str) -> bool:
+    with suppress(DockerError):
+        return await docker_client.containers.get(ident)
+    return None
+
+
+async def volume_from(docker_client: Docker, ident: str) -> bool:
+    with suppress(DockerError):
+        for volume in (await docker_client.volumes.list())["Volumes"]:
+            if volume["Name"].startswith(ident):
+                return volume
+    return None
+
+
+async def remove_image_ident(global_state: GlobalState, docker_client: Docker, ident: str) -> None:
+    report(global_state, "info", f"remove image/tag {ident}", None)
+    await docker_client.images.delete(ident)
+    await update_image_registration(global_state, docker_client, ident)
+
+
+async def delete_container(global_state: GlobalState, docker_client: Docker, container_ident):
+    container = (
+        await container_from(docker_client, container_ident)
+        if isinstance(container_ident, str)
+        else container_ident["container"]
+    )
+
+    report(
+        global_state,
+        "warn",
+        f"force removing container {short_id(container.id)}",
+        container,
+    )
+    await container.delete(force=True, v=True)
+
+    # Container should cleanup itself
+
+    if container := await container_from(docker_client, container_ident):
+        report(
+            global_state,
+            "error",
+            f"container {container_ident} still exists after deletion",
+            container,
+        )
+
+
 async def cleanup(docker_client: Docker, global_state):
     log().info("Cleanup!..")
 
-    report(global_state, "info", f"start cleanup", None)
+    report(global_state, "info", "start cleanup", None)
     try:
         now = int(datetime.now().timestamp())
         # we could go through docker_client.containers, too, but to be more consistent, we work
         # on one structure only
         # also, we have to create a list we can operate on, in order to not modify the structure, we're
         # iterating
         for container_info in list(
             filter(
                 lambda cnt: would_cleanup_container(cnt, now, global_state),
                 global_state.containers.values(),
             )
         ):
             if not global_state.switches.get("remove_container"):
-                log().info(f"skip removal of container {container_info['short_id']}")
+                log().info("skip removal of container %s", container_info["short_id"])
                 continue
-            report(
-                global_state,
-                "warn",
-                f"force removing container {container_info['short_id']}",
-                container_info["container"],
-            )
-            await container_info["container"].delete(force=True, v=True)
+            try:
+                await delete_container(global_state, docker_client, container_info)
+            except DockerError as exc:
+                log().error(
+                    "Could not delete container %s, error was %s", container_info["short_id"], exc
+                )
 
-        for image_info in global_state.images.values():
+        for image_info in list(global_state.images.values()):
             for ident in expired_idents(image_info, now, global_state):
                 if not global_state.switches.get("remove_images"):
-                    log().info(f"skip removal of image/tag {ident}")
+                    log().info("skip removal of image/tag %s", ident)
                     continue
-                report(global_state, "info", f"remove image/tag {ident}", None)
                 try:
-                    await docker_client.images.delete(ident)
+                    await remove_image_ident(global_state, docker_client, ident)
                 except DockerError as exc:
                     log().error("Could not delete image %s, error was %s", ident, exc)
 
         for ident in [
             ident for ident in global_state.images if not await image_from(docker_client, ident)
         ]:
-            log().warning("reference to image %s has not been cleaned up, I'll do it now..", ident)
-            del global_state.images[ident]
+            report(global_state, "warn", f"reference to image {ident} has not been cleaned up")
+            await unregister_image(global_state, ident)
+
+        for ident in [
+            ident
+            for ident in global_state.containers
+            if not await container_from(docker_client, ident)
+        ]:
+            report(global_state, "warn", f"reference to container {ident} has not been cleaned up")
+            del global_state.containers[ident]
+
+        for ident in [
+            ident for ident in global_state.volumes if not await volume_from(docker_client, ident)
+        ]:
+            report(global_state, "warn", f"reference to volume {ident} has not been cleaned up")
+            del global_state.volumes[ident]
     finally:
-        log().info("cleanup done!")
-        report(global_state, "info", f"cleanup done", None)
+        report(global_state, "info", "cleanup done", None)
 
 
-@impatient
-def report(global_state, msg_type, message: str, extra):
+def report(global_state, msg_type, message: str, extra=None):
+    """Report an incident - maybe good or bad"""
     # TODO: cleanup
     # TODO: persist
     log().info(message)
     global_state.messages.insert(0, (datetime.now().timestamp(), msg_type, message, str(extra)))
     global_state.messages = global_state.messages[
         : global_state.additional_values.get("message_history_size", 100)
     ]
 
 
-@impatient
 def reconfigure(global_state: GlobalState) -> None:
-    setup_introspection()
+    """Reacts on changes to the configuration, e.g. applies"""
     for ident, reference in global_state.last_referenced.items():
         reference[1] = expiration_age_from_ident(ident, global_state)
 
+    # todo
+    # global_state.inform("refresh")
 
-def increase_loglevel(*_):
-    """Become one level more verbose.
-    If level is already DEBUG we go back to WARNING.
-    """
-    try:
-        new_level = {
-            logging.WARNING: logging.INFO,
-            logging.INFO: logging.DEBUG,
-            logging.DEBUG: logging.WARNING,
-        }.get(log().level) or logging.INFO
-
-        log().setLevel(new_level)
-        logging.getLogger("docker-shaper.server").setLevel(new_level)
-        level = {
-            logging.CRITICAL: "CRITICAL",
-            logging.ERROR: "ERROR",
-            logging.WARNING: "WARNING",
-            logging.INFO: "INFO",
-            logging.DEBUG: "DEBUG",
-        }[new_level]
-        print(f"increase_loglevel to {level}", file=sys.stderr)
-    except Exception:
-        log().exception("Could not fully write application stack trace")
-
-
-def print_stacktrace_on_signal(sig, frame):
-    """interrupt running process, and provide a python prompt for
-    interactive debugging.
-    see http://stackoverflow.com/questions/132058
-       "showing-the-stack-trace-from-a-running-python-application"
-    """
-    try:
-        print(f"signal {sig} received - print stack trace", file=sys.stderr)
 
-        def print_stack_frame(stack_frame, file):
-            for _f in traceback.format_stack(stack_frame):
-                for _l in _f.splitlines():
-                    print(_l, file=file)
-
-        def print_stack_frames(file):
-            print("++++++ MAIN ++++++++", file=file)
-            print_stack_frame(frame, file)
-            for task in asyncio.all_tasks():
-                print(f"++++++ {task.get_coro().__name__} ++++++++", file=file)
-                for stack in task.get_stack(limit=1000):
-                    print_stack_frame(stack, file)
-
-        print_stack_frames(sys.stderr)
-        with open(Path("~/.docker_shaper/traceback.log").expanduser(), "w") as trace_file:
-            print_stack_frames(trace_file)
-    except Exception:
-        log().exception("Could not fully write application stack trace")
+def setup_introspection():
+    setup_introspection_on_signal()
 
 
-def setup_introspection():
-    """Install signal handlers for some debug stuff"""
+async def response_control_ws(global_state) -> None:
+    """Provides a way to talk with a connected client"""
+    # Only allow clients we know
+    # user_id = websocket.cookies.get("session")
+    # log().debug(f"/control({user_id})")
+    # if not user_id:
+    # websocket.close()
 
-    def setup_signal(sig, func, msg):
-        signal.signal(sig, func)
-        signal.siginterrupt(sig, False)
-        sig_str = {signal.SIGUSR1: "USR1", signal.SIGUSR2: "USR2"}.get(sig, sig)
-        print(f"Run `kill -{sig_str} {os.getpid()}` to {msg}", file=sys.stderr)
+    mqueue = global_state.new_update_queue()
+    await websocket.accept()
 
-    setup_signal(signal.SIGUSR1, increase_loglevel, "increase log level")
-    setup_signal(signal.SIGUSR2, print_stacktrace_on_signal, "print stacktrace")
+    try:
+        while True:
+            message = await mqueue.get()
+            await websocket.send(message)
+            reply = await websocket.receive()
+            log().debug("reply to '%s': '%s'", message, reply)
+    except asyncio.CancelledError:
+        raise
+    except Exception:
+        log().exception("Unhandled exception in control")
+    finally:
+        global_state.remove_queue(mqueue)
+        log().info("Connection closed")
```

### Comparing `docker_shaper-0.1.8/docker_shaper/templates/base.html` & `docker_shaper-0.1.9/docker_shaper/templates/base.html`

 * *Files 15% similar despite different names*

```diff
@@ -2,47 +2,62 @@
 <html>
   <head>
     <title>{{ title }}</title>
     <!--
     <link rel="stylesheet" href="{{ url_for('static', filename='normalize.css') }}">
     <link rel="stylesheet" href="{{ url_for('static', filename='style.css') }}">
     -->
-    <link rel="stylesheet" href="{{ url_for('static', filename='bootstrap.css') }}">
+    <link rel="stylesheet" href="{{ url_for('static', filename='bootstrap.min.css') }}">
     <meta http-equiv="refresh" content="{{ meta.refresh_interval }}" />
   </head>
 
   <body>
+
      <table class="table table-striped"><tr>
       <td>Host: <b>{{meta.hostname}}</b></td>
-      <td></td>
       {% for link in meta.extra_links %}
           <td><a href="{{ meta.extra_links[link] }}">{{link}}</a></td>
-          <td></td>
       {% endfor %}
-    </tr><tr>
+      <td></td>
+      <td></td>
+      <td></td>
+
+     </tr><tr>
 
       <td>configuration at <tt><b>~/.docker_shaper/config.py</b></tt></td>
+      <td>rotate log level: <tt>`<b>kill -USR1 {{meta.self_pid}}</b>`</tt></td>
       <td>backtrace: <tt>`<b>kill -USR2 {{meta.self_pid}}</b>`</tt></td>
+      <td></td>
+      <td></td>
+      <td></td>
+      <td></td>
 
-    </tr><tr>
+     </tr><tr>
+
+      <td><a href="/dashboard">Dashboard</a></td>
+      <td><a href="/containers">Containers</a></td>
+      <td><a href="/images">Images</a></td>
+      <td><a href="/volumes">Volumes</a></td>
+      <td><a href="/rules">Rules</a></td>
+      <td><a href="/messages">Messages</a></td>
+      <td></td>
+
+     </tr></table>
+
+     <table class="table table-striped"><tr>
       <td>intervals:</td>
 
       {% for interval in meta.intervals %}
-          <td>{{interval}} = <b>{{meta.intervals[interval]}}s</b>  </td><td></td>
+          <td>{{interval}} = <b>{{meta.intervals[interval]}}</b>  </td><td></td>
       {% endfor %}
 
-    </tr><tr>
-
-      <td><a href="/">Dashboard</a></td>
-      <td></td>
-      <td><a href="/containers">Containers</a></td>
-      <td></td>
-      <td><a href="/images">Images</a></td>
-
     </tr></table>
 
     <div class="dashboard">
       {% block content %}{% endblock %}
     </div>
 
   </body>
+
+  <script src="{{ url_for('static', filename='docker_shaper.js') }}"></script>
+
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
 
-Host: {{meta.hostname}}                                    {{link}}
-configuration at           backtrace: `kill -USR2 {
-~/.docker_shaper/config.py {meta.self_pid}}`
-intervals:                 {{interval}} = {{meta.intervals
-                           [interval]}}s
-Dashboard                                                  Containers  Images
+Host: {           {{link}}
+{meta.hostname}}
+configuration at  rotate log level: backtrace: `kill -
+~/.docker_shaper/ `kill -USR1 {     USR2 {
+config.py         {meta.self_pid}}` {meta.self_pid}}`
+Dashboard         Containers        Images             Volumes Rules Messages
+intervals: {{interval}} = {{meta.intervals[interval]}}
 {% block content %}{% endblock %}
```

### Comparing `docker_shaper-0.1.8/docker_shaper/templates/dashboard.html` & `docker_shaper-0.1.9/docker_shaper/templates/dashboard.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 {% extends "base.html" %}
 
 {% block content %}
 
   <table class="table table-striped">
     <tr>
-      <td>event_horizon (monitoring since)</td>
-      <td><b>{{meta.event_horizon}}</b></td>
-
+      <td>event_horizon (monitoring since): <b>{{meta.event_horizon}}</b></td>
+      <td>
+        <form method="post" action="cleanup" class="inline">
+          <!--
+          <input type="hidden" name="extra_submit_param" value="extra_submit_value">
+          -->
+          <button name="submit_param" value="submit_value">
+            Cleanup (automatic in {{meta.next_cleanup}})
+          </button>
+        </form>
+      </td>
+      <td></td>
+      <td></td>
+      <td></td>
+      <td></td>
     </tr><tr>
 
       <td>expiration ages:</td>
       {% for age in meta.expiration_ages %}
-          <td>{{age}} = <b>{{meta.expiration_ages[age]}}s</b>  </td><td></td>
+          <td>{{age}} = <b>{{meta.expiration_ages[age]}}</b>  </td>
       {% endfor %}
 
     </tr><tr>
 
       <td>switches:</td>
       {% for switch in meta.switches %}
           <td>{{switch}} = <b>{{meta.switches[switch]}}</b>  </td><td></td>
       {% endfor %}
+      <td></td>
 
     </tr>
   </table>
 
   <h2>containers ({{meta.container_count}})</h2>
   {{ containers_html|safe }}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends "base.html" %} {% block content %}
-event_horizon (monitoring since) {{meta.event_horizon}}
-expiration ages:                 {{age}} = {{meta.expiration_ages[age]}}s
-switches:                        {{switch}} = {{meta.switches[switch]}}
+event_horizon (monitoring since): {   Cleanup (automatic in {
+{meta.event_horizon}}               {meta.next_cleanup}})
+expiration ages:                    {{age}} = {{meta.expiration_ages[age]}}
+switches:                           {{switch}} = {{meta.switches[switch]}}
 ***** containers ({{meta.container_count}}) *****
 {{ containers_html|safe }}
 ***** images ({{meta.image_count}}) *****
 {{ images_html|safe }}
 ***** messages ({{messages|length}}) *****
 {{msg[0]}} {{msg[1]}} {{msg[2]}}
 {% endblock %}
```

### Comparing `docker_shaper-0.1.8/pyproject.toml` & `docker_shaper-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.8"
+version = "0.1.9"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
   {include = "docker_shaper/static"},
@@ -31,14 +31,15 @@
 mypy = "^1.2"
 pylint = "^2.15.3"
 ipython = "^8.8.0"
 types-pyyaml = "^6.0.12.6"
 twine = "^4.0.2"
 yamllint = "^1.29.0"
 pylint-per-file-ignores = "^1.2.1"
+types-python-dateutil = "^2.8.19.13"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
```

### Comparing `docker_shaper-0.1.8/PKG-INFO` & `docker_shaper-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-shaper
-Version: 0.1.8
+Version: 0.1.9
 Summary: Keeps Docker resources in shape based on rules and usage
 Home-page: https://github.com/Checkmk/checkmk-dev-tools
 Author: Frans Fürst
 Author-email: frans.fuerst@checkmk.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -47,26 +47,29 @@
 - [x] bring in dockermon
 - [x] auto update
 - [x] outsource config
 - [x] bring in dgcd
 - [x] new: untag certain tags
 - [x] new: container cleanup
 - [x] Fix `none` image lookup
-- [ ] Exceptions to messages
-- [ ] Clip / persist messages
+- [x] Exceptions to messages
+- [x] Clip
+- [x] Increase/decrease logging via web / signal
+- [x] Link: cleanup (images/containers) now
+- [x] Add volumes list (with recent owners)
+- [ ] Bring in `list_volumes` (volume monitoring)
+- [ ] Containers: show total CPU usage
+- [ ] Containers: list volumes
+- [ ] Volumes: list usage
+- [ ] Persist messages
 - [ ] Instructions to readme
 - [ ] List unmatched / overmatched tags
-- [ ] bring in `list_volumes` (volume monitoring)
-- [ ] Add volumes list (with recent owners)
-- [ ] Increase/decrease logging via web / signal
 - [ ] Links to `delete` / `remove`
 - [ ] Links to jobs
-- [ ] Skipable `wait`
 - [ ] Link: inspect
-- [ ] Link: cleanup (images/containers) now
 - [ ] Graph: cpu / containers (idle/up)
 - [ ] Authenticate (at least if we can modify behavior, like stopping/removing images/containers)
 
 
 ### Setup
```

