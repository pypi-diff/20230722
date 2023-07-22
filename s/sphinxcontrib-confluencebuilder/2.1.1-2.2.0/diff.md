# Comparing `tmp/sphinxcontrib_confluencebuilder-2.1.1.tar.gz` & `tmp/sphinxcontrib_confluencebuilder-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_confluencebuilder-2.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinxcontrib_confluencebuilder-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinxcontrib_confluencebuilder-2.1.1.tar` & `sphinxcontrib_confluencebuilder-2.2.0.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0     1330 2023-05-16 01:08:09.090533 sphinxcontrib_confluencebuilder-2.1.1/AUTHORS
--rw-r--r--   0        0        0     3159 2023-04-07 19:29:44.215004 sphinxcontrib_confluencebuilder-2.1.1/LICENSE
--rw-r--r--   0        0        0      145 2023-01-02 01:52:19.799871 sphinxcontrib_confluencebuilder-2.1.1/MANIFEST.in
--rw-r--r--   0        0        0     4076 2023-05-16 00:58:11.667937 sphinxcontrib_confluencebuilder-2.1.1/README.rst
--rw-r--r--   0        0        0     1828 2023-05-19 23:40:55.298174 sphinxcontrib_confluencebuilder-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    18061 2023-05-19 23:42:25.549873 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__init__.py
--rw-r--r--   0        0        0     3630 2023-04-07 19:29:44.220864 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__main__.py
--rw-r--r--   0        0        0    14586 2023-04-15 14:46:27.000054 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/assets.py
--rw-r--r--   0        0        0    48600 2023-05-13 15:11:25.713682 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/builder.py
--rw-r--r--   0        0        0        0 2023-01-22 17:27:22.404126 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/__init__.py
--rw-r--r--   0        0        0     2442 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/build.py
--rw-r--r--   0        0        0    11521 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/report.py
--rw-r--r--   0        0        0     6780 2023-04-08 16:47:36.734308 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/wipe.py
--rw-r--r--   0        0        0     3476 2023-04-07 19:29:44.224766 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/compat.py
--rw-r--r--   0        0        0     2929 2023-04-08 16:47:36.735307 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/__init__.py
--rw-r--r--   0        0        0    28152 2023-04-17 01:06:14.719799 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/checks.py
--rw-r--r--   0        0        0     4150 2023-04-16 01:30:57.889226 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/defaults.py
--rw-r--r--   0        0        0     1431 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/env.py
--rw-r--r--   0        0        0     3529 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/manager.py
--rw-r--r--   0        0        0     3402 2023-04-08 16:47:36.736308 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/notifications.py
--rw-r--r--   0        0        0    17687 2023-04-07 19:29:44.229651 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/validation.py
--rw-r--r--   0        0        0    11596 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/directives.py
--rw-r--r--   0        0        0     9196 2023-04-07 19:29:44.230626 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/exceptions.py
--rw-r--r--   0        0        0     3057 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/intersphinx.py
--rw-r--r--   0        0        0      432 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/__init__.py
--rw-r--r--   0        0        0      590 2023-01-05 22:53:18.094822 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1387 2023-05-16 00:43:39.061378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      533 2023-01-05 22:53:18.096782 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1330 2023-05-16 00:43:39.062380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.098731 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.063378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      500 2023-01-05 22:53:18.099707 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      526 2023-01-05 22:53:18.100682 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1323 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      579 2023-01-05 22:53:18.101658 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1376 2023-05-16 00:43:39.065377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      499 2023-01-05 22:53:18.103611 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.066377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      503 2023-01-05 22:53:18.104592 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      518 2023-01-05 22:53:18.106543 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1315 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      460 2023-01-05 22:53:18.108080 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.109032 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2023-01-05 22:53:18.110006 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      500 2023-01-05 22:53:18.111962 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2023-01-05 22:53:18.113918 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.070376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      503 2023-01-05 22:53:18.114891 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      507 2023-01-05 22:53:18.116843 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1333 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2023-01-05 22:53:18.117819 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      573 2023-01-05 22:53:18.118796 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1370 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      510 2023-01-05 22:53:18.120751 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1307 2023-05-16 00:43:39.073376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      497 2023-01-05 22:53:18.122701 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1294 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.124656 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      499 2023-01-05 22:53:18.125629 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      492 2023-01-05 22:53:18.127584 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1289 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      609 2023-01-05 22:53:18.128562 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1406 2023-05-16 00:43:39.076379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2023-01-05 22:53:18.130512 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.077376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      535 2023-01-05 22:53:18.133442 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.080380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      509 2023-01-05 22:53:18.135398 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1306 2023-05-16 00:43:39.081380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      551 2023-01-05 22:53:18.137353 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1351 2023-05-16 00:43:39.082381 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      498 2023-01-05 22:53:18.139304 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1295 2023-05-16 00:43:39.083377 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      648 2023-01-05 22:53:18.141258 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1445 2023-05-16 00:43:39.084381 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      513 2023-01-05 22:53:18.143207 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1313 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      546 2023-01-05 22:53:18.144187 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      623 2023-01-05 22:53:18.146138 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1449 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      458 2023-01-05 22:53:18.148092 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      527 2023-01-05 22:53:18.150044 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1324 2023-05-16 00:43:39.087380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      512 2023-01-05 22:53:18.151996 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1338 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      821 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
--rw-r--r--   0        0        0      511 2023-01-05 22:53:18.153947 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1308 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      540 2023-01-05 22:53:18.155966 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1369 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      502 2023-01-05 22:53:18.158443 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.090376 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      546 2023-01-05 22:53:18.160396 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      538 2023-01-05 22:53:18.162349 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1335 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      505 2023-01-05 22:53:18.164303 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      689 2023-01-05 22:53:18.165278 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1486 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      496 2023-01-05 22:53:18.167232 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1293 2023-05-16 00:43:39.093380 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0      504 2023-01-05 22:48:19.243628 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
--rw-r--r--   0        0        0     1304 2023-05-16 00:43:53.313328 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
--rw-r--r--   0        0        0     4581 2023-04-07 19:29:44.232579 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/logger.py
--rw-r--r--   0        0        0     6304 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/nodes.py
--rw-r--r--   0        0        0    49499 2023-05-14 05:04:32.872359 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/publisher.py
--rw-r--r--   0        0        0      430 2023-04-07 19:29:44.234534 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/reportbuilder.py
--rw-r--r--   0        0        0    14702 2023-04-07 19:29:44.235511 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/rest.py
--rw-r--r--   0        0        0     7784 2023-05-13 21:00:30.924232 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/roles.py
--rw-r--r--   0        0        0    11845 2023-04-07 19:29:44.236486 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/singlebuilder.py
--rw-r--r--   0        0        0     9455 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/state.py
--rw-r--r--   0        0        0        0 2023-01-22 17:27:22.418126 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/__init__.py
--rw-r--r--   0        0        0    12663 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/confluence.py
--rw-r--r--   0        0        0      319 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/sphinx.py
--rw-r--r--   0        0        0     2038 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/__init__.py
--rw-r--r--   0        0        0     4747 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/index.py
--rw-r--r--   0        0        0     1189 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/search.py
--rw-r--r--   0        0        0        0 2023-01-22 17:27:22.420125 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
--rw-r--r--   0        0        0     1801 2023-04-07 19:29:44.240391 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
--rw-r--r--   0        0        0     1634 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
--rw-r--r--   0        0        0     2201 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
--rw-r--r--   0        0        0     2323 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
--rw-r--r--   0        0        0      758 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/search.html
--rw-r--r--   0        0        0   136545 2023-05-19 23:40:45.834292 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/translator.py
--rw-r--r--   0        0        0     7571 2023-04-08 04:21:05.378651 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/svg.py
--rw-r--r--   0        0        0    17887 2023-04-22 17:53:45.115343 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/translator.py
--rw-r--r--   0        0        0    12095 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/__init__.py
--rw-r--r--   0        0        0     1910 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
--rw-r--r--   0        0        0     1743 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
--rw-r--r--   0        0        0     2534 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
--rw-r--r--   0        0        0     1556 2023-04-07 19:29:44.248204 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
--rw-r--r--   0        0        0     4240 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
--rw-r--r--   0        0        0     2520 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
--rw-r--r--   0        0        0    11692 2023-05-14 03:23:15.068220 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/util.py
--rw-r--r--   0        0        0      659 2023-04-07 19:29:44.250159 sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/writer.py
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1458 2023-07-15 02:54:05.316919 sphinxcontrib_confluencebuilder-2.2.0/AUTHORS
+-rw-r--r--   0        0        0     3159 2023-04-07 19:29:44.215004 sphinxcontrib_confluencebuilder-2.2.0/LICENSE
+-rw-r--r--   0        0        0      145 2023-01-02 01:52:19.799871 sphinxcontrib_confluencebuilder-2.2.0/MANIFEST.in
+-rw-r--r--   0        0        0     4076 2023-05-16 00:58:11.667937 sphinxcontrib_confluencebuilder-2.2.0/README.rst
+-rw-r--r--   0        0        0     1828 2023-05-19 23:40:55.298174 sphinxcontrib_confluencebuilder-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    19254 2023-07-22 21:09:47.789169 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/__init__.py
+-rw-r--r--   0        0        0     3630 2023-04-07 19:29:44.220864 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/__main__.py
+-rw-r--r--   0        0        0    14586 2023-04-15 14:46:27.000054 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/assets.py
+-rw-r--r--   0        0        0    49852 2023-07-15 02:54:05.323918 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/builder.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.404126 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/__init__.py
+-rw-r--r--   0        0        0     2442 2023-04-07 19:29:44.222817 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/build.py
+-rw-r--r--   0        0        0    11329 2023-07-15 02:54:05.324918 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/report.py
+-rw-r--r--   0        0        0     6710 2023-07-15 02:54:05.325919 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/wipe.py
+-rw-r--r--   0        0        0     3476 2023-04-07 19:29:44.224766 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/compat.py
+-rw-r--r--   0        0        0     2929 2023-04-08 16:47:36.735307 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/__init__.py
+-rw-r--r--   0        0        0    29224 2023-07-14 20:26:29.674403 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/checks.py
+-rw-r--r--   0        0        0     4347 2023-07-14 20:26:26.739130 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/defaults.py
+-rw-r--r--   0        0        0     1431 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/env.py
+-rw-r--r--   0        0        0     3529 2023-04-07 19:29:44.227698 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/manager.py
+-rw-r--r--   0        0        0     3938 2023-07-15 17:51:40.952288 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/notifications.py
+-rw-r--r--   0        0        0    17687 2023-04-07 19:29:44.229651 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/validation.py
+-rw-r--r--   0        0        0    11798 2023-07-14 20:26:26.740128 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/directives.py
+-rw-r--r--   0        0        0    10309 2023-07-22 20:07:30.777500 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/exceptions.py
+-rw-r--r--   0        0        0     3057 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/intersphinx.py
+-rw-r--r--   0        0        0      432 2023-04-07 19:29:44.231602 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/__init__.py
+-rw-r--r--   0        0        0      590 2023-01-05 22:53:18.094822 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1387 2023-05-16 00:43:39.061378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      533 2023-01-05 22:53:18.096782 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1330 2023-05-16 00:43:39.062380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.098731 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.063378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2023-01-05 22:53:18.099707 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      526 2023-01-05 22:53:18.100682 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1323 2023-05-16 00:43:39.064377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      579 2023-01-05 22:53:18.101658 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1376 2023-05-16 00:43:39.065377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2023-01-05 22:53:18.103611 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.066377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2023-01-05 22:53:18.104592 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      518 2023-01-05 22:53:18.106543 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1315 2023-05-16 00:43:39.067377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      460 2023-01-05 22:53:18.108080 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.109032 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.068378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.110006 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      500 2023-01-05 22:53:18.111962 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1297 2023-05-16 00:43:39.069379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.113918 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.070376 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      503 2023-01-05 22:53:18.114891 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1300 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      507 2023-01-05 22:53:18.116843 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1333 2023-05-16 00:43:39.071378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.117819 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      573 2023-01-05 22:53:18.118796 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1370 2023-05-16 00:43:39.072377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      510 2023-01-05 22:53:18.120751 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1307 2023-05-16 00:43:39.073376 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      497 2023-01-05 22:53:18.122701 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1294 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.124656 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1284 2023-05-16 00:43:39.074377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      499 2023-01-05 22:53:18.125629 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1296 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      492 2023-01-05 22:53:18.127584 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1289 2023-05-16 00:43:39.075377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      609 2023-01-05 22:53:18.128562 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1406 2023-05-16 00:43:39.076379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.130512 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.077376 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      535 2023-01-05 22:53:18.133442 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1332 2023-05-16 00:43:39.080380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      509 2023-01-05 22:53:18.135398 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1306 2023-05-16 00:43:39.081380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      551 2023-01-05 22:53:18.137353 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1351 2023-05-16 00:43:39.082381 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      498 2023-01-05 22:53:18.139304 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1295 2023-05-16 00:43:39.083377 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      648 2023-01-05 22:53:18.141258 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1445 2023-05-16 00:43:39.084381 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      513 2023-01-05 22:53:18.143207 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1313 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2023-01-05 22:53:18.144187 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.085380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      623 2023-01-05 22:53:18.146138 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1449 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      458 2023-01-05 22:53:18.148092 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1287 2023-05-16 00:43:39.086379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      527 2023-01-05 22:53:18.150044 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1324 2023-05-16 00:43:39.087380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      512 2023-01-05 22:53:18.151996 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1338 2023-05-16 00:43:39.088379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      821 2023-07-22 20:07:30.778499 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot
+-rw-r--r--   0        0        0      511 2023-01-05 22:53:18.153947 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1308 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      540 2023-01-05 22:53:18.155966 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1369 2023-05-16 00:43:39.089376 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      502 2023-01-05 22:53:18.158443 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.090376 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      546 2023-01-05 22:53:18.160396 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1343 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      538 2023-01-05 22:53:18.162349 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1335 2023-05-16 00:43:39.091378 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      505 2023-01-05 22:53:18.164303 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1302 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      689 2023-01-05 22:53:18.165278 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1486 2023-05-16 00:43:39.092379 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      496 2023-01-05 22:53:18.167232 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1293 2023-05-16 00:43:39.093380 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0      504 2023-01-05 22:48:19.243628 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo
+-rw-r--r--   0        0        0     1304 2023-05-16 00:43:53.313328 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po
+-rw-r--r--   0        0        0     4581 2023-04-07 19:29:44.232579 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/logger.py
+-rw-r--r--   0        0        0     6304 2023-05-13 21:00:30.923234 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/nodes.py
+-rw-r--r--   0        0        0    52073 2023-07-22 20:07:30.779499 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/publisher.py
+-rw-r--r--   0        0        0      430 2023-04-07 19:29:44.234534 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/reportbuilder.py
+-rw-r--r--   0        0        0    14725 2023-07-15 02:54:05.327918 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/rest.py
+-rw-r--r--   0        0        0     7784 2023-05-13 21:00:30.924232 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/roles.py
+-rw-r--r--   0        0        0    11845 2023-04-07 19:29:44.236486 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/singlebuilder.py
+-rw-r--r--   0        0        0     9455 2023-04-07 19:29:44.237465 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/state.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.418126 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/std/__init__.py
+-rw-r--r--   0        0        0    13575 2023-07-15 17:51:40.953289 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/std/confluence.py
+-rw-r--r--   0        0        0      319 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/std/sphinx.py
+-rw-r--r--   0        0        0     2038 2023-04-07 19:29:44.238438 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/__init__.py
+-rw-r--r--   0        0        0     4747 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/index.py
+-rw-r--r--   0        0        0     1189 2023-04-07 19:29:44.239414 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/search.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:27:22.420125 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/__init__.py
+-rw-r--r--   0        0        0     1801 2023-04-07 19:29:44.240391 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html
+-rw-r--r--   0        0        0     1634 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html
+-rw-r--r--   0        0        0     2201 2023-04-07 19:29:44.241370 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html
+-rw-r--r--   0        0        0     2323 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html
+-rw-r--r--   0        0        0      758 2023-04-07 19:29:44.242347 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/search.html
+-rw-r--r--   0        0        0   143286 2023-07-22 20:07:30.781499 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/translator.py
+-rw-r--r--   0        0        0     7571 2023-04-08 04:21:05.378651 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/svg.py
+-rw-r--r--   0        0        0    17887 2023-07-15 17:28:53.955148 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/translator.py
+-rw-r--r--   0        0        0    12095 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/__init__.py
+-rw-r--r--   0        0        0     1910 2023-04-07 19:29:44.246253 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py
+-rw-r--r--   0        0        0     1743 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py
+-rw-r--r--   0        0        0     2534 2023-04-07 19:29:44.247227 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py
+-rw-r--r--   0        0        0     1556 2023-04-07 19:29:44.248204 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py
+-rw-r--r--   0        0        0     4240 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py
+-rw-r--r--   0        0        0     2520 2023-04-07 19:29:44.249180 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py
+-rw-r--r--   0        0        0    11692 2023-05-14 03:23:15.068220 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/util.py
+-rw-r--r--   0        0        0      659 2023-04-07 19:29:44.250159 sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/writer.py
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 sphinxcontrib_confluencebuilder-2.2.0/PKG-INFO
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/AUTHORS` & `sphinxcontrib_confluencebuilder-2.2.0/AUTHORS`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+Aleksandr Musorin <aleksandr.musorin@semrush.com>
 Anthony Shaw <anthony.p.shaw@gmail.com>
 Anton <box4android@gmail.com>
+Brian Pandola <bpandola@gmail.com>
 Colin Starner <colin.starner@gmail.com>
 Daniel Gray <dg.dan.b@gmail.com>
 Dave Finke <dave.finke@artisancells.com>
 Denis Chugunov <Chugunov_official@mail.ru>
 Felix Sherrington-Kendall <sherrinj@tcd.ie>
 Fernando Gargiulo <fernando.gargiulo@enel.com>
 Freek Dijkstra <software@macfreek.nl>
@@ -20,14 +22,15 @@
 Marius van Niekerk <marius.v.niekerk@gmail.com>
 Mateusz Kostyła <mateusz.kostyla@schange.com>
 Michael Kunzmann <michael.kunzmann@gmx.net>
 Michał Sochoń <kaszpir@gmail.com>
 Paul D.Smith <paul@pauldsmith.org.uk>
 Pawel Limanowka <plimanowka@gmail.com>
 Richard Vodden <richard@humanisingautonomy.com>
+Sydney Jones <sydney.u.jones@gmail.com>
 Thomas Malcher <malcher@student.tugraz.at>
 Toni Ruža <toni.ruza@gmail.com>
 Tsvi Mostovicz <ttmost@gmail.com>
 Zed Tan <zed@shootbird.work>
 girivs82 <32936671+girivs82@users.noreply.github.com>
 pyracode <info@pyracode.net>
 sumau <soumaya.mauthoor@gmail.com>
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/LICENSE` & `sphinxcontrib_confluencebuilder-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/README.rst` & `sphinxcontrib_confluencebuilder-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/pyproject.toml` & `sphinxcontrib_confluencebuilder-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__init__.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # load imgmath extension if available to handle math configuration options
 try:
     from sphinx.ext import imgmath
 except ImportError:
     imgmath = None
 
-__version__ = '2.1.1'
+__version__ = '2.2.0'
 
 
 def setup(app):
     ConfluenceLogger.initialize()
     cm = app.config_manager_ = ConfigManager(app)
 
     app.require_sphinx('1.8')
@@ -76,41 +76,43 @@
     # Username to login to Confluence API with.
     cm.add_conf('confluence_server_user')
     # Confluence Space to publish to.
     cm.add_conf('confluence_space_key')
 
     # (configuration - generic)
     # Add page and section numbers if doctree has :numbered: option
-    cm.add_conf_bool('confluence_add_secnumbers', 'env')
+    cm.add_conf_bool('confluence_add_secnumbers', 'confluence')
+    # Specify the color scheme used for displaying code blocks.
+    cm.add_conf('confluence_code_block_theme', 'confluence')
     # Default alignment for tables, figures, etc.
-    cm.add_conf('confluence_default_alignment', 'env')
+    cm.add_conf('confluence_default_alignment', 'confluence')
     # Enablement of a generated domain index documents
     cm.add_conf('confluence_domain_indices')
     # Confluence editor to target for publication.
-    cm.add_conf('confluence_editor', 'env')
+    cm.add_conf('confluence_editor', 'confluence')
     # File to get page header information from.
-    cm.add_conf('confluence_header_file', 'env')
+    cm.add_conf('confluence_header_file', 'confluence')
     # Dictionary to pass to header when rendering template
-    cm.add_conf('confluence_header_data', 'env')
+    cm.add_conf('confluence_header_data', 'confluence')
     # File to get page footer information from.
-    cm.add_conf('confluence_footer_file', 'env')
+    cm.add_conf('confluence_footer_file', 'confluence')
     # Dictionary to pass to footer when rendering template.
-    cm.add_conf('confluence_footer_data', 'env')
+    cm.add_conf('confluence_footer_data', 'confluence')
     # Enablement of a generated search documents
     cm.add_conf_bool('confluence_include_search')
     # Enablement of a "page generated" notice.
-    cm.add_conf_bool('confluence_page_generation_notice', 'env')
+    cm.add_conf_bool('confluence_page_generation_notice', 'confluence')
     # Enablement of publishing pages into a hierarchy from a root toctree.
     cm.add_conf_bool('confluence_page_hierarchy')
     # Show previous/next buttons (bottom, top, both, None).
-    cm.add_conf('confluence_prev_next_buttons_location', 'env')
+    cm.add_conf('confluence_prev_next_buttons_location', 'confluence')
     # Suffix to put after section numbers, before section name
-    cm.add_conf('confluence_secnumber_suffix', 'env')
+    cm.add_conf('confluence_secnumber_suffix', 'confluence')
     # Enablement of a "Edit/Show Source" reference on each document
-    cm.add_conf('confluence_sourcelink', 'env')
+    cm.add_conf('confluence_sourcelink', 'confluence')
     # Enablement of a generated index document
     cm.add_conf_bool('confluence_use_index')
     # Enablement for toctrees for singleconfluence documents.
     cm.add_conf_bool('singleconfluence_toctree', 'singleconfluence')
 
     # (configuration - publishing)
     # Request for publish password to come from interactive session.
@@ -129,58 +131,60 @@
     cm.add_conf_bool('confluence_disable_autogen_title')
     # Explicitly prevent page notifications on update.
     cm.add_conf_bool('confluence_disable_notifications')
     # Define a series of labels to apply to all published pages.
     cm.add_conf('confluence_global_labels')
     # Enablement of configuring root as space's homepage.
     cm.add_conf_bool('confluence_root_homepage')
+    # Translation to override parent page identifier to publish to.
+    cm.add_conf('confluence_parent_override_transform')
     # Parent page's name or identifier to publish documents under.
     cm.add_conf('confluence_parent_page')
     # Perform a dry run of publishing to inspect what publishing will do.
     cm.add_conf_bool('confluence_publish_dryrun')
     # Publish only new content (no page updates, etc.).
     cm.add_conf_bool('confluence_publish_onlynew')
     # Publish orphan pages to Confluence.
     cm.add_conf_bool('confluence_publish_orphan')
     # Container page to publish orphan pages under.
     cm.add_conf_int('confluence_publish_orphan_container')
     # Postfix to apply to title of published pages.
-    cm.add_conf('confluence_publish_postfix', 'env')
+    cm.add_conf('confluence_publish_postfix', 'confluence')
     # Prefix to apply to published pages.
-    cm.add_conf('confluence_publish_prefix', 'env')
+    cm.add_conf('confluence_publish_prefix', 'confluence')
     # Root page's identifier to publish documents into.
     cm.add_conf_int('confluence_publish_root')
     # docname-2-title dictionary for title overrides.
-    cm.add_conf('confluence_title_overrides', 'env')
+    cm.add_conf('confluence_title_overrides', 'confluence')
     # Timeout for network-related calls (publishing).
     cm.add_conf_int('confluence_timeout')
     # Whether or not new content should be watched.
     cm.add_conf_bool('confluence_watch')
 
     # (configuration - advanced publishing)
     # Register additional mime types to be selected for image candidates.
-    cm.add_conf('confluence_additional_mime_types', 'env')
+    cm.add_conf('confluence_additional_mime_types', 'confluence')
     # Whether or not labels will be appended instead of overwriting them.
     cm.add_conf_bool('confluence_append_labels')
     # Forcing all assets to be standalone.
-    cm.add_conf_bool('confluence_asset_force_standalone', 'env')
+    cm.add_conf_bool('confluence_asset_force_standalone', 'confluence')
     # Tri-state asset handling (auto, force push or disable).
     cm.add_conf_bool('confluence_asset_override')
     # File/path to Certificate Authority
     cm.add_conf('confluence_ca_cert')
     # Path to client certificate to use for publishing
     cm.add_conf('confluence_client_cert')
     # Password for client certificate to use for publishing
     cm.add_conf('confluence_client_cert_pass')
     # Disable SSL validation with Confluence server.
     cm.add_conf_bool('confluence_disable_ssl_validation')
-    # Whether to utilize the full width of a Confluence page (v2 only).
-    cm.add_conf_bool('confluence_full_width')
+    # Whether to utilize the full width of a Confluence page.
+    cm.add_conf_bool('confluence_full_width', 'confluence')
     # Ignore adding a titlefix on the index document.
-    cm.add_conf_bool('confluence_ignore_titlefix_on_index', 'env')
+    cm.add_conf_bool('confluence_ignore_titlefix_on_index', 'confluence')
     # Parent page's identifier to publish documents under.
     cm.add_conf_int('confluence_parent_page_id_check')
     # Proxy server needed to communicate with Confluence server.
     cm.add_conf('confluence_proxy')
     # Subset of documents which are allowed to be published.
     cm.add_conf('confluence_publish_allowlist')
     # Enable debugging for publish requests.
@@ -204,57 +208,61 @@
     # Cookie(s) to use for Confluence REST interaction.
     cm.add_conf('confluence_server_cookies')
     # Comment added to confluence version history.
     cm.add_conf('confluence_version_comment')
 
     # (configuration - advanced processing)
     # Filename suffix for generated files.
-    cm.add_conf('confluence_file_suffix', 'env')
+    cm.add_conf('confluence_file_suffix', 'confluence')
     # Translation of docname to a filename.
-    cm.add_conf('confluence_file_transform', 'env')
+    cm.add_conf('confluence_file_transform', 'confluence')
     # Configuration for named JIRA Servers
-    cm.add_conf('confluence_jira_servers', 'env')
+    cm.add_conf('confluence_jira_servers', 'confluence')
     # Translation of a raw language to code block macro language.
-    cm.add_conf('confluence_lang_transform', 'env')
+    cm.add_conf('confluence_lang_transform', 'confluence')
     # Macro configuration for Confluence-managed LaTeX content.
-    cm.add_conf('confluence_latex_macro', 'env')
+    cm.add_conf('confluence_latex_macro', 'confluence')
     # Link suffix for generated files.
-    cm.add_conf('confluence_link_suffix', 'env')
+    cm.add_conf('confluence_link_suffix', 'confluence')
     # Translation of docname to a (partial) URI.
-    cm.add_conf('confluence_link_transform', 'env')
+    cm.add_conf('confluence_link_transform', 'confluence')
     # Mappings for documentation mentions to Confluence keys.
-    cm.add_conf('confluence_mentions', 'env')
+    cm.add_conf('confluence_mentions', 'confluence')
     # Inject navigational hints into the documentation.
     cm.add_conf('confluence_navdocs_transform')
+    # Enablement of permitting raw html blocks to be used in storage format.
+    cm.add_conf('confluence_permit_raw_html', 'confluence')
     # Remove a detected title from generated documents.
-    cm.add_conf_bool('confluence_remove_title', 'env')
+    cm.add_conf_bool('confluence_remove_title', 'confluence')
 
     # (configuration - undocumented)
     # Enablement for bulk archiving of packages (for premium environments).
     cm.add_conf_bool('confluence_adv_bulk_archiving')
     # Flag to permit the use of embedded certificates from requests.
     cm.add_conf_bool('confluence_adv_embedded_certs')
     # List of node types to ignore if no translator support exists.
     cm.add_conf('confluence_adv_ignore_nodes')
     # Unknown node handler dictionary for advanced integrations.
     cm.add_conf('confluence_adv_node_handler')
     # Permit any string value to be provided as the editor.
-    cm.add_conf('confluence_adv_permit_editor', 'env')
-    # Enablement of permitting raw html blocks to be used in storage format.
-    cm.add_conf_bool('confluence_adv_permit_raw_html', 'env')
+    cm.add_conf('confluence_adv_permit_editor', 'confluence')
+    # Flag to tweak code-block CDATA EOFs to prevent publishing issues.
+    cm.add_conf_bool('confluence_adv_quirk_cdata')
     # List of optional features/macros/etc. restricted for use.
-    cm.add_conf('confluence_adv_restricted', 'env')
+    cm.add_conf('confluence_adv_restricted', 'confluence')
     # Enablement of tracing processed data.
     cm.add_conf_bool('confluence_adv_trace_data')
     # Do not cap sections to a maximum of six (6) levels.
-    cm.add_conf_bool('confluence_adv_writer_no_section_cap', 'env')
+    cm.add_conf_bool('confluence_adv_writer_no_section_cap', 'confluence')
 
     # (configuration - deprecated)
     # replaced by confluence_cleanup_search_mode
     cm.add_conf_bool('confluence_adv_aggressive_search')
+    # replaced by confluence_permit_raw_html
+    cm.add_conf_bool('confluence_adv_permit_raw_html')
     # replaced by confluence_root_homepage
     cm.add_conf('confluence_master_homepage')
     # replaced by confluence_publish_allowlist
     cm.add_conf('confluence_publish_subset')
     # replaced by confluence_purge_from_root
     cm.add_conf_bool('confluence_purge_from_master')
     # replaced by confluence_cleanup_from_root
@@ -320,15 +328,28 @@
     app.add_role('confluence_latex', ConfluenceLatexRole)
     app.add_role('confluence_link', ConfluenceLinkRole)
     app.add_role('confluence_mention', ConfluenceMentionRole)
     app.add_role('confluence_status', ConfluenceStatusRole)
     app.add_role('confluence_strike', ConfluenceStrikeRole)
     app.add_role('jira', JiraRole)
 
-    # inject compatible autosummary nodes if the extension is available/loaded
+    # other
+    confluence_autosummary_support(app)
+    confluence_imgmath_support(app)
+    confluence_remove_mathnodemigrator(app)
+
+
+def confluence_autosummary_support(app):
+    """
+    inject compatible autosummary nodes if the extension is available/loaded
+
+    Args:
+        app: the sphinx application
+    """
+
     if autosummary:
         for ext in app.extensions.values():
             if ext.name == 'sphinx.ext.autosummary':
                 app.registry.add_translation_handlers(
                     autosummary.autosummary_table,
                     confluence=(
                         autosummary.autosummary_table_visit_html,
@@ -348,23 +369,41 @@
                     singleconfluence=(
                         autosummary.autosummary_toc_visit_html,
                         autosummary.autosummary_noop,
                     ),
                 )
                 break
 
-    # lazy bind sphinx.ext.imgmath to provide configuration options
-    #
-    # If 'sphinx.ext.imgmath' is not already explicitly loaded, bind it into the
-    # setup process to a configurer can use the same configuration options
-    # outlined in the sphinx.ext.imgmath in this extension.
+
+def confluence_imgmath_support(app):
+    """
+    lazy bind sphinx.ext.imgmath to provide configuration options
+
+    If 'sphinx.ext.imgmath' is not already explicitly loaded, bind it into the
+    setup process to a configurer can use the same configuration options
+    outlined in the sphinx.ext.imgmath in this extension.
+
+    Args:
+        app: the sphinx application
+    """
+
     if imgmath is not None:
         if 'sphinx.ext.imgmath' not in app.config.extensions:
             imgmath.setup(app)
 
-    # remove math-node-migration post-transform as this extension manages both
-    # future and legacy math implementations (removing this transform removes
-    # a warning notification to the user)
+
+def confluence_remove_mathnodemigrator(app):
+    """
+    remove math-node-migration post-transform
+
+    Remove math-node-migration post-transform as this extension manages both
+    future and legacy math implementations (removing this transform removes
+    a warning notification to the user)
+
+    Args:
+        app: the sphinx application
+    """
+
     for transform in app.registry.get_post_transforms():
         if transform.__name__ == 'MathNodeMigrator':
             app.registry.get_post_transforms().remove(transform)
             break
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/__main__.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/__main__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/assets.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/assets.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/builder.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 import tempfile
 
 
 class ConfluenceBuilder(Builder):
     allow_parallel = True
     default_translator_class = ConfluenceStorageFormatTranslator
     name = 'confluence'
-    format = 'confluence_storage'
+    format = 'confluence_storage'  # noqa: A003
     supported_image_types = ConfluenceSupportedImages()
     supported_linkcode = True
     supported_remote_images = True
 
     def __init__(self, app, env=None):
         # As of Sphinx v5.1.0, builders will accept an `env` option to
         # configure against an environment (over later having an environment
@@ -223,15 +223,15 @@
                 targetmtime = path.getmtime(targetname)
             except Exception:
                 targetmtime = 0
             try:
                 srcmtime = path.getmtime(sourcename)
                 if srcmtime > targetmtime:
                     yield docname
-            except EnvironmentError:
+            except OSError:
                 # source doesn't exist anymore
                 pass
 
     def get_target_uri(self, docname, typ=None):
         return self.link_transform(docname)
 
     def prepare_writing(self, docnames):
@@ -358,15 +358,15 @@
         if self.use_index and 'genindex' in nav_docnames:
             nav_docnames.remove('genindex')
 
         if self.use_search and 'search' in nav_docnames:
             nav_docnames.remove('search')
 
         if self.domain_indices:
-            for indexname, indexdata in self.domain_indices.items():
+            for indexname in self.domain_indices:
                 if indexname in nav_docnames:
                     nav_docnames.remove(indexname)
 
         navdocs_transform = self.config.confluence_navdocs_transform
         if navdocs_transform:
             nav_docnames = navdocs_transform(self, nav_docnames)
 
@@ -476,15 +476,15 @@
         outfilename = path.join(self.outdir, self.file_transform(docname))
         if self.writer.output is not None:
             ensuredir(path.dirname(outfilename))
             try:
                 with open(outfilename, 'w', encoding='utf-8') as file:
                     if self.writer.output:
                         file.write(self.writer.output)
-            except (IOError, OSError) as err:
+            except OSError as err:
                 self.warn(f'error writing file {outfilename}: {err}')
 
     def publish_doc(self, docname, output):
         conf = self.config
         title = self.state.title(docname)
         is_root_doc = self.config.root_doc == docname
 
@@ -500,30 +500,26 @@
             # page, override the parent to publish under; either the provided
             # orphan root ID or no parent (zero value)
             orphan_root_id = conf.confluence_publish_orphan_container
             if orphan_root_id is not None:
                 if docname in self.orphan_docnames:
                     parent_id = orphan_root_id
 
-        data = {
-            'content': output,
-            'labels': [],
-        }
-
-        if self.config.confluence_global_labels:
-            data['labels'].extend(self.config.confluence_global_labels)
-
-        metadata = self.metadata[docname]
-        if 'labels' in metadata:
-            data['labels'].extend([v for v in metadata['labels']])
+        data = self._prepare_page_data(docname, output)
 
         if conf.confluence_publish_root and is_root_doc:
             uploaded_id = self.publisher.store_page_by_id(title,
                 conf.confluence_publish_root, data)
         else:
+            po_transform = conf.confluence_parent_override_transform
+            if po_transform:
+                new_parent_id = po_transform(docname, parent_id)
+                if new_parent_id:
+                    parent_id = new_parent_id
+
             uploaded_id = self.publisher.store_page(title, data, parent_id)
         self.state.register_upload_id(docname, uploaded_id)
 
         if self.config.root_doc == docname:
             self.root_doc_page_id = uploaded_id
 
             # populate ancestors to be used to pre-check ancestors assignments
@@ -566,14 +562,51 @@
                     attachments = self.publisher.get_attachments(legacy_page)
                     self.legacy_assets[legacy_page] = attachments
 
         if self.post_cleanup:
             if uploaded_id in self.legacy_pages:
                 self.legacy_pages.remove(uploaded_id)
 
+    def _prepare_page_data(self, docname, output):
+        data = {
+            'content': output,
+            'editor': self.config.confluence_editor,
+            'full-width': None,
+            'labels': [],
+        }
+        metadata = self.metadata[docname]
+
+        # apply editor override (if any)
+        if 'editor' in metadata:
+            data['editor'] = metadata['editor']
+
+        # determine appearance
+        #
+        # Note: we do not have an "OFF" for v1 editor since an
+        # appearance hint is ignored; width management in this
+        # case is managed in the translator
+        if 'fullWidth' in metadata:
+            confluence_full_width = (metadata['fullWidth'] == 'true')
+        else:
+            confluence_full_width = self.config.confluence_full_width
+
+        if confluence_full_width:
+            data['full-width'] = 'full-width'
+        else:
+            data['full-width'] = 'default'
+
+        # add global labels and page-specific labels
+        if self.config.confluence_global_labels:
+            data['labels'].extend(self.config.confluence_global_labels)
+
+        if 'labels' in metadata:
+            data['labels'].extend(list(metadata['labels']))
+
+        return data
+
     def publish_asset(self, key, docname, output, type_, hash_):
         conf = self.config
         publisher = self.publisher
 
         title = self.state.title(docname)
         page_id = self.state.upload_id(docname)
 
@@ -728,19 +761,18 @@
                     verbosity=self._verbose):
                 if self._check_publish_skip(docname):
                     self.verbose(docname + ' skipped due to configuration')
                     continue
                 docfile = path.join(self.outdir, self.file_transform(docname))
 
                 try:
-                    with open(docfile, 'r', encoding='utf-8') as file:
+                    with open(docfile, encoding='utf-8') as file:
                         output = file.read()
                         self.publish_doc(docname, output)
-
-                except (IOError, OSError) as err:
+                except OSError as err:
                     self.warn(f'error reading file {docfile}: {err}')
 
             self.info('building intersphinx... ', nonl=(not self._verbose))
             build_intersphinx(self)
             self.info('done')
 
             if self.config.confluence_publish_intersphinx:
@@ -763,15 +795,15 @@
                     self.verbose(key + ' skipped due to configuration')
                     continue
 
                 try:
                     with open(absfile, 'rb') as file:
                         output = file.read()
                         self.publish_asset(key, docname, output, type_, hash_)
-                except (IOError, OSError) as err:
+                except OSError as err:
                     self.warn(f'error reading asset {key}: {err}')
 
             self.publish_cleanup()
             self.publish_finalize()
 
     def cleanup(self):
         if self.publish:
@@ -808,16 +840,21 @@
         Args:
             docname: the document
             doctree: the doctree to extract metadata from
         """
         metadata = self.metadata.setdefault(docname, {})
 
         for node in findall(doctree, confluence_metadata):
-            labels = metadata.setdefault('labels', [])
-            labels.extend(node.params['labels'])
+            for k, v in node.params.items():
+                if k == 'labels':
+                    labels = metadata.setdefault('labels', [])
+                    labels.extend(v)
+                else:
+                    metadata[k] = v
+
             node.parent.remove(node)
 
     def _find_title_element(self, doctree):
         """
         find (if any) the title element of a document
 
         From a provided document's doctree, attempt to extract a possible title
@@ -861,15 +898,15 @@
 
             if self.config.confluence_header_file is not None:
                 fname = path.join(self.env.srcdir,
                     self.config.confluence_header_file)
                 try:
                     with open(fname, encoding='utf-8') as file:
                         header_template_data = file.read() + '\n'
-                except (IOError, OSError) as err:
+                except OSError as err:
                     self.warn(f'error reading file {fname}: {err}')
 
                 # if no data is supplied, the file is plain text
                 if self.config.confluence_header_data is None:
                     self._cached_header_data = header_template_data
                 else:
                     self._cached_header_data = self.templates.render_string(
@@ -883,15 +920,15 @@
 
             if self.config.confluence_footer_file is not None:
                 fname = path.join(self.env.srcdir,
                     self.config.confluence_footer_file)
                 try:
                     with open(fname, encoding='utf-8') as file:
                         footer_template_data = file.read() + '\n'
-                except (IOError, OSError) as err:
+                except OSError as err:
                     self.warn(f'error reading file {fname}: {err}')
 
                 # if no data is supplied, the file is plain text
                 if self.config.confluence_footer_data is None:
                     self._cached_footer_data = footer_template_data
                 else:
                     self._cached_header_data = self.templates.render_string(
@@ -901,15 +938,15 @@
         # generate/replace the document in the output directory
         fname = path.join(self.outdir, docname + self.file_suffix)
         try:
             with open(fname, 'w', encoding='utf-8') as f:
                 f.write(self._cached_header_data)
                 generator(self, docname, f)
                 f.write(self._cached_footer_data)
-        except (IOError, OSError) as err:
+        except OSError as err:
             self.warn('error writing file %s: %s', docname, err)
 
     def _get_doctree(self, docname):
         """
         override 'get_doctree' method
 
         To support document editing, doctree's may be loaded and manipulated
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/build.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/build.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/report.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,64 +72,60 @@
     # setup sphinx engine to extract configuration
     config = {}
     configuration_load_issue = None
     confluence_instance_info = None
     publisher = ConfluencePublisher()
 
     try:
-        with temp_dir() as tmp_dir:
-            with docutils_namespace():
-                print('fetching configuration information...')
-                builder = ConfluenceReportBuilder.name
-                app = Sphinx(
-                    work_dir,            # document sources
-                    work_dir,            # directory with configuration
-                    tmp_dir,             # output for built documents
-                    tmp_dir,             # output for doctree files
-                    builder,             # builder to execute
-                    status=sys.stdout,   # sphinx status output
-                    warning=sys.stderr)  # sphinx warning output
-
-                # apply environment-based configuration changes
-                apply_env_overrides(app.builder)
-
-                # if the configuration is enabled for publishing, check if
-                # we need to ask for authentication information (to perform
-                # the connection sanity checks)
-                if app.config.confluence_publish:
-                    try:
-                        process_ask_configs(app.config)
-                    except ConfluenceConfigurationError:
-                        offline = True
-
-                # extract configuration information
-                cm = app.config_manager_  # pylint: disable=no-member
-                for k, v in app.config.values.items():
-                    raw = getattr(app.config, k)
-                    if raw is None:
-                        continue
-
-                    if callable(raw):
-                        value = '(callable)'
-                    else:
-                        value = raw
-
-                    if not args.full_config and k not in cm.options:
-                        continue
-
-                    # always extract some known builder configurations
-                    if args.full_config and k.startswith(IGNORE_BUILDER_CONFS):
-                        continue
+        with temp_dir() as tmp_dir, docutils_namespace():
+            print('fetching configuration information...')
+            builder = ConfluenceReportBuilder.name
+            app = Sphinx(
+                work_dir,            # document sources
+                work_dir,            # directory with configuration
+                tmp_dir,             # output for built documents
+                tmp_dir,             # output for doctree files
+                builder,             # builder to execute
+                status=sys.stdout,   # sphinx status output
+                warning=sys.stderr)  # sphinx warning output
+
+            # apply environment-based configuration changes
+            apply_env_overrides(app.builder)
+
+            # if the configuration is enabled for publishing, check if
+            # we need to ask for authentication information (to perform
+            # the connection sanity checks)
+            if app.config.confluence_publish:
+                try:
+                    process_ask_configs(app.config)
+                except ConfluenceConfigurationError:
+                    offline = True
+
+            # extract configuration information
+            cm = app.config_manager_  # pylint: disable=no-member
+            for key in app.config.values:
+                raw = getattr(app.config, key)
+                if raw is None:
+                    continue
+
+                value = '(callable)' if callable(raw) else raw
+
+                if not args.full_config and key not in cm.options:
+                    continue
+
+                # always extract some known builder configurations
+                if args.full_config and key.startswith(IGNORE_BUILDER_CONFS):
+                    continue
 
-                    config[k] = value
+                config[key] = value
 
-                # initialize the publisher (if needed later)
-                publisher.init(app.config)
+            # initialize the publisher (if needed later)
+            publisher.init(app.config)
 
-    except Exception:
+    except Exception:  # noqa: BLE001
         sys.stdout.flush()
         tb_msg = traceback.format_exc()
         logger.error(tb_msg)
         if os.path.isfile(os.path.join(work_dir, 'conf.py')):
             configuration_load_issue = 'unable to load configuration'
             configuration_load_issue += '\n\n' + tb_msg.strip()
         else:
@@ -147,15 +143,15 @@
         try:
             print('connecting to confluence instance...')
             sys.stdout.flush()
 
             publisher.connect()
             info += ' connected: yes\n'
             session = publisher.rest_client.session
-        except Exception:
+        except Exception:  # noqa: BLE001
             sys.stdout.flush()
             logger.error(traceback.format_exc())
             info += ' connected: no\n'
             rv = 1
 
         if session:
             try:
@@ -185,15 +181,15 @@
                     for o in root.findall('buildNumber'):
                         info += '     build: ' + o.text + '\n'
                 else:
                     logger.error('bad response from server ({})'.format(
                         rsp.status_code))
                     info += f'   fetched: error ({rsp.status_code})\n'
                     rv = 1
-            except Exception:
+            except Exception:  # noqa: BLE001
                 sys.stdout.flush()
                 logger.error(traceback.format_exc())
                 info += 'failure to determine confluence data\n'
                 rv = 1
 
         confluence_instance_info = info
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/cmd/wipe.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/cmd/wipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,38 +57,37 @@
         return 1
 
     # check configuration and prepare publisher
     dryrun = False
     publisher = None
 
     try:
-        with temp_dir() as tmp_dir:
-            with docutils_namespace():
-                app = Sphinx(
-                    work_dir,            # document sources
-                    work_dir,            # directory with configuration
-                    tmp_dir,             # output for built documents
-                    tmp_dir,             # output for doctree files
-                    'confluence',        # builder to execute
-                    status=sys.stdout,   # sphinx status output
-                    warning=sys.stderr)  # sphinx warning output
-
-                dryrun = app.config.confluence_publish_dryrun
-                server_url = app.config.confluence_server_url
-                space_key = app.config.confluence_space_key
-                parent_ref = app.config.confluence_parent_page
-
-                # initialize the publisher (if permitted)
-                if app.config.confluence_publish:
-                    process_ask_configs(app.config)
+        with temp_dir() as tmp_dir, docutils_namespace():
+            app = Sphinx(
+                work_dir,            # document sources
+                work_dir,            # directory with configuration
+                tmp_dir,             # output for built documents
+                tmp_dir,             # output for doctree files
+                'confluence',        # builder to execute
+                status=sys.stdout,   # sphinx status output
+                warning=sys.stderr)  # sphinx warning output
+
+            dryrun = app.config.confluence_publish_dryrun
+            server_url = app.config.confluence_server_url
+            space_key = app.config.confluence_space_key
+            parent_ref = app.config.confluence_parent_page
+
+            # initialize the publisher (if permitted)
+            if app.config.confluence_publish:
+                process_ask_configs(app.config)
 
-                    publisher = ConfluencePublisher()
-                    publisher.init(app.config)
+                publisher = ConfluencePublisher()
+                publisher.init(app.config)
 
-    except Exception:
+    except Exception:  # noqa: BLE001
         sys.stdout.flush()
         logger.error(traceback.format_exc())
         if os.path.isfile(os.path.join(work_dir, 'conf.py')):
             logger.error('unable to load configuration')
         else:
             logger.error('no documentation/missing configuration')
         return 1
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/compat.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/compat.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/__init__.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/checks.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,20 @@
 
     # confluence_client_cert_pass
     validator.conf('confluence_client_cert_pass') \
              .string()
 
     # ##################################################################
 
+    # confluence_code_block_theme
+    validator.conf('confluence_code_block_theme') \
+        .string()
+
+    # ##################################################################
+
     # confluence_default_alignment
     try:
         validator.conf('confluence_default_alignment') \
                  .matching('left', 'center', 'right')
     except ConfluenceConfigurationError as e:
         raise ConfluenceConfigurationError('''\
 {msg}
@@ -436,14 +442,20 @@
 
     # confluence_navdocs_transform
     validator.conf('confluence_navdocs_transform') \
              .callable_()
 
     # ##################################################################
 
+    # confluence_parent_override_transform
+    validator.conf('confluence_parent_override_transform') \
+             .callable_()
+
+    # ##################################################################
+
     try:
         validator.conf('confluence_parent_page').string()
     except ConfluenceConfigurationError:
         try:
             validator.conf('confluence_parent_page').int_(positive=True)
         except ConfluenceConfigurationError:
             raise ConfluenceConfigurationError('''\
@@ -464,14 +476,31 @@
 
     # confluence_page_generation_notice
     validator.conf('confluence_page_generation_notice') \
              .bool()
 
     # ##################################################################
 
+    # confluence_permit_raw_html
+    try:
+        validator.conf('confluence_permit_raw_html').bool()
+    except ConfluenceConfigurationError:
+        try:
+            validator.conf('confluence_permit_raw_html').string()
+        except ConfluenceConfigurationError:
+            raise ConfluenceConfigurationError('''\
+confluence_permit_raw_html is not a boolean or a string
+
+The option 'confluence_permit_raw_html' has been provided to indicate that
+raw HTML should be published. This value can either be set to `True` or
+configured to the name of a supported macro identifier.
+''')
+
+    # ##################################################################
+
     # confluence_prev_next_buttons_location
     try:
         validator.conf('confluence_prev_next_buttons_location') \
                  .matching('bottom', 'both', 'top')
     except ConfluenceConfigurationError as e:
         raise ConfluenceConfigurationError('''\
 {msg}
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/defaults.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/defaults.py`

 * *Files 12% similar despite different names*

