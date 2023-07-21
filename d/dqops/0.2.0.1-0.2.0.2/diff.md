# Comparing `tmp/dqops-0.2.0.1.tar.gz` & `tmp/dqops-0.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqops-0.2.0.1.tar", last modified: Thu May 11 11:49:31 2023, max compression
+gzip compressed data, was "dqops-0.2.0.2.tar", last modified: Fri Jul 21 17:09:05 2023, max compression
```

## Comparing `dqops-0.2.0.1.tar` & `dqops-0.2.0.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 11:49:31.445331 dqops-0.2.0.1/
--rw-rw-rw-   0        0        0    11554 2022-05-05 14:08:06.000000 dqops-0.2.0.1/LICENSE
--rw-rw-rw-   0        0        0     4822 2023-05-11 11:49:31.446476 dqops-0.2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3301 2023-05-11 10:17:32.000000 dqops-0.2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 11:49:31.378549 dqops-0.2.0.1/dqops/
--rw-rw-rw-   0        0        0      799 2023-05-11 10:17:32.000000 dqops-0.2.0.1/dqops/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-05-11 10:17:32.000000 dqops-0.2.0.1/dqops/install.py
--rw-rw-rw-   0        0        0     2923 2023-05-11 11:48:41.000000 dqops-0.2.0.1/dqops/startdqo.py
--rw-rw-rw-   0        0        0      974 2023-05-11 11:48:41.000000 dqops-0.2.0.1/dqops/version.py
-drwxrwxrwx   0        0        0        0 2023-05-11 11:49:31.442850 dqops-0.2.0.1/dqops.egg-info/
--rw-rw-rw-   0        0        0     4822 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-11 11:49:31.000000 dqops-0.2.0.1/dqops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      168 2022-05-05 14:08:06.000000 dqops-0.2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      118 2023-05-11 11:49:31.460195 dqops-0.2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     6154 2023-05-11 10:17:32.000000 dqops-0.2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:09:05.184929 dqops-0.2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 17:02:57.000000 dqops-0.2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-21 17:09:05.184929 dqops-0.2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-07-21 17:02:57.000000 dqops-0.2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:09:05.184929 dqops-0.2.0.2/dqops/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/startdqo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-21 17:02:57.000000 dqops-0.2.0.2/dqops/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 17:09:05.184929 dqops-0.2.0.2/dqops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 17:09:05.000000 dqops-0.2.0.2/dqops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-21 17:02:57.000000 dqops-0.2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 17:09:05.184929 dqops-0.2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-07-21 17:02:57.000000 dqops-0.2.0.2/setup.py
```

### Comparing `dqops-0.2.0.1/LICENSE` & `dqops-0.2.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [2022] [Documati Sp. z o.o.]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2022] [Documati Sp. z o.o.]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `dqops-0.2.0.1/dqops/__init__.py` & `dqops-0.2.0.2/dqops/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one or more
-# contributor license agreements.  See the NOTICE file distributed with
-# this work for additional information regarding copyright ownership.
-# The ASF licenses this file to You under the Apache License, Version 2.0
-# (the "License"); you may not use this file except in compliance with
-# the License.  You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
+#
+# Licensed to the Apache Software Foundation (ASF) under one or more
+# contributor license agreements.  See the NOTICE file distributed with
+# this work for additional information regarding copyright ownership.
+# The ASF licenses this file to You under the Apache License, Version 2.0
+# (the "License"); you may not use this file except in compliance with
+# the License.  You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
```

