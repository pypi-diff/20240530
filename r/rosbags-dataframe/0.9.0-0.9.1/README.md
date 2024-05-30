# Comparing `tmp/rosbags-dataframe-0.9.0.tar.gz` & `tmp/rosbags-dataframe-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosbags-dataframe-0.9.0.tar", last modified: Wed May  4 18:45:01 2022, max compression
+gzip compressed data, was "rosbags-dataframe-0.9.1.tar", last modified: Fri Mar  1 10:54:07 2024, max compression
```

## Comparing `rosbags-dataframe-0.9.0.tar` & `rosbags-dataframe-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-04 18:45:01.896316 rosbags-dataframe-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2022-05-04 18:44:45.000000 rosbags-dataframe-0.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3703 2022-05-04 18:45:01.896316 rosbags-dataframe-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2590 2022-05-04 18:44:45.000000 rosbags-dataframe-0.9.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       98 2022-05-04 18:44:45.000000 rosbags-dataframe-0.9.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     3460 2022-05-04 18:45:01.898147 rosbags-dataframe-0.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-04 18:45:01.890824 rosbags-dataframe-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-04 18:45:01.890824 rosbags-dataframe-0.9.0/src/rosbags/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-04 18:45:01.893570 rosbags-dataframe-0.9.0/src/rosbags/dataframe/
--rw-rw-rw-   0 root         (0) root         (0)      288 2022-05-04 18:44:45.000000 rosbags-dataframe-0.9.0/src/rosbags/dataframe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3405 2022-05-04 18:44:45.000000 rosbags-dataframe-0.9.0/src/rosbags/dataframe/dataframe.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-05-04 18:44:45.000000 rosbags-dataframe-0.9.0/src/rosbags/dataframe/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-05-04 18:45:01.896316 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3703 2022-05-04 18:45:01.000000 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2022-05-04 18:45:01.000000 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-04 18:45:01.000000 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-05-04 18:45:01.000000 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      421 2022-05-04 18:45:01.000000 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-05-04 18:45:01.000000 rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.539190 rosbags-dataframe-0.9.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.532190 rosbags-dataframe-0.9.1/.github/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/.github/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/.github/pull_request_template.md
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.528190 rosbags-dataframe-0.9.1/.gitlab/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.532190 rosbags-dataframe-0.9.1/.gitlab/issue_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.533190 rosbags-dataframe-0.9.1/.reuse/
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/.reuse/dep5
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/LICENSE.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.533190 rosbags-dataframe-0.9.1/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    10280 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/LICENSES/Apache-2.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    18375 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/LICENSES/CC-BY-SA-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)     4299 2024-03-01 10:54:07.538190 rosbags-dataframe-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2590 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.534190 rosbags-dataframe-0.9.1/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.534190 rosbags-dataframe-0.9.1/docs/api/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/docs/api/rosbags.dataframe.rst
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/docs/api/rosbags.rst
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/docs/changes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/docs/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.535190 rosbags-dataframe-0.9.1/docs/topics/
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/docs/topics/dataframe.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)    50047 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)    20456 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-01 10:54:07.539190 rosbags-dataframe-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.529190 rosbags-dataframe-0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.529190 rosbags-dataframe-0.9.1/src/rosbags/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.535190 rosbags-dataframe-0.9.1/src/rosbags/dataframe/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/src/rosbags/dataframe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/src/rosbags/dataframe/dataframe.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/src/rosbags/dataframe/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.537190 rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4299 2024-03-01 10:54:07.000000 rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      785 2024-03-01 10:54:07.000000 rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-01 10:54:07.000000 rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-03-01 10:54:07.000000 rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-01 10:54:07.000000 rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-01 10:54:07.537190 rosbags-dataframe-0.9.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2024-03-01 10:53:59.000000 rosbags-dataframe-0.9.1/tests/test_dataframe.py
```

### Comparing `rosbags-dataframe-0.9.0/LICENSE.txt` & `rosbags-dataframe-0.9.1/LICENSE.txt`

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

### Comparing `rosbags-dataframe-0.9.0/PKG-INFO` & `rosbags-dataframe-0.9.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: rosbags-dataframe
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python library to convert ros message streams to pandas dataframes.
-Home-page: https://gitlab.com/ternaris/rosbags-dataframe
-Author: Ternaris
-Author-email: team@ternaris.com
-License: Apache 2.0
-Project-URL: Code, https://gitlab.com/ternaris/rosbags-dataframe
+Author-email: Ternaris <team@ternaris.com>
+License: Apache-2.0
+Project-URL: Homepage, https://gitlab.com/ternaris/rosbags-dataframe
 Project-URL: Documentation, https://ternaris.gitlab.io/rosbags-dataframe
