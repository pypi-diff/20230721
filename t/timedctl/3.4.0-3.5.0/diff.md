# Comparing `tmp/timedctl-3.4.0.tar.gz` & `tmp/timedctl-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-3.4.0.tar", max compression
+gzip compressed data, was "timedctl-3.5.0.tar", max compression
```

## Comparing `timedctl-3.4.0.tar` & `timedctl-3.5.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    34454 2023-07-20 14:12:01.469729 timedctl-3.4.0/LICENSE
--rw-r--r--   0        0        0      810 2023-07-20 14:12:01.469729 timedctl-3.4.0/README.md
--rw-r--r--   0        0        0      849 2023-07-20 14:12:02.513759 timedctl-3.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 14:12:01.469729 timedctl-3.4.0/timedctl/__init__.py
--rwxr-xr-x   0        0        0    16670 2023-07-20 14:12:01.469729 timedctl-3.4.0/timedctl/timedctl.py
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-21 07:55:51.374431 timedctl-3.5.0/LICENSE
+-rw-r--r--   0        0        0      810 2023-07-21 07:55:51.374431 timedctl-3.5.0/README.md
+-rw-r--r--   0        0        0      849 2023-07-21 07:55:52.178449 timedctl-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-21 07:55:51.374431 timedctl-3.5.0/timedctl/__init__.py
+-rw-r--r--   0        0        0    36864 2023-07-21 07:55:51.374431 timedctl-3.5.0/timedctl/http_cache.sqlite
+-rwxr-xr-x   0        0        0    16931 2023-07-21 07:55:51.374431 timedctl-3.5.0/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 timedctl-3.5.0/PKG-INFO
```

### Comparing `timedctl-3.4.0/LICENSE` & `timedctl-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-3.4.0/README.md` & `timedctl-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-3.4.0/pyproject.toml` & `timedctl-3.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "timedctl"
-version = "3.4.0"
+version = "3.5.0"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "^0.2.1"
+libtimed = "^0.3.0"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 click-aliases = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `timedctl-3.4.0/timedctl/timedctl.py` & `timedctl-3.5.0/timedctl/timedctl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 """CLI application for libtimed."""
 
 import datetime
-import tomllib
 import os
 import re
 import sys
 
 import click
 import pyfzf
 import rich
 import terminaltables
+import tomllib
 from click_aliases import ClickAliasedGroup
-from tomlkit import dump
 from libtimed import TimedAPIClient
 from libtimed.oidc import OIDCClient
+from tomlkit import dump
 
 
 def load_config():
     """Load the timedctl config."""
     cfg = {
         "username": "test",
         "timed_url": "https://timed.example.com",
@@ -200,19 +200,20 @@
         {"date": date}, include="task,task.project,task.project.customer"
     )
     table = [["Customer", "Project", "Task", "Comment", "Duration"]]
     for report in reports:
         task_obj = report["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
-        project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"])
+        project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"], cached=True)
         project = project_obj["attributes"]["name"]
 
         customer_obj = timed.customers.get(
-            id=project_obj["relationships"]["customer"]["data"]["id"]
+            id=project_obj["relationships"]["customer"]["data"]["id"],
+            cached=True
         )
         customer = customer_obj["attributes"]["name"]
 
         table.append(
             [
                 customer,
                 project,
@@ -228,36 +229,38 @@
 
 
 @get.command("activities", aliases=["a", "ac", "activity"])
 @click.option("--date", default=None)
 def get_activities(date):
     """Get activities."""
     activities = timed.activities.get(
-        {"day": date}, include="task,task.project,task.project.customer",
+        {"day": date},
+        include="task,task.project,task.project.customer",
     )
     table = [["Activity", "Comment", "Start", "End"]]
-    for activity in activities:
-        task_obj = activity["relationships"]["task"]
+    for activity_obj in activities:
+        task_obj = activity_obj["relationships"]["task"]
         task = task_obj["attributes"]["name"]
 
-        project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"])
+        project_obj = timed.projects.get(id=task_obj["relationships"]["project"]["id"], cached=True)
         project = project_obj["attributes"]["name"]
 
         customer_obj = timed.customers.get(
-            id=project_obj["relationships"]["customer"]["data"]["id"]
+            id=project_obj["relationships"]["customer"]["data"]["id"],
+            cached=True
         )
         customer = customer_obj["attributes"]["name"]
 
         table.append(
             [
                 f"{customer} > {project} > {task}",
-                activity["attributes"]["comment"],
-                activity["attributes"]["from-time"].strftime("%H:%M:%S"),
-                activity["attributes"]["to-time"].strftime("%H:%M:%S")
-                if activity["attributes"]["to-time"] is not None
+                activity_obj["attributes"]["comment"],
+                activity_obj["attributes"]["from-time"].strftime("%H:%M:%S"),
+                activity_obj["attributes"]["to-time"].strftime("%H:%M:%S")
+                if activity_obj["attributes"]["to-time"] is not None
                 else "active",
             ]
         )
     output = terminaltables.SingleTable(table)
     msg(f"Activities for {date if date is not None else 'today'}:")
     click.echo(output.table)
 
@@ -311,39 +314,39 @@
 
 @add.command("report", aliases=["r"])
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 @click.option("--description", default=None)
 @click.option("--duration", default=None)
-def add_report(customer, project, task, description, duration):
+def add_report(customer, project, task, description, duration):  # pylint: disable=R0912
     """Add report(s)."""
-    customers = timed.customers.get()
+    customers = timed.customers.get(cached=True)
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
     if customer:
         customer = [c for c in customers if c["attributes"]["name"] == customer]
         if len(customer) == 0:
             error_handler("ERR_CUSTOMER_NOT_FOUND")
         customer = customer[0]
     else:
         customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
-    projects = timed.projects.get({"customer": customer["id"]})
+    projects = timed.projects.get({"customer": customer["id"]}, cached=True)
     # select a project
     if project:
         project = [p for p in projects if p["attributes"]["name"] == project]
         if len(project) == 0:
             error_handler("ERR_PROJECT_NOT_FOUND")
         project = project[0]
     else:
         project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
-    tasks = timed.tasks.get({"project": project["id"]})
+    tasks = timed.tasks.get({"project": project["id"]}, cached=True)
     # select a task
     if task:
         task = [t for t in tasks if t["attributes"]["name"] == task]
         if len(task) == 0:
             error_handler("ERR_TASK_NOT_FOUND")
         task = task[0]
     else:
@@ -435,37 +438,37 @@
 @activity.command(aliases=["add", "s"])
 @click.argument("comment")
 @click.option("--customer", default=None)
 @click.option("--project", default=None)
 @click.option("--task", default=None)
 def start(comment, customer, project, task):
     """Start recording activity."""
-    customers = timed.customers.get()
+    customers = timed.customers.get(cached=True)
     # ask the user to select a customer
     msg("Select a customer")
     # select a customer
     if customer:
         customer = [c for c in customers if c["attributes"]["name"] == customer]
         if len(customer) == 0:
             error_handler("ERR_CUSTOMER_NOT_FOUND")
         customer = customer[0]
     else:
         customer = fzf_wrapper(customers, ["attributes", "name"], "Select a customer: ")
     # get projects
-    projects = timed.projects.get({"customer": customer["id"]})
+    projects = timed.projects.get({"customer": customer["id"]}, cached=True)
     # select a project
     if project:
         project = [p for p in projects if p["attributes"]["name"] == project]
         if len(project) == 0:
             error_handler("ERR_PROJECT_NOT_FOUND")
         project = project[0]
     else:
         project = fzf_wrapper(projects, ["attributes", "name"], "Select a project: ")
     # get tasks
-    tasks = timed.tasks.get({"project": project["id"]})
+    tasks = timed.tasks.get({"project": project["id"]}, cached=True)
     # select a task
     if task:
         task = [t for t in tasks if t["attributes"]["name"] == task]
         if len(task) == 0:
             error_handler("ERR_TASK_NOT_FOUND")
         task = task[0]
     else:
@@ -478,58 +481,59 @@
     if res.status_code == 201:
         msg(f"Activity {comment} started successfully.")
         return
     # handle exception
     error_handler("ERR_ACTIVITY_START_FAILED")
 
 
-@activity.command()
-def stop(aliases=["end", "finish"]):
+@activity.command(aliases=["end", "finish"])
+def stop():
     """Stop current activity."""
     if not timed.activities.current:
         error_handler("ERR_NO_CURRENT_ACTIVITY")
     else:
         timed.activities.stop()
     msg("Activity stopped successfully.")
 
 
-@activity.command()
-def show(aliases=["s", "get", "info"]):
+@activity.command(aliases=["s", "get", "info"])
+def show():
     """Show current activity."""
     current_activity = timed.activities.current
     if current_activity:
         msg(
-            f"Current activity: {current_activity['attributes']['comment']} (Since {current_activity['attributes']['from-time'].strftime('%H:%M:%S')})"
+            f"Current activity: {current_activity['attributes']['comment']} (Since "
+            + f"{current_activity['attributes']['from-time'].strftime('%H:%M:%S')})"
         )
     else:
         error_handler("ERR_NO_CURRENT_ACTIVITY")
 
 
 @activity.command(aliases=["gts", "ts"])
 def generate_timesheet():
     """Generate the timesheet of the current activities."""
     activities = timed.activities.get()
     if activities:
-        for activity in activities:
-            if not activity["attributes"]["transferred"]:
-                if not activity["attributes"]["to-time"]:
-                    activity["attributes"]["to-time"] = datetime.datetime.now()
-                from_time = activity["attributes"]["from-time"]
-                to_time = activity["attributes"]["to-time"]
+        for activity_obj in activities:
+            if not activity_obj["attributes"]["transferred"]:
+                if not activity_obj["attributes"]["to-time"]:
+                    activity_obj["attributes"]["to-time"] = datetime.datetime.now()
+                from_time = activity_obj["attributes"]["from-time"]
+                to_time = activity_obj["attributes"]["to-time"]
                 duration = to_time - from_time
-                task = activity["relationships"]["task"]["data"]["id"]
+                task = activity_obj["relationships"]["task"]["data"]["id"]
                 timed.reports.post(
                     {
                         "duration": duration,
-                        "comment": activity["attributes"]["comment"],
+                        "comment": activity_obj["attributes"]["comment"],
                     },
                     {"task": task},
                 )
                 timed.activities.patch(
-                    activity["id"], {"transferred": True}, {"task": task}
+                    activity_obj["id"], {"transferred": True}, {"task": task}
                 )
         msg("Timesheet generated successfully.")
     else:
         error_handler("ERR_NO_ACTIVITIES")
 
 
 if __name__ == "__main__":
```

### Comparing `timedctl-3.4.0/PKG-INFO` & `timedctl-3.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 3.4.0
+Version: 3.5.0
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
-Requires-Dist: libtimed (>=0.2.1,<0.3.0)
+Requires-Dist: libtimed (>=0.3.0,<0.4.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