### Comparing `dqops-0.2.0.1/dqops/startdqo.py` & `dqops-0.2.0.2/dqops/startdqo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one or more
-# contributor license agreements.  See the NOTICE file distributed with
-# this work for additional information regarding copyright ownership.
-# The ASF licenses this file to You under the Apache License, Version 2.0
-# (the "License"); you may not use this file except in compliance with
-# the License.  You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-import os
-import sys
-import subprocess
-
-from dqops import install
-
-# ignore those, they are filled by importing version.py
-VERSION = "filled by dqops/version.py"
-PIP_VERSION = "filled by dqops/version.py"
-GITHUB_RELEASE = "filled by dqops/version.py"
-JAVA_VERSION = "filled by dqops/version.py"
-
-try:
-    exec(open(os.path.join(os.path.dirname(os.path.realpath(__file__)), 'version.py')).read())
-except IOError:
-    print("Failed to load DQO version file.", file=sys.stderr)
-    sys.exit(-1)
-
-
-def main():
-    module_dir = os.path.dirname(os.path.realpath(__file__))
-
-    dqo_home = os.environ.get("DQO_HOME")
-    if dqo_home is None:
-        dqo_home = os.path.join(os.path.join(module_dir, 'home'), VERSION)
-        install.install_dqo_home_if_missing(dqo_home)
-
-    # TODO: detect if the user has Java 17 or newer on the JAVA_HOME, we can use it
-    java_install_dir = os.path.join(module_dir, 'jre' + JAVA_VERSION)
-    install.install_jre_if_missing(java_install_dir)
-    java_home = os.path.join(java_install_dir, os.listdir(java_install_dir)[0])
-
-    if os.path.exists(os.path.join(java_home, 'Contents/Home')):
-        java_home = os.path.join(java_home, 'Contents/Home')  # support MacOS correctly
-
-    os_platform = sys.platform.lower()[0:3]
-    dqo_envs = os.environ.copy()
-    dqo_envs['DQO_HOME'] = dqo_home
-    dqo_envs['JAVA_HOME'] = java_home
-    dqo_envs['DQO_PYTHON_INTERPRETER'] = sys.executable
-
-    if os_platform == 'win':
-        # Windows
-        subprocess.call([os.path.join(dqo_home, 'bin/dqo.cmd')] + sys.argv[1:], env=dqo_envs)
-    elif os_platform == 'lin' or os_platform == 'dar':
-        # Linux (lin) or MacOS X (dar)
-        dqo_path = os.path.join(dqo_home, 'bin/dqo')
-        if os.access(dqo_path, os.X_OK):
-            subprocess.call([dqo_path] + sys.argv[1:], env=dqo_envs)
-        else:
-            subprocess.call(['/bin/sh', dqo_path] + sys.argv[1:], env=dqo_envs)
-    else:
-        print("Operating system {0} unsupported".format(sys.platform), file=sys.stderr)
-        sys.exit(-1)
-
-
-if __name__ == "__main__":
-    main()
+#
+# Licensed to the Apache Software Foundation (ASF) under one or more
+# contributor license agreements.  See the NOTICE file distributed with
+# this work for additional information regarding copyright ownership.
+# The ASF licenses this file to You under the Apache License, Version 2.0
+# (the "License"); you may not use this file except in compliance with
+# the License.  You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+import os
+import subprocess
+import sys
+
+from dqops import install
+
+# ignore those, they are filled by importing version.py
+VERSION = "filled by dqops/version.py"
+PIP_VERSION = "filled by dqops/version.py"
+GITHUB_RELEASE = "filled by dqops/version.py"
+JAVA_VERSION = "filled by dqops/version.py"
+
+try:
+    exec(
+        open(
+            os.path.join(os.path.dirname(os.path.realpath(__file__)), "version.py")
+        ).read()
+    )
+except IOError:
+    print("Failed to load DQO version file.", file=sys.stderr)
+    sys.exit(-1)
+
+
+def main():
+    module_dir = os.path.dirname(os.path.realpath(__file__))
+
+    dqo_home = os.environ.get("DQO_HOME")
+    if dqo_home is None:
+        dqo_home = os.path.join(os.path.join(module_dir, "home"), VERSION)
+        install.install_dqo_home_if_missing(dqo_home)
+
+    # TODO: detect if the user has Java 17 or newer on the JAVA_HOME, we can use it
+    java_install_dir = os.path.join(module_dir, "jre" + JAVA_VERSION)
+    install.install_jre_if_missing(java_install_dir)
+    java_home = os.path.join(java_install_dir, os.listdir(java_install_dir)[0])
+
+    if os.path.exists(os.path.join(java_home, "Contents/Home")):
+        java_home = os.path.join(java_home, "Contents/Home")  # support MacOS correctly
+
+    os_platform = sys.platform.lower()[0:3]
+    dqo_envs = os.environ.copy()
+    dqo_envs["DQO_HOME"] = dqo_home
+    dqo_envs["JAVA_HOME"] = java_home
+    dqo_envs["DQO_PYTHON_INTERPRETER"] = sys.executable
+    dqo_envs["DQO_PYTHON_USE_HOST_PYTHON"] = "true"
+
+    if os_platform == "win":
+        # Windows
+        subprocess.call(
+            [os.path.join(dqo_home, "bin/dqo.cmd")] + sys.argv[1:], env=dqo_envs
+        )
+    elif os_platform == "lin" or os_platform == "dar":
+        # Linux (lin) or MacOS X (dar)
+        dqo_path = os.path.join(dqo_home, "bin/dqo")
+        if os.access(dqo_path, os.X_OK):
+            subprocess.call([dqo_path] + sys.argv[1:], env=dqo_envs)
+        else:
+            subprocess.call(["/bin/sh", dqo_path] + sys.argv[1:], env=dqo_envs)
+    else:
+        print("Operating system {0} unsupported".format(sys.platform), file=sys.stderr)
+        sys.exit(-1)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `dqops-0.2.0.1/dqops/version.py` & `dqops-0.2.0.2/dqops/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-#
-# Licensed to the Apache Software Foundation (ASF) under one or more
-# contributor license agreements.  See the NOTICE file distributed with
-# this work for additional information regarding copyright ownership.
-# The ASF licenses this file to You under the Apache License, Version 2.0
-# (the "License"); you may not use this file except in compliance with
-# the License.  You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limit
-
-VERSION = "0.2.0-alpha0"
-PIP_VERSION = "0.2.0.1"
-GITHUB_RELEASE = "v" + VERSION + ""
-JAVA_VERSION = "17"
-
-
-def get_dqo_version():
-    return VERSION, PIP_VERSION, GITHUB_RELEASE, JAVA_VERSION
+#
+# Licensed to the Apache Software Foundation (ASF) under one or more
+# contributor license agreements.  See the NOTICE file distributed with
+# this work for additional information regarding copyright ownership.
+# The ASF licenses this file to You under the Apache License, Version 2.0
+# (the "License"); you may not use this file except in compliance with
+# the License.  You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limit
+
+# WARNING: the next two lines with the version numbers (VERSION =, PIP_VERSION =) should not be modified manually. They are changed by a maven profile at compile time.
+VERSION = "0.2.0-beta2"
+PIP_VERSION = "0.2.0.2"
+GITHUB_RELEASE = "v" + VERSION + ""
+JAVA_VERSION = "17"
+
+
+def get_dqo_version():
+    return VERSION, PIP_VERSION, GITHUB_RELEASE, JAVA_VERSION
```

