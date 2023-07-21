# Comparing `tmp/done-xblock-2.0.5.tar.gz` & `tmp/done-xblock-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "done-xblock-2.0.5.tar", last modified: Tue Nov 15 23:06:06 2022, max compression
+gzip compressed data, was "done-xblock-2.1.0.tar", last modified: Fri Jul 21 14:27:17 2023, max compression
```

## Comparing `done-xblock-2.0.5.tar` & `done-xblock-2.1.0.tar`

### file list

```diff
@@ -1,30 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    34500 2022-11-15 23:06:02.000000 done-xblock-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-11-15 23:06:02.000000 done-xblock-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-11-15 23:06:02.000000 done-xblock-2.0.5/NOTICE
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-11-15 23:06:06.096496 done-xblock-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4370 2022-11-15 23:06:02.000000 done-xblock-2.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/done/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-15 23:06:02.000000 done-xblock-2.0.5/done/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4567 2022-11-15 23:06:02.000000 done-xblock-2.0.5/done/done.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.092496 done-xblock-2.0.5/done/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/done/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2022-11-15 23:06:02.000000 done-xblock-2.0.5/done/static/css/done.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/done/static/html/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-11-15 23:06:02.000000 done-xblock-2.0.5/done/static/html/done.html
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-11-15 23:06:02.000000 done-xblock-2.0.5/done/static/html/studioview.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/done/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/done/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-11-15 23:06:02.000000 done-xblock-2.0.5/done/static/js/src/done.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/done_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5658 2022-11-15 23:06:06.000000 done-xblock-2.0.5/done_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-11-15 23:06:06.000000 done-xblock-2.0.5/done_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 23:06:06.000000 done-xblock-2.0.5/done_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-15 23:06:06.000000 done-xblock-2.0.5/done_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-15 23:06:06.000000 done-xblock-2.0.5/done_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-15 23:06:06.000000 done-xblock-2.0.5/done_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 23:06:06.096496 done-xblock-2.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-11-15 23:06:02.000000 done-xblock-2.0.5/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-11-15 23:06:02.000000 done-xblock-2.0.5/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 23:06:06.096496 done-xblock-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-11-15 23:06:02.000000 done-xblock-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-07-21 14:27:14.000000 done-xblock-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-07-21 14:27:14.000000 done-xblock-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-07-21 14:27:14.000000 done-xblock-2.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)     5658 2023-07-21 14:27:17.918882 done-xblock-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4370 2023-07-21 14:27:14.000000 done-xblock-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5022 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/done.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/public/
+-rw-r--r--   0 runner    (1001) docker     (122)      465 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/public/check-empty.png
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/public/check-full.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     2185 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/static/css/done.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.914882 done-xblock-2.1.0/done/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1496 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/static/js/src/done.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/done/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/templates/done.html
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-07-21 14:27:14.000000 done-xblock-2.1.0/done/templates/studioview.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/done_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5658 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-21 14:27:17.000000 done-xblock-2.1.0/done_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 14:27:17.918882 done-xblock-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-07-21 14:27:14.000000 done-xblock-2.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      565 2023-07-21 14:27:14.000000 done-xblock-2.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-21 14:27:17.918882 done-xblock-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4873 2023-07-21 14:27:14.000000 done-xblock-2.1.0/setup.py
```

### Comparing `done-xblock-2.0.5/LICENSE` & `done-xblock-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `done-xblock-2.0.5/NOTICE` & `done-xblock-2.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `done-xblock-2.0.5/PKG-INFO` & `done-xblock-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: done-xblock
-Version: 2.0.5
+Version: 2.1.0
 Summary: done XBlock
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ##########
         DoneXBlock
         ##########
         | |License: AGPL v3| |Status| |Python CI| |Publish package to PyPi|