```diff
@@ -69,14 +69,18 @@
 
     if conf.confluence_mentions is None:
         conf.confluence_mentions = {}
 
     if conf.confluence_page_hierarchy is None:
         conf.confluence_page_hierarchy = True
 
+    if conf.confluence_permit_raw_html is None and \
+            conf.confluence_adv_permit_raw_html is not None:
+        conf.confluence_permit_raw_html = conf.confluence_adv_permit_raw_html
+
     if conf.confluence_publish_intersphinx is None:
         conf.confluence_publish_intersphinx = True
 
     if conf.confluence_publish_orphan is None:
         conf.confluence_publish_orphan = True
 
     if conf.confluence_remove_title is None:
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/env.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/env.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/manager.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/manager.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/notifications.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/notifications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # SPDX-License-Identifier: BSD-2-Clause
 # Copyright Sphinx Confluence Builder Contributors (AUTHORS)
 
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.std.confluence import EDITORS
+from sphinxcontrib.confluencebuilder.std.confluence import SUPPORTED_CODE_BLOCK_THEMES
 import mimetypes
 
 # dictionary of deprecated configuration entries and associated message
 DEPRECATED_CONFIGS = {
     'confluence_adv_aggressive_search':
         'use "confluence_cleanup_search_mode" instead',
+    'confluence_adv_permit_raw_html':
+        'use "confluence_permit_raw_html" instead',
     'confluence_adv_trace_data':
         'to be removed in a future version',
     'confluence_adv_writer_no_section_cap':
         'to be removed in a future version',
     'confluence_master_homepage':
         'use "confluence_root_homepage" instead',
     'confluence_max_doc_depth':
@@ -67,14 +70,21 @@
     # check if any user defined mime types are unknown
     if config.confluence_additional_mime_types is not None:
         for mime_type in config.confluence_additional_mime_types:
             if not mimetypes.guess_extension(mime_type):
                 logger.warn('confluence_additional_mime_types '
                     'defines an unknown mime type: ' + mime_type)
 
+    # confluence_code_block_theme assigned an unsupported theme
+    if config.confluence_code_block_theme is not None:
+        theme = config.confluence_code_block_theme.lower()
+        if theme not in SUPPORTED_CODE_BLOCK_THEMES:
+            logger.warn('confluence_code_block_theme '
+                        'defines an unknown theme: ' + theme)
+
     # warn when ssl validation is disabled
     if config.confluence_disable_ssl_validation:
         logger.warn('confluence_disable_ssl_validation is set; '
             'consider using confluence_ca_cert instead')
 
     # confluence_file_suffix "cannot" end with a dot
     if (config.confluence_file_suffix and
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/config/validation.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/config/validation.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/directives.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/directives.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from sphinxcontrib.confluencebuilder.nodes import confluence_latex_block
 from sphinxcontrib.confluencebuilder.nodes import confluence_link_card
 from sphinxcontrib.confluencebuilder.nodes import confluence_metadata
 from sphinxcontrib.confluencebuilder.nodes import confluence_newline
 from sphinxcontrib.confluencebuilder.nodes import confluence_toc
 from sphinxcontrib.confluencebuilder.nodes import jira
 from sphinxcontrib.confluencebuilder.nodes import jira_issue
+from sphinxcontrib.confluencebuilder.std.confluence import EDITORS
 from uuid import UUID
 
 
 def string_list(argument):
     """
     string-list validator
 
@@ -179,14 +180,16 @@
 
         return [node]
 
 
 class ConfluenceMetadataDirective(Directive):
     has_content = False
     option_spec = {
+        'editor': lambda x: directives.choice(x, EDITORS),
+        'full-width': lambda x: directives.choice(x, ('true', 'false')),
         'labels': string_list,
     }
 
     def run(self):
         node = confluence_metadata()
 
         for k, v in self.options.items():
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/exceptions.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
 If the above does not appear to be related to the current use case,
 please inform the maintainers of this extension.
 ---
 '''.format(name=page_name))
 
 
-class ConfluenceRateLimited(ConfluenceError):
+class ConfluenceRateLimitedError(ConfluenceError):
     def __init__(self):
         super().__init__('''
 ---
 Request has been rate limited
 
 The configured Confluence instance is reporting that too many requests
 are being made and has instructed to client to limit the amount of
@@ -259,14 +259,43 @@
 
    {url}
 
 ---
 '''.format(url=server_url))
 
 
+class ConfluenceUnexpectedCdataError(ConfluenceError):
+    def __init__(self):
+        super().__init__('''
+---
+Unexpected Confluence XML stream CDATA parsing error
+
+Confluence has reported an error processing a document which contains
+CDATA data (e.g. a code block using `<![CDATA[data]]>`). This is
+unexpected since the data should be properly formed. There is a high
+chance that this is occurring on a Confluence instance which introduced
+some processing logic that incorrectly breaks the parsing of CDATA EOF
+strings (as of Confluence 8.x). This should be addressed in Confluence
+8.3.0 (or newer) release [1].
+
+To workaround this issue for the configured Confluence instance, a user
+can enable the `confluence_adv_quirk_cdata` inside their `conf.py`
+configuration file. For example:
+
+    confluence_adv_quirk_cdata = True
+
+If enabling this option does not resolve the publication issue, then
+this error message does not apply. Feel free to report this issue noting
+the exception message above this message.
+
+[1]: https://jira.atlassian.com/browse/CONFSERVER-82849
+---
+''')
+
+
 class ConfluenceUnreconciledPageError(ConfluenceError):
     def __init__(self, page_name, page_id, url, ex):
         super().__init__('''
 ---
 Unable to update unreconciled page: {name} (id: {id})
 
 Unable to update the target page due to the Confluence instance
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/intersphinx.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/intersphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ar/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bg/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/bn/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ca/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cs/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/cy/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/da/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/de/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/el/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/eo/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/es/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/et/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/eu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/fi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/fr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/he/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/hu/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/id/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/it/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ja/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ko/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lt/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/lv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/mk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/nb/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ne/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/nl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/pt_BR/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ro/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ru/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/si/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sl/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sphinxcontrib.confluencebuilder.pot`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#: sphinxcontrib/confluencebuilder/singlebuilder.py:81
+#: sphinxcontrib/confluencebuilder/singlebuilder.py:78
 msgid "assembling single confluence document"
 msgstr ""
 
