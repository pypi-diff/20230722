# Comparing `tmp/create-fastapi-0.0.6.tar.gz` & `tmp/create_fastapi-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-fastapi-0.0.6.tar", last modified: Sat Jul 22 09:05:54 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `create-fastapi-0.0.6.tar` & `create_fastapi-0.0.7.tar`

### file list

```diff
@@ -1,45 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/
--rw-rw-rw-   0        0        0    11558 2023-07-21 09:43:38.000000 create-fastapi-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    14130 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       20 2023-07-21 09:43:38.000000 create-fastapi-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.235738 create-fastapi-0.0.6/cfa/
--rw-rw-rw-   0        0        0        0 2023-07-21 13:10:51.000000 create-fastapi-0.0.6/cfa/__init__.py
--rw-rw-rw-   0        0        0      401 2023-07-21 16:06:12.000000 create-fastapi-0.0.6/cfa/cli.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.235738 create-fastapi-0.0.6/cfa/commands/
--rw-rw-rw-   0        0        0       93 2023-07-21 09:53:03.000000 create-fastapi-0.0.6/cfa/commands/ICommand.py
--rw-rw-rw-   0        0        0        0 2023-07-21 09:43:42.000000 create-fastapi-0.0.6/cfa/commands/__init__.py
--rw-rw-rw-   0        0        0      873 2023-07-21 12:21:25.000000 create-fastapi-0.0.6/cfa/commands/command_builder.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.251839 create-fastapi-0.0.6/cfa/commands/impl/
--rw-rw-rw-   0        0        0        0 2023-07-21 11:40:39.000000 create-fastapi-0.0.6/cfa/commands/impl/__init__.py
--rw-rw-rw-   0        0        0      548 2023-07-21 12:24:21.000000 create-fastapi-0.0.6/cfa/commands/impl/clone_git.py
--rw-rw-rw-   0        0        0     1067 2023-07-21 12:55:39.000000 create-fastapi-0.0.6/cfa/commands/impl/dependency_installer.py
--rw-rw-rw-   0        0        0      314 2023-07-21 11:42:31.000000 create-fastapi-0.0.6/cfa/commands/impl/dir_creator.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.251839 create-fastapi-0.0.6/cfa/config/
--rw-rw-rw-   0        0        0      341 2023-07-21 13:01:48.000000 create-fastapi-0.0.6/cfa/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.251839 create-fastapi-0.0.6/cfa/helpers/
--rw-rw-rw-   0        0        0        0 2023-07-21 11:36:51.000000 create-fastapi-0.0.6/cfa/helpers/__init__.py
--rw-rw-rw-   0        0        0      279 2023-07-21 11:38:30.000000 create-fastapi-0.0.6/cfa/helpers/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.235738 create-fastapi-0.0.6/cfa/venv/
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/cfa/venv/Scripts/
--rw-rw-rw-   0        0        0     1169 2023-07-21 09:44:48.000000 create-fastapi-0.0.6/cfa/venv/Scripts/activate_this.py
--rw-rw-rw-   0        0        0      696 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2html.py
--rw-rw-rw-   0        0        0      818 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2html4.py
--rw-rw-rw-   0        0        0     1153 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2html5.py
--rw-rw-rw-   0        0        0      895 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2latex.py
--rw-rw-rw-   0        0        0      718 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2man.py
--rw-rw-rw-   0        0        0      884 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2odt.py
--rw-rw-rw-   0        0        0      690 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2odt_prepstyles.py
--rw-rw-rw-   0        0        0      703 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2pseudoxml.py
--rw-rw-rw-   0        0        0      739 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2s5.py
--rw-rw-rw-   0        0        0      975 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2xetex.py
--rw-rw-rw-   0        0        0      704 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rst2xml.py
--rw-rw-rw-   0        0        0      772 2023-07-21 13:10:35.000000 create-fastapi-0.0.6/cfa/venv/Scripts/rstpep2html.py
-drwxrwxrwx   0        0        0        0 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/create_fastapi.egg-info/
--rw-rw-rw-   0        0        0    14130 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      975 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-22 09:05:54.000000 create-fastapi-0.0.6/create_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1201 2023-07-22 09:05:37.000000 create-fastapi-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 09:05:54.267906 create-fastapi-0.0.6/setup.cfg
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/__init__.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/cli.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/ICommand.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/__init__.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/command_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/impl/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/impl/clone_git.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/impl/dependency_installer.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/commands/impl/dir_creator.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/helpers/__init__.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/cfa/helpers/logger.py
+-rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/LICENSE
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/README.md
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 create_fastapi-0.0.7/PKG-INFO
```

### Comparing `create-fastapi-0.0.6/LICENSE` & `create_fastapi-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `create-fastapi-0.0.6/PKG-INFO` & `create_fastapi-0.0.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,225 +1,227 @@
-Metadata-Version: 2.1
-Name: create-fastapi
-Version: 0.0.6
-Summary: create-fastapi-app
-Author-email: Shahar Luftig <shaharluftig@gmail.com>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright [yyyy] [name of copyright owner]
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/shaharluftig/create-fastapi-app
-Keywords: backend,fastapi,create-app,create-fastapi-app,create-fatapi
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# create-fastapi-app
+Metadata-Version: 2.1
+Name: create-fastapi
+Version: 0.0.7
+Summary: create-fastapi-app
+Project-URL: Homepage, https://github.com/shaharluftig/create-fastapi-app
+Author-email: Shahar Luftig <shaharluftig@gmail.com>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright [yyyy] [name of copyright owner]
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+License-File: LICENSE
+Keywords: backend,create-app,create-fastapi-app,create-fatapi,fastapi
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Requires-Dist: gitpython~=3.1.32
+Requires-Dist: typer~=0.9.0
+Requires-Dist: virtualenv~=20.24.1
+Description-Content-Type: text/markdown
+
+# create-fastapi-app
```

### Comparing `create-fastapi-0.0.6/cfa/commands/command_builder.py` & `create_fastapi-0.0.7/cfa/commands/command_builder.py`

 * *Files identical despite different names*

### Comparing `create-fastapi-0.0.6/cfa/commands/impl/clone_git.py` & `create_fastapi-0.0.7/cfa/commands/impl/clone_git.py`

 * *Files identical despite different names*

### Comparing `create-fastapi-0.0.6/cfa/commands/impl/dependency_installer.py` & `create_fastapi-0.0.7/cfa/commands/impl/dependency_installer.py`

 * *Files identical despite different names*

### Comparing `create-fastapi-0.0.6/pyproject.toml` & `create_fastapi-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "create-fastapi"
 description = "create-fastapi-app"
 readme = "README.md"
-version = "0.0.6"
+version = "0.0.7"
 
 authors = [{ name = "Shahar Luftig", email = "shaharluftig@gmail.com" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 
 keywords = [
     "backend",
@@ -35,9 +34,10 @@
 ]
 
 dependencies = ["typer~=0.9.0", "virtualenv~=20.24.1", "GitPython~=3.1.32"]
 
 [project.urls]
 "Homepage" = "https://github.com/shaharluftig/create-fastapi-app"
 
+
 [project.scripts]
 create-fastapi-app = "cfa.cli:main_cli"
```