```

### Comparing `done-xblock-2.0.5/README.rst` & `done-xblock-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `done-xblock-2.0.5/done/done.py` & `done-xblock-2.1.0/done/done.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,50 @@
 Show a toggle which lets students mark things as done.
 """
 
 
 import uuid
 
 import pkg_resources
+from web_fragments.fragment import Fragment
 from xblock.core import XBlock
 from xblock.fields import Boolean, DateTime, Float, Scope, String
-from web_fragments.fragment import Fragment
+from xblockutils.resources import ResourceLoader
+
+resource_loader = ResourceLoader(__name__)
+
+
+def _(text):
+    """
+    Make '_' a no-op, so we can scrape strings
+    """
+    return text
 
 
 def resource_string(path):
     """Handy helper for getting resources from our kit."""
     data = pkg_resources.resource_string(__name__, path)
     return data.decode("utf8")
 
 
+@XBlock.needs('i18n')
 class DoneXBlock(XBlock):
     """
     Show a toggle which lets students mark things as done.
     """
 
     done = Boolean(
         scope=Scope.user_state,
-        help="Is the student done?",
+        help=_("Is the student done?"),
         default=False
     )
 
     align = String(
         scope=Scope.settings,
-        help="Align left/right/center",
+        help=_("Align left/right/center"),
         default="left"
     )
 
     has_score = True
 
     # pylint: disable=unused-argument
     @XBlock.json_handler
@@ -59,37 +70,45 @@
         return {'state': self.done}
 
     def student_view(self, context=None):  # pylint: disable=unused-argument
         """
         The primary view of the DoneXBlock, shown to students
         when viewing courses.
         """
-        html_resource = resource_string("static/html/done.html")
-        html = html_resource.format(done=self.done,
-                                    id=uuid.uuid1(0))
+        frag = Fragment()
+        frag.add_content(resource_loader.render_django_template(
+            'templates/done.html',
+            {
+                'id': uuid.uuid1(0),
+                'done': self.done,
+            },
+            i18n_service=self.runtime.service(self, 'i18n')
+        ))
         (unchecked_png, checked_png) = (
             self.runtime.local_resource_url(self, x) for x in
             ('public/check-empty.png', 'public/check-full.png')
         )
-
-        frag = Fragment(html)
         frag.add_css(resource_string("static/css/done.css"))
         frag.add_javascript(resource_string("static/js/src/done.js"))
         frag.initialize_js("DoneXBlock", {'state': self.done,
                                           'unchecked': unchecked_png,
                                           'checked': checked_png,
                                           'align': self.align.lower()})
         return frag
 
     def studio_view(self, _context=None):
-        '''
+        """
         Minimal view with no configuration options giving some help text.
-        '''
-        html = resource_string("static/html/studioview.html")
-        frag = Fragment(html)
+        """
+        frag = Fragment()
+        frag.add_content(resource_loader.render_django_template(
+            'templates/studioview.html',
+            {},
+            i18n_service=self.runtime.service(self, 'i18n')
+        ))
         return frag
 
     @staticmethod
     def workbench_scenarios():
         """A canned scenario for display in the workbench."""
         return [
             ("DoneXBlock",
@@ -105,40 +124,42 @@
     # https://github.com/openedx/edx-ora2/blob/master/apps/openassessment/
     #        xblock/lms_mixin.py
     # It's needed to keep the LMS+Studio happy.
     # It should be included as a mixin.
 
     display_name = String(
         default="Completion", scope=Scope.settings,
-        help="Display name"
+        help=_("Display name")
     )
 
     start = DateTime(
         default=None, scope=Scope.settings,
-        help="ISO-8601 formatted string representing the start date "
-             "of this assignment. We ignore this."
+        help=_("ISO-8601 formatted string representing the start date of this assignment. We ignore this.")
     )
 
     due = DateTime(
         default=None, scope=Scope.settings,
-        help="ISO-8601 formatted string representing the due date "
-             "of this assignment. We ignore this."
+        help=_("ISO-8601 formatted string representing the due date of this assignment. We ignore this.")
     )
 
     weight = Float(
-        display_name="Problem Weight",
-        help=("Defines the number of points each problem is worth. "
-              "If the value is not set, the problem is worth the sum of the "
-              "option point values."),
+        display_name=_("Problem Weight"),
+        help=_(
+            "Defines the number of points each problem is worth. "
+            "If the value is not set, the problem is worth the sum of the "
+            "option point values."
+        ),
         values={"min": 0, "step": .1},
         scope=Scope.settings
     )
 
     def has_dynamic_children(self):
-        """Do we dynamically determine our children? No, we don't have any.
+        """
+        Do we dynamically determine our children? No, we don't have any.
         """
         return False
 
     def max_score(self):
-        """The maximum raw score of our problem.
+        """
+        The maximum raw score of our problem.
         """
         return 1
```