-Project-URL: Issue tracker, https://gitlab.com/ternaris/rosbags-dataframe/issues
-Keywords: conversion,dataframe,message,msg,pandas,ros,rosbag,rosbag2,rosbags
-Platform: any
+Project-URL: Source, https://gitlab.com/ternaris/rosbags-dataframe
+Project-URL: Issues, https://gitlab.com/ternaris/rosbags-dataframe/issues
+Project-URL: Changelog, https://gitlab.com/ternaris/rosbags-dataframe/-/blob/master/CHANGES.rst
+Keywords: conversion,dataframe,message,msg,pandas,ros,ros2,rosbag,rosbag1,rosbag2,rosbags,series
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
+Requires-Dist: pandas[feather]
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
 
 .. image:: https://gitlab.com/ternaris/rosbags-dataframe/badges/master/pipeline.svg
    :target: https://gitlab.com/ternaris/rosbags-dataframe/-/commits/master
    :alt: pipeline status
 
 .. image:: https://gitlab.com/ternaris/rosbags-dataframe/badges/master/coverage.svg
    :target: https://gitlab.com/ternaris/rosbags-dataframe/-/commits/master
@@ -110,9 +121,7 @@
 The entry point to the local documentation build should be available under ``public/index.html``.
 
 
 Support
 =======
 
 Professional support is available from `Ternaris <https://ternaris.com>`_.
-
-
```

### Comparing `rosbags-dataframe-0.9.0/README.rst` & `rosbags-dataframe-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `rosbags-dataframe-0.9.0/src/rosbags/dataframe/dataframe.py` & `rosbags-dataframe-0.9.1/src/rosbags/dataframe/dataframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Copyright 2019-2022  Ternaris.
+# Copyright 2020 - 2024 Ternaris
 # SPDX-License-Identifier: Apache-2.0
 """Conversion of rosbag topics to dataframes."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-import pandas  # type: ignore
-from rosbags.serde.messages import get_msgdef
-from rosbags.serde.utils import Valtype
+import pandas as pd  # type: ignore[import-untyped]
+
+from rosbags.interfaces import Nodetype
 
 if TYPE_CHECKING:
     from typing import Callable, Sequence, Union
 
     from rosbags.highlevel import AnyReader
 
     AttrValue = Union[str, bool, int, float, object]
 
 
 class DataframeError(Exception):
     """Dataframe conversion error."""
 
 
-def get_dataframe(reader: AnyReader, topicname: str, keys: Sequence[str]) -> pandas.DataFrame:
+def get_dataframe(reader: AnyReader, topicname: str, keys: Sequence[str]) -> pd.DataFrame:
     """Convert messages from a topic into a pandas dataframe.
 
     Read all messages from a topic and extract referenced keys into
     a pandas dataframe. The message timestamps are automatically added
     as the dataframe index.
 
     Keys support a dotted syntax to traverse nested messages.
@@ -41,29 +41,31 @@
 
     Returns:
         Pandas dataframe.
 
     """
     # pylint: disable=too-many-locals
     if not reader.isopen:
-        raise DataframeError('RosbagReader needs to be opened before accessing messages.')
+        msg = 'RosbagReader needs to be opened before accessing messages.'
+        raise DataframeError(msg)
 
     if topicname not in reader.topics:
-        raise DataframeError(f'Requested unknown topic {topicname!r}.')
+        msg = f'Requested unknown topic {topicname!r}.'
+        raise DataframeError(msg)
 
     topic = reader.topics[topicname]
     assert topic.msgtype
 
-    msgdef = get_msgdef(topic.msgtype, reader.typestore)
+    msgdef = reader.typestore.get_msgdef(topic.msgtype)
 
     def create_plain_getter(key: str) -> Callable[[object], AttrValue]:
         """Create getter for plain attribute lookups."""
 
         def getter(msg: object) -> AttrValue:
-            return getattr(msg, key)  # type: ignore
+            return getattr(msg, key)  # type: ignore[no-any-return]
 
         return getter
 
     def create_nested_getter(keys: list[str]) -> Callable[[object], AttrValue]:
         """Create getter for nested lookups."""
 
         def getter(msg: object) -> AttrValue:
@@ -75,32 +77,35 @@
         return getter
 
     getters = []
     for key in keys:
         subkeys = key.split('.')
         subdef = msgdef
         for subkey in subkeys[:-1]:
-            subfield = next((x for x in subdef.fields if x.name == subkey), None)
+            subfield = next((x for x in subdef.fields if x[0] == subkey), None)
             if not subfield:
-                raise DataframeError(f'Field {subkey!r} does not exist on {subdef.name!r}.')
-
-            if subfield.descriptor.valtype != Valtype.MESSAGE:
-                raise DataframeError(f'Field {subkey!r} of {subdef.name!r} is not a message.')
-
-            subdef = subfield.descriptor.args
+                msg = f'Field {subkey!r} does not exist on {subdef.name!r}.'
+                raise DataframeError(msg)
 
-        if subkeys[-1] not in {x.name for x in subdef.fields}:
-            raise DataframeError(f'Field {subkeys[-1]!r} does not exist on {subdef.name!r}.')
+            if subfield[1][0] != Nodetype.NAME:
+                msg = f'Field {subkey!r} of {subdef.name!r} is not a message.'
+                raise DataframeError(msg)
+
+            subdef = reader.typestore.get_msgdef(subfield[1][1])
+
+        if subkeys[-1] not in {x[0] for x in subdef.fields}:
+            msg = f'Field {subkeys[-1]!r} does not exist on {subdef.name!r}.'
+            raise DataframeError(msg)
 
         if len(subkeys) == 1:
             getters.append(create_plain_getter(subkeys[0]))
         else:
             getters.append(create_nested_getter(subkeys))
 
     timestamps = []
     data = []
     for _, timestamp, rawdata in reader.messages(connections=topic.connections):
-        msg = reader.deserialize(rawdata, topic.msgtype)
+        dmsg = reader.deserialize(rawdata, topic.msgtype)
         timestamps.append(timestamp)
-        data.append([x(msg) for x in getters])
+        data.append([x(dmsg) for x in getters])
 
-    return pandas.DataFrame(data, columns=keys, index=pandas.to_datetime(timestamps))
+    return pd.DataFrame(data, columns=tuple(keys), index=pd.to_datetime(timestamps))
```