-#: sphinxcontrib/confluencebuilder/singlebuilder.py:110
+#: sphinxcontrib/confluencebuilder/singlebuilder.py:107
 msgid "writing single confluence document"
 msgstr ""
 
 #: sphinxcontrib/confluencebuilder/storage/templates/domainindex.html:11
 #: sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html:11
 #: sphinxcontrib/confluencebuilder/storage/templates/genindex.html:37
 #: sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html:37
 #: sphinxcontrib/confluencebuilder/storage/templates/search.html:10
-#: sphinxcontrib/confluencebuilder/storage/translator.py:2299
+#: sphinxcontrib/confluencebuilder/storage/translator.py:2459
 msgid "This page has been automatically generated."
 msgstr ""
 
-#: sphinxcontrib/confluencebuilder/storage/translator.py:2323
+#: sphinxcontrib/confluencebuilder/storage/translator.py:2483
 msgid "Edit Source"
 msgstr ""
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sq/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sr_CS/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/sv/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/ta/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/te/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/tr/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.mo`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/uk/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/vi/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/locale/zh_TW/LC_MESSAGES/sphinxcontrib.confluencebuilder.po`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/logger.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/logger.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/nodes.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/nodes.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/publisher.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/publisher.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadServerUrlError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadSpaceError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceConfigurationError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceMissingPageIdError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePermissionError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePublishAncestorError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePublishSelfAncestorError
+from sphinxcontrib.confluencebuilder.exceptions import ConfluenceUnexpectedCdataError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceUnreconciledPageError
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.rest import Rest
 from sphinxcontrib.confluencebuilder.util import ConfluenceUtil
 import json
 import logging
 import time