### Comparing `done-xblock-2.0.5/done/static/css/done.css` & `done-xblock-2.1.0/done/static/css/done.css`

 * *Files 12% similar despite different names*

```diff
@@ -4,118 +4,79 @@
     position:absolute;
     color:rgba(0,0,0,0);
     overflow:hidden;
     height:1px;
     width:1px;
 }
 
-.done_onoffswitch_wrapper {
-    display: flex;
-    flex-direction: row;
-    width: 100%;
+.done_onoffswitch, .done_onoffswitch-label, .done_onoffswitch-inner,  .done_onoffswitch-switch {
+    box-sizing: content-box;
 }
 
 .done_onoffswitch {
-    position: relative; width: 180px;
-    width: 180px;
+    display: inline-block;
     -webkit-user-select:none; -moz-user-select:none; -ms-user-select: none;
 }
 
 .done_onoffswitch-checkbox {
     display: none;
 }
 
 .done_onoffswitch-label {
     display: block; overflow: hidden; cursor: pointer;
     border: 2px solid #999999; border-radius: 10px;
+    height: 30px;
 }
 
 .done_onoffswitch-inner {
-    display: block; width: 200%; margin-left: -100%;
+    display: block;
 }
 
 .done_animated .done_onoffswitch-inner {
     -moz-transition: margin 0.1s ease-in 0s; -webkit-transition: margin 0.1s ease-in 0s;
     -o-transition: margin 0.1s ease-in 0s; transition: margin 0.1s ease-in 0s;
 }
 
-.done_onoffswitch-inner:before, .done_onoffswitch-inner:after {
-    display: block; float: left; width: 50%; height: 30px; padding: 0; line-height: 30px;
+.done_onoffswitch-inner .done_mark, .done_onoffswitch-inner .done_unmark {
+    display: block; height: 30px; padding: 0 10px; line-height: 30px;
     font-size: 14px; color: white; font-family: Trebuchet, Arial, sans-serif; font-weight: bold;
     -moz-box-sizing: border-box; -webkit-box-sizing: border-box; box-sizing: border-box;
+    text-indent: 18px;
 }
 
-.done_onoffswitch-inner:after {
-    content: "Mark as complete";
-    padding-left: 40px;
+.done_onoffswitch-inner .done_mark {
     background-color: rgb(0, 158, 231); color: #FFFFFF;
 }
-.done_onoffswitch-inner:before {
-    content: "Unmark";
-    padding-right: 100px;
+.done_onoffswitch-inner .done_unmark {
     background-color: #EEEEEE; color: #999999;
-    text-align: right;
 }
 
 .done_animated .done_onoffswitch-switch {
     -moz-transition: all 0.1s ease-in 0s; -webkit-transition: all 0.1s ease-in 0s;
-    -o-transition: all 0.1s ease-in 0s; transition: all 0.1s ease-in 0s; 
+    -o-transition: all 0.1s ease-in 0s; transition: all 0.1s ease-in 0s;
 }
 
 .done_onoffswitch-switch {
-    height: 18px;
-    display: block; width: 18px; margin: 6px 6px 6px 6px;
+    height: 17px;
+    display: block; width: 17px; margin: 4px;
     padding: -20px -20px -20px -20px;
     background-position: center;
     border: 2px solid #999999; border-radius: 20px;
-    position: absolute; top: 0; bottom: 0; right: 146px;
-    content: "X";
-    text-color:black;
+    position: absolute;
+    color:black;
 }
 
-.done_onoffswitch-checkbox:checked + .done_onoffswitch-label .done_onoffswitch-inner {
-    margin-left: 0;
+.done_onoffswitch-checkbox + .done_onoffswitch-label .done_onoffswitch-inner {
+    margin-top: -30px;
 }
 
-.done_onoffswitch-checkbox:checked + .done_onoffswitch-label .done_onoffswitch-switch {
-    right: 0px; 
+.done_onoffswitch-checkbox:checked + .done_onoffswitch-label .done_onoffswitch-inner {
+    margin-top: 0;
 }
 
 .done-checked {
     background-color: #018801;
 }
 
 .done-unchecked {
     background-color: #FFFFFF;
 }
-
-.done_grow {
-    flex-grow: 1;
-}
-
-.done_nogrow {
-    flex-grow: 0;
-}
-
-/* Right to left (rtl) language css */
-
-body.rtl .done_onoffswitch-checkbox:checked + .done_onoffswitch-label .done_onoffswitch-inner {
-    margin-right: 0;
-}
-body.rtl .done_onoffswitch-checkbox:checked + .done_onoffswitch-label .done_onoffswitch-switch {
-    right: 0px;
-}
-
-body.rtl .done_onoffswitch-inner {
-    margin-right: -100%;
-}
-
-body.rtl .done_onoffswitch-inner:before {
-    padding-right: 10px;
-    text-align: right;
-}
-
-body.rtl .done_onoffswitch-inner:after {
-    padding-left: 22px;
-    float: left;
-    text-align: left;
-}
```