### Comparing `rosbags-dataframe-0.9.0/src/rosbags_dataframe.egg-info/PKG-INFO` & `rosbags-dataframe-0.9.1/src/rosbags_dataframe.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 Metadata-Version: 2.1
 Name: rosbags-dataframe
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python library to convert ros message streams to pandas dataframes.
-Home-page: https://gitlab.com/ternaris/rosbags-dataframe
-Author: Ternaris
-Author-email: team@ternaris.com
-License: Apache 2.0
-Project-URL: Code, https://gitlab.com/ternaris/rosbags-dataframe
+Author-email: Ternaris <team@ternaris.com>
+License: Apache-2.0
+Project-URL: Homepage, https://gitlab.com/ternaris/rosbags-dataframe
 Project-URL: Documentation, https://ternaris.gitlab.io/rosbags-dataframe
-Project-URL: Issue tracker, https://gitlab.com/ternaris/rosbags-dataframe/issues
-Keywords: conversion,dataframe,message,msg,pandas,ros,rosbag,rosbag2,rosbags
-Platform: any
+Project-URL: Source, https://gitlab.com/ternaris/rosbags-dataframe
+Project-URL: Issues, https://gitlab.com/ternaris/rosbags-dataframe/issues
+Project-URL: Changelog, https://gitlab.com/ternaris/rosbags-dataframe/-/blob/master/CHANGES.rst
+Keywords: conversion,dataframe,message,msg,pandas,ros,ros2,rosbag,rosbag1,rosbag2,rosbags,series
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
+Requires-Dist: pandas[feather]
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
 
 .. image:: https://gitlab.com/ternaris/rosbags-dataframe/badges/master/pipeline.svg
    :target: https://gitlab.com/ternaris/rosbags-dataframe/-/commits/master
    :alt: pipeline status
 
 .. image:: https://gitlab.com/ternaris/rosbags-dataframe/badges/master/coverage.svg
    :target: https://gitlab.com/ternaris/rosbags-dataframe/-/commits/master
@@ -110,9 +121,7 @@
 The entry point to the local documentation build should be available under ``public/index.html``.
 
 
 Support
 =======
 
 Professional support is available from `Ternaris <https://ternaris.com>`_.
-
-
```