@@ -28,27 +29,25 @@
 # key used for managing this extension's properties on a Confluence instance
 PROP_KEY = 'sphinx'
 
 
 class ConfluencePublisher:
     def __init__(self):
         self.cloud = None
-        self.editor = None
         self.space_display_name = None
         self.space_type = None
         self._ancestors_cache = set()
         self._name_cache = {}
 
     def init(self, config, cloud=None):
         self.cloud = cloud
         self.config = config
         self.append_labels = config.confluence_append_labels
         self.debug = config.confluence_publish_debug
         self.dryrun = config.confluence_publish_dryrun
-        self.editor = config.confluence_editor
         self.notify = not config.confluence_disable_notifications
         self.onlynew = config.confluence_publish_onlynew
         self.parent_id = config.confluence_parent_page_id_check
         self.parent_ref = config.confluence_parent_page
         self.server_url = config.confluence_server_url
         self.space_key = config.confluence_space_key
         self.watch = config.confluence_watch
@@ -659,16 +658,16 @@
                 comment = metadata['comment']
 
         if not force and comment:
             parts = comment.split(HASH_KEY + ':', 1)
             if len(parts) > 1:
                 tracked_hash = ''.join(parts[1].split())
                 if hash_ == tracked_hash:
-                    logger.verbose('attachment ({}) is already '
-                        'published to document with same hash'.format(name))
+                    logger.verbose(f'attachment ({name}) is already '
+                        'published to document with same hash')
                     return attachment['id']
 
         if self.dryrun:
             if not attachment:
                 self._dryrun('adding new attachment ' + name)
                 return None
             else:
@@ -793,17 +792,25 @@
                                 self._name_cache[parent_id], parent_id)
                         else:
                             misc += '[new parent page]'
 
                 self._dryrun('updating existing page', page['id'], misc)
                 return page['id']
 
+        # fetch the page data
+        # (expand on certain fields that may be required)
         expand = 'version'
-        if self.append_labels:
+        if parent_id:
+            expand += ',ancestors'
+        if self.append_labels or self.config.confluence_global_labels:
             expand += ',metadata.labels'
+        if data['full-width']:
+            expand += ',metadata.properties.content_appearance_published'
+        if data['editor']:
+            expand += ',metadata.properties.editor'
 
         _, page = self.get_page(page_name, expand=expand)
 
         # if the page is not found, but it determined to be an archived page,
         # Confluence Cloud does not appear to support moving/updating an
         # archived page back into a `current` mode -- instead, try to delete
         # the archived page before generating a new page
@@ -824,20 +831,67 @@
             props = None
 
         # calculate the hash for a page; we will first use this to check if
         # there is a update to apply, and if we do need to update, we will
         # add this value into the page's properties
         new_page_hash = ConfluenceUtil.hash(data['content'])
 
+        # check if we have to force a page update
+        force_publish = self.config.confluence_publish_force
+        if page and not force_publish:
+            metadata = page.get('metadata', {})
+            meta_props = metadata.get('properties', {})
+
+            # if the parent page has changed, force an update
+            if parent_id:
+                parent_changed = True
+                last_ancestor = page.get('ancestors', [])[-1:]
+                if last_ancestor:
+                    if last_ancestor[0].get('id') == str(parent_id):
+                        parent_changed = False
+
+                if parent_changed:
+                    logger.verbose(f'parent changed: {page_name}')
+                    force_publish = True
+
+            # if we are missing any global variables, force publish
+            if self.config.confluence_global_labels:
+                expected_labels = set(self.config.confluence_global_labels)
+                existing_labels = [lbl.get('name')
+                    for lbl in page.get('metadata', {}).get(
+                        'labels', {}).get('results', {})
+                ]
+                if expected_labels.difference(existing_labels):
+                    logger.verbose(f'labels missing: {page_name}')
+                    force_publish = True
+
+            # if instance supports appearance changes and the appearance
+            # looks to be changed, force publish
+            cap_props = meta_props.get('content-appearance-published', {})
+            if cap_props and data['full-width']:
+                current_appearance = cap_props.get('value')
+                if data['full-width'] != current_appearance:
+                    logger.verbose(f'appearance changed: {page_name}')
+                    force_publish = True
+
+            # if instance supports editors and the editor to be changed,
+            # force publish
+            editor_props = meta_props.get('editor', {})
+            if editor_props and data['editor']:
+                current_editor = editor_props.get('value')
+                if data['editor'] != current_editor:
+                    logger.verbose(f'editor changed: {page_name}')
+                    force_publish = True
+
         # if we are not force uploading, check if the new page hash matches
         # the remote hash; if so, do not publish