### Comparing `dqops-0.2.0.1/setup.py` & `dqops-0.2.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,159 +1,169 @@
-#!/usr/bin/env python3
-
-#
-# Licensed to the Apache Software Foundation (ASF) under one or more
-# contributor license agreements.  See the NOTICE file distributed with
-# this work for additional information regarding copyright ownership.
-# The ASF licenses this file to You under the Apache License, Version 2.0
-# (the "License"); you may not use this file except in compliance with
-# the License.  You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-from glob import glob
-import os
-import sys
-import zipfile
-import jdk
-from setuptools import setup
-import importlib.util
-from setuptools.command.install import install
-from shutil import rmtree
-
-# ignore those, they are filled by importing dqops/version.py
-VERSION = "filled by dqops/version.py"
-PIP_VERSION = "filled by dqops/version.py"
-GITHUB_RELEASE = "filled by dqops/version.py"
-JAVA_VERSION = "filled by dqops/version.py"
-
-
-HOME_PATH = "dqops/home"
-JRE_PATH = "dqops/jre"
-DQO_REPO_HOME = os.path.abspath("../../")
-
-try:
-    exec(open('dqops/version.py').read())
-except IOError:
-    print("Failed to load DQO.ai version file for packaging. You must be in dqops' distribution/python dir.",
-          file=sys.stderr)
-    sys.exit(-1)
-
-try:
-    download_module_spec = importlib.util.spec_from_file_location("install", "dqops/install.py")
-    download_module = importlib.util.module_from_spec(download_module_spec)
-    download_module_spec.loader.exec_module(download_module)
-except IOError:
-    print("Failed to load the download module (dqops/install.py) which had to be packaged together.",
-          file=sys.stderr)
-    sys.exit(-1)
-
-# Provide guidance about how to use setup.py
-incorrect_invocation_message = """
-If you are installing DQO from https://github.com/dqops/dqo source, you must first build DQO.
-
-    To build DQO with maven, go to the https://github.com/dqops/dqo root folder and run run:
-      ./mvnw -DskipTests clean package"""
-
-# Figure out where the distribution file is present
-DISTRIBUTION_PATH = os.path.join(DQO_REPO_HOME, "distribution/target/dqo-distribution-{0}-bin.zip".format(VERSION))
-
-in_dqo = os.path.isfile(os.path.join(DQO_REPO_HOME, "pom.xml")) and \
-         os.path.isfile(os.path.join(DQO_REPO_HOME, "dqoai/src/main/java/ai/dqo/cli/CliApplication.java"))
-
-
-class InstallCommand(install):
-    def run(self):
-        install.run(self)
-
-        # download and install DQO
-        if not in_dqo:
-            download_module.install_dqo(HOME_PATH, GITHUB_RELEASE, VERSION)
-
-        os.makedirs(JRE_PATH, exist_ok=True)
-
-        # install a local JRE
-        print("Installing Java JRE %s at %s" % (JAVA_VERSION, JRE_PATH))
-        jdk.install(JAVA_VERSION, jre=True, path=JRE_PATH)
-
-try:
-    if in_dqo:
-        # Create a folder to expand the distribution
-        try:
-            os.mkdir(HOME_PATH)
-        except:
-            print("Cannot create {0}".format(HOME_PATH), file=sys.stderr)
-            sys.exit(-1)
-
-        if not os.path.isfile(DISTRIBUTION_PATH) and not os.path.exists(HOME_PATH):
-            print(incorrect_invocation_message, file=sys.stderr)
-            sys.exit(-1)
-
-        with zipfile.ZipFile(DISTRIBUTION_PATH, "r") as zip_ref:
-            zip_ref.extractall(HOME_PATH)
-
-    with open('README.md') as f:
-        long_description = f.read()
-
-#    home_dirs = [root[len("dqops/"):].replace('\\', '/') + "/*" for (root, dirs, files) in os.walk(HOME_PATH)]
-
-    setup(
-        name='dqops',
-        version=PIP_VERSION,
-        description='DQO Data Quality Operations Center',
-        long_description=long_description,
-        long_description_content_type="text/markdown",
-        author='DQO Developers',
-        author_email='support@dqo.ai',
-        url='https://github.com/dqops/dqo/tree/master/distribution/python',
-        packages=['dqops'],
-#        include_package_data=True,
-        package_dir={
-            'dqops': 'dqops'
-        },
-        # package_data={
-        #     'dqops': home_dirs
-        # },
-        license='http://www.apache.org/licenses/LICENSE-2.0',
-        install_requires=['install-jdk==0.3.0'],
-        python_requires='>=3.6',
-        classifiers=[
-#            'Development Status :: 5 - Production/Stable',
-            'Development Status :: 4 - Beta',
-            'License :: OSI Approved :: Apache Software License',
-            'Programming Language :: Python :: 3.8',
-            'Programming Language :: Python :: 3.9',
-            'Programming Language :: Python :: 3.10',
-            'Programming Language :: Python :: 3.11',
-            'Environment :: Console',
-#            'Framework :: Apache Airflow :: Provider',
-            'Intended Audience :: Developers',
-            'Operating System :: Microsoft :: Windows',
-            'Operating System :: MacOS',
-            'Operating System :: POSIX :: Linux',
-            'Programming Language :: Java',
-            'Programming Language :: SQL',
-            'Topic :: Database',
-            'Topic :: Scientific/Engineering :: Artificial Intelligence',
-            'Topic :: Scientific/Engineering :: Information Analysis',
-            'Topic :: Security',
-            'Topic :: Software Development :: Quality Assurance',
-            'Topic :: Software Development :: Testing',
-            'Topic :: Software Development :: Version Control :: Git',
-            'Programming Language :: Python :: Implementation :: CPython',
-            'Programming Language :: Python :: Implementation :: PyPy'],
-        # cmdclass={
-        #     'install': InstallCommand,
-        # },
-        entry_points={
-            'console_scripts': ['dqo=dqops.startdqo:main'],
-        },
-    )
-finally:
-    if in_dqo:
-        rmtree(HOME_PATH)
+#!/usr/bin/env python3
+
+#
+# Licensed to the Apache Software Foundation (ASF) under one or more
+# contributor license agreements.  See the NOTICE file distributed with
+# this work for additional information regarding copyright ownership.
+# The ASF licenses this file to You under the Apache License, Version 2.0
+# (the "License"); you may not use this file except in compliance with
+# the License.  You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
+from glob import glob
+import os
+import sys
+import zipfile
+import jdk
+from setuptools import setup
+import importlib.util
+from setuptools.command.install import install
+from shutil import rmtree
+
+# ignore those, they are filled by importing dqops/version.py
+VERSION = "filled by dqops/version.py"
+PIP_VERSION = "filled by dqops/version.py"
+GITHUB_RELEASE = "filled by dqops/version.py"
+JAVA_VERSION = "filled by dqops/version.py"
+
+
+HOME_PATH = "dqops/home"
+JRE_PATH = "dqops/jre"
+DQO_REPO_HOME = os.path.abspath("../../")
+
+try:
+    exec(open('dqops/version.py').read())
+except IOError:
+    print("Failed to load DQOps version file for packaging. You must be in dqops' distribution/python dir.",
+          file=sys.stderr)
+    sys.exit(-1)
+
+try:
+    download_module_spec = importlib.util.spec_from_file_location("install", "dqops/install.py")
+    download_module = importlib.util.module_from_spec(download_module_spec)
+    download_module_spec.loader.exec_module(download_module)
+except IOError:
+    print("Failed to load the download module (dqops/install.py) which had to be packaged together.",
+          file=sys.stderr)
+    sys.exit(-1)
+
+# Provide guidance about how to use setup.py
+incorrect_invocation_message = """
+If you are installing DQO from https://github.com/dqops/dqo source, you must first build DQO.
+
+    To build DQO with maven, go to the https://github.com/dqops/dqo root folder and run run:
+      ./mvnw -DskipTests clean package"""
+
+# Figure out where the distribution file is present
+DISTRIBUTION_PATH = os.path.join(DQO_REPO_HOME, "distribution/target/dqo-distribution-{0}-bin.zip".format(VERSION))
+
+in_dqo = os.path.isfile(os.path.join(DQO_REPO_HOME, "pom.xml")) and \
+         os.path.isfile(os.path.join(DQO_REPO_HOME, "dqops/src/main/java/com/dqops/cli/CliApplication.java"))
+
+
+class InstallCommand(install):
+    def run(self):
+        install.run(self)
+
+        # download and install DQO
+        if not in_dqo:
+            download_module.install_dqo(HOME_PATH, GITHUB_RELEASE, VERSION)
+
+        os.makedirs(JRE_PATH, exist_ok=True)
+
+        # install a local JRE
+        print("Installing Java JRE %s at %s" % (JAVA_VERSION, JRE_PATH))
+        jdk.install(JAVA_VERSION, jre=True, path=JRE_PATH)
+
+try:
+    if in_dqo:
+        # Create a folder to expand the distribution
+        try:
+            os.mkdir(HOME_PATH)
+        except:
+            print("Cannot create {0}".format(HOME_PATH), file=sys.stderr)
+            sys.exit(-1)
+
+        if not os.path.isfile(DISTRIBUTION_PATH) and not os.path.exists(HOME_PATH):
+            print(incorrect_invocation_message, file=sys.stderr)
+            sys.exit(-1)
+
+        with zipfile.ZipFile(DISTRIBUTION_PATH, "r") as zip_ref:
+            zip_ref.extractall(HOME_PATH)
+
+    with open('README.md') as f:
+        long_description = f.read()
+
+#    home_dirs = [root[len("dqops/"):].replace('\\', '/') + "/*" for (root, dirs, files) in os.walk(HOME_PATH)]
+
+    setup(
+        name='dqops',
+        version=PIP_VERSION,
+        description='DQO Data Quality Operations Center',
+        long_description=long_description,
+        long_description_content_type="text/markdown",
+        author='DQO Developers',
+        author_email='support@dqops.com',
+        url='https://github.com/dqops/dqo/tree/master/distribution/python',
+        packages=['dqops'],
+        include_package_data=True,
+        package_dir={
+            'dqops': 'dqops'
+        },
+        package_data={
+            'dqops': ['py.typed']
+        },
+        license='http://www.apache.org/licenses/LICENSE-2.0',
+        install_requires=['install-jdk>=1.0.4',
+                          'httpx>=0.15.4,<0.25.0',
+                          'attrs>=21.3.0',
+                          'python-dateutil>=2.8.2',
+                          'numpy>=1.24.3',
+                          'MarkupSafe>=2.1.1',
+                          'Jinja2>=3.0.3',
+                          'six>=1.16.0',
+                          'pandas>=2.0.1',
+                          'scipy>=1.10.1'],
+        python_requires='>=3.8',
+        classifiers=[
+#            'Development Status :: 5 - Production/Stable',
+            'Development Status :: 4 - Beta',
+            'License :: OSI Approved :: Apache Software License',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
+            'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
+            'Programming Language :: Python :: 3.12',
+            'Environment :: Console',
+#            'Framework :: Apache Airflow :: Provider',
+            'Intended Audience :: Developers',
+            'Operating System :: Microsoft :: Windows',
+            'Operating System :: MacOS',
+            'Operating System :: POSIX :: Linux',
+            'Programming Language :: Java',
+            'Programming Language :: SQL',
+            'Topic :: Database',
+            'Topic :: Scientific/Engineering :: Artificial Intelligence',
+            'Topic :: Scientific/Engineering :: Information Analysis',
+            'Topic :: Security',
+            'Topic :: Software Development :: Quality Assurance',
+            'Topic :: Software Development :: Testing',
+            'Topic :: Software Development :: Version Control :: Git',
+            'Programming Language :: Python :: Implementation :: CPython',
+            'Programming Language :: Python :: Implementation :: PyPy'],
+        # cmdclass={
+        #     'install': InstallCommand,
+        # },
+        entry_points={
+            'console_scripts': ['dqo=dqops.startdqo:main'],
+        },
+    )
+finally:
+    if in_dqo:
+        rmtree(HOME_PATH)
```

