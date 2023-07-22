# Comparing `tmp/marketwatchdata-0.0.2.tar.gz` & `tmp/marketwatchdata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marketwatchdata-0.0.2.tar", last modified: Sat Jul 22 14:12:42 2023, max compression
+gzip compressed data, was "marketwatchdata-0.0.3.tar", last modified: Sat Jul 22 14:56:08 2023, max compression
```

## Comparing `marketwatchdata-0.0.2.tar` & `marketwatchdata-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 14:12:42.629695 marketwatchdata-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-07-21 12:14:59.000000 marketwatchdata-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       24 2023-07-22 14:11:34.000000 marketwatchdata-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      797 2023-07-22 14:12:42.629695 marketwatchdata-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       56 2023-07-21 12:14:59.000000 marketwatchdata-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-22 14:12:42.623715 marketwatchdata-0.0.2/marketwatchdata/
--rw-rw-rw-   0        0        0     3305 2023-07-22 13:23:29.000000 marketwatchdata-0.0.2/marketwatchdata/MarketWatch.py
--rw-rw-rw-   0        0        0      428 2023-07-22 14:12:37.000000 marketwatchdata-0.0.2/marketwatchdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:12:42.627702 marketwatchdata-0.0.2/marketwatchdata.egg-info/
--rw-rw-rw-   0        0        0      797 2023-07-22 14:12:42.000000 marketwatchdata-0.0.2/marketwatchdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-07-22 14:12:42.000000 marketwatchdata-0.0.2/marketwatchdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 14:12:42.000000 marketwatchdata-0.0.2/marketwatchdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      223 2023-07-22 14:12:42.000000 marketwatchdata-0.0.2/marketwatchdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-22 14:12:42.000000 marketwatchdata-0.0.2/marketwatchdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      237 2023-07-21 12:14:59.000000 marketwatchdata-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-22 14:12:42.631197 marketwatchdata-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-07-22 13:33:31.000000 marketwatchdata-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:12:42.629695 marketwatchdata-0.0.2/tests/
--rw-rw-rw-   0        0        0       87 2023-07-21 12:14:59.000000 marketwatchdata-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      544 2023-07-22 12:38:15.000000 marketwatchdata-0.0.2/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/marketwatchdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/marketwatchdata/MarketWatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/marketwatchdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/marketwatchdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-22 14:56:08.000000 marketwatchdata-0.0.3/marketwatchdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 14:56:08.821562 marketwatchdata-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-22 14:55:41.000000 marketwatchdata-0.0.3/tests/test_func.py
```

### Comparing `marketwatchdata-0.0.2/LICENSE` & `marketwatchdata-0.0.3/LICENSE`

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
+   Copyright [yyyy] [name of copyright owner]
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

### Comparing `marketwatchdata-0.0.2/marketwatchdata/MarketWatch.py` & `marketwatchdata-0.0.3/marketwatchdata/MarketWatch.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-import time
-import pandas as pd
-import requests
-import json
-
-
-
-
-
-def ohlc(code: str, timeframe: str, timerange: str):
-    """获取日线数据 marketWatch只支持日线级别的
-
-    参数:
-        code: STOCK/US/XNAS/AAPL | TMUBMUSD10Y
-        timeframe: P1D | P1W
-        timerange: P1M P1Y P2Y All
-
-    返回:
-        pandas.dataframe
-
-                    open      high      low   close      volume
-        time
-        2022-07-21  154.500  155.5700  151.940  155.35  65086641.0
-        2022-07-22  155.390  156.2800  153.410  154.09  66675406.0
-        2022-07-25  154.010  155.0400  152.280  152.95  53623953.0
-        2022-07-26  152.265  153.0850  150.800  151.60  55138688.0
-        2022-07-27  152.580  157.3300  152.160  156.79  78620688.0
-        ...             ...       ...      ...     ...         ...
-        2023-07-14  190.230  191.1799  189.630  190.69  41616238.0
-        2023-07-17  191.900  194.3200  191.810  193.99  50520160.0
-        2023-07-18  193.350  194.3300  192.415  193.73  48353770.0
-        2023-07-19  193.100  198.2300  192.650  195.10  80507320.0
-        2023-07-20  195.090  196.4700  192.495  193.13  59581196.0
-
-    抛出:
-
-    示例:
-        df = MW_GetOHLC('STOCK/US/XNAS/AAPL', 'P1D', 'P1Y')
-
-    """
-
-    req_url = (
-        f'https://api-secure.wsj.net/api/michelangelo/timeseries/history?json={{"Step":"{timeframe}","TimeFrame":"{timerange}", '
-        '"EntitlementToken":"cecc4267a0194af89ca343805a3e57af","IncludeMockTick":true,"FilterNullSlots":false,'
-        '"FilterClosedPoints":true,"IncludeClosedSlots":false,"IncludeOfficialClose":true,"InjectOpen":false,'
-        '"ShowPreMarket":false,"ShowAfterHours":false,"UseExtendedTimeFrame":false,"WantPriorClose":true,'
-        '"IncludeCurrentQuotes":false,"ResetTodaysAfterHoursPercentChange":false,'
-        f'"Series":[{{"Key":"{code}","Dialect":"Charting","Kind":"Ticker","SeriesId":"s1",'
-        '"DataTypes":["Open", "High", "Low", "Last", "Volume"]}]}&ckey=cecc4267a0'
-    )
-
-    # print(req_url)
-
-    r = requests.get(
-        req_url,
-        headers={
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:52.0) Gecko/20100101 Firefox/52.0",
-            "Content-Type": "application/json, text/javascript, */*; q=0.01",
-            "Dylan2010.EntitlementToken": "cecc4267a0194af89ca343805a3e57af",
-        },
-    )
-    # Full Return
-    # print(r.text)
-    # return r.text
-
-    # Stock UNIX Dates
-    datajson = json.loads(r.content)
-    times = datajson['TimeInfo']['Ticks']
-    # print(times)
-
-    # Stock Prices
-    data = datajson['Series'][0]['DataPoints']
-    # print(data)
-
-    # temp_df = pd.DataFrame(data, columns=['REPORT_DATE','PUBLISH_DATE', 'VALUE', 'PRE_VALUE'])
-    temp_df = pd.DataFrame(data)
-    temp_df['time'] = times
-    temp_df.columns = ["open", "high", "low", "close", 'volume', 'time']
-
-    temp_df["time"] = pd.to_datetime(temp_df["time"], unit='ms').dt.date
-    # temp_df["time"] = pd.to_datetime(temp_df["time"],unit='ms')
-    temp_df.set_index("time", inplace=True)
-    # print(temp_df.dtypes)
-    temp_df.dropna(inplace=True)
-
-    # print(temp_df)
-    return temp_df
-
-
-if __name__ == "__main__":
-    df = ohlc('TMUBMUSD03M', 'P1D', 'P1Y')
-    print(df)
+import time
+import pandas as pd
+import requests
+import json
+
+
+
+
+
+def ohlc(code: str, timeframe: str, timerange: str):
+    """获取日线数据 marketWatch只支持日线级别的
+
+    参数:
+        code: STOCK/US/XNAS/AAPL | TMUBMUSD10Y
+        timeframe: P1D | P1W
+        timerange: P1M P1Y P2Y All
+
+    返回:
+        pandas.dataframe
+
+                    open      high      low   close      volume
+        time
+        2022-07-21  154.500  155.5700  151.940  155.35  65086641.0
+        2022-07-22  155.390  156.2800  153.410  154.09  66675406.0
+        2022-07-25  154.010  155.0400  152.280  152.95  53623953.0
+        2022-07-26  152.265  153.0850  150.800  151.60  55138688.0
+        2022-07-27  152.580  157.3300  152.160  156.79  78620688.0
+        ...             ...       ...      ...     ...         ...
+        2023-07-14  190.230  191.1799  189.630  190.69  41616238.0
+        2023-07-17  191.900  194.3200  191.810  193.99  50520160.0
+        2023-07-18  193.350  194.3300  192.415  193.73  48353770.0
+        2023-07-19  193.100  198.2300  192.650  195.10  80507320.0
+        2023-07-20  195.090  196.4700  192.495  193.13  59581196.0
+
+    抛出:
+
+    示例:
+        df = MW_GetOHLC('STOCK/US/XNAS/AAPL', 'P1D', 'P1Y')
+
+    """
+
+    req_url = (
+        f'https://api-secure.wsj.net/api/michelangelo/timeseries/history?json={{"Step":"{timeframe}","TimeFrame":"{timerange}", '
+        '"EntitlementToken":"cecc4267a0194af89ca343805a3e57af","IncludeMockTick":true,"FilterNullSlots":false,'
+        '"FilterClosedPoints":true,"IncludeClosedSlots":false,"IncludeOfficialClose":true,"InjectOpen":false,'
+        '"ShowPreMarket":false,"ShowAfterHours":false,"UseExtendedTimeFrame":false,"WantPriorClose":true,'
+        '"IncludeCurrentQuotes":false,"ResetTodaysAfterHoursPercentChange":false,'
+        f'"Series":[{{"Key":"{code}","Dialect":"Charting","Kind":"Ticker","SeriesId":"s1",'
+        '"DataTypes":["Open", "High", "Low", "Last", "Volume"]}]}&ckey=cecc4267a0'
+    )
+
+    # print(req_url)
+
+    r = requests.get(
+        req_url,
+        headers={
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:52.0) Gecko/20100101 Firefox/52.0",
+            "Content-Type": "application/json, text/javascript, */*; q=0.01",
+            "Dylan2010.EntitlementToken": "cecc4267a0194af89ca343805a3e57af",
+        },
+    )
+    # Full Return
+    # print(r.text)
+    # return r.text
+
+    # Stock UNIX Dates
+    datajson = json.loads(r.content)
+    times = datajson['TimeInfo']['Ticks']
+    # print(times)
+
+    # Stock Prices
+    data = datajson['Series'][0]['DataPoints']
+    # print(data)
+
+    # temp_df = pd.DataFrame(data, columns=['REPORT_DATE','PUBLISH_DATE', 'VALUE', 'PRE_VALUE'])
+    temp_df = pd.DataFrame(data)
+    temp_df['time'] = times
+    temp_df.columns = ["open", "high", "low", "close", 'volume', 'time']
+
+    temp_df["time"] = pd.to_datetime(temp_df["time"], unit='ms').dt.date
+    # temp_df["time"] = pd.to_datetime(temp_df["time"],unit='ms')
+    temp_df.set_index("time", inplace=True)
+    # print(temp_df.dtypes)
+    temp_df.dropna(inplace=True)
+
+    # print(temp_df)
+    return temp_df
+
+
+if __name__ == "__main__":
+    df = ohlc('TMUBMUSD03M', 'P1D', 'P1Y')
+    print(df)
```

### Comparing `marketwatchdata-0.0.2/setup.py` & `marketwatchdata-0.0.3/setup.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-#!/usr/bin/env python
-# -*- coding:utf-8 -*-
-"""
-Date: 2023/7/22 22:09
-Desc: PYPI info file
-"""
-import re
-import ast
-
-import setuptools
-
-from marketwatchdata import __version__, __author__,__authoremail__
-
-with open("README.md", "r", encoding="utf-8") as f:
-    long_description = f.read()
-
-requirementsPath = "requirements.txt"
-
-requirementslist = []
-f = open(requirementsPath, 'r')
-for line in f:
-    requirementslist.append(str.strip(line))
-f.close()
-#print(requirementslist)
-
-#print(__version__)
-#print(__author__)
-#print(__authoremail__)
-
-
-setuptools.setup(
-    name="marketwatchdata",
-    version=__version__,
-    author=__author__,
-    author_email=__authoremail__,
-    license="MIT",
-    description="retrieve data from MarketWatch.com",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/yacper/marketwatchdata",
-    packages=setuptools.find_packages(),
-    install_requires=requirementslist,
-    package_data={"": ["*.py", "*.json", "*.pk", "*.js", "*.zip"]},
-    keywords=[
-        "stock",
-        "option",
-        "futures",
-        "fund",
-        "bond",
-        "index",
-        "air",
-        "finance",
-        "spider",
-        "quant",
-        "quantitative",
-        "investment",
-        "trading",
-        "algotrading",
-        "data",
-    ],
-    classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires=">=3.8",
-)
+#!/usr/bin/env python
+# -*- coding:utf-8 -*-
+"""
+Date: 2023/7/22 22:09
+Desc: PYPI info file
+"""
+import re
+import ast
+
+import setuptools
+
+from marketwatchdata import __version__, __author__,__authoremail__
+
+with open("README.md", "r", encoding="utf-8") as f:
+    long_description = f.read()
+
+requirementsPath = "requirements.txt"
+
+requirementslist = []
+f = open(requirementsPath, 'r')
+for line in f:
+    requirementslist.append(str.strip(line))
+f.close()
+#print(requirementslist)
+
+#print(__version__)
+#print(__author__)
+#print(__authoremail__)
+
+
+setuptools.setup(
+    name="marketwatchdata",
+    version=__version__,
+    author=__author__,
+    author_email=__authoremail__,
+    license="MIT",
+    description="retrieve data from MarketWatch.com",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/yacper/marketwatchdata",
+    packages=setuptools.find_packages(),
+    install_requires=requirementslist,
+    package_data={"": ["*.py", "*.json", "*.pk", "*.js", "*.zip"]},
+    keywords=[
+        "stock",
+        "option",
+        "futures",
+        "fund",
+        "bond",
+        "index",
+        "air",
+        "finance",
+        "spider",
+        "quant",
+        "quantitative",
+        "investment",
+        "trading",
+        "algotrading",
+        "data",
+    ],
+    classifiers=[
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires=">=3.8",
+)
```

### Comparing `marketwatchdata-0.0.2/tests/test_func.py` & `marketwatchdata-0.0.3/tests/test_func.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-#!/usr/bin/env python
-# -*- coding:utf-8 -*-
-"""
-Date: 2023/7/21 18:16
-Desc: To test intention, just write test code here!
-"""
-import sys
-
-sys.path.append("../marketwatchdata")
-# print(sys.path)
-
-# from marketwatchdata.MarketWatch import *
-import marketwatchdata.MarketWatch as mw
-
-
-def test_ohlc():
-    """
-    just for test aim
-    :return: assert result
-    :rtype: assert
-    """
-    df = mw.ohlc('TMUBMUSD03M', 'P1D', 'P1Y')
-    print(df)
-    assert df.shape[0] > 0
-
-
-if __name__ == "__main__":
-    test_ohlc()
+#!/usr/bin/env python
+# -*- coding:utf-8 -*-
+"""
+Date: 2023/7/21 18:16
+Desc: To test intention, just write test code here!
+"""
+import sys
+
+sys.path.append("../marketwatchdata")
+# print(sys.path)
+
+# from marketwatchdata.MarketWatch import *
+import marketwatchdata.MarketWatch as mw
+
+
+def test_ohlc():
+    """
+    just for test aim
+    :return: assert result
+    :rtype: assert
+    """
+    df = mw.ohlc('TMUBMUSD03M', 'P1D', 'P1Y')
+    print(df)
+    assert df.shape[0] > 0
+
+
+if __name__ == "__main__":
+    test_ohlc()
```