-        if props and not self.config.confluence_publish_force:
+        if props and not force_publish:
             remote_hash = props.get('value', {}).get('hash')
             if new_page_hash == remote_hash:
-                logger.verbose('no changes in page: {}'.format(page_name))
+                logger.verbose(f'no changes in page: {page_name}')
                 return page['id']
 
         try:
             # new page
             if not page:
                 new_page = self._build_page(page_name, data)
                 self._populate_labels(new_page, data['labels'])
@@ -865,25 +919,28 @@
                     # initial labels need to be applied in their own request
                     labels = new_page['metadata']['labels']
                     if not self.cloud and labels:
                         url = f'content/{uploaded_page_id}/label'
                         self.rest_client.post(url, labels)
 
                 except ConfluenceBadApiError as ex:
+                    if str(ex).find('CDATA block has embedded') != -1:
+                        raise ConfluenceUnexpectedCdataError from ex
+
                     # Check if Confluence reports that the new page request
                     # fails, indicating it already exists. This is usually
                     # (outside of possible permission use cases) that the page
                     # name's casing does not match. In this case, attempt to
                     # re-check for the page in a case-insensitive fashion. If
                     # found, attempt to perform an update request instead.
                     if str(ex).find('title already exists') == -1:
                         raise
 
                     logger.verbose('title already exists warning '
-                        'for page {}'.format(page_name))
+                        f'for page {page_name}')
 
                     _, page = self.get_page_case_insensitive(page_name)
                     if not page:
                         raise
 
                     if self.onlynew:
                         self._onlynew('skipping existing page', page['id'])
@@ -1037,15 +1094,15 @@
             # so, we want to suppress the API error. This is most likely a
             # result of a Confluence instance reporting a page descendant
             # identifier which no longer exists (possibly a caching issue).
             if str(ex).find('No content found with id') == -1:
                 raise
 
             logger.verbose('ignore missing delete for page '
-                'identifier: {}'.format(page_id))
+                f'identifier: {page_id}')
         except ConfluencePermissionError:
             raise ConfluencePermissionError(
                 """Publish user does not have permission to delete """
                 """from the configured space."""
             )
 
     def restrict_ancestors(self, ancestors):
@@ -1116,31 +1173,22 @@
             },
             'version': {
                 'number': 1,
                 'message': self.config.confluence_version_comment,
             },
         }
 
