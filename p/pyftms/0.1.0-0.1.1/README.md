# Comparing `tmp/pyftms-0.1.0.tar.gz` & `tmp/pyftms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftms-0.1.0.tar", max compression
+gzip compressed data, was "pyftms-0.1.1.tar", max compression
```

## Comparing `pyftms-0.1.0.tar` & `pyftms-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11575 2024-05-26 16:19:33.202192 pyftms-0.1.0/LICENSE
--rw-r--r--   0        0        0      754 2024-05-26 07:30:56.482324 pyftms-0.1.0/pyftms/__init__.py
--rw-r--r--   0        0        0      982 2024-05-26 05:28:44.694757 pyftms-0.1.0/pyftms/__main__.py
--rw-r--r--   0        0        0     1891 2024-05-26 07:27:30.178817 pyftms-0.1.0/pyftms/client/__init__.py
--rw-r--r--   0        0        0      381 2024-05-26 06:38:22.551314 pyftms-0.1.0/pyftms/client/backends/__init__.py
--rw-r--r--   0        0        0     8494 2024-05-26 07:27:30.244928 pyftms-0.1.0/pyftms/client/backends/controller.py
--rw-r--r--   0        0        0     3180 2024-05-26 07:27:30.193436 pyftms-0.1.0/pyftms/client/backends/event.py
--rw-r--r--   0        0        0     2134 2024-05-26 06:44:00.924620 pyftms-0.1.0/pyftms/client/backends/updater.py
--rw-r--r--   0        0        0     8808 2024-05-26 07:27:30.239735 pyftms-0.1.0/pyftms/client/client.py
--rw-r--r--   0        0        0     5009 2024-05-26 05:28:44.695758 pyftms-0.1.0/pyftms/client/const.py
--rw-r--r--   0        0        0      905 2024-05-26 05:28:44.695758 pyftms-0.1.0/pyftms/client/machines/__init__.py
--rw-r--r--   0        0        0      584 2024-05-26 05:28:44.695758 pyftms-0.1.0/pyftms/client/machines/cross_trainer.py
--rw-r--r--   0        0        0      543 2024-05-26 05:28:44.696756 pyftms-0.1.0/pyftms/client/machines/indoor_bike.py
--rw-r--r--   0        0        0      509 2024-05-26 05:28:44.696756 pyftms-0.1.0/pyftms/client/machines/rower.py
--rw-r--r--   0        0        0      520 2024-05-26 05:28:44.696756 pyftms-0.1.0/pyftms/client/machines/treadmill.py
--rw-r--r--   0        0        0     6831 2024-05-26 06:39:05.516204 pyftms-0.1.0/pyftms/client/manager.py
--rw-r--r--   0        0        0      716 2024-05-26 07:27:30.160798 pyftms-0.1.0/pyftms/client/properties/__init__.py
--rw-r--r--   0        0        0     1109 2024-05-26 06:51:23.780209 pyftms-0.1.0/pyftms/client/properties/device_info.py
--rw-r--r--   0        0        0     5962 2024-05-26 07:27:30.209485 pyftms-0.1.0/pyftms/client/properties/features.py
--rw-r--r--   0        0        0     2040 2024-05-26 05:28:44.697755 pyftms-0.1.0/pyftms/client/properties/machine_type.py
--rw-r--r--   0        0        0     1281 2024-05-26 07:27:30.167307 pyftms-0.1.0/pyftms/models/__init__.py
--rw-r--r--   0        0        0     2565 2024-05-26 05:28:44.697755 pyftms-0.1.0/pyftms/models/common.py
--rw-r--r--   0        0        0     9837 2024-05-26 07:27:30.263505 pyftms-0.1.0/pyftms/models/control_point.py
--rw-r--r--   0        0        0     6703 2024-05-26 07:27:30.246925 pyftms-0.1.0/pyftms/models/machine_status.py
--rw-r--r--   0        0        0      502 2024-05-26 05:28:44.697755 pyftms-0.1.0/pyftms/models/realtime_data/__init__.py
--rw-r--r--   0        0        0     2954 2024-05-26 05:28:44.698758 pyftms-0.1.0/pyftms/models/realtime_data/common.py
--rw-r--r--   0        0        0     3212 2024-05-26 07:27:30.208484 pyftms-0.1.0/pyftms/models/realtime_data/cross_trainer.py
--rw-r--r--   0        0        0     2431 2024-05-26 05:28:44.698758 pyftms-0.1.0/pyftms/models/realtime_data/indoor_bike.py
--rw-r--r--   0        0        0     3112 2024-05-26 05:28:44.698758 pyftms-0.1.0/pyftms/models/realtime_data/rower.py
--rw-r--r--   0        0        0     2829 2024-05-26 07:27:30.210561 pyftms-0.1.0/pyftms/models/realtime_data/treadmill.py
--rw-r--r--   0        0        0     1319 2024-05-26 05:28:44.698758 pyftms-0.1.0/pyftms/models/spin_down.py
--rw-r--r--   0        0        0     2272 2024-05-26 05:28:44.698758 pyftms-0.1.0/pyftms/models/training_status.py
--rw-r--r--   0        0        0      435 2024-05-26 07:27:30.165303 pyftms-0.1.0/pyftms/serializer/__init__.py
--rw-r--r--   0        0        0      809 2024-05-26 05:28:44.699756 pyftms-0.1.0/pyftms/serializer/list.py
--rw-r--r--   0        0        0     7617 2024-05-26 07:27:30.261506 pyftms-0.1.0/pyftms/serializer/model.py
--rw-r--r--   0        0        0     2157 2024-05-26 05:28:44.699756 pyftms-0.1.0/pyftms/serializer/num.py
--rw-r--r--   0        0        0      619 2024-05-26 05:28:44.699756 pyftms-0.1.0/pyftms/serializer/serializer.py
--rw-r--r--   0        0        0      371 2024-05-26 16:30:56.484859 pyftms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1524 2024-05-26 16:19:42.747923 pyftms-0.1.0/README.md
--rw-r--r--   0        0        0     1910 1970-01-01 00:00:00.000000 pyftms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11374 2024-05-28 12:37:45.517955 pyftms-0.1.1/LICENSE
+-rw-r--r--   0        0        0      861 2024-05-28 12:37:45.517955 pyftms-0.1.1/README.md
+-rw-r--r--   0        0        0     1604 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/__main__.py
+-rw-r--r--   0        0        0     3627 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/__init__.py
+-rw-r--r--   0        0        0     8214 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/controller.py
+-rw-r--r--   0        0        0     5876 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/event.py
+-rw-r--r--   0        0        0     2039 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/backends/updater.py
+-rw-r--r--   0        0        0    11059 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/client.py
+-rw-r--r--   0        0        0     4841 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/const.py
+-rw-r--r--   0        0        0      867 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/cross_trainer.py
+-rw-r--r--   0        0        0      576 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/indoor_bike.py
+-rw-r--r--   0        0        0      542 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/rower.py
+-rw-r--r--   0        0        0      553 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/machines/treadmill.py
+-rw-r--r--   0        0        0    10036 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/manager.py
+-rw-r--r--   0        0        0      685 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/__init__.py
+-rw-r--r--   0        0        0     1063 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/device_info.py
+-rw-r--r--   0        0        0     5826 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/features.py
+-rw-r--r--   0        0        0     2448 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/client/properties/machine_type.py
+-rw-r--r--   0        0        0     1117 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/__init__.py
+-rw-r--r--   0        0        0     2530 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/common.py
+-rw-r--r--   0        0        0     8956 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/control_point.py
+-rw-r--r--   0        0        0     6442 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/machine_status.py
+-rw-r--r--   0        0        0      374 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/__init__.py
+-rw-r--r--   0        0        0     2823 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/common.py
+-rw-r--r--   0        0        0     3075 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/cross_trainer.py
+-rw-r--r--   0        0        0     2324 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/indoor_bike.py
+-rw-r--r--   0        0        0     2973 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/rower.py
+-rw-r--r--   0        0        0     2701 2024-05-28 12:37:45.517955 pyftms-0.1.1/pyftms/models/realtime_data/treadmill.py
+-rw-r--r--   0        0        0     1255 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/models/spin_down.py
+-rw-r--r--   0        0        0     2168 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/models/training_status.py
+-rw-r--r--   0        0        0      471 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/list.py
+-rw-r--r--   0        0        0     7662 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/model.py
+-rw-r--r--   0        0        0     2080 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/num.py
+-rw-r--r--   0        0        0      594 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyftms/serializer/serializer.py
+-rw-r--r--   0        0        0      480 2024-05-28 12:37:45.521955 pyftms-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 pyftms-0.1.1/PKG-INFO
```

### Comparing `pyftms-0.1.0/LICENSE` & `pyftms-0.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
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
-   Copyright 2024 Sergey V. DUDANOV <sergey.dudanov@gmail.com>
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
-   limitations under the License.
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
+   Copyright 2024 Sergey V. DUDANOV <sergey.dudanov@gmail.com>
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
+   limitations under the License.
```

### Comparing `pyftms-0.1.0/pyftms/client/backends/controller.py` & `pyftms-0.1.1/pyftms/client/backends/controller.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import asyncio
-import io
-import logging
-from typing import cast
-
-from bleak import BleakClient
-from bleak.backends.characteristic import BleakGATTCharacteristic
-from bleak.exc import BleakError
-
-from ...models import (
-    CodeSwitchModel,
-    ControlCode,
-    ControlIndicateModel,
-    ControlModel,
-    MachineStatusCode,
-    MachineStatusModel,
-    ResultCode,
-    SpinDownSpeedData,
-    StopPauseCode,
-    TrainingStatusFlags,
-    TrainingStatusModel,
-)
-from ..const import (
-    FITNESS_MACHINE_CONTROL_POINT_UUID,
-    FITNESS_MACHINE_STATUS_UUID,
-    PAUSE,
-    STOP,
-    TRAINING_STATUS_UUID,
-)
-from .event import (
-    ControlEvent,
-    FtmsCallback,
-    SetupEvent,
-    SetupEventData,
-    SpinDownEvent,
-    SpinDownEventData,
-    TrainingStatusEvent,
-    TrainingStatusEventData,
-)
-
-_LOGGER = logging.getLogger(__name__)
-
-
-def _to_setup_event_data(model: CodeSwitchModel) -> SetupEventData:
-    result = model._asdict(nested=True)
-
-    result.pop("code")
-
-    if not result:
-        return {}
-
-    assert len(result) == 1
-
-    k, v = next(iter(result.items()))
-
-    # Handle 'target_time_x'
-    if k[-1].isdecimal():
-        k = k[:-2]
-
-    return cast(SetupEventData, {k: v})  # unsafe cast
-
-
-def _simple_status_events(m: MachineStatusModel) -> ControlEvent | None:
-    match m.code:
-        case MachineStatusCode.RESET:
-            return ControlEvent(event_id="reset", event_source="other")
-
-        case MachineStatusCode.STOP_PAUSE:
-            value = STOP if StopPauseCode(m.stop_pause) == StopPauseCode.STOP else PAUSE
-            return ControlEvent(event_id=value, event_source="user")
-
-        case MachineStatusCode.STOP_SAFETY:
-            return ControlEvent(event_id="stop", event_source="safety")
-
-        case MachineStatusCode.START_RESUME:
-            return ControlEvent(event_id="start", event_source="user")
-
-
-def _simple_control_events(m: ControlModel) -> ControlEvent | None:
-    """Handle simple control requests after success operation indication"""
-    match m.code:
-        case ControlCode.RESET:
-            return ControlEvent(event_id="reset", event_source="callback")
-
-        case ControlCode.STOP_PAUSE:
-            value = STOP if StopPauseCode(m.stop_pause) == StopPauseCode.STOP else PAUSE
-            return ControlEvent(event_id=value, event_source="callback")
-
-        case ControlCode.START_RESUME:
-            return ControlEvent(event_id="start", event_source="callback")
-
-
-class MachineController:
-    def __init__(self, callback: FtmsCallback) -> None:
-        self._indicate: asyncio.Future[bytes]
-        self._subscribed = False
-        self._auth = False
-        self._cb = callback
-
-    async def subscribe(self, cli: BleakClient) -> None:
-        """Subscribe for available notifications."""
-        if self._subscribed:
-            return
-
-        if c := cli.services.get_characteristic(TRAINING_STATUS_UUID):
-            await cli.start_notify(c, self._on_training_status)
-
-        if c := cli.services.get_characteristic(FITNESS_MACHINE_STATUS_UUID):
-            await cli.start_notify(c, self._on_machine_status)
-
-        if c := cli.services.get_characteristic(FITNESS_MACHINE_CONTROL_POINT_UUID):
-            await cli.start_notify(c, self._on_indicate)
-
-        self._subscribed = True
-
-    async def unsubscribe(self, cli: BleakClient) -> None:
-        """Unubscribe from available notifications."""
-        if not self._subscribed:
-            return
-
-        if c := cli.services.get_characteristic(FITNESS_MACHINE_CONTROL_POINT_UUID):
-            await cli.stop_notify(c)
-
-        if c := cli.services.get_characteristic(FITNESS_MACHINE_STATUS_UUID):
-            await cli.stop_notify(c)
-
-        if c := cli.services.get_characteristic(TRAINING_STATUS_UUID):
-            await cli.stop_notify(c)
-
-        self._subscribed = False
-
-    def reset(self):
-        """Resetting state. Call while disconnection event."""
-        self._subscribed = False
-        self._auth = False
-
-    def _on_indicate(self, c: BleakGATTCharacteristic, data: bytes) -> None:
-        """Control indication callback."""
-        if not self._indicate.done():
-            self._indicate.set_result(data)
-
-    async def write_command(
-        self,
-        cli: BleakClient,
-        code: ControlCode | None = None,
-        *,
-        timeout: float = 2.0,
-        **kwargs,
-    ) -> ResultCode:
-        """Writing command to control point."""
-        # Auto-Request control
-        if not self._auth and code != ControlCode.REQUEST_CONTROL:
-            await self.write_command(
-                cli,
-                ControlCode.REQUEST_CONTROL,
-                timeout=timeout,
-            )
-
-        bio = io.BytesIO()
-
-        request = ControlModel(code=code, **kwargs)
-        request._serialize(bio)
-
-        # Write to control point
-
-        await self.subscribe(cli)
-        self._indicate = asyncio.Future()
-
-        try:
-            _, resp = await asyncio.wait_for(
-                asyncio.gather(
-                    cli.write_gatt_char(
-                        FITNESS_MACHINE_CONTROL_POINT_UUID,
-                        bio.getvalue(),
-                        True,
-                    ),
-                    self._indicate,
-                ),
-                timeout=timeout,
-            )
-        except BleakError:
-            self.reset()
-            raise
-
-        bio = io.BytesIO(resp)
-
-        indicate = ControlIndicateModel._deserialize(bio)
-
-        if indicate.request_code != request.code:
-            raise ValueError("Response on another request?..")
-
-        if indicate.result_code != ResultCode.SUCCESS:
-            return indicate.result_code
-
-        if request.code == ControlCode.RESET:
-            self._auth = False
-
-        elif request.code == ControlCode.REQUEST_CONTROL:
-            self._auth = True
-
-            return ResultCode.SUCCESS
-
-        elif request.spin_down is not None:
-            data = SpinDownEventData(code=request.spin_down)
-
-            s = SpinDownSpeedData._get_serializer()
-
-            if speed_bytes := bio.read(s.get_size()):
-                data["target_speed"] = s.deserialize(speed_bytes)
-
-            assert not bio.read(1)
-
-            event = SpinDownEvent(event_id="spin_down", event_data=data)
-
-            self._cb(event)
-
-            return ResultCode.SUCCESS
-
-        # Writing is success. Firing events and update settings data.
-
-        if event := _simple_control_events(request):
-            # reset, start, stop, pause handled
-            self._cb(event)
-
-            return ResultCode.SUCCESS
-
-        # Handling setup requests with parameters
-
-        event = SetupEvent(
-            event_id="setup",
-            event_data=_to_setup_event_data(request),
-            event_source="callback",
-        )
-
-        self._cb(event)
-
-        return ResultCode.SUCCESS
-
-    def _on_machine_status(self, c: BleakGATTCharacteristic, data: bytearray) -> None:
-        """Machine Status notification callback."""
-        bio = io.BytesIO(data)
-        status = MachineStatusModel._deserialize(bio)
-
-        # Handle loosing control
-        if status.code == MachineStatusCode.LOST_CONTROL:
-            self._auth = False
-            return
-
-        if status.code == MachineStatusCode.RESET:
-            self._auth = False
-
-        if p := _simple_status_events(status):
-            # reset, start, stop (and safety), pause handled
-            return self._cb(p)
-
-        event = SetupEvent(
-            event_id="setup",
-            event_data=_to_setup_event_data(status),
-            event_source="other",
-        )
-
-        self._cb(event)
-
-    def _on_training_status(self, c: BleakGATTCharacteristic, data: bytearray) -> None:
-        """Training Status notification callback."""
-        bio = io.BytesIO(data)
-        status = TrainingStatusModel._deserialize(bio)
-
-        status_data = TrainingStatusEventData(code=status.code)
-
-        if TrainingStatusFlags.STRING_PRESENT in status.flags:
-            if b := bio.read():
-                status_data["string"] = b.decode(encoding="utf-8")
-
-        event = TrainingStatusEvent(event_id="training_status", event_data=status_data)
-
-        self._cb(event)
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import asyncio
+import io
+import logging
+from typing import cast
+
+from bleak import BleakClient
+from bleak.backends.characteristic import BleakGATTCharacteristic
+from bleak.exc import BleakError
+
+from ...models import (
+    CodeSwitchModel,
+    ControlCode,
+    ControlIndicateModel,
+    ControlModel,
+    MachineStatusCode,
+    MachineStatusModel,
+    ResultCode,
+    SpinDownSpeedData,
+    StopPauseCode,
+    TrainingStatusFlags,
+    TrainingStatusModel,
+)
+from ..const import (
+    FITNESS_MACHINE_CONTROL_POINT_UUID,
+    FITNESS_MACHINE_STATUS_UUID,
+    PAUSE,
+    STOP,
+    TRAINING_STATUS_UUID,
+)
+from .event import (
+    ControlEvent,
+    FtmsCallback,
+    SetupEvent,
+    SetupEventData,
+    SpinDownEvent,
+    SpinDownEventData,
+    TrainingStatusEvent,
+    TrainingStatusEventData,
+)
+
+_LOGGER = logging.getLogger(__name__)
+
+
+def _to_setup_event_data(model: CodeSwitchModel) -> SetupEventData:
+    result = model._asdict(nested=True)
+
+    result.pop("code")
+
+    if not result:
+        return {}
+
+    assert len(result) == 1
+
+    k, v = next(iter(result.items()))
+
+    # Handle 'target_time_x'
+    if k[-1].isdecimal():
+        k = k[:-2]
+
+    return cast(SetupEventData, {k: v})  # unsafe cast
+
+
+def _simple_status_events(m: MachineStatusModel) -> ControlEvent | None:
+    match m.code:
+        case MachineStatusCode.RESET:
+            return ControlEvent(event_id="reset", event_source="other")
+
+        case MachineStatusCode.STOP_PAUSE:
+            value = STOP if StopPauseCode(m.stop_pause) == StopPauseCode.STOP else PAUSE
+            return ControlEvent(event_id=value, event_source="user")
+
+        case MachineStatusCode.STOP_SAFETY:
+            return ControlEvent(event_id="stop", event_source="safety")
+
+        case MachineStatusCode.START_RESUME:
+            return ControlEvent(event_id="start", event_source="user")
+
+
+def _simple_control_events(m: ControlModel) -> ControlEvent | None:
+    """Handle simple control requests after success operation indication"""
+    match m.code:
+        case ControlCode.RESET:
+            return ControlEvent(event_id="reset", event_source="callback")
+
+        case ControlCode.STOP_PAUSE:
+            value = STOP if StopPauseCode(m.stop_pause) == StopPauseCode.STOP else PAUSE
+            return ControlEvent(event_id=value, event_source="callback")
+
+        case ControlCode.START_RESUME:
+            return ControlEvent(event_id="start", event_source="callback")
+
+
+class MachineController:
+    def __init__(self, callback: FtmsCallback) -> None:
+        self._indicate: asyncio.Future[bytes]
+        self._subscribed = False
+        self._auth = False
+        self._cb = callback
+
+    async def subscribe(self, cli: BleakClient) -> None:
+        """Subscribe for available notifications."""
+        if self._subscribed:
+            return
+
+        if c := cli.services.get_characteristic(TRAINING_STATUS_UUID):
+            await cli.start_notify(c, self._on_training_status)
+
+        if c := cli.services.get_characteristic(FITNESS_MACHINE_STATUS_UUID):
+            await cli.start_notify(c, self._on_machine_status)
+
+        if c := cli.services.get_characteristic(FITNESS_MACHINE_CONTROL_POINT_UUID):
+            await cli.start_notify(c, self._on_indicate)
+
+        self._subscribed = True
+
+    async def unsubscribe(self, cli: BleakClient) -> None:
+        """Unubscribe from available notifications."""
+        if not self._subscribed:
+            return
+
+        if c := cli.services.get_characteristic(FITNESS_MACHINE_CONTROL_POINT_UUID):
+            await cli.stop_notify(c)
+
+        if c := cli.services.get_characteristic(FITNESS_MACHINE_STATUS_UUID):
+            await cli.stop_notify(c)
+
+        if c := cli.services.get_characteristic(TRAINING_STATUS_UUID):
+            await cli.stop_notify(c)
+
+        self._subscribed = False
+
+    def reset(self):
+        """Resetting state. Call while disconnection event."""
+        self._subscribed = False
+        self._auth = False
+
+    def _on_indicate(self, c: BleakGATTCharacteristic, data: bytes) -> None:
+        """Control indication callback."""
+        if not self._indicate.done():
+            self._indicate.set_result(data)
+
+    async def write_command(
+        self,
+        cli: BleakClient,
+        code: ControlCode | None = None,
+        *,
+        timeout: float = 2.0,
+        **kwargs,
+    ) -> ResultCode:
+        """Writing command to control point."""
+        # Auto-Request control
+        if not self._auth and code != ControlCode.REQUEST_CONTROL:
+            await self.write_command(
+                cli,
+                ControlCode.REQUEST_CONTROL,
+                timeout=timeout,
+            )
+
+        bio = io.BytesIO()
+
+        request = ControlModel(code=code, **kwargs)
+        request._serialize(bio)
+
+        # Write to control point
+
+        await self.subscribe(cli)
+        self._indicate = asyncio.Future()
+
+        try:
+            _, resp = await asyncio.wait_for(
+                asyncio.gather(
+                    cli.write_gatt_char(
+                        FITNESS_MACHINE_CONTROL_POINT_UUID,
+                        bio.getvalue(),
+                        True,
+                    ),
+                    self._indicate,
+                ),
+                timeout=timeout,
+            )
+        except BleakError:
+            self.reset()
+            raise
+
+        bio = io.BytesIO(resp)
+
+        indicate = ControlIndicateModel._deserialize(bio)
+
+        if indicate.request_code != request.code:
+            raise ValueError("Response on another request?..")
+
+        if indicate.result_code != ResultCode.SUCCESS:
+            return indicate.result_code
+
+        if request.code == ControlCode.RESET:
+            self._auth = False
+
+        elif request.code == ControlCode.REQUEST_CONTROL:
+            self._auth = True
+
+            return ResultCode.SUCCESS
+
+        elif request.spin_down is not None:
+            data = SpinDownEventData(code=request.spin_down)
+
+            s = SpinDownSpeedData._get_serializer()
+
+            if speed_bytes := bio.read(s.get_size()):
+                data["target_speed"] = s.deserialize(speed_bytes)
+
+            assert not bio.read(1)
+
+            event = SpinDownEvent(event_id="spin_down", event_data=data)
+
+            self._cb(event)
+
+            return ResultCode.SUCCESS
+
+        # Writing is success. Firing events and update settings data.
+
+        if event := _simple_control_events(request):
+            # reset, start, stop, pause handled
+            self._cb(event)
+
+            return ResultCode.SUCCESS
+
+        # Handling setup requests with parameters
+
+        event = SetupEvent(
+            event_id="setup",
+            event_data=_to_setup_event_data(request),
+            event_source="callback",
+        )
+
+        self._cb(event)
+
+        return ResultCode.SUCCESS
+
+    def _on_machine_status(self, c: BleakGATTCharacteristic, data: bytearray) -> None:
+        """Machine Status notification callback."""
+        bio = io.BytesIO(data)
+        status = MachineStatusModel._deserialize(bio)
+
+        # Handle loosing control
+        if status.code == MachineStatusCode.LOST_CONTROL:
+            self._auth = False
+            return
+
+        if status.code == MachineStatusCode.RESET:
+            self._auth = False
+
+        if p := _simple_status_events(status):
+            # reset, start, stop (and safety), pause handled
+            return self._cb(p)
+
+        event = SetupEvent(
+            event_id="setup",
+            event_data=_to_setup_event_data(status),
+            event_source="other",
+        )
+
+        self._cb(event)
+
+    def _on_training_status(self, c: BleakGATTCharacteristic, data: bytearray) -> None:
+        """Training Status notification callback."""
+        bio = io.BytesIO(data)
+        status = TrainingStatusModel._deserialize(bio)
+
+        status_data = TrainingStatusEventData(code=status.code)
+
+        if TrainingStatusFlags.STRING_PRESENT in status.flags:
+            if b := bio.read():
+                status_data["string"] = b.decode(encoding="utf-8")
+
+        event = TrainingStatusEvent(event_id="training_status", event_data=status_data)
+
+        self._cb(event)
```

### Comparing `pyftms-0.1.0/pyftms/client/const.py` & `pyftms-0.1.1/pyftms/client/const.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-# REAL-TIME TRAINING DATA
-
-CADENCE_AVERAGE = "cadence_average"
-CADENCE_INSTANT = "cadence_instant"
-DISTANCE_TOTAL = "distance_total"
-ELEVATION_GAIN_NEGATIVE = "elevation_gain_negative"
-ELEVATION_GAIN_POSITIVE = "elevation_gain_positive"
-ENERGY_PER_HOUR = "energy_per_hour"
-ENERGY_PER_MINUTE = "energy_per_minute"
-ENERGY_TOTAL = "energy_total"
-FORCE_ON_BELT = "force_on_belt"
-HEART_RATE = "heart_rate"
-INCLINATION = "inclination"
-METABOLIC_EQUIVALENT = "metabolic_equivalent"
-MOVEMENT_DIRECTION = "movement_direction"
-PACE_AVERAGE = "pace_average"
-PACE_INSTANT = "pace_instant"
-POWER_AVERAGE = "power_average"
-POWER_INSTANT = "power_instant"
-POWER_OUTPUT = "power_output"
-RAMP_ANGLE = "ramp_angle"
-RESISTANCE_LEVEL = "resistance_level"
-SPEED_AVERAGE = "speed_average"
-SPEED_INSTANT = "speed_instant"
-STEP_RATE_AVERAGE = "step_rate_average"
-STEP_RATE_INSTANT = "step_rate_instant"
-STRIDE_COUNT = "stride_count"
-STROKE_COUNT = "stroke_count"
-STROKE_RATE_AVERAGE = "stroke_rate_average"
-STROKE_RATE_INSTANT = "stroke_rate_instant"
-TIME_ELAPSED = "time_elapsed"
-TIME_REMAINING = "time_remaining"
-INDOOR_BIKE_SIMULATION = "indoor_bike_simulation"
-
-# TARGET SETTINGS ATTRIBUTES
-
-# WITH RANGES
-
-# Optional
-
-TARGET_SPEED = "target_speed"
-TARGET_POWER = "target_power"
-TARGET_HEART_RATE = "target_heart_rate"
-TARGET_INCLINATION = "target_inclination"
-TARGET_RESISTANCE = "target_resistance"
-
-# WITHOUT RANGES
-
-# Mandatory
-
-RESET = "reset"
-START = "start"
-STOP = "stop"
-PAUSE = "pause"
-
-# Optional
-
-BIKE_SIMULATION = "bike_simulation"
-SPIN_DOWN = "spin_down"
-TARGET_CADENCE = "target_cadence"
-TARGET_DISTANCE = "target_distance"
-TARGET_ENERGY = "target_energy"
-TARGET_STEPS = "target_steps"
-TARGET_STRIDES = "target_strides"
-TARGET_TIME = "target_time"
-TARGET_TIME_TWO_ZONES = "target_time_two_zones"
-TARGET_TIME_TIME_THREE_ZONES = "target_time_three_zones"
-TARGET_TIME_TIME_FIVE_ZONES = "target_time_five_zones"
-WHEEL_CIRCUMFERENCE = "wheel_circumference"
-
-# BLE UUIDS
-
-FITNESS_MACHINE_SERVICE_UUID = "00001826-0000-1000-8000-00805f9b34fb"
-"""Fitness Machine Service"""
-
-FITNESS_MACHINE_FEATURE_UUID = "00002acc-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read
-`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
-`Description:` Describes the capabilities supported by the device.
-"""
-
-TREADMILL_DATA_UUID = "00002acd-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Notify
-`Device Type:` Treadmill and walking pad only.
-`Description:` Reports real-time workout data.
-"""
-
-CROSS_TRAINER_DATA_UUID = "00002ace-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Notify
-`Device Type:` Elliptical machines only.
-`Description:` Reports real-time workout data.
-"""
-
-ROWER_DATA_UUID = "00002ad1-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Notify
-`Device Type:` Rower only.
-`Description:` Reports real-time workout data.
-"""
-
-INDOOR_BIKE_DATA_UUID = "00002ad2-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Notify
-`Device Type:` Smart bike only.
-`Description:` Reports real-time workout data.
-"""
-
-TRAINING_STATUS_UUID = "00002ad3-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read/Notify
-`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
-`Description:` Reports the device status data.
-"""
-
-SPEED_RANGE_UUID = "00002ad4-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read
-`Device Type:` Treadmill, walking pad, and smart bike.
-`Description:` Reports the supported speed range.
-"""
-
-INCLINATION_RANGE_UUID = "00002ad5-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read
-`Device Type:` Treadmill and walking pad.
-`Description:` Reports the supported inclination range.
-"""
-
-RESISTANCE_LEVEL_RANGE_UUID = "00002ad6-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read
-`Device Type:` Elliptical machine.
-`Description:` Reports the supported resistance level range.
-"""
-
-POWER_RANGE_UUID = "00002ad8-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read
-`Device Type:` Elliptical machine, rower, and smart bike.
-`Description:` Reports the supported power range.
-"""
-
-HEART_RATE_RANGE_UUID = "00002ad7-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Read
-`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
-`Description:` Reports supported heart rate range.
-"""
-
-FITNESS_MACHINE_CONTROL_POINT_UUID = "00002ad9-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Write/Indicate
-`Device Type:` Optional support for treadmills and walking pads, and mandatory for elliptical machines, rowers, and smart bikes.
-`Description:` Controls the status (paused or resumed) of fitness machine.
-"""
-
-FITNESS_MACHINE_STATUS_UUID = "00002ada-0000-1000-8000-00805f9b34fb"
-"""
-`Property:` Notify
-`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
-`Description:` Reports workout status changes of the fitness machine.
-"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+# REAL-TIME TRAINING DATA
+
+CADENCE_AVERAGE = "cadence_average"
+CADENCE_INSTANT = "cadence_instant"
+DISTANCE_TOTAL = "distance_total"
+ELEVATION_GAIN_NEGATIVE = "elevation_gain_negative"
+ELEVATION_GAIN_POSITIVE = "elevation_gain_positive"
+ENERGY_PER_HOUR = "energy_per_hour"
+ENERGY_PER_MINUTE = "energy_per_minute"
+ENERGY_TOTAL = "energy_total"
+FORCE_ON_BELT = "force_on_belt"
+HEART_RATE = "heart_rate"
+INCLINATION = "inclination"
+METABOLIC_EQUIVALENT = "metabolic_equivalent"
+MOVEMENT_DIRECTION = "movement_direction"
+PACE_AVERAGE = "pace_average"
+PACE_INSTANT = "pace_instant"
+POWER_AVERAGE = "power_average"
+POWER_INSTANT = "power_instant"
+POWER_OUTPUT = "power_output"
+RAMP_ANGLE = "ramp_angle"
+RESISTANCE_LEVEL = "resistance_level"
+SPEED_AVERAGE = "speed_average"
+SPEED_INSTANT = "speed_instant"
+STEP_RATE_AVERAGE = "step_rate_average"
+STEP_RATE_INSTANT = "step_rate_instant"
+STRIDE_COUNT = "stride_count"
+STROKE_COUNT = "stroke_count"
+STROKE_RATE_AVERAGE = "stroke_rate_average"
+STROKE_RATE_INSTANT = "stroke_rate_instant"
+TIME_ELAPSED = "time_elapsed"
+TIME_REMAINING = "time_remaining"
+INDOOR_BIKE_SIMULATION = "indoor_bike_simulation"
+
+# TARGET SETTINGS ATTRIBUTES
+
+# WITH RANGES
+
+# Optional
+
+TARGET_SPEED = "target_speed"
+TARGET_POWER = "target_power"
+TARGET_HEART_RATE = "target_heart_rate"
+TARGET_INCLINATION = "target_inclination"
+TARGET_RESISTANCE = "target_resistance"
+
+# WITHOUT RANGES
+
+# Mandatory
+
+RESET = "reset"
+START = "start"
+STOP = "stop"
+PAUSE = "pause"
+
+# Optional
+
+BIKE_SIMULATION = "bike_simulation"
+SPIN_DOWN = "spin_down"
+TARGET_CADENCE = "target_cadence"
+TARGET_DISTANCE = "target_distance"
+TARGET_ENERGY = "target_energy"
+TARGET_STEPS = "target_steps"
+TARGET_STRIDES = "target_strides"
+TARGET_TIME = "target_time"
+TARGET_TIME_TWO_ZONES = "target_time_two_zones"
+TARGET_TIME_TIME_THREE_ZONES = "target_time_three_zones"
+TARGET_TIME_TIME_FIVE_ZONES = "target_time_five_zones"
+WHEEL_CIRCUMFERENCE = "wheel_circumference"
+
+# BLE UUIDS
+
+FITNESS_MACHINE_SERVICE_UUID = "00001826-0000-1000-8000-00805f9b34fb"
+"""Fitness Machine Service"""
+
+FITNESS_MACHINE_FEATURE_UUID = "00002acc-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read
+`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
+`Description:` Describes the capabilities supported by the device.
+"""
+
+TREADMILL_DATA_UUID = "00002acd-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Notify
+`Device Type:` Treadmill and walking pad only.
+`Description:` Reports real-time workout data.
+"""
+
+CROSS_TRAINER_DATA_UUID = "00002ace-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Notify
+`Device Type:` Elliptical machines only.
+`Description:` Reports real-time workout data.
+"""
+
+ROWER_DATA_UUID = "00002ad1-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Notify
+`Device Type:` Rower only.
+`Description:` Reports real-time workout data.
+"""
+
+INDOOR_BIKE_DATA_UUID = "00002ad2-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Notify
+`Device Type:` Smart bike only.
+`Description:` Reports real-time workout data.
+"""
+
+TRAINING_STATUS_UUID = "00002ad3-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read/Notify
+`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
+`Description:` Reports the device status data.
+"""
+
+SPEED_RANGE_UUID = "00002ad4-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read
+`Device Type:` Treadmill, walking pad, and smart bike.
+`Description:` Reports the supported speed range.
+"""
+
+INCLINATION_RANGE_UUID = "00002ad5-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read
+`Device Type:` Treadmill and walking pad.
+`Description:` Reports the supported inclination range.
+"""
+
+RESISTANCE_LEVEL_RANGE_UUID = "00002ad6-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read
+`Device Type:` Elliptical machine.
+`Description:` Reports the supported resistance level range.
+"""
+
+POWER_RANGE_UUID = "00002ad8-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read
+`Device Type:` Elliptical machine, rower, and smart bike.
+`Description:` Reports the supported power range.
+"""
+
+HEART_RATE_RANGE_UUID = "00002ad7-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Read
+`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
+`Description:` Reports supported heart rate range.
+"""
+
+FITNESS_MACHINE_CONTROL_POINT_UUID = "00002ad9-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Write/Indicate
+`Device Type:` Optional support for treadmills and walking pads, and mandatory for elliptical machines, rowers, and smart bikes.
+`Description:` Controls the status (paused or resumed) of fitness machine.
+"""
+
+FITNESS_MACHINE_STATUS_UUID = "00002ada-0000-1000-8000-00805f9b34fb"
+"""
+`Property:` Notify
+`Device Type:` Treadmill, walking pad, elliptical machine, rower, and smart bike.
+`Description:` Reports workout status changes of the fitness machine.
+"""
```

