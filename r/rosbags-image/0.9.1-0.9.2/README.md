# Comparing `tmp/rosbags-image-0.9.1.tar.gz` & `tmp/rosbags-image-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosbags-image-0.9.1.tar", last modified: Thu Sep  8 11:27:06 2022, max compression
+gzip compressed data, was "rosbags-image-0.9.2.tar", last modified: Fri Mar  1 10:16:17 2024, max compression
```

## Comparing `rosbags-image-0.9.1.tar` & `rosbags-image-0.9.2.tar`

### file list

```diff
@@ -1,19 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 11:27:06.595127 rosbags-image-0.9.1/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2022-09-08 11:26:50.000000 rosbags-image-0.9.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3763 2022-09-08 11:27:06.595127 rosbags-image-0.9.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2643 2022-09-08 11:26:50.000000 rosbags-image-0.9.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-09-08 11:26:50.000000 rosbags-image-0.9.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     3494 2022-09-08 11:27:06.596127 rosbags-image-0.9.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 11:27:06.590127 rosbags-image-0.9.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 11:27:06.590127 rosbags-image-0.9.1/src/rosbags/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 11:27:06.593127 rosbags-image-0.9.1/src/rosbags/image/
--rw-rw-rw-   0 root         (0) root         (0)      490 2022-09-08 11:26:50.000000 rosbags-image-0.9.1/src/rosbags/image/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6724 2022-09-08 11:26:50.000000 rosbags-image-0.9.1/src/rosbags/image/image.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-08 11:26:50.000000 rosbags-image-0.9.1/src/rosbags/image/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-08 11:27:06.594127 rosbags-image-0.9.1/src/rosbags_image.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3763 2022-09-08 11:27:06.000000 rosbags-image-0.9.1/src/rosbags_image.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      375 2022-09-08 11:27:06.000000 rosbags-image-0.9.1/src/rosbags_image.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-08 11:27:06.000000 rosbags-image-0.9.1/src/rosbags_image.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-08 11:27:06.000000 rosbags-image-0.9.1/src/rosbags_image.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      443 2022-09-08 11:27:06.000000 rosbags-image-0.9.1/src/rosbags_image.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-09-08 11:27:06.000000 rosbags-image-0.9.1/src/rosbags_image.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.560397 rosbags-image-0.9.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.554397 rosbags-image-0.9.2/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/.github/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/.github/pull_request_template.md
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.549397 rosbags-image-0.9.2/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.554397 rosbags-image-0.9.2/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.554397 rosbags-image-0.9.2/.reuse/
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/.reuse/dep5
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3384 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.555397 rosbags-image-0.9.2/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18375 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/LICENSES/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)     4378 2024-03-01 10:16:17.560397 rosbags-image-0.9.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2643 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.555397 rosbags-image-0.9.2/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.556397 rosbags-image-0.9.2/docs/api/
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/docs/api/rosbags.image.rst
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/docs/api/rosbags.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.556397 rosbags-image-0.9.2/docs/topics/
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/docs/topics/image.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2829 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)    43444 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)    15054 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 10:16:17.560397 rosbags-image-0.9.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.551397 rosbags-image-0.9.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.551397 rosbags-image-0.9.2/src/rosbags/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.557397 rosbags-image-0.9.2/src/rosbags/image/
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/src/rosbags/image/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6260 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/src/rosbags/image/image.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/src/rosbags/image/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.559397 rosbags-image-0.9.2/src/rosbags_image.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4378 2024-03-01 10:16:17.000000 rosbags-image-0.9.2/src/rosbags_image.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2024-03-01 10:16:17.000000 rosbags-image-0.9.2/src/rosbags_image.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 10:16:17.000000 rosbags-image-0.9.2/src/rosbags_image.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      135 2024-03-01 10:16:17.000000 rosbags-image-0.9.2/src/rosbags_image.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-01 10:16:17.000000 rosbags-image-0.9.2/src/rosbags_image.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:16:17.558397 rosbags-image-0.9.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11851 2024-03-01 10:16:09.000000 rosbags-image-0.9.2/tests/test_image.py
```

### Comparing `rosbags-image-0.9.1/LICENSE.txt` & `rosbags-image-0.9.2/LICENSE.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,202 +1,73 @@
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
 
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
-   Copyright [yyyy] [name of copyright owner]
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
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+
+"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+
+"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+
+"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+
+"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+
+"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+
+"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+
+2. Grant of Copyright License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License. Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+
+4. Redistribution. You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+
+     (a) You must give any other recipients of the Work or Derivative Works a copy of this License; and
+
+     (b) You must cause any modified files to carry prominent notices stating that You changed the files; and
+
+     (c) You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+
+     (d) If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+
+     You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+
+5. Submission of Contributions. Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+
+6. Trademarks. This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty. Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability. In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability. While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
+
+APPENDIX: How to apply the Apache License to your work.
+
+To apply the Apache License to your work, attach the following boilerplate notice, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!)  The text should be enclosed in the appropriate comment syntax for the file format. We also recommend that a file or class name and description of purpose be included on the same "printed page" as the copyright notice for easier identification within third-party archives.
+
+Copyright [yyyy] [name of copyright owner]
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `rosbags-image-0.9.1/PKG-INFO` & `rosbags-image-0.9.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 Metadata-Version: 2.1
 Name: rosbags-image
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pure Python library to convert ros image message data from and to opencv2.
-Home-page: https://gitlab.com/ternaris/rosbags-image
-Author: Ternaris
-Author-email: team@ternaris.com
-License: Apache 2.0
-Project-URL: Code, https://gitlab.com/ternaris/rosbags-image
+Author-email: Ternaris <team@ternaris.com>
+License: Apache-2.0
+Project-URL: Homepage, https://gitlab.com/ternaris/rosbags-image
 Project-URL: Documentation, https://ternaris.gitlab.io/rosbags-image
-Project-URL: Issue tracker, https://gitlab.com/ternaris/rosbags-image/issues
-Keywords: conversion,cv_bridge,image,compressedimage,message,msg,opencv,ros,rosbag,rosbag2,rosbags
-Platform: any
+Project-URL: Source, https://gitlab.com/ternaris/rosbags-image
+Project-URL: Issues, https://gitlab.com/ternaris/rosbags-image/issues
+Project-URL: Changelog, https://gitlab.com/ternaris/rosbags-image/-/blob/master/CHANGES.rst
+Keywords: conversion,cv_bridge,image,compressedimage,message,msg,opencv,ros,ros2,rosbag,rosbag1,rosbag2,rosbags
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.2
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: opencv-python-headless
+Requires-Dist: rosbags>=0.9.20
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: reuse; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 
 .. image:: https://gitlab.com/ternaris/rosbags-image/badges/master/pipeline.svg
    :target: https://gitlab.com/ternaris/rosbags-image/-/commits/master
    :alt: pipeline status
 
 .. image:: https://gitlab.com/ternaris/rosbags-image/badges/master/coverage.svg
    :target: https://gitlab.com/ternaris/rosbags-image/-/commits/master
```