-        if self.editor:
-            page['metadata']['properties'] = {
-                'editor': {
-                    'value': self.editor,
-                },
+        if data['editor']:
+            page['metadata']['properties']['editor'] = {
+                'value': data['editor'],
             }
 
-        if self.config.confluence_full_width is not None:
-            if self.config.confluence_full_width:
-                content_appearance = 'full-width'
-            else:
-                content_appearance = 'default'
-
-            page['metadata']['properties'] = {
-                'content-appearance-published': {
-                    'value': content_appearance,
-                },
+        if data['full-width']:
+            page['metadata']['properties']['content-appearance-published'] = {
+                'value': data['full-width'],
             }
 
         return page
 
     def _update_page(self, page, page_name, data, parent_id=None):
         """
         build a page update and publish it to the confluence instance
@@ -1187,14 +1235,16 @@
         elif parent_id is not None:
             update_page['ancestors'] = [{'id': '1'}]
 
         page_id_explicit = page['id'] + '?status=current'
         try:
             self.rest_client.put('content', page_id_explicit, update_page)
         except ConfluenceBadApiError as ex:
+            if str(ex).find('CDATA block has embedded') != -1:
+                raise ConfluenceUnexpectedCdataError from ex
 
             # Handle select API failures by waiting a moment and retrying the
             # content request. If it happens again, the put request will fail as
             # it normally would.
             retry_errors = [
                 # Confluence Cloud may (rarely) fail to complete a content
                 # request with an OptimisticLockException/
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/rest.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from email.utils import parsedate_tz
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceAuthenticationFailedUrlError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadApiError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceBadServerUrlError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceCertificateError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluencePermissionError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceProxyPermissionError
-from sphinxcontrib.confluencebuilder.exceptions import ConfluenceRateLimited
+from sphinxcontrib.confluencebuilder.exceptions import ConfluenceRateLimitedError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceSeraphAuthenticationFailedUrlError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceSslError
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceTimeoutError
 from sphinxcontrib.confluencebuilder.logger import ConfluenceLogger as logger
 from sphinxcontrib.confluencebuilder.std.confluence import API_REST_BIND_PATH
 from sphinxcontrib.confluencebuilder.std.confluence import NOCHECK
 from sphinxcontrib.confluencebuilder.std.confluence import RSP_HEADER_RETRY_AFTER
@@ -47,15 +47,15 @@
         # SSL context
         if self._config.confluence_client_cert:
             try:
                 cf, kf = self._config.confluence_client_cert
                 pw = self._config.confluence_client_cert_pass
                 context.load_cert_chain(certfile=cf, keyfile=kf, password=pw)
             except ssl.SSLError as ex:
-                raise ConfluenceCertificateError(ex)
+                raise ConfluenceCertificateError(ex) from ex
         # otherwise, load default certificates on the system
         else:
             context.load_default_certs()
 
         if self._config.confluence_disable_ssl_validation:
             context.check_hostname = False
 
@@ -102,15 +102,15 @@
             # delay if requests are going through
             self.last_retry = max(self.last_retry / 2, 1)
 
             attempt = 1
             while True:
                 try:
                     return func(self, *args, **kwargs)
-                except ConfluenceRateLimited as e:
+                except ConfluenceRateLimitedError as e:
                     # if max attempts have been reached, stop any more attempts
                     if attempt > RATE_LIMITED_MAX_RETRIES:
                         raise e
 
                     # determine the amount of delay to wait again -- either from the
                     # provided delay (if any) or exponential backoff
                     if self.next_delay:
@@ -369,8 +369,8 @@
         if rsp.status_code == 401:
             raise ConfluenceAuthenticationFailedUrlError
         if rsp.status_code == 403:
             raise ConfluencePermissionError('rest-call')
         if rsp.status_code == 407:
             raise ConfluenceProxyPermissionError
         if rsp.status_code == 429:
-            raise ConfluenceRateLimited
+            raise ConfluenceRateLimitedError
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/roles.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/roles.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/singlebuilder.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/singlebuilder.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/state.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/state.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/std/confluence.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/std/confluence.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 # The maximum length of a Confluence page is set to 255. This is a Confluence-
 # imposed limitation [1].
 #
 # [1]: confluence-project/confluence-core/confluence/src/
 #       java/com/atlassian/confluence/pages/AbstractPage::isValidTitleLength
 CONFLUENCE_MAX_TITLE_LEN = 255
 
+# maximum width for a non-full-width page (v1; Server/DC)
+#
+# It has been observed that some stock macros would default to a fixed width
+# of "960" (e.g. when using the Widget Connector macro). We will use this as
+# a reference to the max width to ensure no unexpected overflows.
+CONFLUENCE_MAX_WIDTH = 960
+
 # list of supported editors
 EDITORS = [
     'v1',
     'v2',
 ]
 
 # confluence default (paragraph) indent offset (in pixels)
@@ -467,14 +474,33 @@
 # Confluence may response with a `Retry-After` when rate limiting has been
 # imposed on an API request. This entry keeps track of the header key entry
 # which reports the recommended duration till next retry.
 #
 # (see also: https://developer.atlassian.com/cloud/confluence/rate-limiting/)
 RSP_HEADER_RETRY_AFTER = 'Retry-After'
 
+# default code block theme
+DEFAULT_THEME_STYLE = 'default'
+
+# supported code block themes
+#
+# (see also: https://confluence.atlassian.com/doc/code-block-macro-139390.html)
+SUPPORTED_CODE_BLOCK_THEMES = {
+    'confluence': 'Confluence',
+    'django': 'DJango',
+    'eclipse': 'Eclipse',
+    'emacs': 'Emacs',
+    'fadetogrey': 'FadeToGrey',
+    'midnight': 'Midnight',
+    'rdark': 'RDark',
+    # 'Default' is also valid and is usually synonymous with 'Confluence',
+    # unless changed by a user with Confluence Administrator permissions.
+    DEFAULT_THEME_STYLE: 'Default',
+}
+
 # supported image types
 #
 # A list of image types (mostly) supported on a Confluence instance. This
 # includes image types observed in the following Confluence implementation and
 # image typeswhich also observed to be rendering with Confluence Cloud:
 #
 #  confluence/webapp/WEB-INF/classes/mime.types
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/__init__.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/index.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/index.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/search.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/search.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/domainindex_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex.html` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/genindex_v2.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/templates/search.html` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/templates/search.html`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/storage/translator.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/storage/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,31 @@
 from os import path
 from sphinx import addnodes
 from sphinx.locale import _ as SL
 from sphinx.locale import admonitionlabels
 from sphinxcontrib.confluencebuilder.compat import docutils_findall as findall
 from sphinxcontrib.confluencebuilder.exceptions import ConfluenceError
 from sphinxcontrib.confluencebuilder.locale import L
+from sphinxcontrib.confluencebuilder.std.confluence import CONFLUENCE_MAX_WIDTH
 from sphinxcontrib.confluencebuilder.std.confluence import FALLBACK_HIGHLIGHT_STYLE
 from sphinxcontrib.confluencebuilder.std.confluence import FCMMO
 from sphinxcontrib.confluencebuilder.std.confluence import INDENT
 from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_FBMAP_V1
 from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_FBMAP_V2
 from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_MAP_V1
 from sphinxcontrib.confluencebuilder.std.confluence import LITERAL2LANG_MAP_V2
+from sphinxcontrib.confluencebuilder.std.confluence import SUPPORTED_CODE_BLOCK_THEMES
 from sphinxcontrib.confluencebuilder.std.sphinx import DEFAULT_HIGHLIGHT_STYLE
 from sphinxcontrib.confluencebuilder.storage import encode_storage_format
 from sphinxcontrib.confluencebuilder.storage import intern_uri_anchor_value
 from sphinxcontrib.confluencebuilder.translator import ConfluenceBaseTranslator
 from sphinxcontrib.confluencebuilder.util import convert_length
+from sphinxcontrib.confluencebuilder.util import extract_length
 from sphinxcontrib.confluencebuilder.util import first
+import json
 import posixpath
 import re
 import sys
 
 
 class ConfluenceStorageFormatTranslator(ConfluenceBaseTranslator):
     _tracked_unknown_code_lang = []
@@ -41,17 +45,19 @@
     Args:
         document: the document being translated
         builder: the sphinx builder instance
     """
     def __init__(self, document, builder):
         ConfluenceBaseTranslator.__init__(self, document, builder)
         config = builder.config
+        metadata = builder.metadata.get(self.docname, {})
 
         self.add_secnumbers = config.confluence_add_secnumbers
         self.editor = config.confluence_editor
+        self.confluence_full_width = config.confluence_full_width
         self.numfig = config.numfig
         self.numfig_format = config.numfig_format
         self.secnumber_suffix = config.confluence_secnumber_suffix
         self.todo_include_todos = getattr(config, 'todo_include_todos', None)
         self.v2 = config.confluence_editor == 'v2'
         self._building_footnotes = False
         self._figure_context = []
@@ -61,14 +67,24 @@
         self._needs_navnode_spacing = False
         self._reference_context = []
         self._thead_context = []
         self._v2_header_added = False
         self.colspecs = []
         self._tocdepth = self.state.toctree_depth(self.docname)
 
+        # override editor if the document specifies another
+        editor_override = metadata.get('editor')
+        if editor_override:
+            self.editor = editor_override
+
+        # override full-width option if the document hints to override
+        fw_override = metadata.get('fullWidth')
+        if fw_override:
+            self.confluence_full_width = (fw_override == 'true')
+
     def encode(self, text):
         text = encode_storage_format(text)
         return ConfluenceBaseTranslator.encode(self, text)
 
     # ---------
     # structure
     # ---------
@@ -162,28 +178,35 @@
     def pre_body_data(self):
         data = ''
 
         # Confluence's v1 editor ignores a full-width page style on
         # publication (most likely since the concept of page width was
         # developed for v2 and newer). To emulate a non-full-width state with
         # a v1 editor, apply a layout around the page contents.
-        if not self.v2 and self.builder.config.confluence_full_width is False:
-            data += '<ac:layout>'
-            data += '<ac:layout-section ac:type="fixed-width">'
-            data += '<ac:layout-cell>'
+        if not self.v2 and self.confluence_full_width is False:
+            if self.builder.cloud:
+                data += '<ac:layout>'
+                data += '<ac:layout-section ac:type="fixed-width">'
+                data += '<ac:layout-cell>'
+            else:
+                max_width = f'{CONFLUENCE_MAX_WIDTH}px'
+                data += f'<div style="max-width: {max_width}; margin: 0 auto;">'
 
         return data
 
     def post_body_data(self):
         data = ''
 
-        if not self.v2 and self.builder.config.confluence_full_width is False:
-            data += '</ac:layout-cell>'
-            data += '</ac:layout-section>'
-            data += '</ac:layout>'
+        if not self.v2 and self.confluence_full_width is False:
+            if self.builder.cloud:
+                data += '</ac:layout-cell>'
+                data += '</ac:layout-section>'
+                data += '</ac:layout>'
+            else:
+                data += '</div>'
 
         return data
 
     def visit_title(self, node):
         if isinstance(node.parent, (nodes.section, nodes.topic)):
             self.body.append(
                 self._start_tag(node, f'h{self._title_level}'))
@@ -755,17 +778,33 @@
             with suppress(KeyError):
                 firstline = node.attributes['highlight_args']['linenostart']
 
         self.body.append(self._start_ac_macro(node, 'code'))
         self.body.append(self._build_ac_param(node, 'language', lang))
         self.body.append(self._build_ac_param(node, 'linenumbers', num))
 
+        theme = self.builder.config.confluence_code_block_theme
+        theme = theme.lower() if theme else None
+        theme_map = SUPPORTED_CODE_BLOCK_THEMES
+
+        for class_ in node.get('classes', []):
+            if class_.startswith('confluence-theme-'):
+                theme = class_[len('confluence-theme-'):].lower()
+                if theme not in theme_map:
+                    self.warn('confluence-theme-* defined an unknown theme: ' +
+                        theme)
+                break
+
+        theme_id = theme_map.get(theme)
+        if theme_id:
+            self.body.append(self._build_ac_param(node, 'theme', theme_id))
+
         if firstline is not None and firstline > 1:
             self.body.append(
-                self._build_ac_param(node, 'firstline', str(firstline))
+                self._build_ac_param(node, 'firstline', firstline)
             )
 
         if title:
             self.body.append(self._build_ac_param(node, 'title', title))
 
         if 'collapse' in node.get('classes', []):
             self.body.append(self._build_ac_param(node, 'collapse', 'true'))
@@ -2253,15 +2292,15 @@
     # -----------------------------------------
     # sphinx -- extension -- confluence builder
     # -----------------------------------------
 
     def visit_confluence_excerpt(self, node):
         self.body.append(self._start_ac_macro(node, 'excerpt'))
         for k, v in sorted(node.params.items()):
-            self.body.append(self._build_ac_param(node, k, str(v)))
+            self.body.append(self._build_ac_param(node, k, v))
         self.body.append(self._start_ac_rich_text_body_macro(node))
         self.context.append(self._end_ac_rich_text_body_macro(node) +
             self._end_ac_macro(node, suffix=''))
 
     def depart_confluence_excerpt(self, node):
         self.body.append(self.context.pop())  # macro
 
@@ -2283,15 +2322,15 @@
         elif ':' in doclink:
             space_key, doctitle = doclink.split(':', 1)
         else:
             doctitle = doclink
 
         self.body.append(self._start_ac_macro(node, 'excerpt-include'))
         for k, v in sorted(node.params.items()):
-            self.body.append(self._build_ac_param(node, k, str(v)))
+            self.body.append(self._build_ac_param(node, k, v))
 
         attribs = {
             'ri:content-title': doctitle,
         }
         if space_key:
             attribs['ri:space-key'] = space_key
 
@@ -2683,42 +2722,42 @@
     # ------------------------------------------
     # confluence-builder -- enhancements -- jira
     # ------------------------------------------
 
     def _visit_jira_node(self, node):
         self.body.append(self._start_ac_macro(node, 'jira'))
         for k, v in sorted(node.params.items()):
-            self.body.append(self._build_ac_param(node, k, str(v)))
+            self.body.append(self._build_ac_param(node, k, v))
         self.body.append(self._end_ac_macro(node))
 
         raise nodes.SkipNode
 
     visit_jira = _visit_jira_node
     visit_jira_issue = _visit_jira_node
 
     # --------------------------------------------
     # confluence-builder -- enhancements -- status
     # --------------------------------------------
 
     def visit_confluence_status_inline(self, node):
         self.body.append(self._start_ac_macro(node, 'status'))
         for k, v in sorted(node.params.items()):
-            self.body.append(self._build_ac_param(node, k, str(v)))
+            self.body.append(self._build_ac_param(node, k, v))
         self.body.append(self._end_ac_macro(node))
 
         raise nodes.SkipNode
 
     # -----------------------------------------
     # confluence-builder -- enhancements -- toc
     # -----------------------------------------
 
     def visit_confluence_toc(self, node):
         self.body.append(self._start_ac_macro(node, 'toc'))
         for k, v in sorted(node.params.items()):
-            self.body.append(self._build_ac_param(node, k, str(v)))
+            self.body.append(self._build_ac_param(node, k, v))
         self.body.append(self._end_ac_macro(node))
 
         raise nodes.SkipNode
 
     # ---------------------------------------------------
     # sphinx -- extension (third party) -- jupyter-sphinx
     # ---------------------------------------------------
@@ -2790,27 +2829,105 @@
 
     def visit_FancyOutputNode(self, node):
         pass
 
     def depart_FancyOutputNode(self, node):
         pass
 
+    # -------------------------------------------------------
+    # sphinx -- extension (third party) -- sphinx-data-viewer
+    # -------------------------------------------------------
+
+    def visit_DataViewerNode(self, node):
+        data = json.dumps(json.loads(node['data']), indent=4)
+
+        title = node.get('title', None)
+        if title:
+            title = self.encode(title)
+
+        # use the `none` language type by default; however, if it appears
+        # that this configuration supports json rendering, use that instead
+        target_lang = 'none'
+        if self.builder.lang_transform:
+            new_target_lang = self.builder.lang_transform('json')
+            if 'json' in new_target_lang:
+                target_lang = new_target_lang
+
+        self.body.append(self._start_ac_macro(node, 'code'))
+        self.body.append(self._build_ac_param(node, 'language', target_lang))
+
+        if title:
+            self.body.append(self._build_ac_param(node, 'title', title))
+
+        expand = node.get('expand', None)
+        if not expand:
+            self.body.append(self._build_ac_param(node, 'collapse', 'true'))
+
+        self.body.append(self._start_ac_plain_text_body_macro(node))
+        self.body.append(self._escape_cdata(data))
+        self.body.append(self._end_ac_plain_text_body_macro(node))
+        self.body.append(self._end_ac_macro(node))
+
+        raise nodes.SkipNode
+
     # ---------------------------------------------------
     # sphinx -- extension (third party) -- sphinx-toolbox
     # ---------------------------------------------------
 
     def visit_ItalicAbbreviationNode(self, node):
         self.body.append(self._start_tag(node, 'i'))
         self.context.append(self._end_tag(node))
         self.visit_abbreviation(node)
 
     def depart_ItalicAbbreviationNode(self, node):
         self.depart_abbreviation(node)
         self.body.append(self.context.pop())  # i
 
+    # -------------------------------------------------
+    # sphinx -- extension (third party) -- sphinx-video
+    # -------------------------------------------------
+
+    def visit_video_node(self, node):
+        autoplay = node.get('autoplay')
+        height, hu = extract_length(node.get('height'))
+        width, wu = extract_length(node.get('width'))
+        source_path, _ = node.get('primary_src') or (None, None)
+
+        if height:
+            height = convert_length(height, hu)
+            if height is None:
+                self.warn('unsupported unit type for confluence: ' + hu)
+
+        if width:
+            width = convert_length(width, wu)
+            if width is None:
+                self.warn('unsupported unit type for confluence: ' + wu)
+
+        video_key, _, _ = self.assets.add(source_path, self.docname)
+
+        if not video_key:
+            self.warn(f'Unable to find video name: {source_path}')
+            raise nodes.SkipNode
+
+        ri_filename = self._start_ri_attachment(node, video_key) + \
+            self._end_ri_attachment(node)
+
+        self.body.append(self._start_tag(node, 'div'))
+        self.body.append(self._start_ac_macro(node, 'multimedia'))
+        self.body.append(self._build_ac_param(node, 'name', ri_filename))
+        if width:
+            self.body.append(self._build_ac_param(node, 'width', width))
+        if height:
+            self.body.append(self._build_ac_param(node, 'height', height))
+        if autoplay:
+            self.body.append(self._build_ac_param(node, 'autostart', 'true'))
+        self.body.append(self._end_ac_macro(node))
+        self.body.append(self._end_tag(node))
+        raise nodes.SkipNode
+
     # ---------------------------------------------------
     # sphinx -- extension (third party) -- sphinx-youtube
     # ---------------------------------------------------
 
     def _visit_video(self, node, uri):
         height, hu = node.get('height') or (None, None)
         width, wu = node.get('width') or (None, None)
@@ -2833,28 +2950,39 @@
         ri_url = self._start_tag(
             node, 'ri:url', empty=True, **{'ri:value': self.encode(uri)})
 
         self.body.append(self._start_tag(node, 'div', **attribs))
         self.body.append(self._start_ac_macro(node, 'widget'))
         self.body.append(self._build_ac_param(node, 'url', ri_url))
         if height:
-            self.body.append(self._build_ac_param(node, 'height', str(height)))
+            self.body.append(self._build_ac_param(node, 'height', height))
         if width:
-            self.body.append(self._build_ac_param(node, 'width', str(width)))
+            self.body.append(self._build_ac_param(node, 'width', width))
         self.body.append(self._end_ac_macro(node))
         self.body.append(self._end_tag(node))
 
         raise nodes.SkipNode
 
     def visit_vimeo(self, node):
         self._visit_video(node, 'https://vimeo.com/' + node['id'])
 
     def visit_youtube(self, node):
         self._visit_video(node, 'https://www.youtube.com/watch?v=' + node['id'])
 
+    # -------------------------------------------------------
+    # sphinx -- extension (third party) -- sphinxnotes-strike
+    # -------------------------------------------------------
+
+    def visit_strike_node(self, node):
+        self.body.append(self._start_tag(node, 's'))
+        self.context.append(self._end_tag(node, suffix=''))
+
+    def depart_strike_node(self, node):
+        self.body.append(self.context.pop())  # s
+
     # -------------
     # miscellaneous
     # -------------
 
     def visit_abbreviation(self, node):
         attribs = {}
         if 'explanation' in node:
@@ -2943,17 +3071,32 @@
         # providing an advanced option to allow raw html injection in the output
         #
         # This is not always guaranteed to work; the raw html content may not
         # be compatible with Atlassian's storage format. Results may fail to
         # publish or contents may be suppressed on the Confluence instance. This
         # is provided to help users wanted to somewhat support raw HTML content
         # generated from Markdown sources.
-        if self.builder.config.confluence_adv_permit_raw_html:
+        permit_raw_html = self.builder.config.confluence_permit_raw_html
+        if permit_raw_html:
             if 'html' in node.get('format', '').split():
-                self.body.append(self.nl.join(node.astext().splitlines()))
+                raw_html = self.nl.join(node.astext().splitlines())
+
+                # boolean flag -- raw injection of html
+                if isinstance(permit_raw_html, bool):
+                    self.body.append(raw_html)
+                # string value -- placed in an supported HTML macro available
+                # on the user's Confluence instance
+                else:
+                    macro = permit_raw_html
+                    self.body.append(self._start_ac_macro(node, macro))
+                    self.body.append(self._start_ac_plain_text_body_macro(node))
+                    self.body.append(self._escape_cdata(raw_html))
+                    self.body.append(self._end_ac_plain_text_body_macro(node))
+                    self.body.append(self._end_ac_macro(node))
+
                 raise nodes.SkipNode
 
         if 'confluence_storage' in node.get('format', '').split():
             self.body.append(self.nl.join(node.astext().splitlines()))
         else:
             # support deprecated 'confluence' format for an interim
             ConfluenceBaseTranslator.visit_raw(self, node)
@@ -3048,15 +3191,15 @@
             name: the parameter name
             value: the value for the parameter
 
         Returns:
             the content
         """
         return (self._start_tag(node, 'ac:parameter', **{'ac:name': name}) +
-            value + self._end_tag(node))
+            str(value) + self._end_tag(node))
 
     def _start_ac_image(self, node, **kwargs):
         """
         generates a confluence image start tag
 
         A helper used to return content to be appended to a document which
         initializes the start of a storage format image element. The 'ac:image'
@@ -3466,9 +3609,23 @@
 
         Args:
             data: the text
 
         Returns:
             the escaped text
         """
-        data = data.replace(']]>', ']]]]><![CDATA[>')
+
+        # workaround for Confluence 8.0.x to 8.2.x series
+        # (https://jira.atlassian.com/browse/CONFSERVER-82849)
+        #
+        # The else case here should be always working; however, in some
+        # Confluence instances, there was a window where pages could not
+        # be uploaded since Confluence would refuse the EOF sequence for
+        # CDATA blocks. This workaround can help a user get their content
+        # published at the unfortunate tweak of changing any trailing EOF
+        # CDATA blocks to have a space character included.
+        if self.builder.config.confluence_adv_quirk_cdata:
+            data = data.replace(']]>', ']] >')
+        else:
+            data = data.replace(']]>', ']]]]><![CDATA[>')
+
         return ConfluenceBaseTranslator.encode(self, data)
```

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/svg.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/svg.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/translator.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/translator.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/__init__.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_jupyter_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_nbsphinx.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_diagrams.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_gallery.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinx_toolbox.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/transmute/ext_sphinxcontrib_mermaid.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/util.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/util.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/sphinxcontrib/confluencebuilder/writer.py` & `sphinxcontrib_confluencebuilder-2.2.0/sphinxcontrib/confluencebuilder/writer.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_confluencebuilder-2.1.1/PKG-INFO` & `sphinxcontrib_confluencebuilder-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-confluencebuilder
-Version: 2.1.1
+Version: 2.2.0
 Summary: Sphinx extension to build Atlassian Confluence Storage Markup
 Author-email: Anthony Shaw <anthonyshaw@apache.org>
 Maintainer-email: James Knight <james.d.knight@live.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