### Comparing `done-xblock-2.0.5/done/static/html/done.html` & `done-xblock-2.1.0/done/templates/done.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+{% load i18n %}
+
 <div class="done_onoffswitch_wrapper">
   <div class="done_left_spacer"></div>
   <div class="done_onoffswitch">
-    <input type="checkbox" name="onoffswitch" class="done_onoffswitch-checkbox" id="{id}_myonoffswitch" checked="{done}">  </input>
-    <label class="done_onoffswitch-label" for="{id}_myonoffswitch">
-        <span class="done_aria_hidden">I have completed this</span>
-        <span class="done_onoffswitch-inner"></span>
-        <span class="done_onoffswitch-switch"></span>
+    <input type="checkbox" name="onoffswitch" class="done_onoffswitch-checkbox" id="{{id}}_myonoffswitch" checked="{{done}}">  </input>
+    <label class="done_onoffswitch-label" for="{{id}}_myonoffswitch">
+        <span class="done_onoffswitch-switch"><span class="done_aria_hidden">{% trans "X" %}</span></span>
+        <span class="done_aria_hidden">{% trans "I have completed this" %}</span>
+        <span class="done_onoffswitch-inner">
+            <span class="done_unmark">{% trans "Unmark" %}</span>
+            <span class="done_mark">{% trans "Mark as complete" %}</span>
+        </span>
     </label>
   </div>
   <div class="done_right_spacer"></div>
 </div>
```

### Comparing `done-xblock-2.0.5/done/static/js/src/done.js` & `done-xblock-2.1.0/done/static/js/src/done.js`

 * *Files identical despite different names*

### Comparing `done-xblock-2.0.5/done_xblock.egg-info/PKG-INFO` & `done-xblock-2.1.0/done_xblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: done-xblock
-Version: 2.0.5
+Version: 2.1.0
 Summary: done XBlock
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: ##########
         DoneXBlock
         ##########
         | |License: AGPL v3| |Status| |Python CI| |Publish package to PyPi|
```

### Comparing `done-xblock-2.0.5/requirements/constraints.txt` & `done-xblock-2.1.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `done-xblock-2.0.5/setup.py` & `done-xblock-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 import os
 import re
 
 from setuptools import setup
 
 
-def package_data(pkg, root):
+def package_data(pkg, root_list):
     """Generic function to find package_data for `pkg` under `root`."""
     data = []
-    for dirname, _, files in os.walk(os.path.join(pkg, root)):
-        for fname in files:
-            data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
+    for root in root_list:
+        for dirname, _, files in os.walk(os.path.join(pkg, root)):
+            for fname in files:
+                data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 def load_requirements(*requirements_paths):
     """
     Load all requirements from the specified requirements files.
@@ -116,11 +117,11 @@
     ],
     install_requires=load_requirements('requirements/base.in'),
     entry_points={
         'xblock.v1': [
             'done = done:DoneXBlock',
         ]
     },
-    package_data=package_data("done", "static"),
+    package_data=package_data("done", ["static", "templates", "public"]),
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