### Comparing `rosbags-image-0.9.1/README.rst` & `rosbags-image-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `rosbags-image-0.9.1/src/rosbags/image/image.py` & `rosbags-image-0.9.2/src/rosbags/image/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,30 @@
-# Copyright 2019-2022  Ternaris.
+# Copyright 2020 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Image conversion between ROS and OpenCV formats."""
 
 from __future__ import annotations
 
 import re
 import sys
 from contextlib import suppress
 from enum import IntEnum
 from itertools import product
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, cast
 
-import cv2  # type: ignore
-import numpy
-from rosbags.typesys.types import sensor_msgs__msg__CompressedImage as CompressedImage
+import cv2
+import numpy as np
 
 if TYPE_CHECKING:
-    from typing import Any, Optional, Union
+    from rosbags.typesys.stores.latest import (
+        sensor_msgs__msg__CompressedImage as CompressedImage,
+        sensor_msgs__msg__Image as Image,
+    )
 
-    if sys.version_info < (3, 9):
-        Imagebytes = numpy.ndarray[Any, Any]
-    else:
-        from numpy.typing import NDArray
-        Imagebytes = NDArray[Any]
-    from rosbags.typesys.types import sensor_msgs__msg__Image as Image
+    Imagebytes = np.ndarray[None, np.dtype[np.generic]]
 
 ENC_RE = re.compile('(8U|8S|16U|16S|32S|32F|64F)(?:C([0-9]+))?')
 DIGITS_RE = re.compile(r'^\d+')
 
 
 class ImageError(Exception):
     """Unsupported Image Format."""
