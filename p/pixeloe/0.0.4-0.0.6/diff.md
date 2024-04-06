# Comparing `tmp/pixeloe-0.0.4.tar.gz` & `tmp/pixeloe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixeloe-0.0.4.tar", last modified: Sat Mar 30 13:21:53 2024, max compression
+gzip compressed data, was "pixeloe-0.0.6.tar", last modified: Sat Apr  6 13:36:29 2024, max compression
```

## Comparing `pixeloe-0.0.4.tar` & `pixeloe-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 13:21:53.839244 pixeloe-0.0.4/
--rw-rw-rw-   0        0        0    11545 2024-03-28 13:15:23.000000 pixeloe-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      391 2024-03-30 13:21:53.837244 pixeloe-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4208 2024-03-30 09:44:07.000000 pixeloe-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 13:21:53.808916 pixeloe-0.0.4/pixeloe/
--rw-rw-rw-   0        0        0       31 2024-03-28 14:27:48.000000 pixeloe-0.0.4/pixeloe/__init__.py
--rw-rw-rw-   0        0        0     1923 2024-03-30 13:21:08.000000 pixeloe-0.0.4/pixeloe/cli.py
--rw-rw-rw-   0        0        0     1989 2024-03-28 13:33:48.000000 pixeloe-0.0.4/pixeloe/color.py
-drwxrwxrwx   0        0        0        0 2024-03-30 13:21:53.836244 pixeloe-0.0.4/pixeloe/downscale/
--rw-rw-rw-   0        0        0      376 2024-03-30 13:21:20.000000 pixeloe-0.0.4/pixeloe/downscale/__init__.py
--rw-rw-rw-   0        0        0     1155 2024-03-30 07:54:22.000000 pixeloe-0.0.4/pixeloe/downscale/center.py
--rw-rw-rw-   0        0        0     1651 2024-03-30 13:12:14.000000 pixeloe-0.0.4/pixeloe/downscale/contrast_based.py
--rw-rw-rw-   0        0        0      622 2024-03-30 08:45:51.000000 pixeloe-0.0.4/pixeloe/downscale/conventional.py
--rw-rw-rw-   0        0        0     1823 2024-03-30 07:42:24.000000 pixeloe-0.0.4/pixeloe/downscale/k_centroid.py
--rw-rw-rw-   0        0        0     2813 2024-03-30 02:48:16.000000 pixeloe-0.0.4/pixeloe/outline.py
--rw-rw-rw-   0        0        0     1478 2024-03-30 07:35:31.000000 pixeloe-0.0.4/pixeloe/pixelize.py
--rw-rw-rw-   0        0        0      904 2024-03-30 13:07:36.000000 pixeloe-0.0.4/pixeloe/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-30 13:21:53.837244 pixeloe-0.0.4/pixeloe.egg-info/
--rw-rw-rw-   0        0        0      391 2024-03-30 13:21:53.000000 pixeloe-0.0.4/pixeloe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2024-03-30 13:21:53.000000 pixeloe-0.0.4/pixeloe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 13:21:53.000000 pixeloe-0.0.4/pixeloe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-30 13:21:53.000000 pixeloe-0.0.4/pixeloe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-03-28 13:14:12.000000 pixeloe-0.0.4/pixeloe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2024-03-30 13:21:53.000000 pixeloe-0.0.4/pixeloe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-30 13:21:53.000000 pixeloe-0.0.4/pixeloe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 13:21:53.839244 pixeloe-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      560 2024-03-30 13:21:48.000000 pixeloe-0.0.4/setup.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:36:29.394222 pixeloe-0.0.6/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2024-03-29 05:43:29.000000 pixeloe-0.0.6/LICENSE
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-06 13:36:29.393959 pixeloe-0.0.6/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     7508 2024-04-01 04:05:40.000000 pixeloe-0.0.6/README.md
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:36:29.391222 pixeloe-0.0.6/pixeloe/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       31 2024-03-29 05:43:29.000000 pixeloe-0.0.6/pixeloe/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3637 2024-04-06 13:34:12.000000 pixeloe-0.0.6/pixeloe/cli.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2223 2024-04-06 13:28:46.000000 pixeloe-0.0.6/pixeloe/color.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:36:29.393353 pixeloe-0.0.6/pixeloe/downscale/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      363 2024-03-31 16:49:46.000000 pixeloe-0.0.6/pixeloe/downscale/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1113 2024-03-31 16:49:46.000000 pixeloe-0.0.6/pixeloe/downscale/center.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1554 2024-03-31 16:49:46.000000 pixeloe-0.0.6/pixeloe/downscale/contrast_based.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      894 2024-03-31 16:49:46.000000 pixeloe-0.0.6/pixeloe/downscale/conventional.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1772 2024-03-31 16:49:46.000000 pixeloe-0.0.6/pixeloe/downscale/k_centroid.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3189 2024-04-06 13:31:59.000000 pixeloe-0.0.6/pixeloe/outline.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1863 2024-04-06 13:31:13.000000 pixeloe-0.0.6/pixeloe/pixelize.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      951 2024-04-06 13:31:13.000000 pixeloe-0.0.6/pixeloe/utils.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2024-04-06 13:36:29.393708 pixeloe-0.0.6/pixeloe.egg-info/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      407 2024-04-06 13:36:29.000000 pixeloe-0.0.6/pixeloe.egg-info/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      512 2024-04-06 13:36:29.000000 pixeloe-0.0.6/pixeloe.egg-info/SOURCES.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-04-06 13:36:29.000000 pixeloe-0.0.6/pixeloe.egg-info/dependency_links.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       96 2024-04-06 13:36:29.000000 pixeloe-0.0.6/pixeloe.egg-info/entry_points.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2024-03-29 05:49:33.000000 pixeloe-0.0.6/pixeloe.egg-info/not-zip-safe
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       27 2024-04-06 13:36:29.000000 pixeloe-0.0.6/pixeloe.egg-info/requires.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2024-04-06 13:36:29.000000 pixeloe-0.0.6/pixeloe.egg-info/top_level.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2024-04-06 13:36:29.394272 pixeloe-0.0.6/setup.cfg
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      707 2024-04-06 13:36:23.000000 pixeloe-0.0.6/setup.py
```

### Comparing `pixeloe-0.0.4/LICENSE` & `pixeloe-0.0.6/LICENSE`

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
-   Copyright 2024 KohakuBlueLeaf
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
+   Copyright 2024 KohakuBlueLeaf
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

### Comparing `pixeloe-0.0.4/pixeloe/color.py` & `pixeloe-0.0.6/pixeloe/color.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,62 @@
-import numpy as np
-import cv2
-
-
-def match_color(source, target):
-    # Convert RGB to L*a*b*, and then match the std/mean
-    source_lab = cv2.cvtColor(source, cv2.COLOR_BGR2LAB).astype(np.float32) / 255
-    target_lab = cv2.cvtColor(target, cv2.COLOR_BGR2LAB).astype(np.float32) / 255
-    result = (source_lab - np.mean(source_lab)) / np.std(source_lab)
-    result = result * np.std(target_lab) + np.mean(target_lab)
-    source = cv2.cvtColor(
-        (result * 255).clip(0, 255).astype(np.uint8), cv2.COLOR_LAB2BGR
-    )
-
-    source = source.astype(np.float32)
-    # Use wavelet colorfix method to match original low frequency data at first
-    source[:, :, 0] = wavelet_colorfix(source[:, :, 0], target[:, :, 0])
-    source[:, :, 1] = wavelet_colorfix(source[:, :, 1], target[:, :, 1])
-    source[:, :, 2] = wavelet_colorfix(source[:, :, 2], target[:, :, 2])
-    output = source
-    return output.clip(0, 255).astype(np.uint8)
-
-
-def wavelet_colorfix(input, target):
-    input_high, _ = wavelet_decomposition(input, 5)
-    _, target_low = wavelet_decomposition(target, 5)
-    output = input_high + target_low
-    return output
-
-
-def wavelet_decomposition(input, levels):
-    high_freq = np.zeros_like(input)
-    for i in range(1, levels + 1):
-        radius = 2**i
-        low_freq = wavelet_blur(input, radius)
-        high_freq = high_freq + (input - low_freq)
-        input = low_freq
-    return high_freq, low_freq
-
-
-def wavelet_blur(input, radius):
-    kernel_size = 2 * radius + 1
-    output = cv2.GaussianBlur(input, (kernel_size, kernel_size), 0)
-    return output
-
-
-def color_styling(input, saturation=1.2, contrast=1.1):
-    output = input.copy()
-    output = cv2.cvtColor(output, cv2.COLOR_BGR2HSV)
-    output[:, :, 1] = output[:, :, 1] * saturation
-    output[:, :, 2] = output[:, :, 2] * contrast - (contrast - 1)
-    output = np.clip(output, 0, 1)
-    output = cv2.cvtColor(output, cv2.COLOR_HSV2BGR)
-    return output
+import cv2
+import numpy as np
+from PIL import Image
+
+
+def match_color(source, target):
+    # Convert RGB to L*a*b*, and then match the std/mean
+    source_lab = cv2.cvtColor(source, cv2.COLOR_BGR2LAB).astype(np.float32) / 255
+    target_lab = cv2.cvtColor(target, cv2.COLOR_BGR2LAB).astype(np.float32) / 255
+    result = (source_lab - np.mean(source_lab)) / np.std(source_lab)
+    result = result * np.std(target_lab) + np.mean(target_lab)
+    source = cv2.cvtColor(
+        (result * 255).clip(0, 255).astype(np.uint8), cv2.COLOR_LAB2BGR
+    )
+
+    source = source.astype(np.float32)
+    # Use wavelet colorfix method to match original low frequency data at first
+    source[:, :, 0] = wavelet_colorfix(source[:, :, 0], target[:, :, 0])
+    source[:, :, 1] = wavelet_colorfix(source[:, :, 1], target[:, :, 1])
+    source[:, :, 2] = wavelet_colorfix(source[:, :, 2], target[:, :, 2])
+    output = source
+    return output.clip(0, 255).astype(np.uint8)
+
+
+def wavelet_colorfix(input, target):
+    input_high, _ = wavelet_decomposition(input, 5)
+    _, target_low = wavelet_decomposition(target, 5)
+    output = input_high + target_low
+    return output
+
+
+def wavelet_decomposition(input, levels):
+    high_freq = np.zeros_like(input)
+    for i in range(1, levels + 1):
+        radius = 2**i
+        low_freq = wavelet_blur(input, radius)
+        high_freq = high_freq + (input - low_freq)
+        input = low_freq
+    return high_freq, low_freq
+
+
+def wavelet_blur(input, radius):
+    kernel_size = 2 * radius + 1
+    output = cv2.GaussianBlur(input, (kernel_size, kernel_size), 0)
+    return output
+
+
+def color_styling(input, saturation=1.2, contrast=1.1):
+    output = input.copy()
+    output = cv2.cvtColor(output, cv2.COLOR_BGR2HSV)
+    output[:, :, 1] = output[:, :, 1] * saturation
+    output[:, :, 2] = output[:, :, 2] * contrast - (contrast - 1)
+    output = np.clip(output, 0, 1)
+    output = cv2.cvtColor(output, cv2.COLOR_HSV2BGR)
+    return output
+
+
+def kmeans_color_quant(input, colors=32):
+    img = cv2.cvtColor(input, cv2.COLOR_BGR2RGB)
+    img_pil = Image.fromarray(img)
+    img_quant = img_pil.quantize(colors, 1, kmeans=colors).convert("RGB")
+    return cv2.cvtColor(np.array(img_quant), cv2.COLOR_RGB2BGR)
```

### Comparing `pixeloe-0.0.4/pixeloe/downscale/k_centroid.py` & `pixeloe-0.0.6/pixeloe/downscale/k_centroid.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import math
-from itertools import product
-
-import cv2
-import numpy as np
-from PIL import Image
-
-
-def k_centroid_downscale(cv2img, target_size=128, centroids=2):
-    """
-    k-centroid downscaling algorithm from Astropulse, under MIT License.
-    https://github.com/Astropulse/pixeldetector/blob/6e88e18ddbd16529b5dd85b1c615cbb2e5778bf2/k-centroid.py#L19-L44
-    """
-    H, W, C = cv2img.shape
-
-    ratio = W / H
-    target_size = (target_size**2 / ratio) ** 0.5
-    height = int(target_size)
-    width = int(target_size * ratio)
-
-    # Perform outline expansion and color matching
-    image = Image.fromarray(cv2.cvtColor(cv2img, cv2.COLOR_BGR2RGB)).convert("RGB")
-
-    # Downscale outline expanded image with k-centroid
-    # Create an empty array for the downscaled image
-    downscaled = np.zeros((height, width, 3), dtype=np.uint8)
-
-    # Calculate the scaling factors
-    wFactor = image.width / width
-    hFactor = image.height / height
-
-    # Iterate over each tile in the downscaled image
-    for x, y in product(range(width), range(height)):
-        # Crop the tile from the original image
-        tile = image.crop(
-            (x * wFactor, y * hFactor, (x * wFactor) + wFactor, (y * hFactor) + hFactor)
-        )
-
-        # Quantize the colors of the tile using k-means clustering
-        tile = tile.quantize(colors=centroids, method=1, kmeans=centroids).convert(
-            "RGB"
-        )
-
-        # Get the color counts and find the most common color
-        color_counts = tile.getcolors()
-        most_common_color = max(color_counts, key=lambda x: x[0])[1]
-
-        # Assign the most common color to the corresponding pixel in the downscaled image
-        downscaled[y, x, :] = most_common_color
-
-    return cv2.cvtColor(downscaled, cv2.COLOR_RGB2BGR)
+import math
+from itertools import product
+
+import cv2
+import numpy as np
+from PIL import Image
+
+
+def k_centroid_downscale(cv2img, target_size=128, centroids=2):
+    """
+    k-centroid downscaling algorithm from Astropulse, under MIT License.
+    https://github.com/Astropulse/pixeldetector/blob/6e88e18ddbd16529b5dd85b1c615cbb2e5778bf2/k-centroid.py#L19-L44
+    """
+    H, W, C = cv2img.shape
+
+    ratio = W / H
+    target_size = (target_size**2 / ratio) ** 0.5
+    height = int(target_size)
+    width = int(target_size * ratio)
+
+    # Perform outline expansion and color matching
+    image = Image.fromarray(cv2.cvtColor(cv2img, cv2.COLOR_BGR2RGB)).convert("RGB")
+
+    # Downscale outline expanded image with k-centroid
+    # Create an empty array for the downscaled image
+    downscaled = np.zeros((height, width, 3), dtype=np.uint8)
+
+    # Calculate the scaling factors
+    wFactor = image.width / width
+    hFactor = image.height / height
+
+    # Iterate over each tile in the downscaled image
+    for x, y in product(range(width), range(height)):
+        # Crop the tile from the original image
+        tile = image.crop(
+            (x * wFactor, y * hFactor, (x * wFactor) + wFactor, (y * hFactor) + hFactor)
+        )
+
+        # Quantize the colors of the tile using k-means clustering
+        tile = tile.quantize(colors=centroids, method=1, kmeans=centroids).convert(
+            "RGB"
+        )
+
+        # Get the color counts and find the most common color
+        color_counts = tile.getcolors()
+        most_common_color = max(color_counts, key=lambda x: x[0])[1]
+
+        # Assign the most common color to the corresponding pixel in the downscaled image
+        downscaled[y, x, :] = most_common_color
+
+    return cv2.cvtColor(downscaled, cv2.COLOR_RGB2BGR)
```

### Comparing `pixeloe-0.0.4/pixeloe/outline.py` & `pixeloe-0.0.6/pixeloe/outline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,98 @@
-from functools import partial
-
-import numpy as np
-import cv2
-
-from .utils import sigmoid, apply_chunk
-
-
-def expansion_weight(img, k=8, stride=2, avg_scale=10, dist_scale=3):
-    img_y = cv2.cvtColor(img, cv2.COLOR_BGR2LAB)[:, :, 0] / 255
-    avg_y = apply_chunk(img_y, k * 2, stride, partial(np.median, axis=1, keepdims=True))
-    max_y = apply_chunk(img_y, k, stride, partial(np.max, axis=1, keepdims=True))
-    min_y = apply_chunk(img_y, k, stride, partial(np.min, axis=1, keepdims=True))
-    bright_dist = max_y - avg_y
-    dark_dist = avg_y - min_y
-
-    weight = (avg_y - 0.5) * avg_scale
-    weight = weight - (bright_dist - dark_dist) * dist_scale
-
-    output = sigmoid(weight)
-    output = cv2.resize(
-        output,
-        (img.shape[1] // stride, img.shape[0] // stride),
-        interpolation=cv2.INTER_LINEAR,
-    )
-    output = cv2.resize(
-        output, (img.shape[1], img.shape[0]), interpolation=cv2.INTER_LINEAR
-    )
-
-    return (output - np.min(output)) / (np.max(output))
-
-
-kernel_expansion = np.array([[1, 1, 1], [1, 1, 1], [1, 1, 1]]).astype(np.uint8)
-kernel_smoothing = np.array([[0, 1, 0], [1, 1, 1], [0, 1, 0]]).astype(np.uint8)
-
-
-def outline_expansion(img, erode=2, dilate=2, k=16, avg_scale=10, dist_scale=3):
-    weight = expansion_weight(img, k, (k // 4) * 2, avg_scale, dist_scale)[
-        ..., np.newaxis
-    ]
-    orig_weight = sigmoid((weight - 0.5) * 5) * 0.25
-
-    img_erode = img.copy()
-    img_erode = cv2.erode(img_erode, kernel_expansion, iterations=erode).astype(
-        np.float32
-    )
-    img_dilate = img.copy()
-    img_dilate = cv2.dilate(img_dilate, kernel_expansion, iterations=dilate).astype(
-        np.float32
-    )
-
-    output = img_erode * weight + img_dilate * (1 - weight)
-    output = output * (1 - orig_weight) + img.astype(np.float32) * orig_weight
-    output = output.astype(np.uint8).copy()
-
-    output = cv2.erode(output, kernel_smoothing, iterations=erode)
-    output = cv2.dilate(output, kernel_smoothing, iterations=dilate * 2)
-    output = cv2.erode(output, kernel_smoothing, iterations=erode)
-
-    return output
-
-
-if __name__ == "__main__":
-    img = cv2.imread("img/test.png")
-    H, W, C = img.shape
-    ratio = W / H
-    target_pixel_count = (1024**2 / ratio) ** 0.5
-    img = cv2.resize(img, (int(target_pixel_count * ratio), int(target_pixel_count)))
-    img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-    weight_mat = expansion_weight(img, 8, 2, 9, 3)
-    img_out = outline_expansion(img, 1, 1)
-
-    # show the weight mat and output in matplotlib in same window
-    import matplotlib.pyplot as plt
-
-    plt.subplot(1, 3, 1)
-    plt.imshow(img)
-    plt.subplot(1, 3, 2)
-    plt.imshow(weight_mat)
-    plt.subplot(1, 3, 3)
-    plt.imshow(img_out)
-    plt.show()
+from functools import partial
+
+import cv2
+import numpy as np
+
+from .utils import sigmoid, apply_chunk
+
+
+def expansion_weight(img, k=8, stride=2, avg_scale=10, dist_scale=3):
+    img_y = cv2.cvtColor(img, cv2.COLOR_BGR2LAB)[:, :, 0] / 255
+    avg_y = apply_chunk(img_y, k * 2, stride, partial(np.median, axis=1, keepdims=True))
+    max_y = apply_chunk(img_y, k, stride, partial(np.max, axis=1, keepdims=True))
+    min_y = apply_chunk(img_y, k, stride, partial(np.min, axis=1, keepdims=True))
+    bright_dist = max_y - avg_y
+    dark_dist = avg_y - min_y
+
+    weight = (avg_y - 0.5) * avg_scale
+    weight = weight - (bright_dist - dark_dist) * dist_scale
+
+    output = sigmoid(weight)
+    output = cv2.resize(
+        output,
+        (img.shape[1] // stride, img.shape[0] // stride),
+        interpolation=cv2.INTER_LINEAR,
+    )
+    output = cv2.resize(
+        output, (img.shape[1], img.shape[0]), interpolation=cv2.INTER_LINEAR
+    )
+
+    return (output - np.min(output)) / (np.max(output))
+
+
+kernel_expansion = np.array([[1, 1, 1], [1, 1, 1], [1, 1, 1]]).astype(np.uint8)
+kernel_smoothing = np.array([[0, 1, 0], [1, 1, 1], [0, 1, 0]]).astype(np.uint8)
+
+
+def outline_expansion(img, erode=2, dilate=2, k=16, avg_scale=10, dist_scale=3):
+    weight = expansion_weight(img, k, (k // 4) * 2, avg_scale, dist_scale)[
+        ..., np.newaxis
+    ]
+    orig_weight = sigmoid((weight - 0.5) * 5) * 0.25
+
+    img_erode = img.copy()
+    img_erode = cv2.erode(img_erode, kernel_expansion, iterations=erode).astype(
+        np.float32
+    )
+    img_dilate = img.copy()
+    img_dilate = cv2.dilate(img_dilate, kernel_expansion, iterations=dilate).astype(
+        np.float32
+    )
+
+    output = img_erode * weight + img_dilate * (1 - weight)
+    output = output * (1 - orig_weight) + img.astype(np.float32) * orig_weight
+    output = output.astype(np.uint8).copy()
+
+    output = cv2.erode(output, kernel_smoothing, iterations=erode)
+    output = cv2.dilate(output, kernel_smoothing, iterations=dilate * 2)
+    output = cv2.erode(output, kernel_smoothing, iterations=erode)
+
+    return output
+
+
+if __name__ == "__main__":
+    img = cv2.imread("img/dragon-girl.png")
+    H, W, C = img.shape
+    ratio = W / H
+    target_pixel_count = (1024**2 / ratio) ** 0.5
+    img = cv2.resize(img, (int(target_pixel_count * ratio), int(target_pixel_count)))
+    img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+    weight_mat = expansion_weight(img, 8, 2, 9, 3)
+    img_out = outline_expansion(img, 1, 1)
+
+    edge = img_out - img
+    edge = (edge + 255) / 2
+    edge[np.abs(edge - 127) >= 30] = 0
+    edge[np.abs(edge - 127) < 30] = 255
+    edge = cv2.cvtColor(edge.astype(np.uint8), cv2.COLOR_BGR2GRAY) / 255
+
+    # show the weight mat and output in matplotlib in same window
+    import matplotlib.pyplot as plt
+
+    plt.subplot(1, 4, 1)
+    plt.imshow(img)
+    plt.axis("off")
+    plt.title("input")
+    plt.subplot(1, 4, 2)
+    plt.imshow(img_out)
+    plt.axis("off")
+    plt.title("output")
+    plt.subplot(1, 4, 3)
+    plt.imshow(weight_mat, cmap="gray")
+    plt.axis("off")
+    plt.title("weight")
+    plt.subplot(1, 4, 4)
+    plt.imshow(edge, cmap="gray")
+    plt.axis("off")
+    plt.title("edge")
+    plt.show()
```

### Comparing `pixeloe-0.0.4/pixeloe/pixelize.py` & `pixeloe-0.0.6/pixeloe/pixelize.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,72 @@
-from time import time
-
-import cv2
-
-from .color import match_color, color_styling
-from .downscale import downscale_mode
-from .outline import outline_expansion
-
-
-def pixelize(
-    img,
-    mode="contrast-based",
-    target_size=128,
-    patch_size=16,
-    thickness=2,
-    color_matching=True,
-    contrast=1.0,
-    saturation=1.0,
-    colors=None,
-    no_upscale=False,
-):
-    H, W, C = img.shape
-
-    ratio = W / H
-    target_org_size = (target_size**2 * patch_size**2 / ratio) ** 0.5
-    target_org_hw = (int(target_org_size * ratio), int(target_org_size))
-
-    img = cv2.resize(img, target_org_hw)
-    org_img = img.copy()
-
-    if thickness:
-        img = outline_expansion(img, thickness, thickness, patch_size, 9, 4)
-
-    if color_matching:
-        img = match_color(img, org_img)
-
-    img_sm = downscale_mode[mode](img, target_size)
-
-    if contrast != 1 or saturation != 1:
-        img_sm = color_styling(img_sm, saturation, contrast)
-
-    if no_upscale:
-        return img_sm
-
-    img_lg = cv2.resize(img_sm, (W, H), interpolation=cv2.INTER_NEAREST)
-    return img_lg
-
-
-if __name__ == "__main__":
-    t0 = time()
-    img = cv2.imread("img/test.png")
-    t1 = time()
-    img = pixelize(img, 256, patch_size=8)
-    t2 = time()
-    cv2.imwrite("img/test2.png", img)
-    t3 = time()
-
-    print(f"read time: {t1 - t0:.3f}sec")
-    print(f"pixelize time: {t2 - t1:.3f}sec")
-    print(f"write time: {t3 - t2:.3f}sec")
+from time import time
+
+import cv2
+
+from .color import match_color, color_styling, kmeans_color_quant
+from .downscale import downscale_mode
+from .outline import outline_expansion
+from .utils import isiterable
+
+
+def pixelize(
+    img,
+    mode="contrast",
+    target_size=128,
+    patch_size=16,
+    thickness=2,
+    color_matching=True,
+    contrast=1.0,
+    saturation=1.0,
+    colors=None,
+    no_upscale=False,
+    no_downscale=False,
+):
+    H, W, _ = img.shape
+
+    ratio = W / H
+    if isiterable(target_size):
+        target_org_hw = tuple([int(i * patch_size) for i in target_size][:2])
+        target_org_size = target_org_hw[1]
+        target_size = ((target_org_size**2) / (patch_size**2) * ratio) ** 0.5
+    else:
+        target_org_size = (target_size**2 * patch_size**2 / ratio) ** 0.5
+        target_org_hw = (int(target_org_size * ratio), int(target_org_size))
+
+    img = cv2.resize(img, target_org_hw)
+    org_img = img.copy()
+
+    if thickness:
+        img = outline_expansion(img, thickness, thickness, patch_size, 9, 4)
+
+    if color_matching:
+        img = match_color(img, org_img)
+
+    if no_downscale:
+        return img
+    img_sm = downscale_mode[mode](img, target_size)
+
+    if colors is not None:
+        img_sm = kmeans_color_quant(img_sm, colors)
+
+    if contrast != 1 or saturation != 1:
+        img_sm = color_styling(img_sm, saturation, contrast)
+
+    if no_upscale:
+        return img_sm
+
+    img_lg = cv2.resize(img_sm, (W, H), interpolation=cv2.INTER_NEAREST)
+    return img_lg
+
+
+if __name__ == "__main__":
+    t0 = time()
+    img = cv2.imread("img/house.png")
+    t1 = time()
+    img = pixelize(img, target_size=128, patch_size=8)
+    t2 = time()
+    cv2.imwrite("test.png", img)
+    t3 = time()
+
+    print(f"read time: {t1 - t0:.3f}sec")
+    print(f"pixelize time: {t2 - t1:.3f}sec")
+    print(f"write time: {t3 - t2:.3f}sec")
```

### Comparing `pixeloe-0.0.4/pixeloe.egg-info/SOURCES.txt` & `pixeloe-0.0.6/pixeloe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