### Comparing `pyftms-0.1.0/pyftms/client/machines/__init__.py` & `pyftms-0.1.1/pyftms/client/machines/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-from ..client import FitnessMachine
-from ..properties import MachineType
-from .cross_trainer import CrossTrainer
-from .indoor_bike import IndoorBike
-from .rower import Rower
-from .treadmill import Treadmill
-
-
-def get_machine(mt: MachineType) -> type[FitnessMachine]:
-    """Returns Fitness Machine by type."""
-    assert len(mt) == 1
-
-    match mt:
-        case MachineType.TREADMILL:
-            return Treadmill
-
-        case MachineType.CROSS_TRAINER:
-            return CrossTrainer
-
-        case MachineType.ROWER:
-            return Rower
-
-        case MachineType.INDOOR_BIKE:
-            return IndoorBike
-
-    raise NotImplementedError("This Fitness Machine type is not supported.")
-
-
-__all__ = [
-    "CrossTrainer",
-    "IndoorBike",
-    "Rower",
-    "Treadmill",
-    "get_machine",
-]
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+from ..client import FitnessMachine
+from ..properties import MachineType
+from .cross_trainer import CrossTrainer
+from .indoor_bike import IndoorBike
+from .rower import Rower
+from .treadmill import Treadmill
+
+
+def get_machine(mt: MachineType) -> type[FitnessMachine]:
+    """Returns Fitness Machine by type."""
+    assert len(mt) == 1
+
+    match mt:
+        case MachineType.TREADMILL:
+            return Treadmill
+
+        case MachineType.CROSS_TRAINER:
+            return CrossTrainer
+
+        case MachineType.ROWER:
+            return Rower
+
+        case MachineType.INDOOR_BIKE:
+            return IndoorBike
+
+    raise NotImplementedError("This Fitness Machine type is not supported.")
+
+
+__all__ = [
+    "CrossTrainer",
+    "IndoorBike",
+    "Rower",
+    "Treadmill",
+    "get_machine",
+]
```

### Comparing `pyftms-0.1.0/pyftms/client/machines/cross_trainer.py` & `pyftms-0.1.1/pyftms/client/machines/rower.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-from typing import ClassVar
-
-from ...models import CrossTrainerData, RealtimeData
-from ..client import FitnessMachine
-from ..const import CROSS_TRAINER_DATA_UUID
-from ..properties import MachineType
-
-
-class CrossTrainer(FitnessMachine[CrossTrainerData]):
-    """Cross Trainer (Elliptical Trainer)"""
-
-    _machine_type: ClassVar[MachineType] = MachineType.CROSS_TRAINER
-
-    _data_model: ClassVar[type[RealtimeData]] = CrossTrainerData
-
-    _data_uuid: ClassVar[str] = CROSS_TRAINER_DATA_UUID
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+from typing import ClassVar
+
+from ...models import RealtimeData, RowerData
+from ..client import FitnessMachine
+from ..const import ROWER_DATA_UUID
+from ..properties import MachineType
+
+
+class Rower(FitnessMachine):
+    """
+    Rower (Rowing Machine).
+
+    Specific class of `FitnessMachine`.
+    """
+
+    _machine_type: ClassVar[MachineType] = MachineType.ROWER
+
+    _data_model: ClassVar[type[RealtimeData]] = RowerData
+
+    _data_uuid: ClassVar[str] = ROWER_DATA_UUID
```

### Comparing `pyftms-0.1.0/pyftms/client/properties/features.py` & `pyftms-0.1.1/pyftms/client/properties/features.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,202 +1,205 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import io
-import logging
-from enum import STRICT, IntEnum, IntFlag, auto
-from types import MappingProxyType
-from typing import Mapping, NamedTuple
-
-from bleak import BleakClient
-
-from ...serializer import NumSerializer
-from ..const import (
-    FITNESS_MACHINE_FEATURE_UUID,
-    HEART_RATE_RANGE_UUID,
-    INCLINATION_RANGE_UUID,
-    POWER_RANGE_UUID,
-    RESISTANCE_LEVEL_RANGE_UUID,
-    SPEED_RANGE_UUID,
-    TARGET_HEART_RATE,
-    TARGET_INCLINATION,
-    TARGET_POWER,
-    TARGET_RESISTANCE,
-    TARGET_SPEED,
-)
-
-_LOGGER = logging.getLogger(__name__)
-
-SupportedValueTypes = float | int
-
-
-class MovementDirection(IntEnum, boundary=STRICT):
-    """
-    Code of `Stop or Pause` control and status messages.
-
-    Described in section `4.16.2.9: Stop or Pause Procedure`.
-    """
-
-    FORWARD = auto()
-    """Forward"""
-    BACKWARD = auto()
-    """Backward"""
-
-
-class MachineFeatures(IntFlag, boundary=STRICT):
-    """
-    Fitness Machine Features.
-
-    Described in section `4.3.1.1: Fitness Machine Features Field`.
-    """
-
-    AVERAGE_SPEED = auto()
-    """Average Speed Supported"""
-    CADENCE = auto()
-    """Cadence Supported"""
-    DISTANCE = auto()
-    """Total Distance Supported"""
-    INCLINATION = auto()
-    """Inclination Supported"""
-    ELEVATION_GAIN = auto()
-    """Elevation Gain Supported"""
-    PACE = auto()
-    """Pace Supported"""
-    STEP_COUNT = auto()
-    """Step Count Supported"""
-    RESISTANCE = auto()
-    """Resistance Level Supported"""
-    STRIDE_COUNT = auto()
-    """Stride Count Supported"""
-    EXPENDED_ENERGY = auto()
-    """Expended Energy Supported"""
-    HEART_RATE = auto()
-    """Heart Rate Measurement Supported"""
-    METABOLIC_EQUIVALENT = auto()
-    """Metabolic Equivalent Supported"""
-    ELAPSED_TIME = auto()
-    """Elapsed Time Supported"""
-    REMAINING_TIME = auto()
-    """Remaining Time Supported"""
-    POWER_MEASUREMENT = auto()
-    """Power Measurement Supported"""
-    FORCE_ON_BELT_AND_POWER_OUTPUT = auto()
-    """Force on Belt and Power Output Supported"""
-    USER_DATA_RETENTION = auto()
-    """User Data Retention Supported"""
-
-
-class MachineSettings(IntFlag, boundary=STRICT):
-    """
-    Target Setting Features.
-
-    Described in section `4.3.1.2: Target Setting Features Field`.
-    """
-
-    SPEED = auto()
-    """Speed Target Setting Supported"""
-    INCLINE = auto()
-    """Inclination Target Setting Supported"""
-    RESISTANCE = auto()
-    """Resistance Target Setting Supported"""
-    POWER = auto()
-    """Power Target Setting Supported"""
-    HEART_RATE = auto()
-    """Heart Rate Target Setting Supported"""
-    ENERGY = auto()
-    """Targeted Expended Energy Configuration Supported"""
-    STEPS = auto()
-    """Targeted Step Number Configuration Supported"""
-    STRIDES = auto()
-    """Targeted Stride Number Configuration Supported"""
-    DISTANCE = auto()
-    """Targeted Distance Configuration Supported"""
-    TIME = auto()
-    """Targeted Training Time Configuration Supported"""
-    TIME_TWO_ZONES = auto()
-    """Targeted Time in Two Heart Rate Zones Configuration Supported"""
-    TIME_THREE_ZONES = auto()
-    """Targeted Time in Three Heart Rate Zones Configuration Supported"""
-    TIME_FIVE_ZONES = auto()
-    """Targeted Time in Five Heart Rate Zones Configuration Supported"""
-    BIKE_SIMULATION = auto()
-    """Indoor Bike Simulation Parameters Supported"""
-    CIRCUMFERENCE = auto()
-    """Wheel Circumference Configuration Supported"""
-    SPIN_DOWN = auto()
-    """Spin Down Control Supported"""
-    CADENCE = auto()
-    """Targeted Cadence Configuration Supported"""
-
-
-class SettingRange(NamedTuple):
-    """Value range of settings parameter"""
-
-    native_min_value: SupportedValueTypes
-    native_max_value: SupportedValueTypes
-    native_step: SupportedValueTypes
-
-
-async def read_features(cli: BleakClient) -> tuple[MachineFeatures, MachineSettings]:
-    _LOGGER.debug("Reading features and settings.")
-
-    try:
-        data = await cli.read_gatt_char(FITNESS_MACHINE_FEATURE_UUID)
-
-        assert len(data) == 8
-
-        bio, u4 = io.BytesIO(data), NumSerializer("u4")
-
-        features = MachineFeatures(u4.deserialize(bio))
-        settings = MachineSettings(u4.deserialize(bio))
-
-    except Exception:
-        _LOGGER.exception("Failed reading machine features and settings.")
-        raise
-
-    _LOGGER.debug(features)
-    _LOGGER.debug(settings)
-
-    return features, settings
-
-
-async def _range(cli: BleakClient, uuid: str, num: str) -> SettingRange:
-    data = await cli.read_gatt_char(uuid)
-
-    bio, serializer = io.BytesIO(data), NumSerializer(num)
-    result = SettingRange(*(serializer.deserialize(bio) for _ in range(3)))
-
-    assert not bio.read(1)
-
-    return result
-
-
-async def read_supported_ranges(
-    cli: BleakClient,
-    settings: MachineSettings,
-) -> MappingProxyType[str, SettingRange]:
-    result: Mapping[str, SettingRange] = {}
-
-    _LOGGER.debug("Reading settings value ranges.")
-
-    if MachineSettings.SPEED in settings:
-        result[TARGET_SPEED] = await _range(cli, SPEED_RANGE_UUID, "u2.01")
-
-    if MachineSettings.INCLINE in settings:
-        result[TARGET_INCLINATION] = await _range(cli, INCLINATION_RANGE_UUID, "s2.1")
-
-    if MachineSettings.RESISTANCE in settings:
-        result[TARGET_RESISTANCE] = await _range(
-            cli, RESISTANCE_LEVEL_RANGE_UUID, "s2.1"
-        )
-
-    if MachineSettings.POWER in settings:
-        result[TARGET_POWER] = await _range(cli, POWER_RANGE_UUID, "s2")
-
-    if MachineSettings.HEART_RATE in settings:
-        result[TARGET_HEART_RATE] = await _range(cli, HEART_RATE_RANGE_UUID, "u1")
-
-    result = MappingProxyType(result)
-
-    _LOGGER.debug("Settings ranges: %s", result)
-
-    return result
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import io
+import logging
+from enum import STRICT, IntEnum, IntFlag, auto
+from types import MappingProxyType
+from typing import Mapping, NamedTuple
+
+from bleak import BleakClient
+
+from ...serializer import NumSerializer
+from ..const import (
+    FITNESS_MACHINE_FEATURE_UUID,
+    HEART_RATE_RANGE_UUID,
+    INCLINATION_RANGE_UUID,
+    POWER_RANGE_UUID,
+    RESISTANCE_LEVEL_RANGE_UUID,
+    SPEED_RANGE_UUID,
+    TARGET_HEART_RATE,
+    TARGET_INCLINATION,
+    TARGET_POWER,
+    TARGET_RESISTANCE,
+    TARGET_SPEED,
+)
+
+_LOGGER = logging.getLogger(__name__)
+
+SupportedValueTypes = float | int
+
+
+class MovementDirection(IntEnum, boundary=STRICT):
+    """
+    Movement direction. Used by `CrossTrainer` machine only.
+
+    Described in section **4.5.1.1 Flags Field**.
+    """
+
+    FORWARD = auto()
+    """Forward"""
+    BACKWARD = auto()
+    """Backward"""
+
+
+class MachineFeatures(IntFlag, boundary=STRICT):
+    """
+    Fitness Machine Features.
+
+    Described in section `4.3.1.1: Fitness Machine Features Field`.
+    """
+
+    AVERAGE_SPEED = auto()
+    """Average Speed Supported"""
+    CADENCE = auto()
+    """Cadence Supported"""
+    DISTANCE = auto()
+    """Total Distance Supported"""
+    INCLINATION = auto()
+    """Inclination Supported"""
+    ELEVATION_GAIN = auto()
+    """Elevation Gain Supported"""
+    PACE = auto()
+    """Pace Supported"""
+    STEP_COUNT = auto()
+    """Step Count Supported"""
+    RESISTANCE = auto()
+    """Resistance Level Supported"""
+    STRIDE_COUNT = auto()
+    """Stride Count Supported"""
+    EXPENDED_ENERGY = auto()
+    """Expended Energy Supported"""
+    HEART_RATE = auto()
+    """Heart Rate Measurement Supported"""
+    METABOLIC_EQUIVALENT = auto()
+    """Metabolic Equivalent Supported"""
+    ELAPSED_TIME = auto()
+    """Elapsed Time Supported"""
+    REMAINING_TIME = auto()
+    """Remaining Time Supported"""
+    POWER_MEASUREMENT = auto()
+    """Power Measurement Supported"""
+    FORCE_ON_BELT_AND_POWER_OUTPUT = auto()
+    """Force on Belt and Power Output Supported"""
+    USER_DATA_RETENTION = auto()
+    """User Data Retention Supported"""
+
+
+class MachineSettings(IntFlag, boundary=STRICT):
+    """
+    Target Setting Features.
+
+    Described in section `4.3.1.2: Target Setting Features Field`.
+    """
+
+    SPEED = auto()
+    """Speed Target Setting Supported"""
+    INCLINE = auto()
+    """Inclination Target Setting Supported"""
+    RESISTANCE = auto()
+    """Resistance Target Setting Supported"""
+    POWER = auto()
+    """Power Target Setting Supported"""
+    HEART_RATE = auto()
+    """Heart Rate Target Setting Supported"""
+    ENERGY = auto()
+    """Targeted Expended Energy Configuration Supported"""
+    STEPS = auto()
+    """Targeted Step Number Configuration Supported"""
+    STRIDES = auto()
+    """Targeted Stride Number Configuration Supported"""
+    DISTANCE = auto()
+    """Targeted Distance Configuration Supported"""
+    TIME = auto()
+    """Targeted Training Time Configuration Supported"""
+    TIME_TWO_ZONES = auto()
+    """Targeted Time in Two Heart Rate Zones Configuration Supported"""
+    TIME_THREE_ZONES = auto()
+    """Targeted Time in Three Heart Rate Zones Configuration Supported"""
+    TIME_FIVE_ZONES = auto()
+    """Targeted Time in Five Heart Rate Zones Configuration Supported"""
+    BIKE_SIMULATION = auto()
+    """Indoor Bike Simulation Parameters Supported"""
+    CIRCUMFERENCE = auto()
+    """Wheel Circumference Configuration Supported"""
+    SPIN_DOWN = auto()
+    """Spin Down Control Supported"""
+    CADENCE = auto()
+    """Targeted Cadence Configuration Supported"""
+
+
+class SettingRange(NamedTuple):
+    """Value range of settings parameter."""
+
+    min_value: SupportedValueTypes
+    """Minimum value. Inclusive."""
+    max_value: SupportedValueTypes
+    """Maximum value. Inclusive."""
+    step: SupportedValueTypes
+    """Step value."""
+
+
+async def read_features(cli: BleakClient) -> tuple[MachineFeatures, MachineSettings]:
+    _LOGGER.debug("Reading features and settings.")
+
+    try:
+        data = await cli.read_gatt_char(FITNESS_MACHINE_FEATURE_UUID)
+
+        assert len(data) == 8
+
+        bio, u4 = io.BytesIO(data), NumSerializer("u4")
+
+        features = MachineFeatures(u4.deserialize(bio))
+        settings = MachineSettings(u4.deserialize(bio))
+
+    except Exception:
+        _LOGGER.exception("Failed reading machine features and settings.")
+        raise
+
+    _LOGGER.debug(features)
+    _LOGGER.debug(settings)
+
+    return features, settings
+
+
+async def _range(cli: BleakClient, uuid: str, num: str) -> SettingRange:
+    data = await cli.read_gatt_char(uuid)
+
+    bio, serializer = io.BytesIO(data), NumSerializer(num)
+    result = SettingRange(*(serializer.deserialize(bio) for _ in range(3)))
+
+    assert not bio.read(1)
+
+    return result
+
+
+async def read_supported_ranges(
+    cli: BleakClient,
+    settings: MachineSettings,
+) -> MappingProxyType[str, SettingRange]:
+    result: Mapping[str, SettingRange] = {}
+
+    _LOGGER.debug("Reading settings value ranges.")
+
+    if MachineSettings.SPEED in settings:
+        result[TARGET_SPEED] = await _range(cli, SPEED_RANGE_UUID, "u2.01")
+
+    if MachineSettings.INCLINE in settings:
+        result[TARGET_INCLINATION] = await _range(cli, INCLINATION_RANGE_UUID, "s2.1")
+
+    if MachineSettings.RESISTANCE in settings:
+        result[TARGET_RESISTANCE] = await _range(
+            cli, RESISTANCE_LEVEL_RANGE_UUID, "s2.1"
+        )
+
+    if MachineSettings.POWER in settings:
+        result[TARGET_POWER] = await _range(cli, POWER_RANGE_UUID, "s2")
+
+    if MachineSettings.HEART_RATE in settings:
+        result[TARGET_HEART_RATE] = await _range(cli, HEART_RATE_RANGE_UUID, "u1")
+
+    result = MappingProxyType(result)
+
+    _LOGGER.debug("Settings ranges: %s", result)
+
+    return result
```

### Comparing `pyftms-0.1.0/pyftms/client/properties/machine_type.py` & `pyftms-0.1.1/pyftms/client/properties/machine_type.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,95 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import logging
-from enum import Flag, auto
-
-from bleak.backends.scanner import AdvertisementData
-
-from ..const import FITNESS_MACHINE_SERVICE_UUID
-
-_LOGGER = logging.getLogger(__name__)
-
-
-class MachineFlags(Flag):
-    """
-    Fitness Machine Flags.
-
-    Included in the `Service Data AD Type`.
-
-    Described in section `3.1.1: Flags Field`.
-    """
-
-    FITNESS_MACHINE = auto()
-    """Fitness Machine Available"""
-
-
-class MachineType(Flag):
-    """
-    Fitness Machine Type.
-
-    Included in the `Service Data AD Type`.
-
-    Described in section `3.1.2: Fitness Machine Type Field`.
-    """
-
-    TREADMILL = auto()
-    """Treadmill Supported"""
-    CROSS_TRAINER = auto()
-    """Cross Trainer Supported"""
-    STEP_CLIMBER = auto()
-    """Step Climber Supported"""
-    STAIR_CLIMBER = auto()
-    """Stair Climber Supported"""
-    ROWER = auto()
-    """Rower Supported"""
-    INDOOR_BIKE = auto()
-    """Indoor Bike Supported"""
-
-
-class NotFitnessMachineError(Exception):
-    def __init__(self, adv_data: bytes | None) -> None:
-        msg = "No service data"
-
-        if adv_data is not None:
-            msg = f"AD service data: '{adv_data.hex(" ")}'"
-
-        super().__init__(f"Device is not Fitness Machine. {msg}.")
-
-
-def get_machine_type_from_service_data(adv: AdvertisementData) -> MachineType:
-    """Returns Fitness Machine Type from service AD data."""
-    data = adv.service_data.get(FITNESS_MACHINE_SERVICE_UUID)
-
-    if data is None or len(data) != 3:
-        raise NotFitnessMachineError(data)
-
-    # Reading mandatory `Flags` and `Machine Type`.
-    # Machine Type bytes may be reversed on some
-    # machines (it's bug), so I logically ORed them.
-    try:
-        mf, mt = MachineFlags(data[0]), MachineType(data[1] | data[2])
-
-    except ValueError:
-        raise NotFitnessMachineError(data)
-
-    if mf and mt:
-        return mt
-
-    raise NotFitnessMachineError(data)
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import logging
+from enum import Flag, auto
+
+from bleak.backends.scanner import AdvertisementData
+
+from ..const import FITNESS_MACHINE_SERVICE_UUID
+
+_LOGGER = logging.getLogger(__name__)
+
+
+class MachineFlags(Flag):
+    """
+    Fitness Machine Flags.
+
+    Included in the `Service Data AD Type`.
+
+    Described in section `3.1.1: Flags Field`.
+    """
+
+    FITNESS_MACHINE = auto()
+    """Fitness Machine Available"""
+
+
+class MachineType(Flag):
+    """
+    Fitness Machine Type.
+
+    Included in the `Service Data AD Type`.
+
+    Described in section `3.1.2: Fitness Machine Type Field`.
+    """
+
+    TREADMILL = auto()
+    """Treadmill Supported"""
+    CROSS_TRAINER = auto()
+    """Cross Trainer Supported"""
+    STEP_CLIMBER = auto()
+    """Step Climber Supported"""
+    STAIR_CLIMBER = auto()
+    """Stair Climber Supported"""
+    ROWER = auto()
+    """Rower Supported"""
+    INDOOR_BIKE = auto()
+    """Indoor Bike Supported"""
+
+
+class NotFitnessMachineError(Exception):
+    """
+    An exception if the FTMS service is not supported by the Bluetooth device.
+
+    May be raised in `get_machine_type_from_service_data` and `get_client`
+    functions if advertisement data was passed as an argument.
+    """
+
+    def __init__(self, adv_data: bytes | None) -> None:
+        msg = "No service data"
+
+        if adv_data is not None:
+            msg = f"AD service data: '{adv_data.hex(" ")}'"
+
+        super().__init__(f"Device is not Fitness Machine. {msg}.")
+
+
+def get_machine_type_from_service_data(adv_data: AdvertisementData) -> MachineType:
+    """
+    Returns `MachineType` from service advertisement data.
+
+    Parameters:
+    - `adv_data` - Service [advertisement data](https://bleak.readthedocs.io/en/latest/backends/index.html#bleak.backends.scanner.AdvertisementData).
+
+    Return:
+    - `MachineType` - type of fitness machine.
+    """
+
+    data = adv_data.service_data.get(FITNESS_MACHINE_SERVICE_UUID)
+
+    if data is None or len(data) != 3:
+        raise NotFitnessMachineError(data)
+
+    # Reading mandatory `Flags` and `Machine Type`.
+    # Machine Type bytes may be reversed on some
+    # machines (it's bug), so I logically ORed them.
+    try:
+        mf, mt = MachineFlags(data[0]), MachineType(data[1] | data[2])
+
+    except ValueError:
+        raise NotFitnessMachineError(data)
+
+    if mf and mt:
+        return mt
+
+    raise NotFitnessMachineError(data)
```

### Comparing `pyftms-0.1.0/pyftms/models/common.py` & `pyftms-0.1.1/pyftms/models/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,118 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-import io
-import itertools
-from enum import STRICT, IntEnum, auto
-from typing import Any, Generic, TypeVar, cast, override
-
-from ..serializer import BaseModel, ModelMeta, get_serializer, model_meta
-
-
-class StopPauseCode(IntEnum, boundary=STRICT):
-    """
-    Code of `Stop or Pause` control and status messages.
-
-    Described in section `4.16.2.9: Stop or Pause Procedure`.
-    """
-
-    STOP = auto()
-    """Stop"""
-    PAUSE = auto()
-    """Pause"""
-
-
-@dc.dataclass(frozen=True)
-class IndoorBikeSimulationParameters(BaseModel):
-    """
-    Indoor Bike Simulation Parameters
-
-    Described in section `4.16.2.18: Set Indoor Bike Simulation Parameters Procedure`.
-
-    Fields:
-        - `Wind Speed` | Meters Per Second (mps)
-        - `Grade` | Percentage
-        - `Coefficient of Rolling Resistance` | Unitless
-        - `Wind Resistance Coefficient` | Kilogram per Meter (Kg/m)
-    """
-
-    wind_speed: float = dc.field(
-        metadata=model_meta(
-            format="s2.001",
-        )
-    )
-
-    grade: float = dc.field(
-        metadata=model_meta(
-            format="s2.01",
-        )
-    )
-
-    rolling_resistance: float = dc.field(
-        metadata=model_meta(
-            format="u1.0001",
-        )
-    )
-
-    wind_resistance: float = dc.field(
-        metadata=model_meta(
-            format="u1.01",
-        )
-    )
-
-
-T = TypeVar("T", bound=int)
-
-
-@dc.dataclass(frozen=True)
-class CodeSwitchModel(Generic[T], BaseModel):
-    """Base model based on a code attribute and associated parameter attributes."""
-
-    code: T | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-        ),
-    )
-    """Code | Enumeration"""
-
-    @override
-    @classmethod
-    def _deserialize_dict(cls, src: io.IOBase) -> dict[str, Any]:
-        code, kwargs = cast(int, get_serializer("u1").deserialize(src)), {}
-        kwargs["code"] = code
-
-        for k, s in itertools.islice(cls._iter_fields_serializers(), 1, None):
-            meta = cast(ModelMeta, k.metadata)
-
-            if meta["code"] != code:
-                continue
-
-            name, value = k.name, s.deserialize(src)
-
-            # remove digit suffix of 'target_time_x' property
-            if name[-1].isdecimal():
-                name = name[:-2]
-
-            kwargs[name] = value
-
-            break
-
-        assert not src.read()
-
-        return kwargs
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+import io
+from enum import STRICT, IntEnum, auto
+from typing import Any, Generic, TypeVar, cast, override
+
+from ..serializer import BaseModel, ModelMeta, model_meta
+
+
+class StopPauseCode(IntEnum, boundary=STRICT):
+    """
+    Code of `Stop or Pause` control and status messages.
+
+    Described in section `4.16.2.9: Stop or Pause Procedure`.
+    """
+
+    STOP = auto()
+    """Stop."""
+    PAUSE = auto()
+    """Pause."""
+
+
+@dc.dataclass(frozen=True)
+class IndoorBikeSimulationParameters(BaseModel):
+    """
+    Indoor Bike Simulation Parameters
+
+    Described in section **4.16.2.18: Set Indoor Bike Simulation Parameters Procedure**.
+    """
+
+    wind_speed: float = dc.field(
+        metadata=model_meta(
+            format="s2.001",
+        )
+    )
+    """
+    Wind Speed.
+    
+    Units: `meters per second (mps)`.
+    """
+
+    grade: float = dc.field(
+        metadata=model_meta(
+            format="s2.01",
+        )
+    )
+    """
+    Grade.
+    
+    Units: `%`.
+    """
+
+    rolling_resistance: float = dc.field(
+        metadata=model_meta(
+            format="u1.0001",
+        )
+    )
+    """
+    Coefficient of Rolling Resistance.
+    
+    Units: `unitless`.
+    """
+
+    wind_resistance: float = dc.field(
+        metadata=model_meta(
+            format="u1.01",
+        )
+    )
+    """
+    Wind Resistance Coefficient.
+    
+    Units: `kilogram per meter (kg/m)`.
+    """
+
+
+T = TypeVar("T", bound=int)
+
+
+@dc.dataclass(frozen=True)
+class CodeSwitchModel(Generic[T], BaseModel):
+    """Base model based on a code attribute and associated parameter attributes."""
+
+    code: T | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+        ),
+    )
+    """Code | Enumeration"""
+
+    @override
+    @classmethod
+    def _deserialize_asdict(cls, src: io.IOBase) -> dict[str, Any]:
+        kwargs, it = {}, cls._iter_fields_serializers()
+        code = cast(int, next(it)[1].deserialize(src))
+        kwargs["code"] = code
+
+        for field, serializer in it:
+            meta = cast(ModelMeta, field.metadata)
+
+            if meta.get("code") != code:
+                continue
+
+            name, value = field.name, serializer.deserialize(src)
+
+            # remove digit suffix of 'target_time_x' property
+            if name[-1].isdecimal():
+                name = name[:-2]
+
+            kwargs[name] = value
+
+            break
+
+        assert not src.read()
+
+        return kwargs
```

### Comparing `pyftms-0.1.0/pyftms/models/machine_status.py` & `pyftms-0.1.1/pyftms/models/machine_status.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-from enum import STRICT, IntEnum, auto
-
-from .common import (
-    CodeSwitchModel,
-    IndoorBikeSimulationParameters,
-    StopPauseCode,
-    model_meta,
-)
-from .spin_down import SpinDownStatusCode
-
-
-class MachineStatusCode(IntEnum, boundary=STRICT):
-    """
-    Fitness Machine Status.
-
-    Described in section `4.16.1: Fitness Machine Control Point Procedure Requirements`.
-    """
-
-    RESET = auto()
-    """Reset"""
-
-    STOP_PAUSE = auto()
-    """Fitness Machine Stopped or Paused by the User"""
-
-    STOP_SAFETY = auto()
-    """Fitness Machine Stopped by Safety Key"""
-
-    START_RESUME = auto()
-    """Fitness Machine Started or Resumed by the User"""
-
-    SPEED = auto()
-    """Target Speed Changed"""
-
-    INCLINE = auto()
-    """Target Incline Changed"""
-
-    RESISTANCE = auto()
-    """Target Resistance Level Changed"""
-
-    POWER = auto()
-    """Target Power Changed"""
-
-    HEART_RATE = auto()
-    """Target Heart Rate Changed"""
-
-    ENERGY = auto()
-    """Targeted Expended Energy Changed"""
-
-    STEPS_NUMBER = auto()
-    """Targeted Number of Steps Changed"""
-
-    STRIDES_NUMBER = auto()
-    """Targeted Number of Strides Changed"""
-
-    DISTANCE = auto()
-    """Targeted Distance Changed"""
-
-    TIME_1 = auto()
-    """Targeted Training Time Changed"""
-
-    TIME_2 = auto()
-    """Targeted Time in Two Heart Rate Zones Changed"""
-
-    TIME_3 = auto()
-    """Targeted Time in Three Heart Rate Zones Changed"""
-
-    TIME_5 = auto()
-    """Targeted Time in Five Heart Rate Zones Changed"""
-
-    INDOOR_BIKE_SIMULATION = auto()
-    """Indoor Bike Simulation Parameters Changed"""
-
-    WHEEL_CIRCUMFERENCE = auto()
-    """Wheel Circumference Changed"""
-
-    SPIN_DOWN = auto()
-    """Spin Down Status"""
-
-    CADENCE = auto()
-    """Targeted Cadence Changed"""
-
-    LOST_CONTROL = 0xFF
-    """Control Permission Lost"""
-
-
-@dc.dataclass(frozen=True)
-class MachineStatusModel(CodeSwitchModel[MachineStatusCode]):
-    """
-    Structure of the Fitness Machine Status characteristic.
-
-    Described in section `4.17 Fitness Machine Status`.
-    """
-
-    stop_pause: StopPauseCode | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-            code=MachineStatusCode.STOP_PAUSE,
-        ),
-    )
-    """Stopped or Paused Event | Enumeration"""
-
-    target_speed: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.01",
-            code=MachineStatusCode.SPEED,
-        ),
-    )
-    """New Target Speed | Km/h"""
-
-    target_inclination: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2.1",
-            code=MachineStatusCode.INCLINE,
-        ),
-    )
-    """New Target Inclination | Percent"""
-
-    target_resistance: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1.1",
-            code=MachineStatusCode.RESISTANCE,
-        ),
-    )
-    """New Target Resistance Level | Unitless"""
-
-    target_power: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            code=MachineStatusCode.POWER,
-        ),
-    )
-    """New Target Power | Watt"""
-
-    target_heart_rate: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-            code=MachineStatusCode.HEART_RATE,
-        ),
-    )
-    """New Target Heart Rate | BPM"""
-
-    target_energy: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            code=MachineStatusCode.ENERGY,
-        ),
-    )
-    """New Targeted Expended Energy | Calorie"""
-
-    target_steps: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            code=MachineStatusCode.STEPS_NUMBER,
-        ),
-    )
-    """New Targeted Number of Steps | Step"""
-
-    target_strides: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            code=MachineStatusCode.STRIDES_NUMBER,
-        ),
-    )
-    """New Targeted Number of Strides | Stride"""
-
-    target_distance: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u3",
-            code=MachineStatusCode.DISTANCE,
-        ),
-    )
-    """New Targeted Distance | Meter"""
-
-    target_time_1: tuple[int, ...] | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            num=1,
-            code=MachineStatusCode.TIME_1,
-        ),
-    )
-    """New Targeted Training Time | Second"""
-
-    target_time_2: tuple[int, ...] | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            num=2,
-            code=MachineStatusCode.TIME_2,
-        ),
-    )
-    """New Targeted Time in Two Heart Rate Zones"""
-
-    target_time_3: tuple[int, ...] | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            num=3,
-            code=MachineStatusCode.TIME_3,
-        ),
-    )
-    """New Targeted Time in Three Heart Rate Zones"""
-
-    target_time_5: tuple[int, ...] | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            num=5,
-            code=MachineStatusCode.TIME_5,
-        ),
-    )
-    """New Targeted Time in Five Heart Rate Zones"""
-
-    indoor_bike_simulation: IndoorBikeSimulationParameters | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            code=MachineStatusCode.INDOOR_BIKE_SIMULATION,
-        ),
-    )
-    """New Indoor Bike Simulation Parameters"""
-
-    wheel_circumference: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.1",
-            code=MachineStatusCode.WHEEL_CIRCUMFERENCE,
-        ),
-    )
-    """New Wheel Circumference"""
-
-    spin_down_status: SpinDownStatusCode | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-            code=MachineStatusCode.SPIN_DOWN,
-        ),
-    )
-    """Spin Down Control | Enumeration"""
-
-    target_cadence: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.5",
-            code=MachineStatusCode.CADENCE,
-        ),
-    )
-    """New Targeted Cadence | 1/minute"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+from enum import STRICT, IntEnum, auto
+
+from .common import (
+    CodeSwitchModel,
+    IndoorBikeSimulationParameters,
+    StopPauseCode,
+    model_meta,
+)
+from .spin_down import SpinDownStatusCode
+
+
+class MachineStatusCode(IntEnum, boundary=STRICT):
+    """
+    Fitness Machine Status.
+
+    Described in section `4.16.1: Fitness Machine Control Point Procedure Requirements`.
+    """
+
+    RESET = auto()
+    """Reset"""
+
+    STOP_PAUSE = auto()
+    """Fitness Machine Stopped or Paused by the User"""
+
+    STOP_SAFETY = auto()
+    """Fitness Machine Stopped by Safety Key"""
+
+    START_RESUME = auto()
+    """Fitness Machine Started or Resumed by the User"""
+
+    SPEED = auto()
+    """Target Speed Changed"""
+
+    INCLINE = auto()
+    """Target Incline Changed"""
+
+    RESISTANCE = auto()
+    """Target Resistance Level Changed"""
+
+    POWER = auto()
+    """Target Power Changed"""
+
+    HEART_RATE = auto()
+    """Target Heart Rate Changed"""
+
+    ENERGY = auto()
+    """Targeted Expended Energy Changed"""
+
+    STEPS_NUMBER = auto()
+    """Targeted Number of Steps Changed"""
+
+    STRIDES_NUMBER = auto()
+    """Targeted Number of Strides Changed"""
+
+    DISTANCE = auto()
+    """Targeted Distance Changed"""
+
+    TIME_1 = auto()
+    """Targeted Training Time Changed"""
+
+    TIME_2 = auto()
+    """Targeted Time in Two Heart Rate Zones Changed"""
+
+    TIME_3 = auto()
+    """Targeted Time in Three Heart Rate Zones Changed"""
+
+    TIME_5 = auto()
+    """Targeted Time in Five Heart Rate Zones Changed"""
+
+    INDOOR_BIKE_SIMULATION = auto()
+    """Indoor Bike Simulation Parameters Changed"""
+
+    WHEEL_CIRCUMFERENCE = auto()
+    """Wheel Circumference Changed"""
+
+    SPIN_DOWN = auto()
+    """Spin Down Status"""
+
+    CADENCE = auto()
+    """Targeted Cadence Changed"""
+
+    LOST_CONTROL = 0xFF
+    """Control Permission Lost"""
+
+
+@dc.dataclass(frozen=True)
+class MachineStatusModel(CodeSwitchModel[MachineStatusCode]):
+    """
+    Structure of the Fitness Machine Status characteristic.
+
+    Described in section `4.17 Fitness Machine Status`.
+    """
+
+    stop_pause: StopPauseCode | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+            code=MachineStatusCode.STOP_PAUSE,
+        ),
+    )
+    """Stopped or Paused Event | Enumeration"""
+
+    target_speed: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.01",
+            code=MachineStatusCode.SPEED,
+        ),
+    )
+    """New Target Speed | Km/h"""
+
+    target_inclination: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2.1",
+            code=MachineStatusCode.INCLINE,
+        ),
+    )
+    """New Target Inclination | Percent"""
+
+    target_resistance: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1.1",
+            code=MachineStatusCode.RESISTANCE,
+        ),
+    )
+    """New Target Resistance Level | Unitless"""
+
+    target_power: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2",
+            code=MachineStatusCode.POWER,
+        ),
+    )
+    """New Target Power | Watt"""
+
+    target_heart_rate: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+            code=MachineStatusCode.HEART_RATE,
+        ),
+    )
+    """New Target Heart Rate | BPM"""
+
+    target_energy: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            code=MachineStatusCode.ENERGY,
+        ),
+    )
+    """New Targeted Expended Energy | Calorie"""
+
+    target_steps: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            code=MachineStatusCode.STEPS_NUMBER,
+        ),
+    )
+    """New Targeted Number of Steps | Step"""
+
+    target_strides: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            code=MachineStatusCode.STRIDES_NUMBER,
+        ),
+    )
+    """New Targeted Number of Strides | Stride"""
+
+    target_distance: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u3",
+            code=MachineStatusCode.DISTANCE,
+        ),
+    )
+    """New Targeted Distance | Meter"""
+
+    target_time_1: tuple[int, ...] | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            num=1,
+            code=MachineStatusCode.TIME_1,
+        ),
+    )
+    """New Targeted Training Time | Second"""
+
+    target_time_2: tuple[int, ...] | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            num=2,
+            code=MachineStatusCode.TIME_2,
+        ),
+    )
+    """New Targeted Time in Two Heart Rate Zones"""
+
+    target_time_3: tuple[int, ...] | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            num=3,
+            code=MachineStatusCode.TIME_3,
+        ),
+    )
+    """New Targeted Time in Three Heart Rate Zones"""
+
+    target_time_5: tuple[int, ...] | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            num=5,
+            code=MachineStatusCode.TIME_5,
+        ),
+    )
+    """New Targeted Time in Five Heart Rate Zones"""
+
+    indoor_bike_simulation: IndoorBikeSimulationParameters | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            code=MachineStatusCode.INDOOR_BIKE_SIMULATION,
+        ),
+    )
+    """New Indoor Bike Simulation Parameters"""
+
+    wheel_circumference: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.1",
+            code=MachineStatusCode.WHEEL_CIRCUMFERENCE,
+        ),
+    )
+    """New Wheel Circumference"""
+
+    spin_down_status: SpinDownStatusCode | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+            code=MachineStatusCode.SPIN_DOWN,
+        ),
+    )
+    """Spin Down Control | Enumeration"""
+
+    target_cadence: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.5",
+            code=MachineStatusCode.CADENCE,
+        ),
+    )
+    """New Targeted Cadence | 1/minute"""
```

### Comparing `pyftms-0.1.0/pyftms/models/realtime_data/common.py` & `pyftms-0.1.1/pyftms/models/realtime_data/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-import io
-from typing import Any, cast, override
-
-from ...serializer import BaseModel, get_serializer, model_meta
-
-
-@dc.dataclass(frozen=True)
-class RealtimeData(BaseModel):
-    mask: dc.InitVar[int]
-
-    @override
-    @classmethod
-    def _deserialize_dict(cls, src: io.IOBase) -> dict[str, Any]:
-        mask, kwargs = cast(int, get_serializer("u2").deserialize(src)), {}
-        kwargs["mask"] = mask
-        mask ^= 1
-
-        for field, serializer in cls._iter_fields_serializers():
-            if mask & 1:
-                kwargs[field.name] = serializer.deserialize(src)
-
-            mask >>= 1
-
-            if not mask:
-                break
-
-        assert not src.read()
-
-        return kwargs
-
-    @override
-    @classmethod
-    def _calc_size(cls) -> int:
-        return super()._calc_size() + 2
-
-
-@dc.dataclass(frozen=True)
-class RealtimeSpeedData(RealtimeData):
-    speed_instant: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.01",
-        ),
-    )
-    """Instantaneous Speed"""
-
-    speed_average: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.01",
-            features_bit=0,
-        ),
-    )
-    """Average Speed"""
-
-
-@dc.dataclass(frozen=True)
-class StepRateData(BaseModel):
-    step_rate_instant: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Step Rate Instant"""
-
-    step_rate_average: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Step Rate Average"""
-
-
-@dc.dataclass(frozen=True)
-class ElevationGainData(BaseModel):
-    elevation_gain_positive: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Elevation Gain Positive"""
-
-    elevation_gain_negative: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Elevation Gain Negative"""
-
-
-@dc.dataclass(frozen=True)
-class InclinationData(BaseModel):
-    inclination: float = dc.field(
-        metadata=model_meta(
-            format="s2.1",
-        ),
-    )
-    """Inclination"""
-
-    ramp_angle: float = dc.field(
-        metadata=model_meta(
-            format="s2.1",
-        ),
-    )
-    """Ramp Angle"""
-
-
-@dc.dataclass(frozen=True)
-class EnergyData(BaseModel):
-    energy_total: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Total Energy"""
-
-    energy_per_hour: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Per Hour Energy"""
-
-    energy_per_minute: int = dc.field(
-        metadata=model_meta(
-            format="u1",
-        ),
-    )
-    """Per Minute Energy"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+import io
+from typing import Any, cast, override
+
+from ...serializer import BaseModel, get_serializer, model_meta
+
+
+@dc.dataclass(frozen=True)
+class RealtimeData(BaseModel):
+    mask: dc.InitVar[int]
+
+    @override
+    @classmethod
+    def _deserialize_asdict(cls, src: io.IOBase) -> dict[str, Any]:
+        mask, kwargs = cast(int, get_serializer("u2").deserialize(src)), {}
+        kwargs["mask"] = mask
+        mask ^= 1
+
+        for field, serializer in cls._iter_fields_serializers():
+            if mask & 1:
+                kwargs[field.name] = serializer.deserialize(src)
+
+            mask >>= 1
+
+            if not mask:
+                break
+
+        assert not src.read()
+
+        return kwargs
+
+    @override
+    @classmethod
+    def _calc_size(cls) -> int:
+        return super()._calc_size() + 2
+
+
+@dc.dataclass(frozen=True)
+class RealtimeSpeedData(RealtimeData):
+    speed_instant: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.01",
+        ),
+    )
+    """Instantaneous Speed"""
+
+    speed_average: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.01",
+            features_bit=0,
+        ),
+    )
+    """Average Speed"""
+
+
+@dc.dataclass(frozen=True)
+class StepRateData(BaseModel):
+    step_rate_instant: int = dc.field(
+        metadata=model_meta(
+            format="u2",
+        ),
+    )
+    """Step Rate Instant"""
+
+    step_rate_average: int = dc.field(
+        metadata=model_meta(
+            format="u2",
+        ),
+    )
+    """Step Rate Average"""
+
+
+@dc.dataclass(frozen=True)
+class ElevationGainData(BaseModel):
+    elevation_gain_positive: int = dc.field(
+        metadata=model_meta(
+            format="u2",
+        ),
+    )
+    """Elevation Gain Positive"""
+
+    elevation_gain_negative: int = dc.field(
+        metadata=model_meta(
+            format="u2",
+        ),
+    )
+    """Elevation Gain Negative"""
+
+
+@dc.dataclass(frozen=True)
+class InclinationData(BaseModel):
+    inclination: float = dc.field(
+        metadata=model_meta(
+            format="s2.1",
+        ),
+    )
+    """Inclination"""
+
+    ramp_angle: float = dc.field(
+        metadata=model_meta(
+            format="s2.1",
+        ),
+    )
+    """Ramp Angle"""
+
+
+@dc.dataclass(frozen=True)
+class EnergyData(BaseModel):
+    energy_total: int = dc.field(
+        metadata=model_meta(
+            format="u2",
+        ),
+    )
+    """Total Energy"""
+
+    energy_per_hour: int = dc.field(
+        metadata=model_meta(
+            format="u2",
+        ),
+    )
+    """Per Hour Energy"""
+
+    energy_per_minute: int = dc.field(
+        metadata=model_meta(
+            format="u1",
+        ),
+    )
+    """Per Minute Energy"""
```

### Comparing `pyftms-0.1.0/pyftms/models/realtime_data/indoor_bike.py` & `pyftms-0.1.1/pyftms/models/realtime_data/indoor_bike.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-
-from .common import EnergyData, RealtimeSpeedData, model_meta
-
-
-@dc.dataclass(frozen=True)
-class IndoorBikeData(RealtimeSpeedData):
-    cadence_instant: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.5",
-            features_bit=1,
-        ),
-    )
-    """Instantaneous Cadence"""
-
-    cadence_average: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2.5",
-            features_bit=1,
-        ),
-    )
-    """Average Cadence"""
-
-    distance_total: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u3",
-            features_bit=2,
-        ),
-    )
-    """Total Distance"""
-
-    resistance_level: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            features_bit=7,
-        ),
-    )
-    """Resistance Level"""
-
-    power_instant: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            features_bit=14,
-        ),
-    )
-    """Instantaneous Power"""
-
-    power_average: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            features_bit=14,
-        ),
-    )
-    """Average Power"""
-
-    energy: EnergyData | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            features_bit=9,
-        ),
-    )
-    """Energy Data"""
-
-    heart_rate: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-            features_bit=10,
-        ),
-    )
-    """Heart Rate"""
-
-    metabolic_equivalent: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s1.1",
-            features_bit=11,
-        ),
-    )
-    """Metabolic Equivalent"""
-
-    time_elapsed: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=12,
-        ),
-    )
-    """Elapsed Time"""
-
-    time_remaining: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=13,
-        ),
-    )
-    """Remaining Time"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+
+from .common import EnergyData, RealtimeSpeedData, model_meta
+
+
+@dc.dataclass(frozen=True)
+class IndoorBikeData(RealtimeSpeedData):
+    cadence_instant: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.5",
+            features_bit=1,
+        ),
+    )
+    """Instantaneous Cadence"""
+
+    cadence_average: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2.5",
+            features_bit=1,
+        ),
+    )
+    """Average Cadence"""
+
+    distance_total: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u3",
+            features_bit=2,
+        ),
+    )
+    """Total Distance"""
+
+    resistance_level: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2",
+            features_bit=7,
+        ),
+    )
+    """Resistance Level"""
+
+    power_instant: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2",
+            features_bit=14,
+        ),
+    )
+    """Instantaneous Power"""
+
+    power_average: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2",
+            features_bit=14,
+        ),
+    )
+    """Average Power"""
+
+    energy: EnergyData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=9,
+        ),
+    )
+    """Energy Data"""
+
+    heart_rate: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+            features_bit=10,
+        ),
+    )
+    """Heart Rate"""
+
+    metabolic_equivalent: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s1.1",
+            features_bit=11,
+        ),
+    )
+    """Metabolic Equivalent"""
+
+    time_elapsed: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=12,
+        ),
+    )
+    """Elapsed Time"""
+
+    time_remaining: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=13,
+        ),
+    )
+    """Remaining Time"""
```

### Comparing `pyftms-0.1.0/pyftms/models/realtime_data/rower.py` & `pyftms-0.1.1/pyftms/models/realtime_data/treadmill.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,128 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-
-from .common import BaseModel, EnergyData, RealtimeData, model_meta
-
-
-@dc.dataclass(frozen=True)
-class StrokeRateData(BaseModel):
-    stroke_rate_instant: float = dc.field(
-        metadata=model_meta(
-            format="u1.5",
-        ),
-    )
-    """Stroke Rate"""
-
-    stroke_count: int = dc.field(
-        metadata=model_meta(
-            format="u2",
-        ),
-    )
-    """Stroke Count"""
-
-
-@dc.dataclass(frozen=True)
-class RowerData(RealtimeData):
-    stroke_rate: StrokeRateData | None = dc.field(
-        default=None,
-        metadata=model_meta(),
-    )
-    """Stroke Rate Data"""
-
-    stroke_rate_average: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1.5",
-            features_bit=1,
-        ),
-    )
-    """Average Stroke Rate"""
-
-    distance_total: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u3",
-            features_bit=2,
-        ),
-    )
-    """Total Distance"""
-
-    pace_instant: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=5,
-        ),
-    )
-    """Instantaneous Speed"""
-
-    pace_average: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=5,
-        ),
-    )
-    """Average Speed"""
-
-    power_instant: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            features_bit=14,
-        ),
-    )
-    """Instantaneous Power"""
-
-    power_average: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            features_bit=14,
-        ),
-    )
-    """Average Power"""
-
-    resistance_level: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s2",
-            features_bit=7,
-        ),
-    )
-    """Resistance Level"""
-
-    energy: EnergyData | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            features_bit=9,
-        ),
-    )
-    """Energy Data"""
-
-    heart_rate: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-            features_bit=10,
-        ),
-    )
-    """Heart Rate"""
-
-    metabolic_equivalent: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s1.1",
-            features_bit=11,
-        ),
-    )
-    """Metabolic Equivalent"""
-
-    time_elapsed: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=12,
-        ),
-    )
-    """Elapsed Time"""
-
-    time_remaining: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=13,
-        ),
-    )
-    """Remaining Time"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+
+from .common import (
+    BaseModel,
+    ElevationGainData,
+    EnergyData,
+    InclinationData,
+    RealtimeSpeedData,
+    model_meta,
+)
+
+
+@dc.dataclass(frozen=True)
+class ForceOnBeltData(BaseModel):
+    force_on_belt: int = dc.field(
+        metadata=model_meta(
+            format="s2",
+        ),
+    )
+    """Force On Belt"""
+
+    power_output: int = dc.field(
+        metadata=model_meta(
+            format="s2",
+        ),
+    )
+    """Output Power"""
+
+
+@dc.dataclass(frozen=True)
+class TreadmillData(RealtimeSpeedData):
+    distance_total: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u3",
+            features_bit=2,
+        ),
+    )
+    """Total Distance"""
+
+    inclination: InclinationData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=3,
+        ),
+    )
+    """Inclination and Ramp Angle Data"""
+
+    elevation_gain: ElevationGainData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=4,
+        ),
+    )
+    """Elevation Gain Data"""
+
+    pace_instant: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s1.1",
+            features_bit=5,
+        ),
+    )
+    """Instantaneous Speed"""
+
+    pace_average: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s1.1",
+            features_bit=5,
+        ),
+    )
+    """Average Speed"""
+
+    energy: EnergyData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=9,
+        ),
+    )
+    """Energy Data"""
+
+    heart_rate: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+            features_bit=10,
+        ),
+    )
+    """Heart Rate"""
+
+    metabolic_equivalent: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s1.1",
+            features_bit=11,
+        ),
+    )
+    """Metabolic Equivalent"""
+
+    time_elapsed: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=12,
+        ),
+    )
+    """Elapsed Time"""
+
+    time_remaining: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=13,
+        ),
+    )
+    """Remaining Time"""
+
+    force_on_belt: ForceOnBeltData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=15,
+        ),
+    )
+    """Force On Belt and Power Output"""
```

### Comparing `pyftms-0.1.0/pyftms/models/realtime_data/treadmill.py` & `pyftms-0.1.1/pyftms/models/realtime_data/cross_trainer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,137 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-
-from .common import (
-    BaseModel,
-    ElevationGainData,
-    EnergyData,
-    InclinationData,
-    RealtimeSpeedData,
-    model_meta,
-)
-
-
-@dc.dataclass(frozen=True)
-class ForceOnBeltData(BaseModel):
-    force_on_belt: int = dc.field(
-        metadata=model_meta(
-            format="s2",
-        ),
-    )
-    """Force On Belt"""
-
-    power_output: int = dc.field(
-        metadata=model_meta(
-            format="s2",
-        ),
-    )
-    """Output Power"""
-
-
-@dc.dataclass(frozen=True)
-class TreadmillData(RealtimeSpeedData):
-    distance_total: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u3",
-            features_bit=2,
-        ),
-    )
-    """Total Distance"""
-
-    inclination: InclinationData | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            features_bit=3,
-        ),
-    )
-    """Inclination and Ramp Angle Data"""
-
-    elevation_gain: ElevationGainData | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            features_bit=4,
-        ),
-    )
-    """Elevation Gain Data"""
-
-    pace_instant: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s1.1",
-            features_bit=5,
-        ),
-    )
-    """Instantaneous Speed"""
-
-    pace_average: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s1.1",
-            features_bit=5,
-        ),
-    )
-    """Average Speed"""
-
-    energy: EnergyData | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            features_bit=9,
-        ),
-    )
-    """Energy Data"""
-
-    heart_rate: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u1",
-            features_bit=10,
-        ),
-    )
-    """Heart Rate"""
-
-    metabolic_equivalent: float | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="s1.1",
-            features_bit=11,
-        ),
-    )
-    """Metabolic Equivalent"""
-
-    time_elapsed: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=12,
-        ),
-    )
-    """Elapsed Time"""
-
-    time_remaining: int | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            format="u2",
-            features_bit=13,
-        ),
-    )
-    """Remaining Time"""
-
-    force_on_belt: ForceOnBeltData | None = dc.field(
-        default=None,
-        metadata=model_meta(
-            features_bit=15,
-        ),
-    )
-    """Force On Belt and Power Output"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+
+from ...client.properties import MovementDirection
+from .common import (
+    ElevationGainData,
+    EnergyData,
+    InclinationData,
+    RealtimeSpeedData,
+    StepRateData,
+    model_meta,
+)
+
+
+@dc.dataclass(frozen=True)
+class CrossTrainerData(RealtimeSpeedData):
+    distance_total: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u3",
+            features_bit=2,
+        ),
+    )
+    """Total Distance"""
+
+    step_rate: StepRateData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=6,
+        ),
+    )
+    """Step Rate Data"""
+
+    stride_count: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=8,
+        ),
+    )
+    """Stride Count"""
+
+    elevation_gain: ElevationGainData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=4,
+        ),
+    )
+    """Elevation Gain Data"""
+
+    inclination: InclinationData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=3,
+        ),
+    )
+    """Inclination and Ramp Angle Data"""
+
+    resistance_level: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2.1",
+            features_bit=7,
+        ),
+    )
+    """Resistance Level"""
+
+    power_instant: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2",
+            features_bit=14,
+        ),
+    )
+    """Instantaneous Power"""
+
+    power_average: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s2",
+            features_bit=14,
+        ),
+    )
+    """Average Power"""
+
+    energy: EnergyData | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            features_bit=9,
+        ),
+    )
+    """Energy Data"""
+
+    heart_rate: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u1",
+            features_bit=10,
+        ),
+    )
+    """Heart Rate"""
+
+    metabolic_equivalent: float | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="s1.1",
+            features_bit=11,
+        ),
+    )
+    """Metabolic Equivalent"""
+
+    time_elapsed: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=12,
+        ),
+    )
+    """Elapsed Time"""
+
+    time_remaining: int | None = dc.field(
+        default=None,
+        metadata=model_meta(
+            format="u2",
+            features_bit=13,
+        ),
+    )
+    """Remaining Time"""
+
+    movement_direction: MovementDirection = dc.field(init=False)
+    """Movement Direction"""
+
+    def __post_init__(self, mask: int):
+        md = MovementDirection.BACKWARD if mask & 0x8000 else MovementDirection.FORWARD
+        object.__setattr__(self, "movement_direction", md)
```

### Comparing `pyftms-0.1.0/pyftms/models/spin_down.py` & `pyftms-0.1.1/pyftms/models/spin_down.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-from enum import STRICT, IntEnum, auto
-
-from .common import BaseModel, model_meta
-
-
-class SpinDownStatusCode(IntEnum, boundary=STRICT):
-    """
-    Spin Down Status.
-
-    Described in section `4.17 Fitness Machine Status. Table 4.27`.
-    """
-
-    REQUESTED = auto()
-    """Spin Down Requested"""
-
-    SUCCESS = auto()
-    """Success"""
-
-    ERROR = auto()
-    """Error"""
-
-    STOP_PEDALING = auto()
-    """Stop Pedaling"""
-
-
-class SpinDownControlCode(IntEnum, boundary=STRICT):
-    """
-    Spin Down Status.
-
-    Described in section `4.17 Fitness Machine Status. Table 4.27`.
-    """
-
-    START = auto()
-    """Spin Down Requested"""
-
-    IGNORE = auto()
-    """Success"""
-
-
-@dc.dataclass(frozen=True)
-class SpinDownSpeedData(BaseModel):
-    """
-    Response Parameter when the Spin Down Procedure succeeds.
-
-    Described in section `4.16.2.20 Spin Down Control Procedure`.
-    """
-
-    low: float = dc.field(
-        metadata=model_meta(
-            format="u2.01",
-        )
-    )
-    """Target Speed Low | km/h"""
-
-    high: float = dc.field(
-        metadata=model_meta(
-            format="u2.01",
-        )
-    )
-    """Target Speed High | km/h"""
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+from enum import STRICT, IntEnum, auto
+
+from .common import BaseModel, model_meta
+
+
+class SpinDownStatusCode(IntEnum, boundary=STRICT):
+    """
+    Spin Down Status.
+
+    Described in section `4.17 Fitness Machine Status. Table 4.27`.
+    """
+
+    REQUESTED = auto()
+    """Spin Down Requested"""
+
+    SUCCESS = auto()
+    """Success"""
+
+    ERROR = auto()
+    """Error"""
+
+    STOP_PEDALING = auto()
+    """Stop Pedaling"""
+
+
+class SpinDownControlCode(IntEnum, boundary=STRICT):
+    """
+    Spin Down Status.
+
+    Described in section `4.17 Fitness Machine Status. Table 4.27`.
+    """
+
+    START = auto()
+    """Spin Down Requested"""
+
+    IGNORE = auto()
+    """Success"""
+
+
+@dc.dataclass(frozen=True)
+class SpinDownSpeedData(BaseModel):
+    """
+    Response Parameter when the Spin Down Procedure succeeds.
+
+    Described in section `4.16.2.20 Spin Down Control Procedure`.
+    """
+
+    low: float = dc.field(
+        metadata=model_meta(
+            format="u2.01",
+        )
+    )
+    """Target Speed Low | km/h"""
+
+    high: float = dc.field(
+        metadata=model_meta(
+            format="u2.01",
+        )
+    )
+    """Target Speed High | km/h"""
```

### Comparing `pyftms-0.1.0/pyftms/serializer/model.py` & `pyftms-0.1.1/pyftms/serializer/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,267 +1,274 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import dataclasses as dc
-import io
-from types import GenericAlias, MappingProxyType, UnionType
-from typing import (
-    Any,
-    ClassVar,
-    Generic,
-    Optional,
-    Self,
-    TypedDict,
-    TypeVar,
-    Union,
-    cast,
-    get_args,
-    get_origin,
-    overload,
-    override,
-)
-
-from .list import ListSerializer
-from .num import NumSerializer
-from .serializer import Serializer
-
-
-class ModelMeta(TypedDict):
-    format: str
-    features_bit: int | None
-    code: int | None
-    num: int | None
-
-
-def model_meta(
-    *,
-    format: str = "",
-    features_bit: int | None = None,
-    code: int | None = None,
-    num: int | None = None,
-):
-    return ModelMeta(
-        format=format,
-        features_bit=features_bit,
-        code=code,
-        num=num,
-    )
-
-
-@dc.dataclass(frozen=True)
-class BaseModel:
-    _serializers: ClassVar[MappingProxyType[str, Serializer]]
-
-    @staticmethod
-    def _get_field_serializer(field: dc.Field):
-        meta, tp = cast(ModelMeta, field.metadata), field.type
-
-        if get_origin(tp) in (Optional, Union, UnionType):
-            if (tp := get_args(tp)[0]) is None:
-                raise TypeError("Failed to get first type.")
-
-        if isinstance(tp, TypeVar):
-            if (tp := tp.__bound__) is None:
-                raise TypeError("TypeVar must have bound type.")
-
-        def _fun(tp):
-            if issubclass(tp, (int, float)):
-                if fmt := meta.get("format"):
-                    return get_serializer(fmt)
-
-                raise TypeError(f"Format string for field '{field.name}' is required.")
-
-            if issubclass(tp, BaseModel):
-                return get_serializer(tp)
-
-            if isinstance(tp, GenericAlias):
-                if (num := meta.get("num")) is None:
-                    raise TypeError("Number of elements is required.")
-
-                serializer = _fun(get_args(tp)[0])
-
-                return ListSerializer(serializer, num)
-
-            raise TypeError("Unsupported type.")
-
-        return _fun(tp)
-
-    @classmethod
-    def _get_fields_serializers(cls) -> MappingProxyType[str, Serializer]:
-        """Generate tuples of Fields and its Serializers."""
-        if (s := getattr(cls, "_serializers", None)) is None:
-            lst: dict[str, Serializer] = {}
-
-            for field in dc.fields(cls):
-                if field.metadata:
-                    lst[field.name] = cls._get_field_serializer(field)
-
-            setattr(cls, "_serializers", s := MappingProxyType(lst))
-
-        return s
-
-    @classmethod
-    def _iter_fields_serializers(cls):
-        """Generate tuples of Fields and its Serializers."""
-        serializers = cls._get_fields_serializers()
-
-        for field in dc.fields(cls):
-            if (s := serializers.get(field.name)) is not None:
-                yield field, s
-
-    @classmethod
-    def _deserialize_dict(cls, src: io.IOBase) -> dict[str, Any]:
-        kwargs = {}
-
-        for k, s in cls._iter_fields_serializers():
-            val, tp = s._deserialize(src), k.type
-
-            if get_origin(tp) in (Optional, Union, UnionType):
-                if (tp := get_args(tp)[0]) is None:
-                    raise TypeError("Failed to get first type.")
-
-            if isinstance(s, (NumSerializer, ListSerializer)):
-                val = tp(val)
-
-            kwargs[k.name] = val
-
-        return kwargs
-
-    @classmethod
-    def _deserialize(cls, src: io.IOBase) -> Self:
-        return cls(**cls._deserialize_dict(src))
-
-    def _serialize(self, dst: io.IOBase) -> int:
-        written = 0
-
-        for k, s in self._iter_fields_serializers():
-            if (val := getattr(self, k.name)) is not None:
-                written += s.serialize(dst, val)
-
-        return written
-
-    @classmethod
-    def _calc_size(cls) -> int:
-        return sum(s.get_size() for _, s in cls._iter_fields_serializers())
-
-    def _asdict(self, *, nested: bool = False):
-        def _transform(input: dict):
-            for key in tuple(input.keys()):
-                if (value := input[key]) is None:
-                    input.pop(key)
-
-                elif isinstance(value, dict):
-                    _transform(value)
-
-                    if not nested:
-                        input.pop(key)
-                        input |= value
-
-        _transform(result := dc.asdict(self))
-
-        return result
-
-    @classmethod
-    def _get_features(cls, features: int) -> tuple[str, ...]:
-        result = []
-
-        def _get_cls_features(cls):
-            for field in dc.fields(cls):
-                meta, tp = cast(ModelMeta, field.metadata), field.type
-
-                if not meta:
-                    continue
-
-                if get_origin(tp) in (Optional, Union, UnionType):
-                    if (tp := get_args(tp)[0]) is None:
-                        raise TypeError("Failed to get first type.")
-
-                if (bit := meta.get("features_bit")) is None or features & (1 << bit):
-                    if isinstance(tp, type) and issubclass(tp, BaseModel):
-                        _get_cls_features(tp)
-                        continue
-
-                    result.append(field.name)
-
-        _get_cls_features(cls)
-
-        return tuple(result[1:])  # skip 'mask' or 'code' field
-
-    def __post_init__(self, *args, **kwargs):
-        for field in dc.fields(self):
-            if (val := getattr(self, field.name)) is None:
-                continue
-
-            meta = cast(ModelMeta, field.metadata)
-
-            if (num := meta.get("num")) and len(val) != num:
-                raise ValueError(f"Length of field '{field.name}' must be {num}.")
-
-    @classmethod
-    def _get_serializer(cls) -> Serializer[Self]:
-        return get_serializer(cls)
-
-
-# MODEL SERIALIZER
-
-BaseModelT = TypeVar("BaseModelT", bound="BaseModel")
-
-
-class ModelSerializer(Generic[BaseModelT], Serializer[BaseModelT]):
-    """Model Serializer"""
-
-    def __init__(self, cls: type[BaseModelT]) -> None:
-        self._cls = cls
-
-    @override
-    def _deserialize(self, src: io.IOBase) -> BaseModelT:
-        return self._cls._deserialize(src)
-
-    @override
-    def serialize(self, writer: io.IOBase, value: BaseModelT) -> int:
-        return value._serialize(writer)
-
-    @override
-    def get_size(self) -> int:
-        return self._cls._calc_size()
-
-
-# SERIALIZERS REGISTRY
-
-_registry: dict[str | type[BaseModel], Serializer] = {}
-"""Serializers Registry"""
-
-
-@overload
-def get_serializer(arg: str, num: None = None) -> NumSerializer: ...
-
-
-@overload
-def get_serializer(
-    arg: type[BaseModelT], num: None = None
-) -> ModelSerializer[BaseModelT]: ...
-
-
-@overload
-def get_serializer(arg: str, num: int) -> ListSerializer[NumSerializer]: ...
-
-
-@overload
-def get_serializer(
-    arg: type[BaseModelT], num: int
-) -> ListSerializer[ModelSerializer[BaseModelT]]: ...
-
-
-def get_serializer(arg: str | type[BaseModel], num: int | None = None):
-    if (serializer := _registry.get(arg)) is None:
-        if isinstance(arg, str):
-            serializer = NumSerializer(arg)
-
-        elif isinstance(arg, type) and issubclass(arg, BaseModel):
-            serializer = ModelSerializer(arg)
-
-        else:
-            raise TypeError(f"Unsupported type {arg}.")
-
-        _registry[arg] = serializer
-
-    return serializer if num is None else ListSerializer(serializer, num)
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import dataclasses as dc
+import io
+from types import GenericAlias, MappingProxyType, UnionType
+from typing import (
+    Any,
+    ClassVar,
+    Generic,
+    Iterator,
+    Optional,
+    Self,
+    TypedDict,
+    TypeVar,
+    Union,
+    cast,
+    get_args,
+    get_origin,
+    overload,
+    override,
+)
+
+from .list import ListSerializer
+from .num import NumSerializer
+from .serializer import Serializer
+
+
+class ModelMeta(TypedDict, total=False):
+    format: str
+    features_bit: int
+    code: int
+    num: int
+
+
+def model_meta(
+    *,
+    format: str = "",
+    features_bit: int | None = None,
+    code: int | None = None,
+    num: int | None = None,
+) -> ModelMeta:
+    result = ModelMeta(format=format)
+
+    if features_bit is not None:
+        result["features_bit"] = features_bit
+
+    if code is not None:
+        result["code"] = code
+
+    if num is not None:
+        result["num"] = num
+
+    return result
+
+
+def _get_model_field_serializer(field: dc.Field):
+    meta, type_ = cast(ModelMeta, field.metadata), field.type
+
+    if get_origin(type_) in (Optional, Union, UnionType):
+        if (type_ := get_args(type_)[0]) is None:
+            raise TypeError("Failed to get first type.")
+
+    if isinstance(type_, TypeVar):
+        if (type_ := type_.__bound__) is None:
+            raise TypeError("'TypeVar' must have bound type.")
+
+    def _get_serializer(type_) -> Serializer:
+        if issubclass(type_, (int, float)):
+            if fmt := meta.get("format"):
+                return get_serializer(fmt)
+
+            raise TypeError(f"Format string for field '{field.name}' is required.")
+
+        if issubclass(type_, BaseModel):
+            return get_serializer(type_)
+
+        if isinstance(type_, GenericAlias):
+            if (num := meta.get("num")) is None:
+                raise TypeError("Number of elements is required.")
+
+            serializer = _get_serializer(get_args(type_)[0])
+
+            return ListSerializer(serializer, num)
+
+        raise TypeError("Unsupported type.")
+
+    return _get_serializer(type_)
+
+
+def _get_model_serializers(cls: type["BaseModel"]) -> MappingProxyType[str, Serializer]:
+    """Generate tuples of Fields and its Serializers."""
+    if (serializers_ := getattr(cls, "_model_serializers", None)) is None:
+        result: dict[str, Serializer] = {}
+
+        for field in dc.fields(cls):
+            if field.metadata:
+                result[field.name] = _get_model_field_serializer(field)
+
+        setattr(cls, "_model_serializers", serializers_ := MappingProxyType(result))
+
+    return serializers_
+
+
+@dc.dataclass(frozen=True)
+class BaseModel:
+    _model_serializers: ClassVar[MappingProxyType[str, Serializer]]
+
+    @classmethod
+    def _iter_fields_serializers(cls) -> Iterator[tuple[dc.Field, Serializer]]:
+        """Generate tuples of Fields and its Serializers."""
+        serializers = _get_model_serializers(cls)
+
+        for field in dc.fields(cls):
+            if (serializer := serializers.get(field.name)) is not None:
+                yield field, serializer
+
+    @classmethod
+    def _deserialize_asdict(cls, src: io.IOBase) -> dict[str, Any]:
+        kwargs = {}
+
+        for field, serializer in cls._iter_fields_serializers():
+            value, type_ = serializer._deserialize(src), field.type
+
+            if get_origin(type_) in (Optional, Union, UnionType):
+                if (type_ := get_args(type_)[0]) is None:
+                    raise TypeError("Failed to get first type.")
+
+            if isinstance(serializer, (NumSerializer, ListSerializer)):
+                value = type_(value)
+
+            kwargs[field.name] = value
+
+        return kwargs
+
+    @classmethod
+    def _deserialize(cls, src: io.IOBase) -> Self:
+        return cls(**cls._deserialize_asdict(src))
+
+    def _serialize(self, dst: io.IOBase) -> int:
+        written = 0
+
+        for field, serializer in self._iter_fields_serializers():
+            if (val := getattr(self, field.name)) is not None:
+                written += serializer.serialize(dst, val)
+
+        return written
+
+    @classmethod
+    def _calc_size(cls) -> int:
+        return sum(s.get_size() for _, s in cls._iter_fields_serializers())
+
+    def _asdict(self, *, nested: bool = False):
+        def _transform(input: dict):
+            for key in tuple(input.keys()):
+                if (value := input[key]) is None:
+                    input.pop(key)
+
+                elif isinstance(value, dict):
+                    _transform(value)
+
+                    if not nested:
+                        input.pop(key)
+                        input |= value
+
+        _transform(result := dc.asdict(self))
+
+        return result
+
+    @classmethod
+    def _get_features(cls, features: int) -> tuple[str, ...]:
+        result = []
+
+        def _get_cls_features(cls):
+            for field in dc.fields(cls):
+                meta, tp = cast(ModelMeta, field.metadata), field.type
+
+                if not meta:
+                    continue
+
+                if get_origin(tp) in (Optional, Union, UnionType):
+                    if (tp := get_args(tp)[0]) is None:
+                        raise TypeError("Failed to get first type.")
+
+                if (bit := meta.get("features_bit")) is None or features & (1 << bit):
+                    if isinstance(tp, type) and issubclass(tp, BaseModel):
+                        _get_cls_features(tp)
+                        continue
+
+                    result.append(field.name)
+
+        _get_cls_features(cls)
+
+        return tuple(result[1:])  # skip 'mask' or 'code' field
+
+    def __post_init__(self, *args, **kwargs):
+        for field in dc.fields(self):
+            if (val := getattr(self, field.name)) is None:
+                continue
+
+            meta = cast(ModelMeta, field.metadata)
+
+            if (num := meta.get("num")) and len(val) != num:
+                raise ValueError(f"Length of field '{field.name}' must be {num}.")
+
+    @classmethod
+    def _get_serializer(cls) -> Serializer[Self]:
+        return get_serializer(cls)
+
+
+# MODEL SERIALIZER
+
+BaseModelT = TypeVar("BaseModelT", bound="BaseModel")
+
+
+class ModelSerializer(Generic[BaseModelT], Serializer[BaseModelT]):
+    """Model Serializer"""
+
+    def __init__(self, cls: type[BaseModelT]) -> None:
+        self._cls = cls
+
+    @override
+    def _deserialize(self, src: io.IOBase) -> BaseModelT:
+        return self._cls._deserialize(src)
+
+    @override
+    def serialize(self, writer: io.IOBase, value: BaseModelT) -> int:
+        return value._serialize(writer)
+
+    @override
+    def get_size(self) -> int:
+        return self._cls._calc_size()
+
+
+# SERIALIZERS REGISTRY
+
+_registry: dict[str | type[BaseModel], Serializer] = {}
+"""Serializers Registry"""
+
+
+@overload
+def get_serializer(arg: str, num: None = None) -> NumSerializer: ...
+
+
+@overload
+def get_serializer(
+    arg: type[BaseModelT], num: None = None
+) -> ModelSerializer[BaseModelT]: ...
+
+
+@overload
+def get_serializer(arg: str, num: int) -> ListSerializer[NumSerializer]: ...
+
+
+@overload
+def get_serializer(
+    arg: type[BaseModelT], num: int
+) -> ListSerializer[ModelSerializer[BaseModelT]]: ...
+
+
+def get_serializer(arg: str | type[BaseModel], num: int | None = None):
+    if (serializer := _registry.get(arg)) is None:
+        if isinstance(arg, str):
+            serializer = NumSerializer(arg)
+
+        elif isinstance(arg, type) and issubclass(arg, BaseModel):
+            serializer = ModelSerializer(arg)
+
+        else:
+            raise TypeError(f"Unsupported type {arg}.")
+
+        _registry[arg] = serializer
+
+    return serializer if num is None else ListSerializer(serializer, num)
```

### Comparing `pyftms-0.1.0/pyftms/serializer/num.py` & `pyftms-0.1.1/pyftms/serializer/num.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# Copyright 2024, Sergey Dudanov
-# SPDX-License-Identifier: Apache-2.0
-
-import io
-import re
-from typing import override
-
-from .serializer import Serializer
-
-SupportedNumbers = int | float
-
-_PARAM_PATTERN = re.compile(r"[us][1-8](\.\d{1,8})?$")
-
-
-def _parse_fmt(fmt: str) -> tuple[int, float | None, bool]:
-    if m := _PARAM_PATTERN.match(fmt):
-        x = m.group(1)
-        return int(fmt[1]), None if x is None else float(x), fmt[0] == "s"
-    raise ValueError("Wrong serializer format.")
-
-
-class NumSerializer(Serializer[SupportedNumbers]):
-    """
-    A simple class for reading/writing numbers from/to a stream.
-
-    Stores the necessary parameters, including those for autoscaling during operations.
-    """
-
-    __slots__ = "size", "factor", "sign"
-
-    def __init__(self, format: str) -> None:
-        self.size, self.factor, self.sign = _parse_fmt(format)
-
-    @override
-    def _deserialize(self, src: io.IOBase) -> SupportedNumbers:
-        """
-        Reads a number from a stream, scaling it if necessary.
-
-        Raise an `EOFError` exception if the stream ends unexpectedly.
-
-        Parameters:
-            reader: IOBase - I/O reader.
-        Returns:
-            SupportedValueTypes - readed value.
-        """
-        data = src.read(self.size)
-
-        if len(data) != self.size:
-            raise EOFError("Unexpected end of stream.")
-
-        val = int.from_bytes(data, "little", signed=self.sign)
-
-        if self.factor:
-            val *= self.factor
-
-        return val
-
-    @override
-    def serialize(self, dst: io.IOBase, value: SupportedNumbers) -> int:
-        """
-        Writes a number to a stream, pre-scaling if necessary.
-
-        Parameters:
-            writer: IOBase - I/O writer.
-            value: SupportedValueTypes - value to write.
-        Returns:
-            int - number of written bytes.
-        """
-        if self.factor:
-            value /= self.factor
-
-        b = int(value).to_bytes(self.size, "little", signed=self.sign)
-        return dst.write(b)
-
-    @override
-    def get_size(self) -> int:
-        return self.size
+# Copyright 2024, Sergey Dudanov
+# SPDX-License-Identifier: Apache-2.0
+
+import io
+import re
+from typing import override
+
+from .serializer import Serializer
+
+SupportedNumbers = int | float
+
+_PARAM_PATTERN = re.compile(r"[us][1-8](\.\d{1,8})?$")
+
+
+def _parse_fmt(fmt: str) -> tuple[int, float | None, bool]:
+    if m := _PARAM_PATTERN.match(fmt):
+        x = m.group(1)
+        return int(fmt[1]), None if x is None else float(x), fmt[0] == "s"
+    raise ValueError("Wrong serializer format.")
+
+
+class NumSerializer(Serializer[SupportedNumbers]):
+    """
+    A simple class for reading/writing numbers from/to a stream.
+
+    Stores the necessary parameters, including those for autoscaling during operations.
+    """
+
+    __slots__ = "size", "factor", "sign"
+
+    def __init__(self, format: str) -> None:
+        self.size, self.factor, self.sign = _parse_fmt(format)
+
+    @override
+    def _deserialize(self, src: io.IOBase) -> SupportedNumbers:
+        """
+        Reads a number from a stream, scaling it if necessary.
+
+        Raise an `EOFError` exception if the stream ends unexpectedly.
+
+        Parameters:
+            reader: IOBase - I/O reader.
+        Returns:
+            SupportedValueTypes - readed value.
+        """
+        data = src.read(self.size)
+
+        if len(data) != self.size:
+            raise EOFError("Unexpected end of stream.")
+
+        val = int.from_bytes(data, "little", signed=self.sign)
+
+        if self.factor:
+            val *= self.factor
+
+        return val
+
+    @override
+    def serialize(self, dst: io.IOBase, value: SupportedNumbers) -> int:
+        """
+        Writes a number to a stream, pre-scaling if necessary.
+
+        Parameters:
+            writer: IOBase - I/O writer.
+            value: SupportedValueTypes - value to write.
+        Returns:
+            int - number of written bytes.
+        """
+        if self.factor:
+            value /= self.factor
+
+        b = int(value).to_bytes(self.size, "little", signed=self.sign)
+        return dst.write(b)
+
+    @override
+    def get_size(self) -> int:
+        return self.size
```