@@ -114,15 +111,16 @@
 
     if mat := ENC_RE.fullmatch(encoding):
         depth, nchan = mat.groups()
         mat = DIGITS_RE.search(depth)
         assert mat
         return (int(mat.group()), Format.GENERIC, DEPTHMAP[depth], int(nchan or 1))
 
-    raise ImageFormatError(f'Format {encoding!r} is not supported')
+    msg = f'Format {encoding!r} is not supported'
+    raise ImageFormatError(msg)
 
 
 def convert_color(src: Imagebytes, src_color_space: str, dst_color_space: str) -> Imagebytes:
     """Convert color space.
 
     Args:
         src: Source image.
@@ -142,94 +140,84 @@
 
     src_depth, src_fmt, src_typestr, src_nchan = to_cvtype(src_color_space)
     dst_depth, dst_fmt, dst_typestr, dst_nchan = to_cvtype(dst_color_space)
 
     try:
         conversion = CONVERSIONS[(src_fmt, dst_fmt)]
     except KeyError:
-        if Format.GENERIC not in (src_fmt, dst_fmt) or src_nchan != dst_nchan:
-            raise ImageConversionError(
-                f'Conversion {src_color_space!r} -> {dst_color_space!r} is not supported',
-            ) from None
+        if Format.GENERIC not in {src_fmt, dst_fmt} or src_nchan != dst_nchan:
+            msg = f'Conversion {src_color_space!r} -> {dst_color_space!r} is not supported'
+            raise ImageConversionError(msg) from None
         conversion = None
 
     if conversion:
-        src = cv2.cvtColor(src, conversion)  # pyright: ignore  # pylint: disable=no-member
+        src = cv2.cvtColor(src, conversion)
 
     if src_typestr != dst_typestr:
         if src_depth == 8 and dst_depth == 16:
-            return numpy.multiply(  # type: ignore
-                src.astype(dst_typestr, copy=False),
-                65535. / 255.,
-            )
+            return np.multiply(src.astype(dst_typestr, copy=False), 65535.0 / 255.0)
         if src_depth == 16 and dst_depth == 8:
-            return numpy.multiply(  # type: ignore
-                src,
-                255. / 65535.,
-            ).astype(dst_typestr, copy=False)
+            return np.multiply(src, 255.0 / 65535.0).astype(dst_typestr, copy=False)
         return src.astype(dst_typestr, copy=False)
     return src
 
 
-def image_to_cvimage(msg: Image, color_space: Optional[str] = None) -> Imagebytes:
+def image_to_cvimage(msg: Image, color_space: str | None = None) -> Imagebytes:
     """Convert sensor_msg/msg/Image to OpenCV image.
 
     Args:
         msg: Image message.
         color_space: Color space of output image.
 
     Returns:
         OpenCV image.
 
     """
     _, _, typestr, nchan = to_cvtype(msg.encoding)
     shape = (msg.height, msg.width) if nchan == 1 else (msg.height, msg.width, nchan)
-    dtype = numpy.dtype(typestr)  # .newbyteorder('>' if msg.is_bigendian else '<')
-    img: Imagebytes = numpy.ndarray(shape=shape, dtype=dtype, buffer=msg.data)
+    dtype = np.dtype(typestr)  # .newbyteorder('>' if msg.is_bigendian else '<')
+    img: Imagebytes = np.ndarray(shape=shape, dtype=dtype, buffer=msg.data)
     if msg.is_bigendian != (sys.byteorder != 'little'):
-        img.byteswap(inplace=True)
+        img = img.byteswap()
 
     if color_space:
         return convert_color(img, msg.encoding, color_space)
     return img
 
 
 def compressed_image_to_cvimage(
     msg: CompressedImage,
-    color_space: Optional[str] = None,
+    color_space: str | None = None,
 ) -> Imagebytes:
     """Convert sensor_msg/msg/CompressedImage to OpenCV image.
 
     Args:
         msg: CompressedImage message.
         color_space: Color space of output image.
 
     Returns:
         OpenCV image.
 
     """
-    img: Imagebytes = cv2.imdecode(  # pyright: ignore  # pylint: disable=no-member
-        numpy.frombuffer(msg.data, numpy.uint8),
-        cv2.IMREAD_ANYCOLOR,  # pyright: ignore  # pylint: disable=no-member
-    )
+    img: Imagebytes = cv2.imdecode(np.frombuffer(msg.data, np.uint8), cv2.IMREAD_ANYCOLOR)
     if color_space:
         return convert_color(img, 'bgr8', color_space)
     return img
 
 
 def message_to_cvimage(
-    msg: Union[CompressedImage, Image],
-    color_space: Optional[str] = None,
+    msg: CompressedImage | Image,
+    color_space: str | None = None,
 ) -> Imagebytes:
     """Convert ROS message to OpenCV image.
 
     Args:
         msg: CompressedImage or Image message.
         color_space: Color space of output image.
 
     Returns:
         OpenCV image.
 
     """
-    if isinstance(msg, CompressedImage):
-        return compressed_image_to_cvimage(msg, color_space)
+    if hasattr(msg, 'format'):
+        return compressed_image_to_cvimage(cast('CompressedImage', msg), color_space)
     return image_to_cvimage(msg, color_space)
```

### Comparing `rosbags-image-0.9.1/src/rosbags_image.egg-info/PKG-INFO` & `rosbags-image-0.9.2/src/rosbags_image.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 Metadata-Version: 2.1
 Name: rosbags-image
-Version: 0.9.1
+Version: 0.9.2
 Summary: Pure Python library to convert ros image message data from and to opencv2.
-Home-page: https://gitlab.com/ternaris/rosbags-image
-Author: Ternaris
-Author-email: team@ternaris.com
-License: Apache 2.0
-Project-URL: Code, https://gitlab.com/ternaris/rosbags-image
+Author-email: Ternaris <team@ternaris.com>
+License: Apache-2.0
+Project-URL: Homepage, https://gitlab.com/ternaris/rosbags-image
 Project-URL: Documentation, https://ternaris.gitlab.io/rosbags-image
-Project-URL: Issue tracker, https://gitlab.com/ternaris/rosbags-image/issues
-Keywords: conversion,cv_bridge,image,compressedimage,message,msg,opencv,ros,rosbag,rosbag2,rosbags
-Platform: any
+Project-URL: Source, https://gitlab.com/ternaris/rosbags-image
+Project-URL: Issues, https://gitlab.com/ternaris/rosbags-image/issues
+Project-URL: Changelog, https://gitlab.com/ternaris/rosbags-image/-/blob/master/CHANGES.rst
+Keywords: conversion,cv_bridge,image,compressedimage,message,msg,opencv,ros,ros2,rosbag,rosbag1,rosbag2,rosbags
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8.2
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: opencv-python-headless
+Requires-Dist: rosbags>=0.9.20
+Provides-Extra: dev
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: reuse; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: sphinx; extra == "dev"
+Requires-Dist: sphinx-autodoc-typehints; extra == "dev"
+Requires-Dist: sphinx-rtd-theme; extra == "dev"
 
 .. image:: https://gitlab.com/ternaris/rosbags-image/badges/master/pipeline.svg
    :target: https://gitlab.com/ternaris/rosbags-image/-/commits/master
    :alt: pipeline status
 
 .. image:: https://gitlab.com/ternaris/rosbags-image/badges/master/coverage.svg
    :target: https://gitlab.com/ternaris/rosbags-image/-/commits/master
```

