# Comparing `tmp/umap_project-1.4.3.tar.gz` & `tmp/umap_project-1.4.4.tar.gz`

## Comparing `umap_project-1.4.3.tar` & `umap_project-1.4.4.tar`

### file list

```diff
@@ -1,409 +1,410 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/admin.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/apps.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/autocomplete.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/context_processors.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/decorators.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/fields.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/forms.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/managers.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/middleware.py
--rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/models.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/urls.py
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/utils.py
--rw-r--r--   0        0        0    30650 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/views.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/wsgi.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/bin/__init__.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/am_ET/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/am_ET/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ast/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ast/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/br/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/br/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/cs_CZ/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11150 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15479 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/eu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/fa_IR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11267 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/gl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11901 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/hu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/is/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11512 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ms/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ms/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/no/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/si/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/si/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sk_SK/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11122 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    12639 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13899 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/th_TH/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13272 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/uk_UA/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/zh/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11531 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/management/commands/__init__.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/management/commands/anonymous_edit_url.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/management/commands/generate_js_locale.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/management/commands/import_pictograms.py
--rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0001_initial.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0002_tilelayer_tms.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0003_add_tilelayer.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0004_add_licence.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0005_remove_map_tilelayer.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0006_auto_20190407_0719.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0007_auto_20190416_1757.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0008_alter_map_settings.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/0009_star.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/migrations/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/settings/__init__.py
--rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/settings/base.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/settings/dev.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/settings/local.py.sample
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/favicon.ico
--rw-r--r--   0        0        0    17598 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/base.css
--rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/bitbucket.png
--rw-r--r--   0        0        0     6651 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/content.css
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font.css
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/github.png
--rw-r--r--   0        0        0    32792 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/map.css
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/nav.css
--rw-r--r--   0        0        0    19408 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/openstreetmap.png
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/theme.css
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/twitter.png
--rwxr-xr-x   0        0        0   182984 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font/FiraSans-Light.woff
--rwxr-xr-x   0        0        0   129180 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font/FiraSans-Light.woff2
--rwxr-xr-x   0        0        0   191400 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font/FiraSans-LightItalic.woff
--rwxr-xr-x   0        0        0   135744 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font/FiraSans-LightItalic.woff2
--rwxr-xr-x   0        0        0   198128 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font/FiraSans-SemiBold.woff
--rwxr-xr-x   0        0        0   140168 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/font/FiraSans-SemiBold.woff2
--rw-r--r--   0        0        0    23555 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/16-white.svg
--rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/16.svg
--rw-r--r--   0        0        0    17550 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/24-white.svg
--rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/24.svg
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/edit.svg
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/icon-bg.png
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/logo.svg
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/logo_filigree.png
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/marker.png
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/opensource.svg
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/osm.svg
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/search.gif
--rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/source/16-white.svg
--rw-r--r--   0        0        0    34515 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/source/16.svg
--rw-r--r--   0        0        0    29251 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/source/24-white.svg
--rw-r--r--   0        0        0    38901 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/img/source/24.svg
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.autocomplete.js
--rw-r--r--   0        0        0    48099 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.controls.js
--rw-r--r--   0        0        0    20980 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.core.js
--rw-r--r--   0        0        0    32598 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.features.js
--rw-r--r--   0        0        0    27740 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.forms.js
--rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.icon.js
--rw-r--r--   0        0        0    63273 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.js
--rw-r--r--   0        0        0    33648 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.layer.js
--rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.permissions.js
--rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.popup.js
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.slideshow.js
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.tableeditor.js
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.ui.js
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/js/umap.xhr.js
--rw-r--r--   0        0        0    28228 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/am_ET.js
--rw-r--r--   0        0        0    28157 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/am_ET.json
--rw-r--r--   0        0        0    24122 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ar.js
--rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ar.json
--rw-r--r--   0        0        0    23655 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ast.js
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ast.json
--rw-r--r--   0        0        0    27368 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/bg.js
--rw-r--r--   0        0        0    27303 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/bg.json
--rw-r--r--   0        0        0    24466 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/br.js
--rw-r--r--   0        0        0    24401 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/br.json
--rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ca.js
--rw-r--r--   0        0        0    24697 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ca.json
--rw-r--r--   0        0        0    25433 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/cs_CZ.js
--rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/cs_CZ.json
--rw-r--r--   0        0        0    24068 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/da.js
--rw-r--r--   0        0        0    24003 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/da.json
--rw-r--r--   0        0        0    25526 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/de.js
--rw-r--r--   0        0        0    25461 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/de.json
--rw-r--r--   0        0        0    35541 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/el.js
--rw-r--r--   0        0        0    35476 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/el.json
--rw-r--r--   0        0        0    23655 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/en.js
--rw-r--r--   0        0        0    23590 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/en.json
--rw-r--r--   0        0        0    23300 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/en_US.json
--rw-r--r--   0        0        0    25770 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/es.js
--rw-r--r--   0        0        0    25705 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/es.json
--rw-r--r--   0        0        0    23910 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/et.js
--rw-r--r--   0        0        0    23845 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/et.json
--rw-r--r--   0        0        0    23456 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/eu.js
--rw-r--r--   0        0        0    23391 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/eu.json
--rw-r--r--   0        0        0    30888 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/fa_IR.js
--rw-r--r--   0        0        0    30817 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/fa_IR.json
--rw-r--r--   0        0        0    24670 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/fi.js
--rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/fi.json
--rw-r--r--   0        0        0    25893 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/fr.js
--rw-r--r--   0        0        0    25828 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/fr.json
--rw-r--r--   0        0        0    25274 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/gl.js
--rw-r--r--   0        0        0    25209 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/gl.json
--rw-r--r--   0        0        0    27649 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/he.js
--rw-r--r--   0        0        0    27584 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/he.json
--rw-r--r--   0        0        0    23867 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/hr.js
--rw-r--r--   0        0        0    23802 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/hr.json
--rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/hu.js
--rw-r--r--   0        0        0    26721 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/hu.json
--rw-r--r--   0        0        0    23653 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/id.js
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/id.json
--rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/is.js
--rw-r--r--   0        0        0    25110 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/is.json
--rw-r--r--   0        0        0    25316 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/it.js
--rw-r--r--   0        0        0    25251 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/it.json
--rw-r--r--   0        0        0    26677 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ja.js
--rw-r--r--   0        0        0    26612 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ja.json
--rw-r--r--   0        0        0    23904 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ko.js
--rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ko.json
--rw-r--r--   0        0        0    24591 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/lt.js
--rw-r--r--   0        0        0    24526 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/lt.json
--rw-r--r--   0        0        0    24908 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ms.js
--rw-r--r--   0        0        0    24843 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ms.json
--rw-r--r--   0        0        0    25208 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/nl.js
--rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/nl.json
--rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/no.js
--rw-r--r--   0        0        0    23862 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/no.json
--rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pl.js
--rw-r--r--   0        0        0    25029 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pl.json
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pl_PL.json
--rw-r--r--   0        0        0    25261 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pt.js
--rw-r--r--   0        0        0    25196 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pt.json
--rw-r--r--   0        0        0    25250 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pt_BR.js
--rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pt_BR.json
--rw-r--r--   0        0        0    25267 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pt_PT.js
--rw-r--r--   0        0        0    25196 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/pt_PT.json
--rw-r--r--   0        0        0    23714 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ro.js
--rw-r--r--   0        0        0    23649 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ro.json
--rw-r--r--   0        0        0    32137 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ru.js
--rw-r--r--   0        0        0    32072 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/ru.json
--rw-r--r--   0        0        0    23838 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/si.js
--rw-r--r--   0        0        0    23773 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/si.json
--rw-r--r--   0        0        0    25122 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sk_SK.js
--rw-r--r--   0        0        0    25051 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sk_SK.json
--rw-r--r--   0        0        0    24964 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sl.js
--rw-r--r--   0        0        0    24899 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sl.json
--rw-r--r--   0        0        0    28361 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sr.js
--rw-r--r--   0        0        0    28296 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sr.json
--rw-r--r--   0        0        0    24842 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sv.js
--rw-r--r--   0        0        0    24777 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/sv.json
--rw-r--r--   0        0        0    23659 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/th_TH.js
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/th_TH.json
--rw-r--r--   0        0        0    25475 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/tr.js
--rw-r--r--   0        0        0    25410 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/tr.json
--rw-r--r--   0        0        0    31714 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/uk_UA.js
--rw-r--r--   0        0        0    31643 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/uk_UA.json
--rw-r--r--   0        0        0    24032 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/vi.js
--rw-r--r--   0        0        0    23967 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/vi.json
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/vi_VN.json
--rw-r--r--   0        0        0    23277 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/zh.js
--rw-r--r--   0        0        0    23212 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/zh.json
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/zh_CN.json
--rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/zh_TW.Big5.json
--rw-r--r--   0        0        0    23289 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/zh_TW.js
--rw-r--r--   0        0        0    23218 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/locale/zh_TW.json
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/.eslintrc
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Controls.js
--rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/DataLayer.js
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Feature.js
--rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Map.js
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Marker.js
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Permissions.js
--rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Polygon.js
--rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Polyline.js
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/TableEditor.js
--rw-r--r--   0        0        0    17100 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/Util.js
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/_pre.js
--rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/test/index.html
--rw-r--r--   0        0        0    57721 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/choropleth/choropleth.js
--rw-r--r--   0        0        0    46174 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/chroma/chroma.min.js
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
--rw-r--r--   0        0        0    16343 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
--rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
--rw-r--r--   0        0        0    15029 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/csv2geojson/csv2geojson.js
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/csv2geojson/index.js
--rw-r--r--   0        0        0    62738 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/dompurify/purify.js
--rw-r--r--   0        0        0    74768 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/editable/Leaflet.Editable.js
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/editable/Path.Drag.js
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/editinosm/edit-in-osm.png
--rw-r--r--   0        0        0    12301 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/fullscreen/fullscreen.png
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/hash/leaflet-hash.js
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/heat/leaflet-heat.js
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/i18n/Leaflet.i18n.js
--rw-r--r--   0        0        0   424589 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
--rw-r--r--   0        0        0   866200 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0        0        0   455791 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.js
--rw-r--r--   0        0        0   866292 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.js.map
--rw-r--r--   0        0        0    14806 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet.css
--rw-r--r--   0        0        0   147552 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet.js
--rw-r--r--   0        0        0   225544 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet.js.map
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/layers-2x.png
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/layers.png
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/marker-icon.png
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/marker-shadow.png
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/loading/Control.Loading.css
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/loading/Control.Loading.js
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
--rw-r--r--   0        0        0    30907 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/MarkerCluster.css
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
--rw-r--r--   0        0        0    80271 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
--rw-r--r--   0        0        0   157229 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
--rw-r--r--   0        0        0    33679 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
--rw-r--r--   0        0        0    27566 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/minimap/Control.MiniMap.css
--rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/minimap/Control.MiniMap.js
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/minimap/images/toggle.png
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/minimap/images/toggle.svg
--rw-r--r--   0        0        0    35642 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
--rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/photon/leaflet.photon.js
--rw-r--r--   0        0        0    44559 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/print/leaflet.browser.print.js
--rw-r--r--   0        0        0    23442 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/print/leaflet.browser.print.min.js
--rw-r--r--   0        0        0    18098 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/togeojson/togeojson.js
--rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/togpx/togpx.js
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/tokml/tokml.js
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
--rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/404.html
--rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/500.html
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/base.html
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/auth/user_detail.html
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/auth/user_stars.html
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/registration/login.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/about.html
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/about_summary.html
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/content.html
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/content_footer.html
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/css.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/footer.html
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/home.html
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/js.html
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/locale.js
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/login_popup_end.html
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/map_detail.html
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/map_fragment.html
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/map_init.html
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/map_list.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/map_messages.html
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/map_table.html
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/messages.html
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/navigation.html
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/password_change.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/password_change_done.html
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/search.html
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/search_bar.html
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/success.html
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templates/umap/user_dashboard.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templatetags/__init__.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/templatetags/umap_tags.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/__init__.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/base.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/conftest.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/settings.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_datalayer.py
--rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_datalayer_views.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_licence.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_map.py
--rw-r--r--   0        0        0    21981 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_map_views.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_tilelayer.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_utils.py
--rw-r--r--   0        0        0     8128 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/test_views.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_data.csv
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_data.gpx
--rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_data.json
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_data.kml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_empty_coordinates.json
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_missing_name.json
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 umap_project-1.4.3/umap/tests/fixtures/test_upload_non_linear_ring.json
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 umap_project-1.4.3/.gitignore
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 umap_project-1.4.3/LICENSE
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 umap_project-1.4.3/README.md
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 umap_project-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 umap_project-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/admin.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/apps.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/autocomplete.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/context_processors.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/decorators.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/fields.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/forms.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/managers.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/middleware.py
+-rw-r--r--   0        0        0    12273 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/models.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/urls.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/utils.py
+-rw-r--r--   0        0        0    30662 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/views.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/wsgi.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/bin/__init__.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/am_ET/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/am_ET/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10225 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ast/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ast/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/br/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11990 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/br/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/cs_CZ/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11150 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11526 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15479 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11589 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5388 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/eu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7971 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12770 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8731 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11267 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/gl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11901 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9170 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7646 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11969 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6762 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11502 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/is/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11715 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11615 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11512 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6127 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11167 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ms/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12063 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ms/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/no/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11330 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11371 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8211 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/si/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/si/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sk_SK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6132 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11122 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12639 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9199 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13899 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/th_TH/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13272 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/uk_UA/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9872 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/zh/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11531 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/management/commands/__init__.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/management/commands/anonymous_edit_url.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/management/commands/generate_js_locale.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/management/commands/import_pictograms.py
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0001_initial.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0002_tilelayer_tms.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0003_add_tilelayer.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0004_add_licence.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0005_remove_map_tilelayer.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0006_auto_20190407_0719.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0007_auto_20190416_1757.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0008_alter_map_settings.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0009_star.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/0010_alter_map_edit_status_alter_map_share_status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/migrations/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/settings/__init__.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/settings/base.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/settings/dev.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/settings/local.py.sample
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/favicon.ico
+-rw-r--r--   0        0        0    17598 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/base.css
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/bitbucket.png
+-rw-r--r--   0        0        0     6651 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/content.css
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font.css
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/github.png
+-rw-r--r--   0        0        0    32792 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/map.css
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/nav.css
+-rw-r--r--   0        0        0    19408 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/openstreetmap.png
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/theme.css
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/twitter.png
+-rwxr-xr-x   0        0        0   182984 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font/FiraSans-Light.woff
+-rwxr-xr-x   0        0        0   129180 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font/FiraSans-Light.woff2
+-rwxr-xr-x   0        0        0   191400 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font/FiraSans-LightItalic.woff
+-rwxr-xr-x   0        0        0   135744 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font/FiraSans-LightItalic.woff2
+-rwxr-xr-x   0        0        0   198128 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font/FiraSans-SemiBold.woff
+-rwxr-xr-x   0        0        0   140168 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/font/FiraSans-SemiBold.woff2
+-rw-r--r--   0        0        0    23555 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/16-white.svg
+-rw-r--r--   0        0        0    14049 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/16.svg
+-rw-r--r--   0        0        0    17550 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/24-white.svg
+-rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/24.svg
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/edit.svg
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/icon-bg.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/logo.svg
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/logo_filigree.png
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/marker.png
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/opensource.svg
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/osm.svg
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/search.gif
+-rw-r--r--   0        0        0    53366 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/source/16-white.svg
+-rw-r--r--   0        0        0    34515 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/source/16.svg
+-rw-r--r--   0        0        0    29251 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/source/24-white.svg
+-rw-r--r--   0        0        0    38901 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/img/source/24.svg
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.autocomplete.js
+-rw-r--r--   0        0        0    48099 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.controls.js
+-rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.core.js
+-rw-r--r--   0        0        0    32606 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.features.js
+-rw-r--r--   0        0        0    27740 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.forms.js
+-rw-r--r--   0        0        0     6339 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.icon.js
+-rw-r--r--   0        0        0    63273 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.js
+-rw-r--r--   0        0        0    33648 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.layer.js
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.permissions.js
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.popup.js
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.slideshow.js
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.tableeditor.js
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.ui.js
+-rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/js/umap.xhr.js
+-rw-r--r--   0        0        0    28228 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/am_ET.js
+-rw-r--r--   0        0        0    28157 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/am_ET.json
+-rw-r--r--   0        0        0    24122 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ar.js
+-rw-r--r--   0        0        0    24057 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ar.json
+-rw-r--r--   0        0        0    23655 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ast.js
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ast.json
+-rw-r--r--   0        0        0    27368 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/bg.js
+-rw-r--r--   0        0        0    27303 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/bg.json
+-rw-r--r--   0        0        0    25106 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/br.js
+-rw-r--r--   0        0        0    25041 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/br.json
+-rw-r--r--   0        0        0    24762 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ca.js
+-rw-r--r--   0        0        0    24697 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ca.json
+-rw-r--r--   0        0        0    25433 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/cs_CZ.js
+-rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/cs_CZ.json
+-rw-r--r--   0        0        0    24068 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/da.js
+-rw-r--r--   0        0        0    24003 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/da.json
+-rw-r--r--   0        0        0    25526 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/de.js
+-rw-r--r--   0        0        0    25461 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/de.json
+-rw-r--r--   0        0        0    35541 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/el.js
+-rw-r--r--   0        0        0    35476 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/el.json
+-rw-r--r--   0        0        0    23655 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/en.js
+-rw-r--r--   0        0        0    23590 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/en.json
+-rw-r--r--   0        0        0    23300 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/en_US.json
+-rw-r--r--   0        0        0    25770 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/es.js
+-rw-r--r--   0        0        0    25705 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/es.json
+-rw-r--r--   0        0        0    23910 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/et.js
+-rw-r--r--   0        0        0    23845 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/et.json
+-rw-r--r--   0        0        0    23456 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/eu.js
+-rw-r--r--   0        0        0    23391 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/eu.json
+-rw-r--r--   0        0        0    30888 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/fa_IR.js
+-rw-r--r--   0        0        0    30817 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/fa_IR.json
+-rw-r--r--   0        0        0    24670 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/fi.js
+-rw-r--r--   0        0        0    24605 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/fi.json
+-rw-r--r--   0        0        0    25893 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/fr.js
+-rw-r--r--   0        0        0    25828 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/fr.json
+-rw-r--r--   0        0        0    25274 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/gl.js
+-rw-r--r--   0        0        0    25209 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/gl.json
+-rw-r--r--   0        0        0    27649 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/he.js
+-rw-r--r--   0        0        0    27584 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/he.json
+-rw-r--r--   0        0        0    23867 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/hr.js
+-rw-r--r--   0        0        0    23802 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/hr.json
+-rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/hu.js
+-rw-r--r--   0        0        0    26721 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/hu.json
+-rw-r--r--   0        0        0    23653 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/id.js
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/id.json
+-rw-r--r--   0        0        0    25175 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/is.js
+-rw-r--r--   0        0        0    25110 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/is.json
+-rw-r--r--   0        0        0    25316 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/it.js
+-rw-r--r--   0        0        0    25251 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/it.json
+-rw-r--r--   0        0        0    26677 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ja.js
+-rw-r--r--   0        0        0    26612 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ja.json
+-rw-r--r--   0        0        0    23904 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ko.js
+-rw-r--r--   0        0        0    23839 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ko.json
+-rw-r--r--   0        0        0    24591 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/lt.js
+-rw-r--r--   0        0        0    24526 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/lt.json
+-rw-r--r--   0        0        0    24908 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ms.js
+-rw-r--r--   0        0        0    24843 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ms.json
+-rw-r--r--   0        0        0    25208 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/nl.js
+-rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/nl.json
+-rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/no.js
+-rw-r--r--   0        0        0    23862 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/no.json
+-rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pl.js
+-rw-r--r--   0        0        0    25029 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pl.json
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pl_PL.json
+-rw-r--r--   0        0        0    25261 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pt.js
+-rw-r--r--   0        0        0    25196 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pt.json
+-rw-r--r--   0        0        0    25250 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pt_BR.js
+-rw-r--r--   0        0        0    25179 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pt_BR.json
+-rw-r--r--   0        0        0    25267 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pt_PT.js
+-rw-r--r--   0        0        0    25196 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/pt_PT.json
+-rw-r--r--   0        0        0    23714 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ro.js
+-rw-r--r--   0        0        0    23649 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ro.json
+-rw-r--r--   0        0        0    32137 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ru.js
+-rw-r--r--   0        0        0    32072 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/ru.json
+-rw-r--r--   0        0        0    23838 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/si.js
+-rw-r--r--   0        0        0    23773 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/si.json
+-rw-r--r--   0        0        0    25122 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sk_SK.js
+-rw-r--r--   0        0        0    25051 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sk_SK.json
+-rw-r--r--   0        0        0    24964 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sl.js
+-rw-r--r--   0        0        0    24899 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sl.json
+-rw-r--r--   0        0        0    28361 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sr.js
+-rw-r--r--   0        0        0    28296 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sr.json
+-rw-r--r--   0        0        0    24842 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sv.js
+-rw-r--r--   0        0        0    24777 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/sv.json
+-rw-r--r--   0        0        0    23659 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/th_TH.js
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/th_TH.json
+-rw-r--r--   0        0        0    25475 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/tr.js
+-rw-r--r--   0        0        0    25410 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/tr.json
+-rw-r--r--   0        0        0    31714 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/uk_UA.js
+-rw-r--r--   0        0        0    31643 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/uk_UA.json
+-rw-r--r--   0        0        0    24032 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/vi.js
+-rw-r--r--   0        0        0    23967 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/vi.json
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/vi_VN.json
+-rw-r--r--   0        0        0    23277 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/zh.js
+-rw-r--r--   0        0        0    23212 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/zh.json
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/zh_CN.json
+-rw-r--r--   0        0        0    23588 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/zh_TW.Big5.json
+-rw-r--r--   0        0        0    23289 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/zh_TW.js
+-rw-r--r--   0        0        0    23218 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/locale/zh_TW.json
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/.eslintrc
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Controls.js
+-rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/DataLayer.js
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Feature.js
+-rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Map.js
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Marker.js
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Permissions.js
+-rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Polygon.js
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Polyline.js
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/TableEditor.js
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/Util.js
+-rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/_pre.js
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/test/index.html
+-rw-r--r--   0        0        0    57721 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/choropleth/choropleth.js
+-rw-r--r--   0        0        0    46174 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/chroma/chroma.min.js
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
+-rw-r--r--   0        0        0    16343 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
+-rw-r--r--   0        0        0     8994 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
+-rw-r--r--   0        0        0    15029 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/csv2geojson/csv2geojson.js
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/csv2geojson/index.js
+-rw-r--r--   0        0        0    62738 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/dompurify/purify.js
+-rw-r--r--   0        0        0    74768 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/editable/Leaflet.Editable.js
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/editable/Path.Drag.js
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/editinosm/edit-in-osm.png
+-rw-r--r--   0        0        0    12301 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/fullscreen/fullscreen.png
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/hash/leaflet-hash.js
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/heat/leaflet-heat.js
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/i18n/Leaflet.i18n.js
+-rw-r--r--   0        0        0   424589 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
+-rw-r--r--   0        0        0   866200 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
+-rw-r--r--   0        0        0   455791 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.js
+-rw-r--r--   0        0        0   866292 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.js.map
+-rw-r--r--   0        0        0    14806 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet.css
+-rw-r--r--   0        0        0   147552 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet.js
+-rw-r--r--   0        0        0   225544 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet.js.map
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/marker-shadow.png
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/loading/Control.Loading.css
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/loading/Control.Loading.js
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
+-rw-r--r--   0        0        0    30907 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/MarkerCluster.css
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
+-rw-r--r--   0        0        0    80271 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
+-rw-r--r--   0        0        0   157229 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
+-rw-r--r--   0        0        0    33679 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
+-rw-r--r--   0        0        0    27566 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/minimap/Control.MiniMap.css
+-rw-r--r--   0        0        0    12129 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/minimap/Control.MiniMap.js
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/minimap/images/toggle.png
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/minimap/images/toggle.svg
+-rw-r--r--   0        0        0    35642 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
+-rw-r--r--   0        0        0    14433 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/photon/leaflet.photon.js
+-rw-r--r--   0        0        0    44559 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/print/leaflet.browser.print.js
+-rw-r--r--   0        0        0    23442 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/print/leaflet.browser.print.min.js
+-rw-r--r--   0        0        0    18098 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/togeojson/togeojson.js
+-rw-r--r--   0        0        0    17936 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/togpx/togpx.js
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/tokml/tokml.js
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/404.html
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/500.html
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/base.html
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/auth/user_detail.html
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/auth/user_stars.html
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/registration/login.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/about.html
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/about_summary.html
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/content.html
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/content_footer.html
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/css.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/footer.html
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/home.html
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/js.html
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/locale.js
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/login_popup_end.html
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/map_detail.html
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/map_fragment.html
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/map_init.html
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/map_list.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/map_messages.html
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/map_table.html
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/messages.html
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/navigation.html
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/password_change.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/password_change_done.html
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/search.html
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/search_bar.html
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/success.html
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templates/umap/user_dashboard.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templatetags/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/templatetags/umap_tags.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/base.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/conftest.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/settings.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_datalayer.py
+-rw-r--r--   0        0        0     7724 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_datalayer_views.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_licence.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_map.py
+-rw-r--r--   0        0        0    21981 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_map_views.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_tilelayer.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_utils.py
+-rw-r--r--   0        0        0     8128 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/test_views.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_data.csv
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_data.gpx
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_data.json
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_data.kml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_empty_coordinates.json
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_missing_name.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 umap_project-1.4.4/umap/tests/fixtures/test_upload_non_linear_ring.json
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 umap_project-1.4.4/.gitignore
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 umap_project-1.4.4/LICENSE
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 umap_project-1.4.4/README.md
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 umap_project-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 umap_project-1.4.4/PKG-INFO
```

### Comparing `umap_project-1.4.3/umap/admin.py` & `umap_project-1.4.4/umap/admin.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/decorators.py` & `umap_project-1.4.4/umap/decorators.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/fields.py` & `umap_project-1.4.4/umap/fields.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/forms.py` & `umap_project-1.4.4/umap/forms.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/middleware.py` & `umap_project-1.4.4/umap/middleware.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/models.py` & `umap_project-1.4.4/umap/models.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/urls.py` & `umap_project-1.4.4/umap/urls.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/utils.py` & `umap_project-1.4.4/umap/utils.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/views.py` & `umap_project-1.4.4/umap/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
             url = validate_url(self.request)
         except AssertionError:
             return HttpResponseBadRequest()
         headers = {"User-Agent": "uMapProxy +http://wiki.openstreetmap.org/wiki/UMap"}
         request = Request(url, headers=headers)
         opener = build_opener()
         try:
-            proxied_request = opener.open(request)
+            proxied_request = opener.open(request, timeout=10)
         except HTTPError as e:
             return HttpResponse(e.msg, status=e.code, content_type="text/plain")
         except URLError:
             return HttpResponseBadRequest("URL error")
         except InvalidURL:
             return HttpResponseBadRequest("Invalid URL")
         else:
```

### Comparing `umap_project-1.4.3/umap/wsgi.py` & `umap_project-1.4.4/umap/wsgi.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/am_ET/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/am_ET/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/am_ET/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/am_ET/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ar/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ar/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ast/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/bg/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/bg/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/br/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/fi/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,461 +1,461 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Dren Ar Frankig <hadrienlouque@gmail.com>, 2023
-# Dren Ar Frankig <hadrienlouque@gmail.com>, 2023
+# Antti Castrén, 2014
+# Antti Castrén, 2013-2014
+# Jaakko Helleranta <jaakko@helleranta.com>, 2013
+# Jaakko Helleranta <jaakko@helleranta.com>, 2013
+# Jaakko Helleranta <jaakko@helleranta.com>, 2013
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-19 13:43+0000\n"
+"POT-Creation-Date: 2023-07-17 13:14+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: Dren Ar Frankig <hadrienlouque@gmail.com>, 2023\n"
-"Language-Team: Breton (http://app.transifex.com/openstreetmap/umap/language/br/)\n"
+"Last-Translator: Jaakko Helleranta <jaakko@helleranta.com>, 2013\n"
+"Language-Team: Finnish (http://app.transifex.com/openstreetmap/umap/language/fi/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: br\n"
-"Plural-Forms: nplurals=5; plural=((n%10 == 1) && (n%100 != 11) && (n%100 !=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && (n%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 > 19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != 0 && n % 1000000 == 0) ? 3 : 4);\n"
+"Language: fi\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: forms.py:43
 #, python-format
 msgid "Secret edit link is %s"
-msgstr ""
+msgstr "Salainen muokkauslinkki on %s"
 
 #: forms.py:47
 msgid "Everyone can edit"
-msgstr "An holl a c'hall kemmañ"
+msgstr "Kuka tahansa saa muokata"
 
 #: forms.py:48
 msgid "Only editable with secret edit link"
-msgstr ""
+msgstr "Muokattavissa vain salaisella muokkauslinkillä"
 
 #: middleware.py:14
 msgid "Site is readonly for maintenance"
 msgstr ""
 
 #: models.py:40
 msgid "name"
-msgstr "anv"
+msgstr "nimi"
 
 #: models.py:71
 msgid "details"
-msgstr "munudoù"
+msgstr "tarkemmat tiedot"
 
 #: models.py:72
 msgid "Link to a page where the licence is detailed."
-msgstr ""
+msgstr "Linkki sivulle, jossa lisenssi on määritetty yksityiskohtaisesti."
 
 #: models.py:82
 msgid "URL template using OSM tile format"
-msgstr ""
+msgstr "OSM-karttatiiliformaattia mukaileva URL-sapluuna"
 
 #: models.py:88
 msgid "Order of the tilelayers in the edit box"
-msgstr ""
+msgstr "Taustakarttojen järjestys muokkauslaatikossa"
 
 #: models.py:134
 msgid "Everyone"
-msgstr "An holl"
+msgstr ""
 
 #: models.py:135 models.py:141
 msgid "Editors only"
-msgstr "Aozerien nemetken"
+msgstr ""
 
 #: models.py:136
 msgid "Owner only"
-msgstr "Perc'henner nemetken"
+msgstr ""
 
 #: models.py:139
 msgid "Everyone (public)"
-msgstr "An holl (publik)"
+msgstr ""
 
 #: models.py:140
 msgid "Anyone with link"
-msgstr "Piv bennak en deus ul liamm"
+msgstr ""
 
 #: models.py:142
 msgid "Blocked"
-msgstr "Stanket"
+msgstr ""
 
 #: models.py:145 models.py:295
 msgid "description"
-msgstr "deskrivadur"
+msgstr "kuvaus"
 
 #: models.py:146
 msgid "center"
-msgstr "kreizañ"
+msgstr "keskitä"
 
 #: models.py:147
 msgid "zoom"
-msgstr "zoumañ"
+msgstr "zoomaa"
 
 #: models.py:149
 msgid "locate"
-msgstr "lec'hiañ"
+msgstr "paikanna"
 
 #: models.py:149
 msgid "Locate user on load?"
-msgstr ""
+msgstr "Paikanna käyttäjä sivua ladattaessa?"
 
 #: models.py:153
 msgid "Choose the map licence."
-msgstr "Dibabit aotre-implijout ar gartenn."
+msgstr "Valitse kartan lisenssi"
 
 #: models.py:154
 msgid "licence"
-msgstr "aotre"
+msgstr "lisenssi"
 
 #: models.py:164
 msgid "owner"
-msgstr "perc'henner"
+msgstr "omistaja"
 
 #: models.py:168
 msgid "editors"
-msgstr "aozerien"
+msgstr "julkaisija"
 
 #: models.py:171
 msgid "edit status"
-msgstr ""
+msgstr "muokkaa tilaa"
 
 #: models.py:174
 msgid "share status"
-msgstr ""
+msgstr "jaa status"
 
 #: models.py:177
 msgid "settings"
-msgstr "arventennoù"
+msgstr "asetukset"
 
 #: models.py:250
 msgid "Clone of"
-msgstr ""
+msgstr "Kloonattu kartasta"
 
 #: models.py:299
 msgid "display on load"
-msgstr ""
+msgstr "näytä ladattaessa"
 
 #: models.py:300
 msgid "Display this layer on load."
-msgstr ""
+msgstr "Näytä tämä kerros ladattaessa."
 
 #: templates/404.html:6
 msgid "Take me to the home page"
-msgstr "Distreiñ d'ar bajenn degemer"
+msgstr ""
 
 #: templates/auth/user_detail.html:5
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "Merdeiñ e kartennoù %(current_user)s"
+msgstr "Selaa %(current_user)s:n karttoja"
 
 #: templates/auth/user_detail.html:12
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr "%(current_user)s n'en/he deus kartenn ebet."
+msgstr ""
 
 #: templates/auth/user_stars.html:5
 #, python-format
 msgid "Browse %(current_user)s's starred maps"
-msgstr "Merdeiñ e kartennoù spilhennet %(current_user)s"
+msgstr ""
 
 #: templates/auth/user_stars.html:12
 #, python-format
 msgid "%(current_user)s has no starred maps yet."
-msgstr "%(current_user)s n'en/he deus kartenn spilhennet ebet."
+msgstr ""
 
 #: templates/base.html:12
 msgid ""
 "uMap lets you create maps with OpenStreetMap layers in a minute and embed "
 "them in your site."
 msgstr ""
 
 #: templates/registration/login.html:3
 msgid "Please log in with your account"
-msgstr "Kevreit gant ho kont mar plij"
+msgstr ""
 
 #: templates/registration/login.html:15
 msgid "Username"
-msgstr "Anv implijer"
+msgstr ""
 
 #: templates/registration/login.html:18
 msgid "Password"
-msgstr "Ger-tremen"
+msgstr ""
 
 #: templates/registration/login.html:19
 msgid "Login"
-msgstr "Kevreañ"
+msgstr ""
 
 #: templates/registration/login.html:24
 msgid "Please choose a provider"
-msgstr "Dibabit ur pourchaser mar plij"
+msgstr "Valitse mieleisesi palveluntarjoaja"
 
 #: templates/umap/about_summary.html:11
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
-msgstr "uMap a ro tro deoc'h da grouiñ kartennoù en ur serr-lagad gant foñsoù <a href=\"%(osm_url)s\" />OpenStreetMap</a> ha d'o enframmañ e-barzh ho lec'hienn."
+msgstr ""
 
 #: templates/umap/about_summary.html:21
 msgid "Choose the layers of your map"
-msgstr "Dibab ar gwiskadoù evit ho kartenn"
+msgstr "Valitse karttaasi sopivat taustakartat ja data-kerrokset"
 
 #: templates/umap/about_summary.html:22
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "Ouzhpennañ \"poentoù heverk\": balizennoù, linennoù, lieskornoù..."
+msgstr "Lisää tarvittavat POIt: karttamerkkejä, viivoja, monikulmioita..."
 
 #: templates/umap/about_summary.html:23
 msgid "Manage POIs colours and icons"
-msgstr "Dibab livioù an ikonoù hag ar poentoù heverk"
+msgstr "Valitse ja hallinnoi POI-merkintöjen värit ja karttakuvakkeet"
 
 #: templates/umap/about_summary.html:24
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr ""
+msgstr "Hallitse kartta-optiot: näytä mini-kartta, paikanna käyttäjä sivun latauksessa, ..."
 
 #: templates/umap/about_summary.html:25
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Enporzhiañ roadennoù geografek a-vern (geojson, gpx, kml, osm...)"
+msgstr "Geostrukturoidun datan (geojson, gpx, kml, osm...) tuonti eräajona "
 
 #: templates/umap/about_summary.html:26
 msgid "Choose the license for your data"
-msgstr "Dibab aotre-implijout ho roadennoù"
+msgstr "Valitse tiedoillesi lisenssi"
 
 #: templates/umap/about_summary.html:27
 msgid "Embed and share your map"
-msgstr "Enframmañ ha rannañ ho kartenn"
+msgstr "Jaa karttasi muille ja/tai liitä se muihin sivustoihin"
 
 #: templates/umap/about_summary.html:37
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Hag <a href=\"%(repo_url)s\">open source</a> eo!"
+msgstr "<a href=\"%(repo_url)s\">Avoin lähdekoodi</a> rulettaa!"
 
 #: templates/umap/about_summary.html:48 templates/umap/navigation.html:42
 #: templates/umap/user_dashboard.html:18
 msgid "Create a map"
-msgstr "Krouiñ ur gartenn"
+msgstr "Luo uusi kartta"
 
 #: templates/umap/about_summary.html:51
 msgid "Play with the demo"
-msgstr "Amprouiñ an demo!"
+msgstr "Tongi demoa sielusi kyllyydestä!"
 
 #: templates/umap/content.html:23
 msgid ""
 "This instance of uMap is currently in read only mode, no creation/edit is "
 "allowed."
 msgstr ""
 
 #: templates/umap/content.html:31
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr ""
+msgstr "Tämä on uMapin demo-instanssi, jota käytetään testaamiseen ja väliversioille. Jos tarvitset vakaan version, niin käytäthän <a href=\"%(stable_url)s\">%(stable_url)s</a> :a. Voit myös tarjota oman instanssin - <a href=\"%(repo_url)s\">avoin lähdekoodi</a> rulettaa!"
 
 #: templates/umap/home.html:8
 msgid "Map of the uMaps"
-msgstr ""
+msgstr "Kartta uMapeista"
 
 #: templates/umap/home.html:13
 msgid "Get inspired, browse maps"
-msgstr "Bezit awenet en ur furchal ar c'hartennoù"
+msgstr "Inspiroidu selaamalla karttoja"
 
 #: templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Kevreet oc'h. Gortozit ur pennadig..."
+msgstr "Sisäänkirjautumisesi onnistui. Jatketahan..."
 
 #: templates/umap/map_list.html:9 views.py:281
 msgid "by"
-msgstr "gant"
+msgstr "taholta"
 
 #: templates/umap/map_list.html:17 templates/umap/map_table.html:39
 msgid "More"
-msgstr "Muioc'h"
+msgstr "Lisää"
 
 #: templates/umap/map_table.html:6
 msgid "Map"
-msgstr "Kartenn"
+msgstr ""
 
 #: templates/umap/map_table.html:7
 msgid "Name"
-msgstr "Anv"
+msgstr ""
 
 #: templates/umap/map_table.html:8
 msgid "Who can see / edit"
-msgstr "Piv a c'hall gwelet / aozañ"
+msgstr ""
 
 #: templates/umap/map_table.html:9
 msgid "Last save"
-msgstr "Enrollet da ziwezhañ"
+msgstr ""
 
 #: templates/umap/map_table.html:10
 msgid "Owner"
-msgstr "Perc'henner"
+msgstr ""
 
 #: templates/umap/map_table.html:11
 msgid "Actions"
-msgstr "Oberoù"
+msgstr ""
 
 #: templates/umap/map_table.html:28
 msgid "Share"
-msgstr "Rannañ"
+msgstr ""
 
 #: templates/umap/map_table.html:29
 msgid "Edit"
-msgstr "Aozañ"
+msgstr ""
 
 #: templates/umap/map_table.html:30
 msgid "Download"
-msgstr "Pellgargañ"
+msgstr ""
 
 #: templates/umap/navigation.html:12
 msgid "My maps"
-msgstr "Ma c'hartennoù"
+msgstr "Omat kartat"
 
 #: templates/umap/navigation.html:15
 msgid "Starred maps"
-msgstr "Kartennoù spilhennet"
+msgstr ""
 
 #: templates/umap/navigation.html:19
 msgid "Log in"
-msgstr "Kevreañ"
+msgstr "Kirjaudu palveluun"
 
 #: templates/umap/navigation.html:19
 msgid "Sign in"
-msgstr "Krouiñ ur gont"
+msgstr "Kirjaudu palveluun"
 
 #: templates/umap/navigation.html:23
 msgid "About"
-msgstr "Diwar-benn"
+msgstr "Tietoja"
 
 #: templates/umap/navigation.html:26
 msgid "Help"
-msgstr "Skoazell"
+msgstr ""
 
 #: templates/umap/navigation.html:31
 msgid "Change password"
-msgstr "Cheñch ar ger-tremen"
+msgstr ""
 
 #: templates/umap/navigation.html:35
 msgid "Log out"
-msgstr "Digevreañ"
+msgstr "Kirjaudu ulos palvelusta"
 
 #: templates/umap/password_change.html:4
 msgid "Password change"
-msgstr "Cheñch ar ger-tremen"
+msgstr ""
 
 #: templates/umap/password_change.html:6
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
 msgstr ""
 
 #: templates/umap/password_change.html:13
 msgid "Old password"
-msgstr "Ger-tremen kozh"
+msgstr ""
 
 #: templates/umap/password_change.html:18
 msgid "New password"
-msgstr "Ger-tremen nevez"
+msgstr ""
 
 #: templates/umap/password_change.html:22
 msgid "New password confirmation"
-msgstr "Kadarnaat ar ger-tremen nevez"
+msgstr ""
 
 #: templates/umap/password_change.html:23
 msgid "Change my password"
-msgstr "Cheñch ar ger-tremen"
+msgstr ""
 
 #: templates/umap/password_change_done.html:4
 msgid "Password change successful"
-msgstr "Cheñchet eo bet ar ger-tremen gant berzh"
+msgstr ""
 
 #: templates/umap/password_change_done.html:5
 msgid "Your password was changed."
-msgstr "Cheñchet eo bet ho ker-tremen."
+msgstr ""
 
 #: templates/umap/search.html:10
 #, python-format
 msgid "%(count)s map found:"
 msgid_plural "%(count)s maps found:"
-msgstr[0] "%(count)s gartenn kavet :"
-msgstr[1] "%(count)s gartenn kavet :"
-msgstr[2] "%(count)s c'hartenn kavet :"
-msgstr[3] "%(count)s kartenn kavet :"
-msgstr[4] "%(count)s kartenn kavet :"
+msgstr[0] ""
+msgstr[1] ""
 
 #: templates/umap/search.html:18
 msgid "No map found."
-msgstr "Kartenn ebet kavet."
+msgstr ""
 
 #: templates/umap/search.html:21
 msgid "Latest created maps"
-msgstr "Kartennoù krouet da ziwezhañ"
+msgstr ""
 
 #: templates/umap/search_bar.html:3
 msgid "Search maps"
-msgstr "Klask kartennoù"
+msgstr "Etsi karttoja"
 
 #: templates/umap/search_bar.html:14
 msgid "Search"
-msgstr "Klask"
+msgstr "Etsi"
 
 #: templates/umap/user_dashboard.html:4 templates/umap/user_dashboard.html:9
 msgid "My dashboard"
-msgstr "Ma zaolenn-vourzh"
+msgstr ""
 
 #: templates/umap/user_dashboard.html:7
 msgid "Search my maps"
 msgstr ""
 
 #: templates/umap/user_dashboard.html:18
 msgid "You have no map yet."
-msgstr "N'ho peus kartenn ebet c'hoazh."
+msgstr ""
 
 #: views.py:286
 msgid "View the map"
-msgstr "Diskouez ar gartenn"
+msgstr "Katso karttaa"
 
 #: views.py:607
 msgid "Map has been updated!"
-msgstr "Hizivaet eo bet ar gartenn!"
+msgstr "Kartta on päivitetty!"
 
 #: views.py:632
 msgid "Map editors updated with success!"
-msgstr "Aozerien ar gartenn bet hizivaet gant berzh!"
+msgstr "Kartan toimittajat päivitetty onnistuneesti!"
 
 #: views.py:670
 #, python-format
 msgid "The uMap edit link for your map: %(map_name)s"
 msgstr ""
 
 #: views.py:673
 #, python-format
 msgid "Here is your secret edit link: %(link)s"
 msgstr ""
 
 #: views.py:679
 #, python-format
 msgid "Email sent to %(email)s"
-msgstr "Postel kaset da %(email)s"
+msgstr ""
 
 #: views.py:690
 msgid "Only its owner can delete the map."
-msgstr "N'eus nemet perc'henner ar gartenn a c'hall he dilemel."
+msgstr "Vain kartan omistaja voi poistaa kartan."
 
 #: views.py:713
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr ""
+msgstr "Karttasi on kloonattu! Jos haluat muokata tätä karttaa joltain muulta tietokoneelta, käytä tätä linkkiä: %(anonymous_url)s"
 
 #: views.py:718
 msgid "Congratulations, your map has been cloned!"
-msgstr "Eilet eo bet ho kartenn gant berzh!"
+msgstr "Onneksi olkoon! Karttasi on kloonattu!"
 
-#: views.py:897
+#: views.py:884
 msgid "Layer successfully deleted."
-msgstr "Gwiskad dilamet gant berzh."
+msgstr "Kerros onnistuneesti poistettu. Pysyvästi."
```

### Comparing `umap_project-1.4.3/umap/locale/ca/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ca/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/cs_CZ/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/cs_CZ/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/da/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/da/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/de/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/de/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/el/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/el/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/en/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/es/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/es/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/et/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/et/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/eu/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/eu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/eu/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/fa_IR/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/fa_IR/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/fi/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/fi/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/sl/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Antti Castrén, 2014
-# Antti Castrén, 2013-2014
-# Jaakko Helleranta <jaakko@helleranta.com>, 2013
-# Jaakko Helleranta <jaakko@helleranta.com>, 2013
-# Jaakko Helleranta <jaakko@helleranta.com>, 2013
+# Matej Urbančič <>, 2018
+# Štefan Baebler <stefan.baebler@gmail.com>, 2019
+# Štefan Baebler <stefan.baebler@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-07-17 13:14+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: Jaakko Helleranta <jaakko@helleranta.com>, 2013\n"
-"Language-Team: Finnish (http://app.transifex.com/openstreetmap/umap/language/fi/)\n"
+"Last-Translator: Štefan Baebler <stefan.baebler@gmail.com>, 2019\n"
+"Language-Team: Slovenian (http://app.transifex.com/openstreetmap/umap/language/sl/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fi\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: sl\n"
+"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n%100==4 ? 2 : 3);\n"
 
 #: forms.py:43
 #, python-format
 msgid "Secret edit link is %s"
-msgstr "Salainen muokkauslinkki on %s"
+msgstr "Skrivna povezava za urejanje je %s"
 
 #: forms.py:47
 msgid "Everyone can edit"
-msgstr "Kuka tahansa saa muokata"
+msgstr "Vsakdo lahko ureja"
 
 #: forms.py:48
 msgid "Only editable with secret edit link"
-msgstr "Muokattavissa vain salaisella muokkauslinkillä"
+msgstr "Urejanje je mogoče le prek posebne skrivne povezave"
 
 #: middleware.py:14
 msgid "Site is readonly for maintenance"
-msgstr ""
+msgstr "Zaradi vzdrževanja je strežnik na voljo samo za ogled."
 
 #: models.py:40
 msgid "name"
-msgstr "nimi"
+msgstr "ime"
 
 #: models.py:71
 msgid "details"
-msgstr "tarkemmat tiedot"
+msgstr "podrobnosti"
 
 #: models.py:72
 msgid "Link to a page where the licence is detailed."
-msgstr "Linkki sivulle, jossa lisenssi on määritetty yksityiskohtaisesti."
+msgstr "Povezava do strani, kjer je objavljeno dovoljenje."
 
 #: models.py:82
 msgid "URL template using OSM tile format"
-msgstr "OSM-karttatiiliformaattia mukaileva URL-sapluuna"
+msgstr "Predloga naslova URL z uporabo zapisa OSM."
 
 #: models.py:88
 msgid "Order of the tilelayers in the edit box"
-msgstr "Taustakarttojen järjestys muokkauslaatikossa"
+msgstr "Vrstni red plasti v urejevalniku"
 
 #: models.py:134
 msgid "Everyone"
 msgstr ""
 
 #: models.py:135 models.py:141
 msgid "Editors only"
@@ -81,85 +79,85 @@
 
 #: models.py:142
 msgid "Blocked"
 msgstr ""
 
 #: models.py:145 models.py:295
 msgid "description"
-msgstr "kuvaus"
+msgstr "opis"
 
 #: models.py:146
 msgid "center"
-msgstr "keskitä"
+msgstr "središče"
 
 #: models.py:147
 msgid "zoom"
-msgstr "zoomaa"
+msgstr "približaj"
 
 #: models.py:149
 msgid "locate"
-msgstr "paikanna"
+msgstr "določi mesto"
 
 #: models.py:149
 msgid "Locate user on load?"
-msgstr "Paikanna käyttäjä sivua ladattaessa?"
+msgstr "Al naj se ob zagonu določi trenutno mesto uporabnika?"
 
 #: models.py:153
 msgid "Choose the map licence."
-msgstr "Valitse kartan lisenssi"
+msgstr "Izbor dovoljenja za zemljevid."
 
 #: models.py:154
 msgid "licence"
-msgstr "lisenssi"
+msgstr "dovoljenje"
 
 #: models.py:164
 msgid "owner"
-msgstr "omistaja"
+msgstr "lastnik"
 
 #: models.py:168
 msgid "editors"
-msgstr "julkaisija"
+msgstr "uredniki"
 
 #: models.py:171
 msgid "edit status"
-msgstr "muokkaa tilaa"
+msgstr "stanje urejanja"
 
 #: models.py:174
 msgid "share status"
-msgstr "jaa status"
+msgstr "stanje souporabe"
 
 #: models.py:177
 msgid "settings"
-msgstr "asetukset"
+msgstr "nastavitve"
 
 #: models.py:250
 msgid "Clone of"
-msgstr "Kloonattu kartasta"
+msgstr "Klon zemljevida"
 
 #: models.py:299
 msgid "display on load"
-msgstr "näytä ladattaessa"
+msgstr "pokaži ob zagonu"
 
 #: models.py:300
 msgid "Display this layer on load."
-msgstr "Näytä tämä kerros ladattaessa."
+msgstr "Pokaži to plast med nalaganjem."
 
 #: templates/404.html:6
 msgid "Take me to the home page"
-msgstr ""
+msgstr "Nazaj na začetno stran"
 
 #: templates/auth/user_detail.html:5
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "Selaa %(current_user)s:n karttoja"
+msgstr "Prebrskaj zemljevide (%(current_user)s)"
 
 #: templates/auth/user_detail.html:12
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr ""
+msgstr "%(current_user)s nima nobenega zemljevida."
 
 #: templates/auth/user_stars.html:5
 #, python-format
 msgid "Browse %(current_user)s's starred maps"
 msgstr ""
 
 #: templates/auth/user_stars.html:12
@@ -171,115 +169,115 @@
 msgid ""
 "uMap lets you create maps with OpenStreetMap layers in a minute and embed "
 "them in your site."
 msgstr ""
 
 #: templates/registration/login.html:3
 msgid "Please log in with your account"
-msgstr ""
+msgstr "Prijavite se z računom"
 
 #: templates/registration/login.html:15
 msgid "Username"
-msgstr ""
+msgstr "Uporabniško ime"
 
 #: templates/registration/login.html:18
 msgid "Password"
-msgstr ""
+msgstr "Geslo"
 
 #: templates/registration/login.html:19
 msgid "Login"
-msgstr ""
+msgstr "Prijava"
 
 #: templates/registration/login.html:24
 msgid "Please choose a provider"
-msgstr "Valitse mieleisesi palveluntarjoaja"
+msgstr "Izbor ponudnika"
 
 #: templates/umap/about_summary.html:11
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
 msgstr ""
 
 #: templates/umap/about_summary.html:21
 msgid "Choose the layers of your map"
-msgstr "Valitse karttaasi sopivat taustakartat ja data-kerrokset"
+msgstr "Izbor plasti na zemljevidu"
 
 #: templates/umap/about_summary.html:22
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "Lisää tarvittavat POIt: karttamerkkejä, viivoja, monikulmioita..."
+msgstr "Dodajanje točk POI: označbe, črte, polja ..."
 
 #: templates/umap/about_summary.html:23
 msgid "Manage POIs colours and icons"
-msgstr "Valitse ja hallinnoi POI-merkintöjen värit ja karttakuvakkeet"
+msgstr "Prilagajanje ikon in barv točk POI"
 
 #: templates/umap/about_summary.html:24
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr "Hallitse kartta-optiot: näytä mini-kartta, paikanna käyttäjä sivun latauksessa, ..."
+msgstr "Upravljanje možnosti zemljevidov: določanje uporabnikov, vrst prikaza ..."
 
 #: templates/umap/about_summary.html:25
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Geostrukturoidun datan (geojson, gpx, kml, osm...) tuonti eräajona "
+msgstr "Paketno uvažanje geografskih podatkov (geojson, gpx, kml, osm ...)"
 
 #: templates/umap/about_summary.html:26
 msgid "Choose the license for your data"
-msgstr "Valitse tiedoillesi lisenssi"
+msgstr "Izbor dovoljenja za vpisane podatke"
 
 #: templates/umap/about_summary.html:27
 msgid "Embed and share your map"
-msgstr "Jaa karttasi muille ja/tai liitä se muihin sivustoihin"
+msgstr "Vstavljanje in objavljanje zemljevida"
 
 #: templates/umap/about_summary.html:37
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "<a href=\"%(repo_url)s\">Avoin lähdekoodi</a> rulettaa!"
+msgstr "Povrh vsega pa je projekt še <a href=\"%(repo_url)s\">odprtokoden</a>!"
 
 #: templates/umap/about_summary.html:48 templates/umap/navigation.html:42
 #: templates/umap/user_dashboard.html:18
 msgid "Create a map"
-msgstr "Luo uusi kartta"
+msgstr "Ustvari zemljevid"
 
 #: templates/umap/about_summary.html:51
 msgid "Play with the demo"
-msgstr "Tongi demoa sielusi kyllyydestä!"
+msgstr "Pokaži preizkusne strani"
 
 #: templates/umap/content.html:23
 msgid ""
 "This instance of uMap is currently in read only mode, no creation/edit is "
 "allowed."
 msgstr ""
 
 #: templates/umap/content.html:31
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Tämä on uMapin demo-instanssi, jota käytetään testaamiseen ja väliversioille. Jos tarvitset vakaan version, niin käytäthän <a href=\"%(stable_url)s\">%(stable_url)s</a> :a. Voit myös tarjota oman instanssin - <a href=\"%(repo_url)s\">avoin lähdekoodi</a> rulettaa!"
+msgstr "Preizkusna različica je na voljo za pregled in spoznavanje funkcionalnosti. Če potrebujete stabilno različico, uporabite <a href=\"%(stable_url)s\">%(stable_url)s</a>. Seveda lahko vzpostavite svoj strežnik, saj je orodje <a href=\"%(repo_url)s\">odprtokodno</a>!"
 
 #: templates/umap/home.html:8
 msgid "Map of the uMaps"
-msgstr "Kartta uMapeista"
+msgstr "Zemljevid spletišča uMaps"
 
 #: templates/umap/home.html:13
 msgid "Get inspired, browse maps"
-msgstr "Inspiroidu selaamalla karttoja"
+msgstr "Poiščite zamisli, prebrskajte zemljevide"
 
 #: templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Sisäänkirjautumisesi onnistui. Jatketahan..."
+msgstr "Prijava je uspešno končana. Poteka nalaganje vsebine ..."
 
 #: templates/umap/map_list.html:9 views.py:281
 msgid "by"
-msgstr "taholta"
+msgstr "–"
 
 #: templates/umap/map_list.html:17 templates/umap/map_table.html:39
 msgid "More"
-msgstr "Lisää"
+msgstr "Več"
 
 #: templates/umap/map_table.html:6
 msgid "Map"
 msgstr ""
 
 #: templates/umap/map_table.html:7
 msgid "Name"
@@ -311,100 +309,102 @@
 
 #: templates/umap/map_table.html:30
 msgid "Download"
 msgstr ""
 
 #: templates/umap/navigation.html:12
 msgid "My maps"
-msgstr "Omat kartat"
+msgstr "Moji zemljevidi"
 
 #: templates/umap/navigation.html:15
 msgid "Starred maps"
 msgstr ""
 
 #: templates/umap/navigation.html:19
 msgid "Log in"
-msgstr "Kirjaudu palveluun"
+msgstr "Prijava"
 
 #: templates/umap/navigation.html:19
 msgid "Sign in"
-msgstr "Kirjaudu palveluun"
+msgstr "Vpis"
 
 #: templates/umap/navigation.html:23
 msgid "About"
-msgstr "Tietoja"
+msgstr "O projektu"
 
 #: templates/umap/navigation.html:26
 msgid "Help"
 msgstr ""
 
 #: templates/umap/navigation.html:31
 msgid "Change password"
-msgstr ""
+msgstr "Zamenjaj geslo"
 
 #: templates/umap/navigation.html:35
 msgid "Log out"
-msgstr "Kirjaudu ulos palvelusta"
+msgstr "Odjava"
 
 #: templates/umap/password_change.html:4
 msgid "Password change"
-msgstr ""
+msgstr "Spremeni geslo"
 
 #: templates/umap/password_change.html:6
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
-msgstr ""
+msgstr "Iz varnostnih razlogov morate vpisati staro geslo in nato še dvakrat vpisati novo, da se prepričate v pravilnost vpisa."
 
 #: templates/umap/password_change.html:13
 msgid "Old password"
-msgstr ""
+msgstr "Staro geslo"
 
 #: templates/umap/password_change.html:18
 msgid "New password"
-msgstr ""
+msgstr "Novo geslo"
 
 #: templates/umap/password_change.html:22
 msgid "New password confirmation"
-msgstr ""
+msgstr "Potrditev novega gesla"
 
 #: templates/umap/password_change.html:23
 msgid "Change my password"
-msgstr ""
+msgstr "Spremeni geslo"
 
 #: templates/umap/password_change_done.html:4
 msgid "Password change successful"
-msgstr ""
+msgstr "Geslo je uspešno spremenjeno."
 
 #: templates/umap/password_change_done.html:5
 msgid "Your password was changed."
-msgstr ""
+msgstr "Geslo je spremenjeno."
 
 #: templates/umap/search.html:10
 #, python-format
 msgid "%(count)s map found:"
 msgid_plural "%(count)s maps found:"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: templates/umap/search.html:18
 msgid "No map found."
 msgstr ""
 
 #: templates/umap/search.html:21
 msgid "Latest created maps"
 msgstr ""
 
 #: templates/umap/search_bar.html:3
 msgid "Search maps"
-msgstr "Etsi karttoja"
+msgstr "Poišči zemljevide"
 
 #: templates/umap/search_bar.html:14
 msgid "Search"
-msgstr "Etsi"
+msgstr "Poišči"
 
 #: templates/umap/user_dashboard.html:4 templates/umap/user_dashboard.html:9
 msgid "My dashboard"
 msgstr ""
 
 #: templates/umap/user_dashboard.html:7
 msgid "Search my maps"
@@ -412,23 +412,23 @@
 
 #: templates/umap/user_dashboard.html:18
 msgid "You have no map yet."
 msgstr ""
 
 #: views.py:286
 msgid "View the map"
-msgstr "Katso karttaa"
+msgstr "Pogled zemljevida"
 
 #: views.py:607
 msgid "Map has been updated!"
-msgstr "Kartta on päivitetty!"
+msgstr "Zemljevid je posodobljen!"
 
 #: views.py:632
 msgid "Map editors updated with success!"
-msgstr "Kartan toimittajat päivitetty onnistuneesti!"
+msgstr "seznam urednikov je posodobljen!"
 
 #: views.py:670
 #, python-format
 msgid "The uMap edit link for your map: %(map_name)s"
 msgstr ""
 
 #: views.py:673
@@ -439,23 +439,23 @@
 #: views.py:679
 #, python-format
 msgid "Email sent to %(email)s"
 msgstr ""
 
 #: views.py:690
 msgid "Only its owner can delete the map."
-msgstr "Vain kartan omistaja voi poistaa kartan."
+msgstr "Zemljevid lahko izbriše le lastnik."
 
 #: views.py:713
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "Karttasi on kloonattu! Jos haluat muokata tätä karttaa joltain muulta tietokoneelta, käytä tätä linkkiä: %(anonymous_url)s"
+msgstr "Zemljevid je kloniran! Za urejanje z drugega računalnika uporabite povezavo: %(anonymous_url)s"
 
 #: views.py:718
 msgid "Congratulations, your map has been cloned!"
-msgstr "Onneksi olkoon! Karttasi on kloonattu!"
+msgstr "Zemljevid je uspešno kloniran!"
 
 #: views.py:884
 msgid "Layer successfully deleted."
-msgstr "Kerros onnistuneesti poistettu. Pysyvästi."
+msgstr "Plast je uspešno izbrisana."
```

### Comparing `umap_project-1.4.3/umap/locale/fr/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/fr/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/gl/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/gl/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/he/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/he/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/hr/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/hr/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/hu/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/hu/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/id/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/is/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/is/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/it/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/it/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ja/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ja/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ko/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ko/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/lt/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/lt/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ms/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ms/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ms/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/nl/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/nl/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/no/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pl/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pl/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pt/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pt/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pt_BR/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pt_BR/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pt_PT/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/pt_PT/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ro/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ro/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ru/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/ru/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/si/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/si/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sk_SK/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sk_SK/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sl/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sl/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/sv/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Matej Urbančič <>, 2018
-# Štefan Baebler <stefan.baebler@gmail.com>, 2019
-# Štefan Baebler <stefan.baebler@gmail.com>, 2019
+# d402bbf52766ea36c1c6bd472b2de8fb_a8a94ad, 2020
+# carlbacker, 2020
+# d402bbf52766ea36c1c6bd472b2de8fb_a8a94ad, 2020
+# carlbacker, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-07-17 13:14+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: Štefan Baebler <stefan.baebler@gmail.com>, 2019\n"
-"Language-Team: Slovenian (http://app.transifex.com/openstreetmap/umap/language/sl/)\n"
+"Last-Translator: carlbacker, 2020\n"
+"Language-Team: Swedish (http://app.transifex.com/openstreetmap/umap/language/sv/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sl\n"
-"Plural-Forms: nplurals=4; plural=(n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || n%100==4 ? 2 : 3);\n"
+"Language: sv\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: forms.py:43
 #, python-format
 msgid "Secret edit link is %s"
-msgstr "Skrivna povezava za urejanje je %s"
+msgstr "Privat redigeringslänk är %s"
 
 #: forms.py:47
 msgid "Everyone can edit"
-msgstr "Vsakdo lahko ureja"
+msgstr "Alla kan redigera"
 
 #: forms.py:48
 msgid "Only editable with secret edit link"
-msgstr "Urejanje je mogoče le prek posebne skrivne povezave"
+msgstr "Redigering är bara tillåten med privat redigeringslänk"
 
 #: middleware.py:14
 msgid "Site is readonly for maintenance"
-msgstr "Zaradi vzdrževanja je strežnik na voljo samo za ogled."
+msgstr "Webbplatsen är skrivskyddad för underhållsarbete."
 
 #: models.py:40
 msgid "name"
-msgstr "ime"
+msgstr "namn"
 
 #: models.py:71
 msgid "details"
-msgstr "podrobnosti"
+msgstr "detaljer"
 
 #: models.py:72
 msgid "Link to a page where the licence is detailed."
-msgstr "Povezava do strani, kjer je objavljeno dovoljenje."
+msgstr "Länk till sida med detaljerad licens information."
 
 #: models.py:82
 msgid "URL template using OSM tile format"
-msgstr "Predloga naslova URL z uporabo zapisa OSM."
+msgstr "URL-mall med OSM:s tile-format"
 
 #: models.py:88
 msgid "Order of the tilelayers in the edit box"
-msgstr "Vrstni red plasti v urejevalniku"
+msgstr "Ordningen för tile-lager i redigeringsrutan"
 
 #: models.py:134
 msgid "Everyone"
 msgstr ""
 
 #: models.py:135 models.py:141
 msgid "Editors only"
@@ -79,85 +80,85 @@
 
 #: models.py:142
 msgid "Blocked"
 msgstr ""
 
 #: models.py:145 models.py:295
 msgid "description"
-msgstr "opis"
+msgstr "beskrivning"
 
 #: models.py:146
 msgid "center"
-msgstr "središče"
+msgstr "centrera"
 
 #: models.py:147
 msgid "zoom"
-msgstr "približaj"
+msgstr "zooma"
 
 #: models.py:149
 msgid "locate"
-msgstr "določi mesto"
+msgstr "lokalisera"
 
 #: models.py:149
 msgid "Locate user on load?"
-msgstr "Al naj se ob zagonu določi trenutno mesto uporabnika?"
+msgstr "Lokalisera användaren vid uppstart?"
 
 #: models.py:153
 msgid "Choose the map licence."
-msgstr "Izbor dovoljenja za zemljevid."
+msgstr "Välj licens för kartan."
 
 #: models.py:154
 msgid "licence"
-msgstr "dovoljenje"
+msgstr "licens"
 
 #: models.py:164
 msgid "owner"
-msgstr "lastnik"
+msgstr "ägare"
 
 #: models.py:168
 msgid "editors"
-msgstr "uredniki"
+msgstr "redaktörer"
 
 #: models.py:171
 msgid "edit status"
-msgstr "stanje urejanja"
+msgstr "redigeringsstatus"
 
 #: models.py:174
 msgid "share status"
-msgstr "stanje souporabe"
+msgstr "delningsstatus"
 
 #: models.py:177
 msgid "settings"
-msgstr "nastavitve"
+msgstr "inställningar"
 
 #: models.py:250
 msgid "Clone of"
-msgstr "Klon zemljevida"
+msgstr "Kopia av"
 
 #: models.py:299
 msgid "display on load"
-msgstr "pokaži ob zagonu"
+msgstr "visa vid uppstart"
 
 #: models.py:300
 msgid "Display this layer on load."
-msgstr "Pokaži to plast med nalaganjem."
+msgstr "Visa detta lager från start."
 
 #: templates/404.html:6
 msgid "Take me to the home page"
-msgstr "Nazaj na začetno stran"
+msgstr "Ta mig till startsidan"
 
 #: templates/auth/user_detail.html:5
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "Prebrskaj zemljevide (%(current_user)s)"
+msgstr "Bläddra bland %(current_user)ss kartor"
 
 #: templates/auth/user_detail.html:12
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr "%(current_user)s nima nobenega zemljevida."
+msgstr "%(current_user)s har inga kartor."
 
 #: templates/auth/user_stars.html:5
 #, python-format
 msgid "Browse %(current_user)s's starred maps"
 msgstr ""
 
 #: templates/auth/user_stars.html:12
@@ -169,115 +170,115 @@
 msgid ""
 "uMap lets you create maps with OpenStreetMap layers in a minute and embed "
 "them in your site."
 msgstr ""
 
 #: templates/registration/login.html:3
 msgid "Please log in with your account"
-msgstr "Prijavite se z računom"
+msgstr "Vänligen logga in med ditt konto"
 
 #: templates/registration/login.html:15
 msgid "Username"
-msgstr "Uporabniško ime"
+msgstr "Användarnamn"
 
 #: templates/registration/login.html:18
 msgid "Password"
-msgstr "Geslo"
+msgstr "Lösenord"
 
 #: templates/registration/login.html:19
 msgid "Login"
-msgstr "Prijava"
+msgstr "Logga in"
 
 #: templates/registration/login.html:24
 msgid "Please choose a provider"
-msgstr "Izbor ponudnika"
+msgstr "Välj en leverantör"
 
 #: templates/umap/about_summary.html:11
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
-msgstr ""
+msgstr "Med uMap kan du på minuter skapa egna kartor med <a href=\"%(osm_url)s\" />OpenStreetMap</a> lager och sedan bädda in dem på din webbsida."
 
 #: templates/umap/about_summary.html:21
 msgid "Choose the layers of your map"
-msgstr "Izbor plasti na zemljevidu"
+msgstr "Välj lager för din karta"
 
 #: templates/umap/about_summary.html:22
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "Dodajanje točk POI: označbe, črte, polja ..."
+msgstr "Lägg till POI:er, markörer, linjer, polygoner..."
 
 #: templates/umap/about_summary.html:23
 msgid "Manage POIs colours and icons"
-msgstr "Prilagajanje ikon in barv točk POI"
+msgstr "Ändra färger och ikoner för POI:er"
 
 #: templates/umap/about_summary.html:24
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr "Upravljanje možnosti zemljevidov: določanje uporabnikov, vrst prikaza ..."
+msgstr "Hantera kartalternativ: visa en minikarta, lokalisera användaren..."
 
 #: templates/umap/about_summary.html:25
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Paketno uvažanje geografskih podatkov (geojson, gpx, kml, osm ...)"
+msgstr "Importera strukturerad geodata (geojson, gpx, kml, osm...)"
 
 #: templates/umap/about_summary.html:26
 msgid "Choose the license for your data"
-msgstr "Izbor dovoljenja za vpisane podatke"
+msgstr "Välj licens för dina data"
 
 #: templates/umap/about_summary.html:27
 msgid "Embed and share your map"
-msgstr "Vstavljanje in objavljanje zemljevida"
+msgstr "Bädda in och dela din karta"
 
 #: templates/umap/about_summary.html:37
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Povrh vsega pa je projekt še <a href=\"%(repo_url)s\">odprtokoden</a>!"
+msgstr "Och det är <a href=\"%(repo_url)s\">öppen källkod</a>!"
 
 #: templates/umap/about_summary.html:48 templates/umap/navigation.html:42
 #: templates/umap/user_dashboard.html:18
 msgid "Create a map"
-msgstr "Ustvari zemljevid"
+msgstr "Skapa en karta"
 
 #: templates/umap/about_summary.html:51
 msgid "Play with the demo"
-msgstr "Pokaži preizkusne strani"
+msgstr "Lek med demotjänsten"
 
 #: templates/umap/content.html:23
 msgid ""
 "This instance of uMap is currently in read only mode, no creation/edit is "
 "allowed."
 msgstr ""
 
 #: templates/umap/content.html:31
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Preizkusna različica je na voljo za pregled in spoznavanje funkcionalnosti. Če potrebujete stabilno različico, uporabite <a href=\"%(stable_url)s\">%(stable_url)s</a>. Seveda lahko vzpostavite svoj strežnik, saj je orodje <a href=\"%(repo_url)s\">odprtokodno</a>!"
+msgstr "Det här är en demo-instans, som används för tester och förhandsversioner. Om du behöver en stabil instans, använd <a href=\"%(stable_url)s\">%(stable_url)s</a>. Du kan också vara värd för din egen instans med <a href=\"%(repo_url)s\">öppen källkod</a>!"
 
 #: templates/umap/home.html:8
 msgid "Map of the uMaps"
-msgstr "Zemljevid spletišča uMaps"
+msgstr "Karta över uMap-kartor."
 
 #: templates/umap/home.html:13
 msgid "Get inspired, browse maps"
-msgstr "Poiščite zamisli, prebrskajte zemljevide"
+msgstr "Inspireras av andra kartor"
 
 #: templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Prijava je uspešno končana. Poteka nalaganje vsebine ..."
+msgstr "Du är nu inloggad. Fortsätter..."
 
 #: templates/umap/map_list.html:9 views.py:281
 msgid "by"
-msgstr "–"
+msgstr "av"
 
 #: templates/umap/map_list.html:17 templates/umap/map_table.html:39
 msgid "More"
-msgstr "Več"
+msgstr "Mer"
 
 #: templates/umap/map_table.html:6
 msgid "Map"
 msgstr ""
 
 #: templates/umap/map_table.html:7
 msgid "Name"
@@ -309,102 +310,100 @@
 
 #: templates/umap/map_table.html:30
 msgid "Download"
 msgstr ""
 
 #: templates/umap/navigation.html:12
 msgid "My maps"
-msgstr "Moji zemljevidi"
+msgstr "Mina kartor"
 
 #: templates/umap/navigation.html:15
 msgid "Starred maps"
 msgstr ""
 
 #: templates/umap/navigation.html:19
 msgid "Log in"
-msgstr "Prijava"
+msgstr "Logga in"
 
 #: templates/umap/navigation.html:19
 msgid "Sign in"
-msgstr "Vpis"
+msgstr "Logga in"
 
 #: templates/umap/navigation.html:23
 msgid "About"
-msgstr "O projektu"
+msgstr "Om"
 
 #: templates/umap/navigation.html:26
 msgid "Help"
 msgstr ""
 
 #: templates/umap/navigation.html:31
 msgid "Change password"
-msgstr "Zamenjaj geslo"
+msgstr "Byt lösenord"
 
 #: templates/umap/navigation.html:35
 msgid "Log out"
-msgstr "Odjava"
+msgstr "Logga ut"
 
 #: templates/umap/password_change.html:4
 msgid "Password change"
-msgstr "Spremeni geslo"
+msgstr "Byte av lösenord"
 
 #: templates/umap/password_change.html:6
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
-msgstr "Iz varnostnih razlogov morate vpisati staro geslo in nato še dvakrat vpisati novo, da se prepričate v pravilnost vpisa."
+msgstr "Fyll i ditt nuvarande lösenord för säkerhets skull, och sedan ditt nya lösenord två gånger så vi kan undvika felskrivningar. "
 
 #: templates/umap/password_change.html:13
 msgid "Old password"
-msgstr "Staro geslo"
+msgstr "Nuvarande lösenord"
 
 #: templates/umap/password_change.html:18
 msgid "New password"
-msgstr "Novo geslo"
+msgstr "Nytt lösenord"
 
 #: templates/umap/password_change.html:22
 msgid "New password confirmation"
-msgstr "Potrditev novega gesla"
+msgstr "Bekräfta nytt lösenord"
 
 #: templates/umap/password_change.html:23
 msgid "Change my password"
-msgstr "Spremeni geslo"
+msgstr "Ändra mitt lösenord"
 
 #: templates/umap/password_change_done.html:4
 msgid "Password change successful"
-msgstr "Geslo je uspešno spremenjeno."
+msgstr "Lösenordet har ändrats!"
 
 #: templates/umap/password_change_done.html:5
 msgid "Your password was changed."
-msgstr "Geslo je spremenjeno."
+msgstr "Ditt lösenord har ändrats."
 
 #: templates/umap/search.html:10
 #, python-format
 msgid "%(count)s map found:"
 msgid_plural "%(count)s maps found:"
 msgstr[0] ""
 msgstr[1] ""
-msgstr[2] ""
-msgstr[3] ""
 
 #: templates/umap/search.html:18
 msgid "No map found."
 msgstr ""
 
 #: templates/umap/search.html:21
 msgid "Latest created maps"
 msgstr ""
 
 #: templates/umap/search_bar.html:3
 msgid "Search maps"
-msgstr "Poišči zemljevide"
+msgstr "Sök karta"
 
 #: templates/umap/search_bar.html:14
 msgid "Search"
-msgstr "Poišči"
+msgstr "Sök"
 
 #: templates/umap/user_dashboard.html:4 templates/umap/user_dashboard.html:9
 msgid "My dashboard"
 msgstr ""
 
 #: templates/umap/user_dashboard.html:7
 msgid "Search my maps"
@@ -412,23 +411,23 @@
 
 #: templates/umap/user_dashboard.html:18
 msgid "You have no map yet."
 msgstr ""
 
 #: views.py:286
 msgid "View the map"
-msgstr "Pogled zemljevida"
+msgstr "Se kartan"
 
 #: views.py:607
 msgid "Map has been updated!"
-msgstr "Zemljevid je posodobljen!"
+msgstr "Kartan har uppdaterats!"
 
 #: views.py:632
 msgid "Map editors updated with success!"
-msgstr "seznam urednikov je posodobljen!"
+msgstr "Kartans redaktörer har uppdaterats!"
 
 #: views.py:670
 #, python-format
 msgid "The uMap edit link for your map: %(map_name)s"
 msgstr ""
 
 #: views.py:673
@@ -439,23 +438,23 @@
 #: views.py:679
 #, python-format
 msgid "Email sent to %(email)s"
 msgstr ""
 
 #: views.py:690
 msgid "Only its owner can delete the map."
-msgstr "Zemljevid lahko izbriše le lastnik."
+msgstr "Bara ägaren kan radera kartan."
 
 #: views.py:713
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "Zemljevid je kloniran! Za urejanje z drugega računalnika uporabite povezavo: %(anonymous_url)s"
+msgstr "Din karta har kopierats! Om du vill redigera den här kartan från en annan dator, använd denna länk: %(anonymous_url)s"
 
 #: views.py:718
 msgid "Congratulations, your map has been cloned!"
-msgstr "Zemljevid je uspešno kloniran!"
+msgstr "Grattis, din karta har kopierats!"
 
 #: views.py:884
 msgid "Layer successfully deleted."
-msgstr "Plast je uspešno izbrisana."
+msgstr "Lagret har raderats."
```

### Comparing `umap_project-1.4.3/umap/locale/sr/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sr/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sv/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/sv/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/tr/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# d402bbf52766ea36c1c6bd472b2de8fb_a8a94ad, 2020
-# carlbacker, 2020
-# d402bbf52766ea36c1c6bd472b2de8fb_a8a94ad, 2020
-# carlbacker, 2020
+# Emrah Yılmaz <emrahy@yahoo.com>, 2020
+# irem TACYILDIZ <iremeriaia@gmail.com>, 2021
+# Roman Neumüller, 2020
+# Roman Neumüller, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-07-17 13:14+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: carlbacker, 2020\n"
-"Language-Team: Swedish (http://app.transifex.com/openstreetmap/umap/language/sv/)\n"
+"Last-Translator: Roman Neumüller, 2020\n"
+"Language-Team: Turkish (http://app.transifex.com/openstreetmap/umap/language/tr/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: sv\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: tr\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 
 #: forms.py:43
 #, python-format
 msgid "Secret edit link is %s"
-msgstr "Privat redigeringslänk är %s"
+msgstr "Saklı düzenleme bağlantısı şu: %s"
 
 #: forms.py:47
 msgid "Everyone can edit"
-msgstr "Alla kan redigera"
+msgstr "Herkes düzeltebilir"
 
 #: forms.py:48
 msgid "Only editable with secret edit link"
-msgstr "Redigering är bara tillåten med privat redigeringslänk"
+msgstr "Yalnızca gizli düzenleme bağlantısı ile düzenlenebilir"
 
 #: middleware.py:14
 msgid "Site is readonly for maintenance"
-msgstr "Webbplatsen är skrivskyddad för underhållsarbete."
+msgstr "Sitenin bakım modu olduğu için salt okunur"
 
 #: models.py:40
 msgid "name"
-msgstr "namn"
+msgstr "adı"
 
 #: models.py:71
 msgid "details"
-msgstr "detaljer"
+msgstr "ayrıntılar"
 
 #: models.py:72
 msgid "Link to a page where the licence is detailed."
-msgstr "Länk till sida med detaljerad licens information."
+msgstr "Lisansın detaylandırıldığı bir sayfaya bağlantı"
 
 #: models.py:82
 msgid "URL template using OSM tile format"
-msgstr "URL-mall med OSM:s tile-format"
+msgstr "URL şablonu OSM döşeme biçimini kullanıyor"
 
 #: models.py:88
 msgid "Order of the tilelayers in the edit box"
-msgstr "Ordningen för tile-lager i redigeringsrutan"
+msgstr "Harita katmanları sırası düzenleme kutusunda"
 
 #: models.py:134
 msgid "Everyone"
 msgstr ""
 
 #: models.py:135 models.py:141
 msgid "Editors only"
@@ -80,85 +80,85 @@
 
 #: models.py:142
 msgid "Blocked"
 msgstr ""
 
 #: models.py:145 models.py:295
 msgid "description"
-msgstr "beskrivning"
+msgstr "açıklama"
 
 #: models.py:146
 msgid "center"
-msgstr "centrera"
+msgstr "ortalaştır"
 
 #: models.py:147
 msgid "zoom"
-msgstr "zooma"
+msgstr "yakınlaştır"
 
 #: models.py:149
 msgid "locate"
-msgstr "lokalisera"
+msgstr "yerini belirt"
 
 #: models.py:149
 msgid "Locate user on load?"
-msgstr "Lokalisera användaren vid uppstart?"
+msgstr "Yüklenen kullanıcılar bulunsun mu?"
 
 #: models.py:153
 msgid "Choose the map licence."
-msgstr "Välj licens för kartan."
+msgstr "Harita lisansi seç"
 
 #: models.py:154
 msgid "licence"
-msgstr "licens"
+msgstr "lisans"
 
 #: models.py:164
 msgid "owner"
-msgstr "ägare"
+msgstr "sahibi"
 
 #: models.py:168
 msgid "editors"
-msgstr "redaktörer"
+msgstr "editörler"
 
 #: models.py:171
 msgid "edit status"
-msgstr "redigeringsstatus"
+msgstr "düzeltme durumu"
 
 #: models.py:174
 msgid "share status"
-msgstr "delningsstatus"
+msgstr "durum paylaş"
 
 #: models.py:177
 msgid "settings"
-msgstr "inställningar"
+msgstr "ayarlar"
 
 #: models.py:250
 msgid "Clone of"
-msgstr "Kopia av"
+msgstr "Kopya"
 
 #: models.py:299
 msgid "display on load"
-msgstr "visa vid uppstart"
+msgstr "yüklerken görüntüle"
 
 #: models.py:300
 msgid "Display this layer on load."
-msgstr "Visa detta lager från start."
+msgstr "Yüklerken bu katman görüntüle"
 
 #: templates/404.html:6
 msgid "Take me to the home page"
-msgstr "Ta mig till startsidan"
+msgstr "Anasayfa aç"
 
 #: templates/auth/user_detail.html:5
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "Bläddra bland %(current_user)ss kartor"
+msgstr "%(current_user)s'nın haritaları görüntüle"
 
 #: templates/auth/user_detail.html:12
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr "%(current_user)s har inga kartor."
+msgstr "%(current_user)s'nın haritaları yok."
 
 #: templates/auth/user_stars.html:5
 #, python-format
 msgid "Browse %(current_user)s's starred maps"
 msgstr ""
 
 #: templates/auth/user_stars.html:12
@@ -170,115 +170,115 @@
 msgid ""
 "uMap lets you create maps with OpenStreetMap layers in a minute and embed "
 "them in your site."
 msgstr ""
 
 #: templates/registration/login.html:3
 msgid "Please log in with your account"
-msgstr "Vänligen logga in med ditt konto"
+msgstr "Lütfen hesabınızla giriş yapın"
 
 #: templates/registration/login.html:15
 msgid "Username"
-msgstr "Användarnamn"
+msgstr "Kullanıcı adı"
 
 #: templates/registration/login.html:18
 msgid "Password"
-msgstr "Lösenord"
+msgstr "Şifre"
 
 #: templates/registration/login.html:19
 msgid "Login"
-msgstr "Logga in"
+msgstr "Giriş yap"
 
 #: templates/registration/login.html:24
 msgid "Please choose a provider"
-msgstr "Välj en leverantör"
+msgstr "Lütfen bir sağlayıcı seçin"
 
 #: templates/umap/about_summary.html:11
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
-msgstr "Med uMap kan du på minuter skapa egna kartor med <a href=\"%(osm_url)s\" />OpenStreetMap</a> lager och sedan bädda in dem på din webbsida."
+msgstr "uMap ile bir dakikada <a href=\"%(osm_url)s\" />OpenStreetMap</a> katmanları kullanıp kendi sitenize gömmesi özel haritalar oluşturmanıza sağlar."
 
 #: templates/umap/about_summary.html:21
 msgid "Choose the layers of your map"
-msgstr "Välj lager för din karta"
+msgstr "Haritanızın katmanlarını seçin"
 
 #: templates/umap/about_summary.html:22
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "Lägg till POI:er, markörer, linjer, polygoner..."
+msgstr "İlgi noktaları ekle: işaretler, çizgiler, çokgenler"
 
 #: templates/umap/about_summary.html:23
 msgid "Manage POIs colours and icons"
-msgstr "Ändra färger och ikoner för POI:er"
+msgstr "Renkleri ve sembolleri yönet"
 
 #: templates/umap/about_summary.html:24
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr "Hantera kartalternativ: visa en minikarta, lokalisera användaren..."
+msgstr "Harita seçeneklerini yönet: bir mini harita göster, yükleyen kullanıcıyı göster"
 
 #: templates/umap/about_summary.html:25
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Importera strukturerad geodata (geojson, gpx, kml, osm...)"
+msgstr "Coğrafi yapılandırılmış verileri yığın olarak içe aktar (geojson, gpx, kml, osm...)"
 
 #: templates/umap/about_summary.html:26
 msgid "Choose the license for your data"
-msgstr "Välj licens för dina data"
+msgstr "Verileriniz için lisansı seçin"
 
 #: templates/umap/about_summary.html:27
 msgid "Embed and share your map"
-msgstr "Bädda in och dela din karta"
+msgstr "Haritanızı yerleştirin ve paylaşın"
 
 #: templates/umap/about_summary.html:37
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Och det är <a href=\"%(repo_url)s\">öppen källkod</a>!"
+msgstr "Ve üsttelik <a href=\"%(repo_url)s\">açık kaynak kodlu</a>!"
 
 #: templates/umap/about_summary.html:48 templates/umap/navigation.html:42
 #: templates/umap/user_dashboard.html:18
 msgid "Create a map"
-msgstr "Skapa en karta"
+msgstr "Bir harita oluştur"
 
 #: templates/umap/about_summary.html:51
 msgid "Play with the demo"
-msgstr "Lek med demotjänsten"
+msgstr "Deneme sayfalarla oyna"
 
 #: templates/umap/content.html:23
 msgid ""
 "This instance of uMap is currently in read only mode, no creation/edit is "
 "allowed."
 msgstr ""
 
 #: templates/umap/content.html:31
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Det här är en demo-instans, som används för tester och förhandsversioner. Om du behöver en stabil instans, använd <a href=\"%(stable_url)s\">%(stable_url)s</a>. Du kan också vara värd för din egen instans med <a href=\"%(repo_url)s\">öppen källkod</a>!"
+msgstr "Bu örnek, testler ve yayın öncesi sürümler için kullanılan bir demo örneğidir. Kararlı bir örneğe ihtiyacınız varsa, lütfen <a href=\"%(stable_url)s\">%(stable_url)s</a> kullanın. Kendi örneğinizi de barındırabilirsiniz, cünkü <a href=\"%(repo_url)s\">açık kaynak yazılım</a>!"
 
 #: templates/umap/home.html:8
 msgid "Map of the uMaps"
-msgstr "Karta över uMap-kartor."
+msgstr "uMaps'in haritası"
 
 #: templates/umap/home.html:13
 msgid "Get inspired, browse maps"
-msgstr "Inspireras av andra kartor"
+msgstr "İlham alın, haritalara göz atın"
 
 #: templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Du är nu inloggad. Fortsätter..."
+msgstr "Giriş tamamlandı. Devam..."
 
 #: templates/umap/map_list.html:9 views.py:281
 msgid "by"
-msgstr "av"
+msgstr "tarafından"
 
 #: templates/umap/map_list.html:17 templates/umap/map_table.html:39
 msgid "More"
-msgstr "Mer"
+msgstr "Daha fazla"
 
 #: templates/umap/map_table.html:6
 msgid "Map"
 msgstr ""
 
 #: templates/umap/map_table.html:7
 msgid "Name"
@@ -310,77 +310,77 @@
 
 #: templates/umap/map_table.html:30
 msgid "Download"
 msgstr ""
 
 #: templates/umap/navigation.html:12
 msgid "My maps"
-msgstr "Mina kartor"
+msgstr "Haritalarım"
 
 #: templates/umap/navigation.html:15
 msgid "Starred maps"
 msgstr ""
 
 #: templates/umap/navigation.html:19
 msgid "Log in"
-msgstr "Logga in"
+msgstr "Oturum aç"
 
 #: templates/umap/navigation.html:19
 msgid "Sign in"
-msgstr "Logga in"
+msgstr "Katıl"
 
 #: templates/umap/navigation.html:23
 msgid "About"
-msgstr "Om"
+msgstr "Hakkında"
 
 #: templates/umap/navigation.html:26
 msgid "Help"
 msgstr ""
 
 #: templates/umap/navigation.html:31
 msgid "Change password"
-msgstr "Byt lösenord"
+msgstr "Şifre değiştir"
 
 #: templates/umap/navigation.html:35
 msgid "Log out"
-msgstr "Logga ut"
+msgstr "Oturum kapat"
 
 #: templates/umap/password_change.html:4
 msgid "Password change"
-msgstr "Byte av lösenord"
+msgstr "Şifre değiştirme işlemi"
 
 #: templates/umap/password_change.html:6
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
-msgstr "Fyll i ditt nuvarande lösenord för säkerhets skull, och sedan ditt nya lösenord två gånger så vi kan undvika felskrivningar. "
+msgstr "Güvenlik açısından lütfen eski şifrenizi girip ardından doğru girdiğinizi doğrulayabilmemiz için yeni şifrenizi iki kez girin."
 
 #: templates/umap/password_change.html:13
 msgid "Old password"
-msgstr "Nuvarande lösenord"
+msgstr "Eski şifre"
 
 #: templates/umap/password_change.html:18
 msgid "New password"
-msgstr "Nytt lösenord"
+msgstr "Yeni şifre"
 
 #: templates/umap/password_change.html:22
 msgid "New password confirmation"
-msgstr "Bekräfta nytt lösenord"
+msgstr "Yeni şifre tekrar"
 
 #: templates/umap/password_change.html:23
 msgid "Change my password"
-msgstr "Ändra mitt lösenord"
+msgstr "Şifrem değiştir"
 
 #: templates/umap/password_change_done.html:4
 msgid "Password change successful"
-msgstr "Lösenordet har ändrats!"
+msgstr "Şifrenin değiştirmesi başarıyla tamamlandı"
 
 #: templates/umap/password_change_done.html:5
 msgid "Your password was changed."
-msgstr "Ditt lösenord har ändrats."
+msgstr "Şifren değiştirildi."
 
 #: templates/umap/search.html:10
 #, python-format
 msgid "%(count)s map found:"
 msgid_plural "%(count)s maps found:"
 msgstr[0] ""
 msgstr[1] ""
@@ -391,19 +391,19 @@
 
 #: templates/umap/search.html:21
 msgid "Latest created maps"
 msgstr ""
 
 #: templates/umap/search_bar.html:3
 msgid "Search maps"
-msgstr "Sök karta"
+msgstr "Harita ara"
 
 #: templates/umap/search_bar.html:14
 msgid "Search"
-msgstr "Sök"
+msgstr "Ara"
 
 #: templates/umap/user_dashboard.html:4 templates/umap/user_dashboard.html:9
 msgid "My dashboard"
 msgstr ""
 
 #: templates/umap/user_dashboard.html:7
 msgid "Search my maps"
@@ -411,23 +411,23 @@
 
 #: templates/umap/user_dashboard.html:18
 msgid "You have no map yet."
 msgstr ""
 
 #: views.py:286
 msgid "View the map"
-msgstr "Se kartan"
+msgstr "Haritayı görüntüle"
 
 #: views.py:607
 msgid "Map has been updated!"
-msgstr "Kartan har uppdaterats!"
+msgstr "Harita güncellendi!"
 
 #: views.py:632
 msgid "Map editors updated with success!"
-msgstr "Kartans redaktörer har uppdaterats!"
+msgstr "Haritanın editörleri başarıyla güncellendi!"
 
 #: views.py:670
 #, python-format
 msgid "The uMap edit link for your map: %(map_name)s"
 msgstr ""
 
 #: views.py:673
@@ -438,23 +438,23 @@
 #: views.py:679
 #, python-format
 msgid "Email sent to %(email)s"
 msgstr ""
 
 #: views.py:690
 msgid "Only its owner can delete the map."
-msgstr "Bara ägaren kan radera kartan."
+msgstr "Salt haritanın sahibi haritayı silebilir."
 
 #: views.py:713
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "Din karta har kopierats! Om du vill redigera den här kartan från en annan dator, använd denna länk: %(anonymous_url)s"
+msgstr "Haritanız çoğaltıldı! Eğer bu haritayı başka bir bilgisayardan düzenlemek isterseniz, lütfen bu bağlantıyı kullanın: %(anonymous_url)s"
 
 #: views.py:718
 msgid "Congratulations, your map has been cloned!"
-msgstr "Grattis, din karta har kopierats!"
+msgstr "Tebrikler, haritanız çoğaltıldı!"
 
 #: views.py:884
 msgid "Layer successfully deleted."
-msgstr "Lagret har raderats."
+msgstr "Katman başarıyla silindi"
```

### Comparing `umap_project-1.4.3/umap/locale/th_TH/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/th_TH/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/tr/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/tr/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/br/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,460 +1,461 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # 
 # Translators:
-# Emrah Yılmaz <emrahy@yahoo.com>, 2020
-# irem TACYILDIZ <iremeriaia@gmail.com>, 2021
-# Roman Neumüller, 2020
-# Roman Neumüller, 2020
+# Dren Ar Frankig <hadrienlouque@gmail.com>, 2023
+# Dren Ar Frankig <hadrienlouque@gmail.com>, 2023
 msgid ""
 msgstr ""
 "Project-Id-Version: uMap\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-07-17 13:14+0000\n"
+"POT-Creation-Date: 2023-07-19 13:43+0000\n"
 "PO-Revision-Date: 2013-11-22 14:00+0000\n"
-"Last-Translator: Roman Neumüller, 2020\n"
-"Language-Team: Turkish (http://app.transifex.com/openstreetmap/umap/language/tr/)\n"
+"Last-Translator: Dren Ar Frankig <hadrienlouque@gmail.com>, 2023\n"
+"Language-Team: Breton (http://app.transifex.com/openstreetmap/umap/language/br/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: tr\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Language: br\n"
+"Plural-Forms: nplurals=5; plural=((n%10 == 1) && (n%100 != 11) && (n%100 !=71) && (n%100 !=91) ? 0 :(n%10 == 2) && (n%100 != 12) && (n%100 !=72) && (n%100 !=92) ? 1 :(n%10 ==3 || n%10==4 || n%10==9) && (n%100 < 10 || n% 100 > 19) && (n%100 < 70 || n%100 > 79) && (n%100 < 90 || n%100 > 99) ? 2 :(n != 0 && n % 1000000 == 0) ? 3 : 4);\n"
 
 #: forms.py:43
 #, python-format
 msgid "Secret edit link is %s"
-msgstr "Saklı düzenleme bağlantısı şu: %s"
+msgstr "Liamm aozañ kuzh: %s"
 
 #: forms.py:47
 msgid "Everyone can edit"
-msgstr "Herkes düzeltebilir"
+msgstr "An holl a c'hall kemmañ"
 
 #: forms.py:48
 msgid "Only editable with secret edit link"
-msgstr "Yalnızca gizli düzenleme bağlantısı ile düzenlenebilir"
+msgstr "N'haller he c'hemmañ nemet gant ul liamm aozañ kuzh"
 
 #: middleware.py:14
 msgid "Site is readonly for maintenance"
-msgstr "Sitenin bakım modu olduğu için salt okunur"
+msgstr ""
 
 #: models.py:40
 msgid "name"
-msgstr "adı"
+msgstr "anv"
 
 #: models.py:71
 msgid "details"
-msgstr "ayrıntılar"
+msgstr "munudoù"
 
 #: models.py:72
 msgid "Link to a page where the licence is detailed."
-msgstr "Lisansın detaylandırıldığı bir sayfaya bağlantı"
+msgstr "Liamm war-zu ur bajenn a zispleg an aotre-implijout."
 
 #: models.py:82
 msgid "URL template using OSM tile format"
-msgstr "URL şablonu OSM döşeme biçimini kullanıyor"
+msgstr "Patrom URL a implij furmad teol OSM"
 
 #: models.py:88
 msgid "Order of the tilelayers in the edit box"
-msgstr "Harita katmanları sırası düzenleme kutusunda"
+msgstr ""
 
 #: models.py:134
 msgid "Everyone"
-msgstr ""
+msgstr "An holl"
 
 #: models.py:135 models.py:141
 msgid "Editors only"
-msgstr ""
+msgstr "Aozerien nemetken"
 
 #: models.py:136
 msgid "Owner only"
-msgstr ""
+msgstr "Ar perc'henner hepken"
 
 #: models.py:139
 msgid "Everyone (public)"
-msgstr ""
+msgstr "An holl (publik)"
 
 #: models.py:140
 msgid "Anyone with link"
-msgstr ""
+msgstr "Piv bennak en deus ul liamm"
 
 #: models.py:142
 msgid "Blocked"
-msgstr ""
+msgstr "Stanket"
 
 #: models.py:145 models.py:295
 msgid "description"
-msgstr "açıklama"
+msgstr "deskrivadur"
 
 #: models.py:146
 msgid "center"
-msgstr "ortalaştır"
+msgstr "kreizañ"
 
 #: models.py:147
 msgid "zoom"
-msgstr "yakınlaştır"
+msgstr "zoumañ"
 
 #: models.py:149
 msgid "locate"
-msgstr "yerini belirt"
+msgstr "lec'hiañ"
 
 #: models.py:149
 msgid "Locate user on load?"
-msgstr "Yüklenen kullanıcılar bulunsun mu?"
+msgstr "Lec'hiañ an implijer en ur gargañ?"
 
 #: models.py:153
 msgid "Choose the map licence."
-msgstr "Harita lisansi seç"
+msgstr "Dibabit aotre-implijout ar gartenn."
 
 #: models.py:154
 msgid "licence"
-msgstr "lisans"
+msgstr "aotre"
 
 #: models.py:164
 msgid "owner"
-msgstr "sahibi"
+msgstr "perc'henner"
 
 #: models.py:168
 msgid "editors"
-msgstr "editörler"
+msgstr "aozerien"
 
 #: models.py:171
 msgid "edit status"
-msgstr "düzeltme durumu"
+msgstr "statud aozañ"
 
 #: models.py:174
 msgid "share status"
-msgstr "durum paylaş"
+msgstr "digor da biv?"
 
 #: models.py:177
 msgid "settings"
-msgstr "ayarlar"
+msgstr "arventennoù"
 
 #: models.py:250
 msgid "Clone of"
-msgstr "Kopya"
+msgstr "Eilenn eus"
 
 #: models.py:299
 msgid "display on load"
-msgstr "yüklerken görüntüle"
+msgstr "diskwel pa vez karget"
 
 #: models.py:300
 msgid "Display this layer on load."
-msgstr "Yüklerken bu katman görüntüle"
+msgstr ""
 
 #: templates/404.html:6
 msgid "Take me to the home page"
-msgstr "Anasayfa aç"
+msgstr "Distreiñ d'ar bajenn degemer"
 
 #: templates/auth/user_detail.html:5
 #, python-format
 msgid "Browse %(current_user)s's maps"
-msgstr "%(current_user)s'nın haritaları görüntüle"
+msgstr "Merdeiñ e kartennoù %(current_user)s"
 
 #: templates/auth/user_detail.html:12
 #, python-format
 msgid "%(current_user)s has no maps."
-msgstr "%(current_user)s'nın haritaları yok."
+msgstr "%(current_user)s n'en/he deus kartenn ebet."
 
 #: templates/auth/user_stars.html:5
 #, python-format
 msgid "Browse %(current_user)s's starred maps"
-msgstr ""
+msgstr "Merdeiñ e kartennoù spilhennet %(current_user)s"
 
 #: templates/auth/user_stars.html:12
 #, python-format
 msgid "%(current_user)s has no starred maps yet."
-msgstr ""
+msgstr "%(current_user)s n'en/he deus kartenn spilhennet ebet."
 
 #: templates/base.html:12
 msgid ""
 "uMap lets you create maps with OpenStreetMap layers in a minute and embed "
 "them in your site."
-msgstr ""
+msgstr "uMap a ro tro deoc'h da grouiñ kartennoù en ur serr-lagad gant foñsoù OpenStreetMap ha d'o enframmañ e-barzh ho lec'hienn."
 
 #: templates/registration/login.html:3
 msgid "Please log in with your account"
-msgstr "Lütfen hesabınızla giriş yapın"
+msgstr "Kevreit gant ho kont mar plij"
 
 #: templates/registration/login.html:15
 msgid "Username"
-msgstr "Kullanıcı adı"
+msgstr "Anv implijer"
 
 #: templates/registration/login.html:18
 msgid "Password"
-msgstr "Şifre"
+msgstr "Ger-tremen"
 
 #: templates/registration/login.html:19
 msgid "Login"
-msgstr "Giriş yap"
+msgstr "Kevreañ"
 
 #: templates/registration/login.html:24
 msgid "Please choose a provider"
-msgstr "Lütfen bir sağlayıcı seçin"
+msgstr "Dibabit ur pourchaser mar plij"
 
 #: templates/umap/about_summary.html:11
 #, python-format
 msgid ""
 "uMap lets you create maps with <a href=\"%(osm_url)s\" />OpenStreetMap</a> "
 "layers in a minute and embed them in your site."
-msgstr "uMap ile bir dakikada <a href=\"%(osm_url)s\" />OpenStreetMap</a> katmanları kullanıp kendi sitenize gömmesi özel haritalar oluşturmanıza sağlar."
+msgstr "uMap a ro tro deoc'h da grouiñ kartennoù en ur serr-lagad gant foñsoù <a href=\"%(osm_url)s\" />OpenStreetMap</a> ha d'o enframmañ e-barzh ho lec'hienn."
 
 #: templates/umap/about_summary.html:21
 msgid "Choose the layers of your map"
-msgstr "Haritanızın katmanlarını seçin"
+msgstr "Dibab ar gwiskadoù evit ho kartenn"
 
 #: templates/umap/about_summary.html:22
 msgid "Add POIs: markers, lines, polygons..."
-msgstr "İlgi noktaları ekle: işaretler, çizgiler, çokgenler"
+msgstr "Ouzhpennañ \"poentoù heverk\": balizennoù, linennoù, lieskornoù..."
 
 #: templates/umap/about_summary.html:23
 msgid "Manage POIs colours and icons"
-msgstr "Renkleri ve sembolleri yönet"
+msgstr "Dibab livioù hag ikonoù ar poentoù heverk"
 
 #: templates/umap/about_summary.html:24
 msgid "Manage map options: display a minimap, locate user on load…"
-msgstr "Harita seçeneklerini yönet: bir mini harita göster, yükleyen kullanıcıyı göster"
+msgstr "Merañ dibarzhioù ar gartenn: diskwel ar gartennig, lec'hiañ an implijer..."
 
 #: templates/umap/about_summary.html:25
 msgid "Batch import geostructured data (geojson, gpx, kml, osm...)"
-msgstr "Coğrafi yapılandırılmış verileri yığın olarak içe aktar (geojson, gpx, kml, osm...)"
+msgstr "Enporzhiañ roadennoù geografek a-vern (geojson, gpx, kml, osm...)"
 
 #: templates/umap/about_summary.html:26
 msgid "Choose the license for your data"
-msgstr "Verileriniz için lisansı seçin"
+msgstr "Diuzañ aotre-implijout ho roadennoù"
 
 #: templates/umap/about_summary.html:27
 msgid "Embed and share your map"
-msgstr "Haritanızı yerleştirin ve paylaşın"
+msgstr "Enframmañ ha rannañ ho kartenn"
 
 #: templates/umap/about_summary.html:37
 #, python-format
 msgid "And it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Ve üsttelik <a href=\"%(repo_url)s\">açık kaynak kodlu</a>!"
+msgstr "Hag <a href=\"%(repo_url)s\">open source</a> eo!"
 
 #: templates/umap/about_summary.html:48 templates/umap/navigation.html:42
 #: templates/umap/user_dashboard.html:18
 msgid "Create a map"
-msgstr "Bir harita oluştur"
+msgstr "Krouiñ ur gartenn"
 
 #: templates/umap/about_summary.html:51
 msgid "Play with the demo"
-msgstr "Deneme sayfalarla oyna"
+msgstr "Amprouiñ an demo!"
 
 #: templates/umap/content.html:23
 msgid ""
 "This instance of uMap is currently in read only mode, no creation/edit is "
 "allowed."
 msgstr ""
 
 #: templates/umap/content.html:31
 #, python-format
 msgid ""
 "This is a demo instance, used for tests and pre-rolling releases. If you "
 "need a stable instance, please use <a "
 "href=\"%(stable_url)s\">%(stable_url)s</a>. You can also host your own "
 "instance, it's <a href=\"%(repo_url)s\">open source</a>!"
-msgstr "Bu örnek, testler ve yayın öncesi sürümler için kullanılan bir demo örneğidir. Kararlı bir örneğe ihtiyacınız varsa, lütfen <a href=\"%(stable_url)s\">%(stable_url)s</a> kullanın. Kendi örneğinizi de barındırabilirsiniz, cünkü <a href=\"%(repo_url)s\">açık kaynak yazılım</a>!"
+msgstr ""
 
 #: templates/umap/home.html:8
 msgid "Map of the uMaps"
-msgstr "uMaps'in haritası"
+msgstr "Kartenn an uMapoù"
 
 #: templates/umap/home.html:13
 msgid "Get inspired, browse maps"
-msgstr "İlham alın, haritalara göz atın"
+msgstr "Bezit awenet en ur furchal kartennoù"
 
 #: templates/umap/login_popup_end.html:2
 msgid "You are logged in. Continuing..."
-msgstr "Giriş tamamlandı. Devam..."
+msgstr "Kevreet oc'h. Gortozit ur pennadig..."
 
 #: templates/umap/map_list.html:9 views.py:281
 msgid "by"
-msgstr "tarafından"
+msgstr "gant"
 
 #: templates/umap/map_list.html:17 templates/umap/map_table.html:39
 msgid "More"
-msgstr "Daha fazla"
+msgstr "Muioc'h"
 
 #: templates/umap/map_table.html:6
 msgid "Map"
-msgstr ""
+msgstr "Kartenn"
 
 #: templates/umap/map_table.html:7
 msgid "Name"
-msgstr ""
+msgstr "Anv"
 
 #: templates/umap/map_table.html:8
 msgid "Who can see / edit"
-msgstr ""
+msgstr "Piv a c'hall gwelet / aozañ"
 
 #: templates/umap/map_table.html:9
 msgid "Last save"
-msgstr ""
+msgstr "Enrollet da ziwezhañ"
 
 #: templates/umap/map_table.html:10
 msgid "Owner"
-msgstr ""
+msgstr "Perc'henner"
 
 #: templates/umap/map_table.html:11
 msgid "Actions"
-msgstr ""
+msgstr "Oberoù"
 
 #: templates/umap/map_table.html:28
 msgid "Share"
-msgstr ""
+msgstr "Rannañ"
 
 #: templates/umap/map_table.html:29
 msgid "Edit"
-msgstr ""
+msgstr "Aozañ"
 
 #: templates/umap/map_table.html:30
 msgid "Download"
-msgstr ""
+msgstr "Pellgargañ"
 
 #: templates/umap/navigation.html:12
 msgid "My maps"
-msgstr "Haritalarım"
+msgstr "Ma c'hartennoù"
 
 #: templates/umap/navigation.html:15
 msgid "Starred maps"
-msgstr ""
+msgstr "Kartennoù spilhennet"
 
 #: templates/umap/navigation.html:19
 msgid "Log in"
-msgstr "Oturum aç"
+msgstr "Kevreañ"
 
 #: templates/umap/navigation.html:19
 msgid "Sign in"
-msgstr "Katıl"
+msgstr "Krouiñ ur gont"
 
 #: templates/umap/navigation.html:23
 msgid "About"
-msgstr "Hakkında"
+msgstr "Diwar-benn"
 
 #: templates/umap/navigation.html:26
 msgid "Help"
-msgstr ""
+msgstr "Skoazell"
 
 #: templates/umap/navigation.html:31
 msgid "Change password"
-msgstr "Şifre değiştir"
+msgstr "Cheñch ar ger-tremen"
 
 #: templates/umap/navigation.html:35
 msgid "Log out"
-msgstr "Oturum kapat"
+msgstr "Digevreañ"
 
 #: templates/umap/password_change.html:4
 msgid "Password change"
-msgstr "Şifre değiştirme işlemi"
+msgstr "Cheñch ar ger-tremen"
 
 #: templates/umap/password_change.html:6
 msgid ""
 "Please enter your old password, for security's sake, and then enter your new"
 " password twice so we can verify you typed it in correctly."
-msgstr "Güvenlik açısından lütfen eski şifrenizi girip ardından doğru girdiğinizi doğrulayabilmemiz için yeni şifrenizi iki kez girin."
+msgstr "Enankit ho ker-tremen kozh ha div wezh ho ker-tremen nevez war-lerc'h mar plij."
 
 #: templates/umap/password_change.html:13
 msgid "Old password"
-msgstr "Eski şifre"
+msgstr "Ger-tremen kozh"
 
 #: templates/umap/password_change.html:18
 msgid "New password"
-msgstr "Yeni şifre"
+msgstr "Ger-tremen nevez"
 
 #: templates/umap/password_change.html:22
 msgid "New password confirmation"
-msgstr "Yeni şifre tekrar"
+msgstr "Kadarnaat ar ger-tremen nevez"
 
 #: templates/umap/password_change.html:23
 msgid "Change my password"
-msgstr "Şifrem değiştir"
+msgstr "Cheñch ar ger-tremen"
 
 #: templates/umap/password_change_done.html:4
 msgid "Password change successful"
-msgstr "Şifrenin değiştirmesi başarıyla tamamlandı"
+msgstr "Cheñchet eo bet ar ger-tremen gant berzh"
 
 #: templates/umap/password_change_done.html:5
 msgid "Your password was changed."
-msgstr "Şifren değiştirildi."
+msgstr "Cheñchet eo bet ho ker-tremen."
 
 #: templates/umap/search.html:10
 #, python-format
 msgid "%(count)s map found:"
 msgid_plural "%(count)s maps found:"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "%(count)s gartenn kavet :"
+msgstr[1] "%(count)s gartenn kavet :"
+msgstr[2] "%(count)s c'hartenn kavet :"
+msgstr[3] "%(count)s kartenn kavet :"
+msgstr[4] "%(count)s kartenn kavet :"
 
 #: templates/umap/search.html:18
 msgid "No map found."
-msgstr ""
+msgstr "Kartenn ebet kavet."
 
 #: templates/umap/search.html:21
 msgid "Latest created maps"
-msgstr ""
+msgstr "Kartennoù krouet da ziwezhañ"
 
 #: templates/umap/search_bar.html:3
 msgid "Search maps"
-msgstr "Harita ara"
+msgstr "Klask kartennoù"
 
 #: templates/umap/search_bar.html:14
 msgid "Search"
-msgstr "Ara"
+msgstr "Klask"
 
 #: templates/umap/user_dashboard.html:4 templates/umap/user_dashboard.html:9
 msgid "My dashboard"
-msgstr ""
+msgstr "Ma zaolenn-vourzh"
 
 #: templates/umap/user_dashboard.html:7
 msgid "Search my maps"
-msgstr ""
+msgstr "Klask em c'hartennoù"
 
 #: templates/umap/user_dashboard.html:18
 msgid "You have no map yet."
-msgstr ""
+msgstr "N'ho peus kartenn ebet c'hoazh."
 
 #: views.py:286
 msgid "View the map"
-msgstr "Haritayı görüntüle"
+msgstr "Diskouez ar gartenn"
 
 #: views.py:607
 msgid "Map has been updated!"
-msgstr "Harita güncellendi!"
+msgstr "Hizivaet eo bet ar gartenn!"
 
 #: views.py:632
 msgid "Map editors updated with success!"
-msgstr "Haritanın editörleri başarıyla güncellendi!"
+msgstr "Aozerien ar gartenn bet hizivaet gant berzh!"
 
 #: views.py:670
 #, python-format
 msgid "The uMap edit link for your map: %(map_name)s"
-msgstr ""
+msgstr "Al liamm uMap evit aozañ ho kartenn: %(map_name)s"
 
 #: views.py:673
 #, python-format
 msgid "Here is your secret edit link: %(link)s"
-msgstr ""
+msgstr "Setu ho liamm aozañ kuzh: %(link)s"
 
 #: views.py:679
 #, python-format
 msgid "Email sent to %(email)s"
-msgstr ""
+msgstr "Postel kaset da %(email)s"
 
 #: views.py:690
 msgid "Only its owner can delete the map."
-msgstr "Salt haritanın sahibi haritayı silebilir."
+msgstr "N'eus nemet perc'henner ar gartenn a c'hall he dilemel."
 
 #: views.py:713
 #, python-format
 msgid ""
 "Your map has been cloned! If you want to edit this map from another "
 "computer, please use this link: %(anonymous_url)s"
-msgstr "Haritanız çoğaltıldı! Eğer bu haritayı başka bir bilgisayardan düzenlemek isterseniz, lütfen bu bağlantıyı kullanın: %(anonymous_url)s"
+msgstr "Eilet eo bet ho kartenn! M'ho peus c'hoant d'he c'hemmañ diwar un urzhiataer all, implijit al liamm-mañ: %(anonymous_url)s"
 
 #: views.py:718
 msgid "Congratulations, your map has been cloned!"
-msgstr "Tebrikler, haritanız çoğaltıldı!"
+msgstr "Eilet eo bet ho kartenn gant berzh!"
 
-#: views.py:884
+#: views.py:897
 msgid "Layer successfully deleted."
-msgstr "Katman başarıyla silindi"
+msgstr "Gwiskad dilamet gant berzh."
```

### Comparing `umap_project-1.4.3/umap/locale/uk_UA/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/uk_UA/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/vi/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/vi/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/zh/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/zh/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/zh_TW/LC_MESSAGES/django.mo` & `umap_project-1.4.4/umap/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/locale/zh_TW/LC_MESSAGES/django.po` & `umap_project-1.4.4/umap/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/management/commands/anonymous_edit_url.py` & `umap_project-1.4.4/umap/management/commands/anonymous_edit_url.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/management/commands/generate_js_locale.py` & `umap_project-1.4.4/umap/management/commands/generate_js_locale.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/management/commands/import_pictograms.py` & `umap_project-1.4.4/umap/management/commands/import_pictograms.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/migrations/0001_initial.py` & `umap_project-1.4.4/umap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/migrations/0003_add_tilelayer.py` & `umap_project-1.4.4/umap/migrations/0003_add_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/migrations/0004_add_licence.py` & `umap_project-1.4.4/umap/migrations/0004_add_licence.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/migrations/0007_auto_20190416_1757.py` & `umap_project-1.4.4/umap/migrations/0007_auto_20190416_1757.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/migrations/0009_star.py` & `umap_project-1.4.4/umap/migrations/0009_star.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/settings/__init__.py` & `umap_project-1.4.4/umap/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/settings/base.py` & `umap_project-1.4.4/umap/settings/base.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/settings/local.py.sample` & `umap_project-1.4.4/umap/settings/local.py.sample`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/favicon.ico` & `umap_project-1.4.4/umap/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/base.css` & `umap_project-1.4.4/umap/static/umap/base.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/bitbucket.png` & `umap_project-1.4.4/umap/static/umap/bitbucket.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/content.css` & `umap_project-1.4.4/umap/static/umap/content.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font.css` & `umap_project-1.4.4/umap/static/umap/font.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/github.png` & `umap_project-1.4.4/umap/static/umap/github.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/map.css` & `umap_project-1.4.4/umap/static/umap/map.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/nav.css` & `umap_project-1.4.4/umap/static/umap/nav.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/openstreetmap.png` & `umap_project-1.4.4/umap/static/umap/openstreetmap.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/twitter.png` & `umap_project-1.4.4/umap/static/umap/twitter.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font/FiraSans-Light.woff` & `umap_project-1.4.4/umap/static/umap/font/FiraSans-Light.woff`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font/FiraSans-Light.woff2` & `umap_project-1.4.4/umap/static/umap/font/FiraSans-Light.woff2`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font/FiraSans-LightItalic.woff` & `umap_project-1.4.4/umap/static/umap/font/FiraSans-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font/FiraSans-LightItalic.woff2` & `umap_project-1.4.4/umap/static/umap/font/FiraSans-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font/FiraSans-SemiBold.woff` & `umap_project-1.4.4/umap/static/umap/font/FiraSans-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/font/FiraSans-SemiBold.woff2` & `umap_project-1.4.4/umap/static/umap/font/FiraSans-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/16-white.svg` & `umap_project-1.4.4/umap/static/umap/img/16-white.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/16.svg` & `umap_project-1.4.4/umap/static/umap/img/16.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/24-white.svg` & `umap_project-1.4.4/umap/static/umap/img/24-white.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/24.svg` & `umap_project-1.4.4/umap/static/umap/img/24.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/edit.svg` & `umap_project-1.4.4/umap/static/umap/img/edit.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/logo_filigree.png` & `umap_project-1.4.4/umap/static/umap/img/logo_filigree.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/osm.svg` & `umap_project-1.4.4/umap/static/umap/img/osm.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/search.gif` & `umap_project-1.4.4/umap/static/umap/img/search.gif`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/source/16-white.svg` & `umap_project-1.4.4/umap/static/umap/img/source/16-white.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/source/16.svg` & `umap_project-1.4.4/umap/static/umap/img/source/16.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/source/24-white.svg` & `umap_project-1.4.4/umap/static/umap/img/source/24-white.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/img/source/24.svg` & `umap_project-1.4.4/umap/static/umap/img/source/24.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.autocomplete.js` & `umap_project-1.4.4/umap/static/umap/js/umap.autocomplete.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.controls.js` & `umap_project-1.4.4/umap/static/umap/js/umap.controls.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.core.js` & `umap_project-1.4.4/umap/static/umap/js/umap.core.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -172,15 +172,15 @@
             value = value[path[i]]
             if (value === undefined) break
         }
         return value
     }
 
     return str.replace(
-        /\{ *([\w_\:\.\|@]+)(?:\|("[^"]*"))? *\}/g,
+        /\{ *([^\{\}/\-]+)(?:\|("[^"]*"))? *\}/g,
         (str, key, staticFallback) => {
             const vars = key.split('|')
             let value
             let path
             if (staticFallback !== undefined) {
                 vars.push(staticFallback)
             }
```

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.features.js` & `umap_project-1.4.4/umap/static/umap/js/umap.features.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -581,15 +581,15 @@
     _initIcon: function() {
         this.options.icon = this.getIcon()
         L.Marker.prototype._initIcon.call(this)
         this.resetTooltip()
     },
 
     _getTooltipAnchor: function() {
-        const anchor = this.options.icon.options.tooltipAnchor,
+        const anchor = this.options.icon.options.tooltipAnchor.clone(),
             direction = this.getOption('labelDirection')
         if (direction === 'left') {
             anchor.x *= -1
         } else if (direction === 'bottom') {
             anchor.x = 0
             anchor.y = 0
         } else if (direction === 'top') {
```

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.forms.js` & `umap_project-1.4.4/umap/static/umap/js/umap.forms.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.icon.js` & `umap_project-1.4.4/umap/static/umap/js/umap.icon.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.js` & `umap_project-1.4.4/umap/static/umap/js/umap.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.layer.js` & `umap_project-1.4.4/umap/static/umap/js/umap.layer.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.permissions.js` & `umap_project-1.4.4/umap/static/umap/js/umap.permissions.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.popup.js` & `umap_project-1.4.4/umap/static/umap/js/umap.popup.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.slideshow.js` & `umap_project-1.4.4/umap/static/umap/js/umap.slideshow.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.tableeditor.js` & `umap_project-1.4.4/umap/static/umap/js/umap.tableeditor.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.ui.js` & `umap_project-1.4.4/umap/static/umap/js/umap.ui.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/js/umap.xhr.js` & `umap_project-1.4.4/umap/static/umap/js/umap.xhr.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/am_ET.js` & `umap_project-1.4.4/umap/static/umap/locale/am_ET.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/am_ET.json` & `umap_project-1.4.4/umap/static/umap/locale/am_ET.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ar.js` & `umap_project-1.4.4/umap/static/umap/locale/ar.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ar.json` & `umap_project-1.4.4/umap/static/umap/locale/ar.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ast.js` & `umap_project-1.4.4/umap/static/umap/locale/ast.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ast.json` & `umap_project-1.4.4/umap/static/umap/locale/ast.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/bg.js` & `umap_project-1.4.4/umap/static/umap/locale/bg.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/bg.json` & `umap_project-1.4.4/umap/static/umap/locale/bg.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/br.js` & `umap_project-1.4.4/umap/static/umap/locale/br.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,404 +1,404 @@
 const locale = {
     "Add symbol": "Ouzhpennañ un arouez",
     "Allow scroll wheel zoom?": "Aotren ar zoum gant ar rodell?",
     "Automatic": "Emgefreek",
-    "Ball": "Ball",
+    "Ball": "Spilhenn",
     "Cancel": "Nullañ",
     "Caption": "Alc'hwez",
     "Change symbol": "Cheñch arouez",
     "Choose the data format": "Diuzañ furmad ar roadennoù",
-    "Choose the layer of the feature": "Choose the layer of the feature",
-    "Circle": "Kelc'hiañ",
+    "Choose the layer of the feature": "Diuzañ gwiskad an elfenn",
+    "Circle": "Kelc'h",
     "Clustered": "Clustered",
     "Data browser": "Furchal ar roadennoù",
     "Default": "Dre ziouer",
-    "Default zoom level": "Default zoom level",
+    "Default zoom level": "Live zoum dre ziouer",
     "Default: name": "Dre ziouer: anv",
     "Display label": "Diskouez un dikedenn",
-    "Display the control to open OpenStreetMap editor": "Display the control to open OpenStreetMap editor",
+    "Display the control to open OpenStreetMap editor": "Diskwel an afell evit digeriñ an aozer OpenStreetMap",
     "Display the data layers control": "Display the data layers control",
-    "Display the embed control": "Display the embed control",
-    "Display the fullscreen control": "Display the fullscreen control",
-    "Display the locate control": "Display the locate control",
+    "Display the embed control": "Diskwel an afell \"enframmañ\"",
+    "Display the fullscreen control": "Diskwel an afell \"skramm a-bezh\"",
+    "Display the locate control": "Diskwel an afell \"lec'hiañ\"",
     "Display the measure control": "Display the measure control",
-    "Display the search control": "Display the search control",
-    "Display the tile layers control": "Display the tile layers control",
-    "Display the zoom control": "Display the zoom control",
-    "Do you want to display a caption bar?": "Do you want to display a caption bar?",
-    "Do you want to display a minimap?": "Do you want to display a minimap?",
+    "Display the search control": "Diskwel an afell \"klask\"",
+    "Display the tile layers control": "Diskwel an afell \"cheñch foñs ar gartenn\"",
+    "Display the zoom control": "Diskwel an afelloù \"zoumañ\" ha \"dizoumañ\"",
+    "Do you want to display a caption bar?": "Fellout a ra deoc'h diskwel ur varrenn alc'hwez?",
+    "Do you want to display a minimap?": "Fellout a ra deoc'h diskwel ur gartennig evit en em lec'hiañ?",
     "Do you want to display a panel on load?": "Do you want to display a panel on load?",
     "Do you want to display popup footer?": "Do you want to display popup footer?",
     "Do you want to display the scale control?": "Fellout a ra deoc'h diskouez skeul ar gartenn?",
     "Do you want to display the «more» control?": "Fellout a ra deoc'h diskwel an afell \"muioc'h\"?",
-    "Drop": "Drop",
-    "GeoRSS (only link)": "GeoRSS (only link)",
+    "Drop": "Takenn",
+    "GeoRSS (only link)": "GeoRSS (liamm hepken)",
     "GeoRSS (title + image)": "GeoRSS (titl + skeudenn)",
     "Heatmap": "Heatmap",
     "Icon shape": "Furm an ikon",
     "Icon symbol": "Arouez an ikon",
-    "Inherit": "Inherit",
+    "Inherit": "Heritañ",
     "Label direction": "Durc'hadur an dikedenn",
     "Label key": "Label key",
-    "Labels are clickable": "Labels are clickable",
+    "Labels are clickable": "An dikedennoù a c'haller klikañ",
     "None": "Hini ebet",
     "On the bottom": "D'an traoñ",
     "On the left": "A-gleiz",
     "On the right": "A-zehoù",
     "On the top": "D'an nec'h",
     "Popup content template": "Popup content template",
     "Set symbol": "Termenañ an arouez",
     "Side panel": "Panell gostez",
-    "Simplify": "Simplify",
+    "Simplify": "Eeunaat",
     "Symbol or url": "Arouez pe URL",
     "Table": "Taolenn",
     "always": "bepred",
     "clear": "skarzhañ",
-    "collapsed": "collapsed",
+    "collapsed": "serret",
     "color": "liv",
-    "dash array": "dash array",
+    "dash array": "Barrennoùigoù",
     "define": "termenañ",
     "description": "deskrivadur",
-    "expanded": "expanded",
+    "expanded": "digor",
     "fill": "leuniañ",
     "fill color": "liv leuniañ",
-    "fill opacity": "fill opacity",
+    "fill opacity": "demerez al leuniañ",
     "hidden": "kuzhet",
     "iframe": "iframe",
-    "inherit": "inherit",
+    "inherit": "heritañ",
     "name": "anv",
     "never": "morse",
     "new window": "prenestr nevez",
     "no": "ket",
     "on hover": "on hover",
     "opacity": "demerez",
     "parent window": "prenestr kar",
-    "stroke": "stroke",
+    "stroke": "tres",
     "weight": "tevder",
     "yes": "ya",
     "{delay} seconds": "{delay} segondenn",
-    "# one hash for main heading": "# one hash for main heading",
-    "## two hashes for second heading": "## two hashes for second heading",
-    "### three hashes for third heading": "### three hashes for third heading",
+    "# one hash for main heading": "# un diezenn evit an titl pennañ",
+    "## two hashes for second heading": "## div ziezenn evit an eil titl",
+    "### three hashes for third heading": "### teir diezenn evit an trede titl",
     "**double star for bold**": "**div steredennig evit tevaat**",
     "A comma separated list of numbers that defines the stroke dash pattern. Ex.: \"5, 10, 15\".": "A comma separated list of numbers that defines the stroke dash pattern. Ex.: \"5, 10, 15\".",
     "About": "Diwar-benn",
-    "Action not allowed :(": "Action not allowed :(",
-    "Activate slideshow mode": "Activate slideshow mode",
+    "Action not allowed :(": "N'oc'h ket aotreet d'ober-se :(",
+    "Activate slideshow mode": "Gweredekaat ar mod diaporama",
     "Add a layer": "Ouzhpennañ ur gwiskad",
     "Add a line to the current multi": "Add a line to the current multi",
     "Add a new property": "Ouzhpennañ ur perzh nevez",
     "Add a polygon to the current multi": "Add a polygon to the current multi",
     "Advanced actions": "Oberoù araokaet",
     "Advanced properties": "Perzhioù araokaet",
-    "All properties are imported.": "All properties are imported.",
+    "All properties are imported.": "Enporzhiet eo bet an holl berzhioù.",
     "Allow interactions": "Allow interactions",
-    "An error occured": "Ur fazi zo bet",
+    "An error occured": "Ur fazi ez eus bet",
     "Are you sure you want to cancel your changes?": "Ha sur oc'h e faot deoc'h nullañ ho kemmoù?",
-    "Are you sure you want to clone this map and all its datalayers?": "Are you sure you want to clone this map and all its datalayers?",
+    "Are you sure you want to clone this map and all its datalayers?": "Ha sur oc'h e faot deoc'h arredaoliñ ar gartenn-mañ hag he holl wiskadoù roadennoù?",
     "Are you sure you want to delete the feature?": "Ha sur oc'h e faot deoc'h dilemel an elfenn-mañ?",
     "Are you sure you want to delete this layer?": "Ha sur oc'h e faot deoc'h dilemel ar gwiskad-mañ?",
     "Are you sure you want to delete this map?": "Ha sur oc'h e faot deoc'h dilemel ar gartenn-mañ?",
     "Are you sure you want to delete this property on all the features?": "Ha sur oc'h a faot deoc'h lemel ar perzh-mañ diwar an holl elfennoù?",
     "Are you sure you want to restore this version?": "Ha sur oc'h e faot deoc'h adsevel ar stumm-mañ?",
     "Attach the map to my account": "Stagañ ar gartenn d'am c'hont",
     "Auto": "Auto",
-    "Autostart when map is loaded": "Autostart when map is loaded",
-    "Bring feature to center": "Bring feature to center",
+    "Autostart when map is loaded": "Loc'hañ pa vez karget ar gartenn",
+    "Bring feature to center": "Kreizañ ar gartenn war an elfenn-mañ",
     "Browse data": "Furchal ar roadennoù",
     "Cancel edits": "Nullañ ar c'hemmoù",
-    "Center map on your location": "Center map on your location",
+    "Center map on your location": "Kreizañ ar gartenn war al lec'h m'emaoc'h",
     "Change map background": "Cheñch foñs ar gartenn",
     "Change tilelayers": "Cheñch foñs ar gartenn",
-    "Choose a preset": "Choose a preset",
-    "Choose the format of the data to import": "Choose the format of the data to import",
-    "Choose the layer to import in": "Choose the layer to import in",
-    "Click last point to finish shape": "Click last point to finish shape",
+    "Choose a preset": "Diuzañ ur rakdibab",
+    "Choose the format of the data to import": "Diuzañ furmad ar roadennoù da enporzhiañ",
+    "Choose the layer to import in": "Diuzañ ar gwiskad evit enporzhiañ e-barzh",
+    "Click last point to finish shape": "Klikañ war ar poent diwezhañ evit echuiñ an tres",
     "Click to add a marker": "Klikañ evit ouzhpennañ ur valizenn",
-    "Click to continue drawing": "Click to continue drawing",
+    "Click to continue drawing": "Klikañ evit kenderc'hel da dresañ",
     "Click to edit": "Klikañ evit aozañ",
     "Click to start drawing a line": "Klikañ evit tresañ ul linenn",
     "Click to start drawing a polygon": "Klikañ evit tresañ ul lieskorn",
     "Clone": "Arredaoliñ",
-    "Clone of {name}": "Clone of {name}",
+    "Clone of {name}": "Eilenn eus {name}",
     "Clone this feature": "Arredaoliñ an elfenn-mañ",
     "Clone this map": "Arredaoliñ ar gartenn-mañ",
     "Close": "Serriñ",
     "Clustering radius": "Clustering radius",
     "Comma separated list of properties to use when filtering features": "Comma separated list of properties to use when filtering features",
     "Comma, tab or semi-colon separated values. SRS WGS84 is implied. Only Point geometries are imported. The import will look at the column headers for any mention of «lat» and «lon» at the begining of the header, case insensitive. All other column are imported as properties.": "Comma, tab or semi-colon separated values. SRS WGS84 is implied. Only Point geometries are imported. The import will look at the column headers for any mention of «lat» and «lon» at the begining of the header, case insensitive. All other column are imported as properties.",
-    "Continue line": "Kenderc'hel al liamm",
+    "Continue line": "Kenderc'hel al linenn",
     "Continue line (Ctrl+Click)": "Kenderc'hel al linenn (Reol+Klikañ)",
     "Coordinates": "Daveennoù",
     "Credits": "Kredadoù",
-    "Current view instead of default map view?": "Current view instead of default map view?",
+    "Current view instead of default map view?": "Gwel a-vremañ e-lec'h ar gwel dre ziouer?",
     "Custom background": "Foñs personelaet",
-    "Data is browsable": "Data is browsable",
+    "Data is browsable": "Roadennoù a c'hall merdeiñ",
     "Default interaction options": "Default interaction options",
     "Default properties": "Perzhioù dre ziouer",
     "Default shape properties": "Default shape properties",
     "Define link to open in a new window on polygon click.": "Define link to open in a new window on polygon click.",
-    "Delay between two transitions when in play mode": "Delay between two transitions when in play mode",
+    "Delay between two transitions when in play mode": "Dale etre daou dremen pa vez e mod lenn",
     "Delete": "Dilemel",
     "Delete all layers": "Dilemel kement gwiskad",
     "Delete layer": "Dilemel ar gwiskad",
     "Delete this feature": "Dilemel an elfenn-mañ",
     "Delete this property on all the features": "Dilemel ar perzh-mañ",
-    "Delete this shape": "Delete this shape",
+    "Delete this shape": "Dilemel an tres-mañ",
     "Delete this vertex (Alt+Click)": "Dilemel ar poent-mañ (Erl+Klik)",
-    "Directions from here": "Directions from here",
-    "Disable editing": "Disable editing",
+    "Directions from here": "Heñchadurioù adalek amañ",
+    "Disable editing": "Paouez da aozañ",
     "Display measure": "Diskouez ar muzulioù",
-    "Display on load": "Display on load",
+    "Display on load": "Diskwel en ur gargañ",
     "Download": "Pellgargañ",
     "Download data": "Pellgargañ ar roadennoù",
-    "Drag to reorder": "Drag to reorder",
+    "Drag to reorder": "Riklañ evit adurzhiañ",
     "Draw a line": "Tresañ ul linenn",
     "Draw a marker": "Ouzhpennañ ur valizenn",
     "Draw a polygon": "Tresañ ul lieskorn",
     "Draw a polyline": "Tresañ ul linenn",
-    "Dynamic": "Dynamic",
-    "Dynamic properties": "Dynamic properties",
+    "Dynamic": "Buhezek",
+    "Dynamic properties": "Perzhioù buhezek",
     "Edit": "Aozañ",
-    "Edit feature's layer": "Edit feature's layer",
+    "Edit feature's layer": "Kemmañ gwiskad an elfenn",
     "Edit map properties": "Aozañ perzhioù ar gartenn",
     "Edit map settings": "Kemmañ arventennoù ar gartenn",
     "Edit properties in a table": "Aozañ ar perzhioù en un daolenn",
     "Edit this feature": "Kemmañ an elfenn-mañ",
     "Editing": "Oc'h aozañ",
     "Embed and share this map": "Ezporzhiañ ha rannañ ar gartenn",
     "Embed the map": "Enframmañ ar gartenn",
     "Empty": "Goullonderiñ",
-    "Enable editing": "Enable editing",
-    "Error in the tilelayer URL": "Error in the tilelayer URL",
-    "Error while fetching {url}": "Error while fetching {url}",
+    "Enable editing": "Kregiñ da aozañ",
+    "Error in the tilelayer URL": "Ur fazi zo en URL foñs ar gartenn",
+    "Error while fetching {url}": "Ur fazi ez eus bet en ur c'hervel an URL {url}",
     "Exit Fullscreen": "Kuitaat ar mod skramm a-bezh",
     "Extract shape to separate feature": "Extract shape to separate feature",
     "Fetch data each time map view changes.": "Fetch data each time map view changes.",
     "Filter keys": "Filter keys",
     "Filter…": "Silañ...",
     "Format": "Furmad",
-    "From zoom": "From zoom",
+    "From zoom": "Adalek ar zoum",
     "Full map data": "Roadennoù klok ar gartenn",
     "Go to «{feature}»": "Mont da «{feature}»",
     "Heatmap intensity property": "Heatmap intensity property",
     "Heatmap radius": "Heatmap radius",
     "Help": "Skoazell",
-    "Hide controls": "Hide controls",
+    "Hide controls": "Kuzhat ar binvioù",
     "Home": "Degemer",
     "How much to simplify the polyline on each zoom level (more = better performance and smoother look, less = more accurate)": "How much to simplify the polyline on each zoom level (more = better performance and smoother look, less = more accurate)",
     "If false, the polygon will act as a part of the underlying map.": "If false, the polygon will act as a part of the underlying map.",
-    "Iframe with custom height (in px): {{{http://iframe.url.com|height}}}": "Iframe with custom height (in px): {{{http://iframe.url.com|height}}}",
-    "Iframe with custom height and width (in px): {{{http://iframe.url.com|height*width}}}": "Iframe with custom height and width (in px): {{{http://iframe.url.com|height*width}}}",
+    "Iframe with custom height (in px): {{{http://iframe.url.com|height}}}": "Iframe gant uhelder personelaet (e pikselioù): {{{http://iframe.url.com|height}}}",
+    "Iframe with custom height and width (in px): {{{http://iframe.url.com|height*width}}}": "Iframe gant mentoù personelaet (e pikselioù): {{{http://iframe.url.com|height*width}}}",
     "Iframe: {{{http://iframe.url.com}}}": "Iframe: {{{http://iframe.url.com}}}",
-    "Image with custom width (in px): {{http://image.url.com|width}}": "Image with custom width (in px): {{http://image.url.com|width}}",
+    "Image with custom width (in px): {{http://image.url.com|width}}": "Skeudenn gant ledander personelaet (e pikselioù): {{http://image.url.com|width}}",
     "Image: {{http://image.url.com}}": "Skeudenn: {{http://image.url.com}}",
     "Import": "Enporzhiañ",
     "Import data": "Enporzhiañ roadennoù",
     "Import in a new layer": "Enporzhiañ ur gwiskad nevez",
-    "Imports all umap data, including layers and settings.": "Imports all umap data, including layers and settings.",
-    "Include full screen link?": "Include full screen link?",
+    "Imports all umap data, including layers and settings.": "Enporzhiañ an holl roadennoù ar gartenn, ar gwiskadoù hag an arventennoù en o zouez.",
+    "Include full screen link?": "Lakaat ul liamm \"skramm a-bezh\" e-barzh?",
     "Interaction options": "Interaction options",
     "Invalid umap data": "Roadennoù umap direizh",
     "Invalid umap data in {filename}": "Roadennoù umap direizh e-barzh {filename}",
-    "Keep current visible layers": "Keep current visible layers",
+    "Keep current visible layers": "Derc'hel ar gwiskadoù a c'haller gwelet bremañ",
     "Latitude": "Ledred",
     "Layer": "Gwiskad",
     "Layer properties": "Perzhioù ar gwiskad",
     "Licence": "Aotre-implijout",
-    "Limit bounds": "Limit bounds",
+    "Limit bounds": "Bevennoù geografek",
     "Link to…": "Liamm etrezek...",
     "Link with text: [[http://example.com|text of the link]]": "Liamm gant testenn: [[http://skouer.bzh|testenn al liamm]]",
     "Long credits": "Kredadoù hir",
     "Longitude": "Hedred",
-    "Make main shape": "Make main shape",
+    "Make main shape": "Tres pennañ",
     "Manage layers": "Merañ ar gwiskadoù",
-    "Map background credits": "Map background credits",
+    "Map background credits": "Kredadoù foñs ar gartenn",
     "Map has been attached to your account": "Staget eo bet ar gartenn d'ho kont",
-    "Map has been saved!": "Enrollet eo bet ar gartenn",
-    "Map user content has been published under licence": "Map user content has been published under licence",
+    "Map has been saved!": "Enrollet eo bet ar gartenn!",
+    "Map user content has been published under licence": "Endalc'had ar gartenn zo bet embannet gant an aotre-implijout",
     "Map's editors": "Aozerien ar gartenn",
     "Map's owner": "Perc'henner ar gartenn",
     "Merge lines": "Kendeuziñ al linennoù",
     "More controls": "Binvioù all",
     "Must be a valid CSS value (eg.: DarkBlue or #123456)": "Rankout a ra bezañ un talvoud CSS reizh (da sk.: DarkBlue pe #123456)",
     "No licence has been set": "Aotre-implijout ebet bet termenet",
     "No results": "Disoc'h ebet",
     "Only visible features will be downloaded.": "An elfennoù hewel hepken a vo pellgarget.",
-    "Open download panel": "Open download panel",
+    "Open download panel": "Digeriñ prenestr ar pellgargadurioù",
     "Open link in…": "Digeriñ al liamm e...",
     "Open this map extent in a map editor to provide more accurate data to OpenStreetMap": "Open this map extent in a map editor to provide more accurate data to OpenStreetMap",
     "Optional intensity property for heatmap": "Optional intensity property for heatmap",
-    "Optional. Same as color if not set.": "Optional. Same as color if not set.",
+    "Optional. Same as color if not set.": "Diret. Al liv pennañ a vo implijet ma ne vez ket termenet.",
     "Override clustering radius (default 80)": "Override clustering radius (default 80)",
     "Override heatmap radius (default 25)": "Override heatmap radius (default 25)",
-    "Please be sure the licence is compliant with your use.": "Please be sure the licence is compliant with your use.",
+    "Please be sure the licence is compliant with your use.": "Gwiriit m'az oc'h aotreet da implijout ar roadennoù-mañ mar plij.",
     "Please choose a format": "Diuzit ur furmad mar plij",
-    "Please enter the name of the property": "Please enter the name of the property",
-    "Please enter the new name of this property": "Please enter the new name of this property",
-    "Problem in the response": "Problem in the response",
-    "Problem in the response format": "Problem in the response format",
-    "Properties imported:": "Properties imported:",
-    "Provide an URL here": "Provide an URL here",
-    "Proxy request": "Proxy request",
-    "Remote data": "Remote data",
+    "Please enter the name of the property": "Enankit anv ar perzh mar plij",
+    "Please enter the new name of this property": "Enankit anv nevez ar perzh-mañ mar plij",
+    "Problem in the response": "Kudenn e respont ar servijer",
+    "Problem in the response format": "Kudenn gant furmadiñ ar respont",
+    "Properties imported:": "Perzhioù enporzhiet:",
+    "Provide an URL here": "Pourchas un URL amañ",
+    "Proxy request": "Reked proksi",
+    "Remote data": "Rouedadoù a-bell",
     "Remove shape from the multi": "Remove shape from the multi",
     "Rename this property on all the features": "Adenvel ar perzh-mañ",
-    "Replace layer content": "Replace layer content",
+    "Replace layer content": "Erlec'hiañ endalc'had ar gwiskad",
     "Restore this version": "Adsevel ar stumm-mañ?",
     "Save": "Enrollañ",
     "Save anyway": "Enrollañ evelkent",
-    "Save current edits": "Save current edits",
+    "Save current edits": "Enrollañ ar c'hemmoù a-vremañ ",
     "Save this center and zoom": "Save this center and zoom",
-    "Save this location as new feature": "Save this location as new feature",
+    "Save this location as new feature": "Enrollañ al lec'h-mañ evel un elfenn nevez",
     "Search a place name": "Klask un anv-lec'h ",
-    "Search location": "Search location",
-    "Secret edit link is:<br>{link}": "Secret edit link is:<br>{link}",
+    "Search location": "Klask ul lec'h",
+    "Secret edit link is:<br>{link}": "Liamm aozañ kuzh:<br>{link}",
     "See all": "Gwelet pep tra",
     "See data layers": "Diskouez ar gwiskadoù",
     "See full screen": "Gwelet e skramm a-bezh",
-    "Set it to false to hide this layer from the slideshow, the data browser, the popup navigation…": "Set it to false to hide this layer from the slideshow, the data browser, the popup navigation…",
-    "Shape properties": "Shape properties",
+    "Set it to false to hide this layer from the slideshow, the data browser, the popup navigation…": "Diweredekaat evit kuzhat ar gwiskad-mañ ouzh an diaporama, ar merdeer roadennoù...",
+    "Shape properties": "Perzhioù ar furm",
     "Short URL": "URL berr",
     "Short credits": "Kredadoù berr",
     "Show/hide layer": "Diskouez/kuzhat ar gwiskad",
     "Simple link: [[http://example.com]]": "Liamm eeun: [[http://skouer.bzh]]",
     "Slideshow": "Diaporama",
     "Sort key": "Sort key",
     "Split line": "Disrannañ al linenn",
     "Start a hole here": "Ouzhpennañ un toull e-barzh",
     "Start editing": "Kregiñ da aozañ",
     "Start slideshow": "Lenn",
     "Stop editing": "Paouez da aozañ",
     "Stop slideshow": "Ehan",
-    "Supported scheme": "Supported scheme",
+    "Supported scheme": "Steuñv skoret",
     "Supported variables that will be dynamically replaced": "Supported variables that will be dynamically replaced",
     "TMS format": "Furmad TMS",
     "Text color for the cluster label": "Text color for the cluster label",
     "Text formatting": "Furmaozañ an destenn",
     "To use if remote server doesn't allow cross domain (slower)": "To use if remote server doesn't allow cross domain (slower)",
-    "To zoom": "To zoom",
+    "To zoom": "Betek ar zoum",
     "Transfer shape to edited feature": "Transfer shape to edited feature",
-    "Transform to lines": "Transform to lines",
-    "Transform to polygon": "Transform to polygon",
+    "Transform to lines": "Treiñ da linennoù",
+    "Transform to polygon": "Treiñ d'ul lieskorn",
     "Type of layer": "Seurt ar gwiskad",
     "Unable to detect format of file {filename}": "N'haller ket anavezout furmad ar restr {filename}",
     "Untitled layer": "Gwiskad dizanv",
     "Untitled map": "Kartenn dizanv",
     "Update permissions": "Kemmañ an aotreoù",
     "Update permissions and editors": "Kemmañ an aotreoù hag an aozerien",
-    "Url": "Url",
-    "Use current bounds": "Use current bounds",
+    "Url": "URL",
+    "Use current bounds": "Implij ar gwel a-vremañ",
     "Use placeholders with feature properties between brackets, eg. &#123;name&#125;, they will be dynamically replaced by the corresponding values.": "Use placeholders with feature properties between brackets, eg. &#123;name&#125;, they will be dynamically replaced by the corresponding values.",
-    "User content credits": "User content credits",
+    "User content credits": "Kredadoù evit danvez an implijer",
     "User interface options": "Dibarzhioù etrefas an implijer",
     "Versions": "Stummoù",
     "View Fullscreen": "Mont e mod skramm a-bezh",
-    "Where do we go from here?": "Where do we go from here?",
-    "Whether to display or not polygons paths.": "Whether to display or not polygons paths.",
-    "Whether to fill polygons with color.": "Whether to fill polygons with color.",
+    "Where do we go from here?": "Dre belec'h ez eomp adalek amañ?",
+    "Whether to display or not polygons paths.": "Diskouez trolinennoù al lieskornoù",
+    "Whether to fill polygons with color.": "Leuniañ al lieskornoù gant liv",
     "Who can edit": "Piv a c'hall aozañ",
     "Who can view": "Piv a c'hall gwelet",
-    "Will be displayed in the bottom right corner of the map": "Will be displayed in the bottom right corner of the map",
-    "Will be visible in the caption of the map": "Will be visible in the caption of the map",
+    "Will be displayed in the bottom right corner of the map": "Diskwelet e vo e traoñ a-zehoù ar gartenn",
+    "Will be visible in the caption of the map": "Gwelus e vo en alc'hwez ar gartenn",
     "Woops! Someone else seems to have edited the data. You can save anyway, but this will erase the changes made by others.": "Chaous! Seblant a ra ez eus bet kemmet ar gartenn gant unan bennak all. Gallout a rit enrollañ koulskoude, kollet e vo e roadennoù avat.",
     "You have unsaved changes.": "N'ho peus ket enrollet ho kemmoù.",
     "Zoom in": "Zoumañ",
-    "Zoom level for automatic zooms": "Zoom level for automatic zooms",
+    "Zoom level for automatic zooms": "Live ar zoum emgefreek",
     "Zoom out": "Dizoumañ",
-    "Zoom to layer extent": "Zoom to layer extent",
+    "Zoom to layer extent": "Zoumañ evit gwelet ar gwiskad en e bezh",
     "Zoom to the next": "War-lerc'h",
     "Zoom to the previous": "Kent",
-    "Zoom to this feature": "Zoom to this feature",
+    "Zoom to this feature": "Zoumañ war an elfenn-mañ",
     "Zoom to this place": "Zoumañ war al lec'h-mañ",
     "attribution": "attribution",
     "by": "gant",
     "display name": "anv diskwel",
     "height": "uhelder",
     "licence": "aotre-implijout",
     "max East": "bevenn reterañ",
     "max North": "bevenn norzhañ",
     "max South": "bevenn suañ",
     "max West": "bevenn gornôgañ",
-    "max zoom": "max zoom",
-    "min zoom": "min zoom",
+    "max zoom": "zoum brasañ",
+    "min zoom": "zoum bihanañ",
     "next": "war-lerc'h",
     "previous": "kent",
     "width": "ledander",
     "{count} errors during import: {message}": "{count} fazi zo bet en ur enporzhiañ: {message}",
     "Measure distances": "Muzuliañ pellderioù",
-    "NM": "milmor",
+    "NM": "NM",
     "kilometers": "kilometroù",
     "km": "km",
     "mi": "mi",
     "miles": "miltirioù",
-    "nautical miles": "milmor",
+    "nautical miles": "milmorioù",
     "1 day": "1 deiz",
     "1 hour": "1 eur",
     "5 min": "5 min",
     "Cache proxied request": "Cache proxied request",
     "No cache": "No cache",
-    "Popup": "Popup",
-    "Popup (large)": "Popup (large)",
+    "Popup": "Diflugell",
+    "Popup (large)": "Diflugell (vras)",
     "Popup content style": "Popup content style",
-    "Popup shape": "Popup shape",
+    "Popup shape": "Stumm an diflugell",
     "Skipping unknown geometry.type: {type}": "Skipping unknown geometry.type: {type}",
     "Optional.": "Diret.",
     "Paste your data here": "Pegit ho roadennoù amañ",
     "Please save the map first": "Ret eo deoc'h enrollañ ar gartenn da gentañ",
-    "Feature identifier key": "Feature identifier key",
+    "Feature identifier key": "Alc'hwez anaout un elfenn",
     "Open current feature on load": "Open current feature on load",
     "Permalink": "Liamm pad",
     "The name of the property to use as feature unique identifier.": "The name of the property to use as feature unique identifier.",
-    "Advanced filter keys": "Advanced filter keys",
+    "Advanced filter keys": "Alc'hwezioù silañ araokaet",
     "Comma separated list of properties to use for checkbox filtering": "Comma separated list of properties to use for checkbox filtering",
     "Data filters": "Silañ ar roadennoù",
-    "Do you want to display caption menus?": "Do you want to display caption menus?",
+    "Do you want to display caption menus?": "Fellout a ra deoc'h diskwel lañser an alc'hwezioù?",
     "Example: key1,key2,key3": "Skouer: key1,key2,key3",
     "Invalid latitude or longitude": "Hedred pe ledred direizh",
-    "Invalide property name: {name}": "Invalide property name: {name}",
+    "Invalide property name: {name}": "Anv ar perzh direizh: {name}",
     "No results for these filters": "Disoc'h ebet evit ar siloù-mañ",
-    "Permanent credits": "Permanent credits",
+    "Permanent credits": "Kredadoù padus",
     "Permanent credits background": "Permanent credits background",
     "Select data": "Diuzañ ar roadennoù",
-    "Will be permanently visible in the bottom left corner of the map": "Will be permanently visible in the bottom left corner of the map",
+    "Will be permanently visible in the bottom left corner of the map": "Diskwel dalc'hmat e traoñ a-gleiz ar gartenn",
     "{area}&#8239;acres": "{area} erv",
     "{area}&#8239;ha": "{area} ha",
     "{area}&#8239;m&sup2;": "{area} m&sup2;",
     "{area}&#8239;mi&sup2;": "{area} mi&sup2;",
     "{area}&#8239;yd&sup2;": "{area} yd&sup2;",
     "{distance}&#8239;NM": "{distance} NM",
     "{distance}&#8239;km": "{distance} km",
     "{distance}&#8239;m": "{distance} m",
     "{distance}&#8239;miles": "{distance} miltir",
     "{distance}&#8239;yd": "{distance} yd",
     " (area: {measure})": "(gorread: {measure})",
-    " (length: {measure})": "(hirder: {measure})",
-    "Animated transitions": "Animated transitions",
-    "Background overlay url": "Background overlay url",
-    "Custom overlay": "Custom overlay",
+    " (length: {measure})": "(pellder: {measure})",
+    "Animated transitions": "Tremenoù buhezek",
+    "Background overlay url": "URL ar foñs",
+    "Custom overlay": "Gwiskad personelaet",
     "Display the star map button": "Diskouez an afell evit spilhennañ ar gartenn",
-    "Error in the overlay URL": "Error in the overlay URL",
+    "Error in the overlay URL": "URL foñs ar gartenn direizh",
     "Map has been starred": "Spilhennet eo bet ar gartenn",
     "Map has been unstarred": "Dispilhennet eo bet ar gartenn",
     "Opacity": "Demerez",
     "Star this map": "Spilhennañ ar gartenn-mañ",
     "Symbol can be either a unicode character or an URL. You can use feature properties as variables: ex.: with \"http://myserver.org/images/{name}.png\", the {name} variable will be replaced by the \"name\" value of each marker.": "Symbol can be either a unicode character or an URL. You can use feature properties as variables: ex.: with \"http://myserver.org/images/{name}.png\", the {name} variable will be replaced by the \"name\" value of each marker.",
     "Direct link": "Liamm eeun",
-    "Export options": "Ezporzhiañ an dibarzhioù",
+    "Export options": "Dibarzhioù ezporzhiañ",
     "The zoom and center have been modified.": "The zoom and center have been modified.",
     "Congratulations, your map has been created!": "Gourc'hemennoù, ho kartenn zo bet krouet!",
     "Copy link": "Eilañ an ere",
     "Email": "Postel",
-    "Secret edit link copied to clipboard!": "Secret edit link copied to clipboard!",
+    "Secret edit link copied to clipboard!": "Liamm aozañ kuzh eilet er golver!",
     "Send me the link": "Kas al liamm din",
-    "Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:": "Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:",
+    "Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:": "Krouet eo bet ho kartenn! Peogwir n'oc'h ket kevreet, setu al liamm kuzh evit aozañ ar gartenn diwezhatoc'h, diwallit mat anezhañ !",
     "Comma separated list of properties to use for sorting features. To reverse the sort, put a minus sign (-) before. Eg. mykey,-otherkey.": "Comma separated list of properties to use for sorting features. To reverse the sort, put a minus sign (-) before. Eg. mykey,-otherkey.",
-    "Issue reaching that URL (network problem or CORS protection)": "Issue reaching that URL (network problem or CORS protection)",
-    "Toggle edit mode (⇧+Click)": "Toggle edit mode (⇧+Click)",
+    "Issue reaching that URL (network problem or CORS protection)": "Ur fazi ez eus bet en ur gargañ an URL-mañ (kudenn rouedad pe gwarez CORS)",
+    "Toggle edit mode (⇧+Click)": "Gweredekaat ar mod aozañ (⇧+Click)",
     "icon opacity": "Demerez an ikon",
     "*single star for italic*": "*ur steredennig simpl evit italek*",
-    "--- for a horizontal rule": "--- for a horizontal rule",
+    "--- for a horizontal rule": "--- evit ul linenn-disparti a-blaen",
     "The name of the property to use as feature label (eg.: \"nom\"). You can also use properties inside brackets to use more than one or mix with static content (eg.: \"{name} in {place}\")": "The name of the property to use as feature label (eg.: \"nom\"). You can also use properties inside brackets to use more than one or mix with static content (eg.: \"{name} in {place}\")"
 }
 L.registerLocale("br", locale)
 L.setLocale("br")
```

### Comparing `umap_project-1.4.3/umap/static/umap/locale/br.json` & `umap_project-1.4.4/umap/static/umap/locale/br.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8425%*

 * *Differences: {'"Edit feature\'s layer"': "'Kemmañ gwiskad an elfenn'",*

 * * "' (length: {measure})'": "'(pellder: {measure})'",*

 * * "'# one hash for main heading'": "'# un diezenn evit an titl pennañ'",*

 * * "'## two hashes for second heading'": "'## div ziezenn evit an eil titl'",*

 * * "'### three hashes for third heading'": "'### teir diezenn evit an trede titl'",*

 * * "'--- for a horizontal rule'": "'--- evit ul linenn-disparti a-blaen'",*

 * * "'Action not allowed :('": '"N\'oc\'h ket aotreet d\'ober-se :("',*

 * * "'Activate slideshow mode'":  […]*

```diff
@@ -1,393 +1,393 @@
 {
     " (area: {measure})": "(gorread: {measure})",
-    " (length: {measure})": "(hirder: {measure})",
-    "# one hash for main heading": "# one hash for main heading",
-    "## two hashes for second heading": "## two hashes for second heading",
-    "### three hashes for third heading": "### three hashes for third heading",
+    " (length: {measure})": "(pellder: {measure})",
+    "# one hash for main heading": "# un diezenn evit an titl penna\u00f1",
+    "## two hashes for second heading": "## div ziezenn evit an eil titl",
+    "### three hashes for third heading": "### teir diezenn evit an trede titl",
     "**double star for bold**": "**div steredennig evit tevaat**",
     "*single star for italic*": "*ur steredennig simpl evit italek*",
-    "--- for a horizontal rule": "--- for a horizontal rule",
+    "--- for a horizontal rule": "--- evit ul linenn-disparti a-blaen",
     "1 day": "1 deiz",
     "1 hour": "1 eur",
     "5 min": "5 min",
     "A comma separated list of numbers that defines the stroke dash pattern. Ex.: \"5, 10, 15\".": "A comma separated list of numbers that defines the stroke dash pattern. Ex.: \"5, 10, 15\".",
     "About": "Diwar-benn",
-    "Action not allowed :(": "Action not allowed :(",
-    "Activate slideshow mode": "Activate slideshow mode",
+    "Action not allowed :(": "N'oc'h ket aotreet d'ober-se :(",
+    "Activate slideshow mode": "Gweredekaat ar mod diaporama",
     "Add a layer": "Ouzhpenna\u00f1 ur gwiskad",
     "Add a line to the current multi": "Add a line to the current multi",
     "Add a new property": "Ouzhpenna\u00f1 ur perzh nevez",
     "Add a polygon to the current multi": "Add a polygon to the current multi",
     "Add symbol": "Ouzhpenna\u00f1 un arouez",
     "Advanced actions": "Obero\u00f9 araokaet",
-    "Advanced filter keys": "Advanced filter keys",
+    "Advanced filter keys": "Alc'hwezio\u00f9 sila\u00f1 araokaet",
     "Advanced properties": "Perzhio\u00f9 araokaet",
-    "All properties are imported.": "All properties are imported.",
+    "All properties are imported.": "Enporzhiet eo bet an holl berzhio\u00f9.",
     "Allow interactions": "Allow interactions",
     "Allow scroll wheel zoom?": "Aotren ar zoum gant ar rodell?",
-    "An error occured": "Ur fazi zo bet",
-    "Animated transitions": "Animated transitions",
+    "An error occured": "Ur fazi ez eus bet",
+    "Animated transitions": "Tremeno\u00f9 buhezek",
     "Are you sure you want to cancel your changes?": "Ha sur oc'h e faot deoc'h nulla\u00f1 ho kemmo\u00f9?",
-    "Are you sure you want to clone this map and all its datalayers?": "Are you sure you want to clone this map and all its datalayers?",
+    "Are you sure you want to clone this map and all its datalayers?": "Ha sur oc'h e faot deoc'h arredaoli\u00f1 ar gartenn-ma\u00f1 hag he holl wiskado\u00f9 roadenno\u00f9?",
     "Are you sure you want to delete the feature?": "Ha sur oc'h e faot deoc'h dilemel an elfenn-ma\u00f1?",
     "Are you sure you want to delete this layer?": "Ha sur oc'h e faot deoc'h dilemel ar gwiskad-ma\u00f1?",
     "Are you sure you want to delete this map?": "Ha sur oc'h e faot deoc'h dilemel ar gartenn-ma\u00f1?",
     "Are you sure you want to delete this property on all the features?": "Ha sur oc'h a faot deoc'h lemel ar perzh-ma\u00f1 diwar an holl elfenno\u00f9?",
     "Are you sure you want to restore this version?": "Ha sur oc'h e faot deoc'h adsevel ar stumm-ma\u00f1?",
     "Attach the map to my account": "Staga\u00f1 ar gartenn d'am c'hont",
     "Auto": "Auto",
     "Automatic": "Emgefreek",
-    "Autostart when map is loaded": "Autostart when map is loaded",
-    "Background overlay url": "Background overlay url",
-    "Ball": "Ball",
-    "Bring feature to center": "Bring feature to center",
+    "Autostart when map is loaded": "Loc'ha\u00f1 pa vez karget ar gartenn",
+    "Background overlay url": "URL ar fo\u00f1s",
+    "Ball": "Spilhenn",
+    "Bring feature to center": "Kreiza\u00f1 ar gartenn war an elfenn-ma\u00f1",
     "Browse data": "Furchal ar roadenno\u00f9",
     "Cache proxied request": "Cache proxied request",
     "Cancel": "Nulla\u00f1",
     "Cancel edits": "Nulla\u00f1 ar c'hemmo\u00f9",
     "Caption": "Alc'hwez",
-    "Center map on your location": "Center map on your location",
+    "Center map on your location": "Kreiza\u00f1 ar gartenn war al lec'h m'emaoc'h",
     "Change map background": "Che\u00f1ch fo\u00f1s ar gartenn",
     "Change symbol": "Che\u00f1ch arouez",
     "Change tilelayers": "Che\u00f1ch fo\u00f1s ar gartenn",
-    "Choose a preset": "Choose a preset",
+    "Choose a preset": "Diuza\u00f1 ur rakdibab",
     "Choose the data format": "Diuza\u00f1 furmad ar roadenno\u00f9",
-    "Choose the format of the data to import": "Choose the format of the data to import",
-    "Choose the layer of the feature": "Choose the layer of the feature",
-    "Choose the layer to import in": "Choose the layer to import in",
-    "Circle": "Kelc'hia\u00f1",
-    "Click last point to finish shape": "Click last point to finish shape",
+    "Choose the format of the data to import": "Diuza\u00f1 furmad ar roadenno\u00f9 da enporzhia\u00f1",
+    "Choose the layer of the feature": "Diuza\u00f1 gwiskad an elfenn",
+    "Choose the layer to import in": "Diuza\u00f1 ar gwiskad evit enporzhia\u00f1 e-barzh",
+    "Circle": "Kelc'h",
+    "Click last point to finish shape": "Klika\u00f1 war ar poent diwezha\u00f1 evit echui\u00f1 an tres",
     "Click to add a marker": "Klika\u00f1 evit ouzhpenna\u00f1 ur valizenn",
-    "Click to continue drawing": "Click to continue drawing",
+    "Click to continue drawing": "Klika\u00f1 evit kenderc'hel da dresa\u00f1",
     "Click to edit": "Klika\u00f1 evit aoza\u00f1",
     "Click to start drawing a line": "Klika\u00f1 evit tresa\u00f1 ul linenn",
     "Click to start drawing a polygon": "Klika\u00f1 evit tresa\u00f1 ul lieskorn",
     "Clone": "Arredaoli\u00f1",
-    "Clone of {name}": "Clone of {name}",
+    "Clone of {name}": "Eilenn eus {name}",
     "Clone this feature": "Arredaoli\u00f1 an elfenn-ma\u00f1",
     "Clone this map": "Arredaoli\u00f1 ar gartenn-ma\u00f1",
     "Close": "Serri\u00f1",
     "Clustered": "Clustered",
     "Clustering radius": "Clustering radius",
     "Comma separated list of properties to use for checkbox filtering": "Comma separated list of properties to use for checkbox filtering",
     "Comma separated list of properties to use for sorting features. To reverse the sort, put a minus sign (-) before. Eg. mykey,-otherkey.": "Comma separated list of properties to use for sorting features. To reverse the sort, put a minus sign (-) before. Eg. mykey,-otherkey.",
     "Comma separated list of properties to use when filtering features": "Comma separated list of properties to use when filtering features",
     "Comma, tab or semi-colon separated values. SRS WGS84 is implied. Only Point geometries are imported. The import will look at the column headers for any mention of \u00ablat\u00bb and \u00ablon\u00bb at the begining of the header, case insensitive. All other column are imported as properties.": "Comma, tab or semi-colon separated values. SRS WGS84 is implied. Only Point geometries are imported. The import will look at the column headers for any mention of \u00ablat\u00bb and \u00ablon\u00bb at the begining of the header, case insensitive. All other column are imported as properties.",
     "Congratulations, your map has been created!": "Gourc'hemenno\u00f9, ho kartenn zo bet krouet!",
-    "Continue line": "Kenderc'hel al liamm",
+    "Continue line": "Kenderc'hel al linenn",
     "Continue line (Ctrl+Click)": "Kenderc'hel al linenn (Reol+Klika\u00f1)",
     "Coordinates": "Daveenno\u00f9",
     "Copy link": "Eila\u00f1 an ere",
     "Credits": "Kredado\u00f9",
-    "Current view instead of default map view?": "Current view instead of default map view?",
+    "Current view instead of default map view?": "Gwel a-vrema\u00f1 e-lec'h ar gwel dre ziouer?",
     "Custom background": "Fo\u00f1s personelaet",
-    "Custom overlay": "Custom overlay",
+    "Custom overlay": "Gwiskad personelaet",
     "Data browser": "Furchal ar roadenno\u00f9",
     "Data filters": "Sila\u00f1 ar roadenno\u00f9",
-    "Data is browsable": "Data is browsable",
+    "Data is browsable": "Roadenno\u00f9 a c'hall merdei\u00f1",
     "Default": "Dre ziouer",
     "Default interaction options": "Default interaction options",
     "Default properties": "Perzhio\u00f9 dre ziouer",
     "Default shape properties": "Default shape properties",
-    "Default zoom level": "Default zoom level",
+    "Default zoom level": "Live zoum dre ziouer",
     "Default: name": "Dre ziouer: anv",
     "Define link to open in a new window on polygon click.": "Define link to open in a new window on polygon click.",
-    "Delay between two transitions when in play mode": "Delay between two transitions when in play mode",
+    "Delay between two transitions when in play mode": "Dale etre daou dremen pa vez e mod lenn",
     "Delete": "Dilemel",
     "Delete all layers": "Dilemel kement gwiskad",
     "Delete layer": "Dilemel ar gwiskad",
     "Delete this feature": "Dilemel an elfenn-ma\u00f1",
     "Delete this property on all the features": "Dilemel ar perzh-ma\u00f1",
-    "Delete this shape": "Delete this shape",
+    "Delete this shape": "Dilemel an tres-ma\u00f1",
     "Delete this vertex (Alt+Click)": "Dilemel ar poent-ma\u00f1 (Erl+Klik)",
     "Direct link": "Liamm eeun",
-    "Directions from here": "Directions from here",
-    "Disable editing": "Disable editing",
+    "Directions from here": "He\u00f1chadurio\u00f9 adalek ama\u00f1",
+    "Disable editing": "Paouez da aoza\u00f1",
     "Display label": "Diskouez un dikedenn",
     "Display measure": "Diskouez ar muzulio\u00f9",
-    "Display on load": "Display on load",
-    "Display the control to open OpenStreetMap editor": "Display the control to open OpenStreetMap editor",
+    "Display on load": "Diskwel en ur garga\u00f1",
+    "Display the control to open OpenStreetMap editor": "Diskwel an afell evit digeri\u00f1 an aozer OpenStreetMap",
     "Display the data layers control": "Display the data layers control",
-    "Display the embed control": "Display the embed control",
-    "Display the fullscreen control": "Display the fullscreen control",
-    "Display the locate control": "Display the locate control",
+    "Display the embed control": "Diskwel an afell \"enframma\u00f1\"",
+    "Display the fullscreen control": "Diskwel an afell \"skramm a-bezh\"",
+    "Display the locate control": "Diskwel an afell \"lec'hia\u00f1\"",
     "Display the measure control": "Display the measure control",
-    "Display the search control": "Display the search control",
+    "Display the search control": "Diskwel an afell \"klask\"",
     "Display the star map button": "Diskouez an afell evit spilhenna\u00f1 ar gartenn",
-    "Display the tile layers control": "Display the tile layers control",
-    "Display the zoom control": "Display the zoom control",
-    "Do you want to display a caption bar?": "Do you want to display a caption bar?",
-    "Do you want to display a minimap?": "Do you want to display a minimap?",
+    "Display the tile layers control": "Diskwel an afell \"che\u00f1ch fo\u00f1s ar gartenn\"",
+    "Display the zoom control": "Diskwel an afello\u00f9 \"zouma\u00f1\" ha \"dizouma\u00f1\"",
+    "Do you want to display a caption bar?": "Fellout a ra deoc'h diskwel ur varrenn alc'hwez?",
+    "Do you want to display a minimap?": "Fellout a ra deoc'h diskwel ur gartennig evit en em lec'hia\u00f1?",
     "Do you want to display a panel on load?": "Do you want to display a panel on load?",
-    "Do you want to display caption menus?": "Do you want to display caption menus?",
+    "Do you want to display caption menus?": "Fellout a ra deoc'h diskwel la\u00f1ser an alc'hwezio\u00f9?",
     "Do you want to display popup footer?": "Do you want to display popup footer?",
     "Do you want to display the scale control?": "Fellout a ra deoc'h diskouez skeul ar gartenn?",
     "Do you want to display the \u00abmore\u00bb control?": "Fellout a ra deoc'h diskwel an afell \"muioc'h\"?",
     "Download": "Pellgarga\u00f1",
     "Download data": "Pellgarga\u00f1 ar roadenno\u00f9",
-    "Drag to reorder": "Drag to reorder",
+    "Drag to reorder": "Rikla\u00f1 evit adurzhia\u00f1",
     "Draw a line": "Tresa\u00f1 ul linenn",
     "Draw a marker": "Ouzhpenna\u00f1 ur valizenn",
     "Draw a polygon": "Tresa\u00f1 ul lieskorn",
     "Draw a polyline": "Tresa\u00f1 ul linenn",
-    "Drop": "Drop",
-    "Dynamic": "Dynamic",
-    "Dynamic properties": "Dynamic properties",
+    "Drop": "Takenn",
+    "Dynamic": "Buhezek",
+    "Dynamic properties": "Perzhio\u00f9 buhezek",
     "Edit": "Aoza\u00f1",
-    "Edit feature's layer": "Edit feature's layer",
+    "Edit feature's layer": "Kemma\u00f1 gwiskad an elfenn",
     "Edit map properties": "Aoza\u00f1 perzhio\u00f9 ar gartenn",
     "Edit map settings": "Kemma\u00f1 arventenno\u00f9 ar gartenn",
     "Edit properties in a table": "Aoza\u00f1 ar perzhio\u00f9 en un daolenn",
     "Edit this feature": "Kemma\u00f1 an elfenn-ma\u00f1",
     "Editing": "Oc'h aoza\u00f1",
     "Email": "Postel",
     "Embed and share this map": "Ezporzhia\u00f1 ha ranna\u00f1 ar gartenn",
     "Embed the map": "Enframma\u00f1 ar gartenn",
     "Empty": "Goullonderi\u00f1",
-    "Enable editing": "Enable editing",
-    "Error in the overlay URL": "Error in the overlay URL",
-    "Error in the tilelayer URL": "Error in the tilelayer URL",
-    "Error while fetching {url}": "Error while fetching {url}",
+    "Enable editing": "Kregi\u00f1 da aoza\u00f1",
+    "Error in the overlay URL": "URL fo\u00f1s ar gartenn direizh",
+    "Error in the tilelayer URL": "Ur fazi zo en URL fo\u00f1s ar gartenn",
+    "Error while fetching {url}": "Ur fazi ez eus bet en ur c'hervel an URL {url}",
     "Example: key1,key2,key3": "Skouer: key1,key2,key3",
     "Exit Fullscreen": "Kuitaat ar mod skramm a-bezh",
-    "Export options": "Ezporzhia\u00f1 an dibarzhio\u00f9",
+    "Export options": "Dibarzhio\u00f9 ezporzhia\u00f1",
     "Extract shape to separate feature": "Extract shape to separate feature",
-    "Feature identifier key": "Feature identifier key",
+    "Feature identifier key": "Alc'hwez anaout un elfenn",
     "Fetch data each time map view changes.": "Fetch data each time map view changes.",
     "Filter keys": "Filter keys",
     "Filter\u2026": "Sila\u00f1...",
     "Format": "Furmad",
-    "From zoom": "From zoom",
+    "From zoom": "Adalek ar zoum",
     "Full map data": "Roadenno\u00f9 klok ar gartenn",
-    "GeoRSS (only link)": "GeoRSS (only link)",
+    "GeoRSS (only link)": "GeoRSS (liamm hepken)",
     "GeoRSS (title + image)": "GeoRSS (titl + skeudenn)",
     "Go to \u00ab{feature}\u00bb": "Mont da \u00ab{feature}\u00bb",
     "Heatmap": "Heatmap",
     "Heatmap intensity property": "Heatmap intensity property",
     "Heatmap radius": "Heatmap radius",
     "Help": "Skoazell",
-    "Hide controls": "Hide controls",
+    "Hide controls": "Kuzhat ar binvio\u00f9",
     "Home": "Degemer",
     "How much to simplify the polyline on each zoom level (more = better performance and smoother look, less = more accurate)": "How much to simplify the polyline on each zoom level (more = better performance and smoother look, less = more accurate)",
     "Icon shape": "Furm an ikon",
     "Icon symbol": "Arouez an ikon",
     "If false, the polygon will act as a part of the underlying map.": "If false, the polygon will act as a part of the underlying map.",
-    "Iframe with custom height (in px): {{{http://iframe.url.com|height}}}": "Iframe with custom height (in px): {{{http://iframe.url.com|height}}}",
-    "Iframe with custom height and width (in px): {{{http://iframe.url.com|height*width}}}": "Iframe with custom height and width (in px): {{{http://iframe.url.com|height*width}}}",
+    "Iframe with custom height (in px): {{{http://iframe.url.com|height}}}": "Iframe gant uhelder personelaet (e pikselio\u00f9): {{{http://iframe.url.com|height}}}",
+    "Iframe with custom height and width (in px): {{{http://iframe.url.com|height*width}}}": "Iframe gant mento\u00f9 personelaet (e pikselio\u00f9): {{{http://iframe.url.com|height*width}}}",
     "Iframe: {{{http://iframe.url.com}}}": "Iframe: {{{http://iframe.url.com}}}",
-    "Image with custom width (in px): {{http://image.url.com|width}}": "Image with custom width (in px): {{http://image.url.com|width}}",
+    "Image with custom width (in px): {{http://image.url.com|width}}": "Skeudenn gant ledander personelaet (e pikselio\u00f9): {{http://image.url.com|width}}",
     "Image: {{http://image.url.com}}": "Skeudenn: {{http://image.url.com}}",
     "Import": "Enporzhia\u00f1",
     "Import data": "Enporzhia\u00f1 roadenno\u00f9",
     "Import in a new layer": "Enporzhia\u00f1 ur gwiskad nevez",
-    "Imports all umap data, including layers and settings.": "Imports all umap data, including layers and settings.",
-    "Include full screen link?": "Include full screen link?",
-    "Inherit": "Inherit",
+    "Imports all umap data, including layers and settings.": "Enporzhia\u00f1 an holl roadenno\u00f9 ar gartenn, ar gwiskado\u00f9 hag an arventenno\u00f9 en o zouez.",
+    "Include full screen link?": "Lakaat ul liamm \"skramm a-bezh\" e-barzh?",
+    "Inherit": "Herita\u00f1",
     "Interaction options": "Interaction options",
     "Invalid latitude or longitude": "Hedred pe ledred direizh",
     "Invalid umap data": "Roadenno\u00f9 umap direizh",
     "Invalid umap data in {filename}": "Roadenno\u00f9 umap direizh e-barzh {filename}",
-    "Invalide property name: {name}": "Invalide property name: {name}",
-    "Issue reaching that URL (network problem or CORS protection)": "Issue reaching that URL (network problem or CORS protection)",
-    "Keep current visible layers": "Keep current visible layers",
+    "Invalide property name: {name}": "Anv ar perzh direizh: {name}",
+    "Issue reaching that URL (network problem or CORS protection)": "Ur fazi ez eus bet en ur garga\u00f1 an URL-ma\u00f1 (kudenn rouedad pe gwarez CORS)",
+    "Keep current visible layers": "Derc'hel ar gwiskado\u00f9 a c'haller gwelet brema\u00f1",
     "Label direction": "Durc'hadur an dikedenn",
     "Label key": "Label key",
-    "Labels are clickable": "Labels are clickable",
+    "Labels are clickable": "An dikedenno\u00f9 a c'haller klika\u00f1",
     "Latitude": "Ledred",
     "Layer": "Gwiskad",
     "Layer properties": "Perzhio\u00f9 ar gwiskad",
     "Licence": "Aotre-implijout",
-    "Limit bounds": "Limit bounds",
+    "Limit bounds": "Bevenno\u00f9 geografek",
     "Link to\u2026": "Liamm etrezek...",
     "Link with text: [[http://example.com|text of the link]]": "Liamm gant testenn: [[http://skouer.bzh|testenn al liamm]]",
     "Long credits": "Kredado\u00f9 hir",
     "Longitude": "Hedred",
-    "Make main shape": "Make main shape",
+    "Make main shape": "Tres penna\u00f1",
     "Manage layers": "Mera\u00f1 ar gwiskado\u00f9",
-    "Map background credits": "Map background credits",
+    "Map background credits": "Kredado\u00f9 fo\u00f1s ar gartenn",
     "Map has been attached to your account": "Staget eo bet ar gartenn d'ho kont",
-    "Map has been saved!": "Enrollet eo bet ar gartenn",
+    "Map has been saved!": "Enrollet eo bet ar gartenn!",
     "Map has been starred": "Spilhennet eo bet ar gartenn",
     "Map has been unstarred": "Dispilhennet eo bet ar gartenn",
-    "Map user content has been published under licence": "Map user content has been published under licence",
+    "Map user content has been published under licence": "Endalc'had ar gartenn zo bet embannet gant an aotre-implijout",
     "Map's editors": "Aozerien ar gartenn",
     "Map's owner": "Perc'henner ar gartenn",
     "Measure distances": "Muzulia\u00f1 pellderio\u00f9",
     "Merge lines": "Kendeuzi\u00f1 al linenno\u00f9",
     "More controls": "Binvio\u00f9 all",
     "Must be a valid CSS value (eg.: DarkBlue or #123456)": "Rankout a ra beza\u00f1 un talvoud CSS reizh (da sk.: DarkBlue pe #123456)",
-    "NM": "milmor",
+    "NM": "NM",
     "No cache": "No cache",
     "No licence has been set": "Aotre-implijout ebet bet termenet",
     "No results": "Disoc'h ebet",
     "No results for these filters": "Disoc'h ebet evit ar silo\u00f9-ma\u00f1",
     "None": "Hini ebet",
     "On the bottom": "D'an trao\u00f1",
     "On the left": "A-gleiz",
     "On the right": "A-zeho\u00f9",
     "On the top": "D'an nec'h",
     "Only visible features will be downloaded.": "An elfenno\u00f9 hewel hepken a vo pellgarget.",
     "Opacity": "Demerez",
     "Open current feature on load": "Open current feature on load",
-    "Open download panel": "Open download panel",
+    "Open download panel": "Digeri\u00f1 prenestr ar pellgargadurio\u00f9",
     "Open link in\u2026": "Digeri\u00f1 al liamm e...",
     "Open this map extent in a map editor to provide more accurate data to OpenStreetMap": "Open this map extent in a map editor to provide more accurate data to OpenStreetMap",
     "Optional intensity property for heatmap": "Optional intensity property for heatmap",
     "Optional.": "Diret.",
-    "Optional. Same as color if not set.": "Optional. Same as color if not set.",
+    "Optional. Same as color if not set.": "Diret. Al liv penna\u00f1 a vo implijet ma ne vez ket termenet.",
     "Override clustering radius (default 80)": "Override clustering radius (default 80)",
     "Override heatmap radius (default 25)": "Override heatmap radius (default 25)",
     "Paste your data here": "Pegit ho roadenno\u00f9 ama\u00f1",
     "Permalink": "Liamm pad",
-    "Permanent credits": "Permanent credits",
+    "Permanent credits": "Kredado\u00f9 padus",
     "Permanent credits background": "Permanent credits background",
-    "Please be sure the licence is compliant with your use.": "Please be sure the licence is compliant with your use.",
+    "Please be sure the licence is compliant with your use.": "Gwiriit m'az oc'h aotreet da implijout ar roadenno\u00f9-ma\u00f1 mar plij.",
     "Please choose a format": "Diuzit ur furmad mar plij",
-    "Please enter the name of the property": "Please enter the name of the property",
-    "Please enter the new name of this property": "Please enter the new name of this property",
+    "Please enter the name of the property": "Enankit anv ar perzh mar plij",
+    "Please enter the new name of this property": "Enankit anv nevez ar perzh-ma\u00f1 mar plij",
     "Please save the map first": "Ret eo deoc'h enrolla\u00f1 ar gartenn da genta\u00f1",
-    "Popup": "Popup",
-    "Popup (large)": "Popup (large)",
+    "Popup": "Diflugell",
+    "Popup (large)": "Diflugell (vras)",
     "Popup content style": "Popup content style",
     "Popup content template": "Popup content template",
-    "Popup shape": "Popup shape",
-    "Problem in the response": "Problem in the response",
-    "Problem in the response format": "Problem in the response format",
-    "Properties imported:": "Properties imported:",
-    "Provide an URL here": "Provide an URL here",
-    "Proxy request": "Proxy request",
-    "Remote data": "Remote data",
+    "Popup shape": "Stumm an diflugell",
+    "Problem in the response": "Kudenn e respont ar servijer",
+    "Problem in the response format": "Kudenn gant furmadi\u00f1 ar respont",
+    "Properties imported:": "Perzhio\u00f9 enporzhiet:",
+    "Provide an URL here": "Pourchas un URL ama\u00f1",
+    "Proxy request": "Reked proksi",
+    "Remote data": "Rouedado\u00f9 a-bell",
     "Remove shape from the multi": "Remove shape from the multi",
     "Rename this property on all the features": "Adenvel ar perzh-ma\u00f1",
-    "Replace layer content": "Replace layer content",
+    "Replace layer content": "Erlec'hia\u00f1 endalc'had ar gwiskad",
     "Restore this version": "Adsevel ar stumm-ma\u00f1?",
     "Save": "Enrolla\u00f1",
     "Save anyway": "Enrolla\u00f1 evelkent",
-    "Save current edits": "Save current edits",
+    "Save current edits": "Enrolla\u00f1 ar c'hemmo\u00f9 a-vrema\u00f1 ",
     "Save this center and zoom": "Save this center and zoom",
-    "Save this location as new feature": "Save this location as new feature",
+    "Save this location as new feature": "Enrolla\u00f1 al lec'h-ma\u00f1 evel un elfenn nevez",
     "Search a place name": "Klask un anv-lec'h ",
-    "Search location": "Search location",
-    "Secret edit link copied to clipboard!": "Secret edit link copied to clipboard!",
-    "Secret edit link is:<br>{link}": "Secret edit link is:<br>{link}",
+    "Search location": "Klask ul lec'h",
+    "Secret edit link copied to clipboard!": "Liamm aoza\u00f1 kuzh eilet er golver!",
+    "Secret edit link is:<br>{link}": "Liamm aoza\u00f1 kuzh:<br>{link}",
     "See all": "Gwelet pep tra",
     "See data layers": "Diskouez ar gwiskado\u00f9",
     "See full screen": "Gwelet e skramm a-bezh",
     "Select data": "Diuza\u00f1 ar roadenno\u00f9",
     "Send me the link": "Kas al liamm din",
-    "Set it to false to hide this layer from the slideshow, the data browser, the popup navigation\u2026": "Set it to false to hide this layer from the slideshow, the data browser, the popup navigation\u2026",
+    "Set it to false to hide this layer from the slideshow, the data browser, the popup navigation\u2026": "Diweredekaat evit kuzhat ar gwiskad-ma\u00f1 ouzh an diaporama, ar merdeer roadenno\u00f9...",
     "Set symbol": "Termena\u00f1 an arouez",
-    "Shape properties": "Shape properties",
+    "Shape properties": "Perzhio\u00f9 ar furm",
     "Short URL": "URL berr",
     "Short credits": "Kredado\u00f9 berr",
     "Show/hide layer": "Diskouez/kuzhat ar gwiskad",
     "Side panel": "Panell gostez",
     "Simple link: [[http://example.com]]": "Liamm eeun: [[http://skouer.bzh]]",
-    "Simplify": "Simplify",
+    "Simplify": "Eeunaat",
     "Skipping unknown geometry.type: {type}": "Skipping unknown geometry.type: {type}",
     "Slideshow": "Diaporama",
     "Sort key": "Sort key",
     "Split line": "Disranna\u00f1 al linenn",
     "Star this map": "Spilhenna\u00f1 ar gartenn-ma\u00f1",
     "Start a hole here": "Ouzhpenna\u00f1 un toull e-barzh",
     "Start editing": "Kregi\u00f1 da aoza\u00f1",
     "Start slideshow": "Lenn",
     "Stop editing": "Paouez da aoza\u00f1",
     "Stop slideshow": "Ehan",
-    "Supported scheme": "Supported scheme",
+    "Supported scheme": "Steu\u00f1v skoret",
     "Supported variables that will be dynamically replaced": "Supported variables that will be dynamically replaced",
     "Symbol can be either a unicode character or an URL. You can use feature properties as variables: ex.: with \"http://myserver.org/images/{name}.png\", the {name} variable will be replaced by the \"name\" value of each marker.": "Symbol can be either a unicode character or an URL. You can use feature properties as variables: ex.: with \"http://myserver.org/images/{name}.png\", the {name} variable will be replaced by the \"name\" value of each marker.",
     "Symbol or url": "Arouez pe URL",
     "TMS format": "Furmad TMS",
     "Table": "Taolenn",
     "Text color for the cluster label": "Text color for the cluster label",
     "Text formatting": "Furmaoza\u00f1 an destenn",
     "The name of the property to use as feature label (eg.: \"nom\"). You can also use properties inside brackets to use more than one or mix with static content (eg.: \"{name} in {place}\")": "The name of the property to use as feature label (eg.: \"nom\"). You can also use properties inside brackets to use more than one or mix with static content (eg.: \"{name} in {place}\")",
     "The name of the property to use as feature unique identifier.": "The name of the property to use as feature unique identifier.",
     "The zoom and center have been modified.": "The zoom and center have been modified.",
     "To use if remote server doesn't allow cross domain (slower)": "To use if remote server doesn't allow cross domain (slower)",
-    "To zoom": "To zoom",
-    "Toggle edit mode (\u21e7+Click)": "Toggle edit mode (\u21e7+Click)",
+    "To zoom": "Betek ar zoum",
+    "Toggle edit mode (\u21e7+Click)": "Gweredekaat ar mod aoza\u00f1 (\u21e7+Click)",
     "Transfer shape to edited feature": "Transfer shape to edited feature",
-    "Transform to lines": "Transform to lines",
-    "Transform to polygon": "Transform to polygon",
+    "Transform to lines": "Trei\u00f1 da linenno\u00f9",
+    "Transform to polygon": "Trei\u00f1 d'ul lieskorn",
     "Type of layer": "Seurt ar gwiskad",
     "Unable to detect format of file {filename}": "N'haller ket anavezout furmad ar restr {filename}",
     "Untitled layer": "Gwiskad dizanv",
     "Untitled map": "Kartenn dizanv",
     "Update permissions": "Kemma\u00f1 an aotreo\u00f9",
     "Update permissions and editors": "Kemma\u00f1 an aotreo\u00f9 hag an aozerien",
-    "Url": "Url",
-    "Use current bounds": "Use current bounds",
+    "Url": "URL",
+    "Use current bounds": "Implij ar gwel a-vrema\u00f1",
     "Use placeholders with feature properties between brackets, eg. &#123;name&#125;, they will be dynamically replaced by the corresponding values.": "Use placeholders with feature properties between brackets, eg. &#123;name&#125;, they will be dynamically replaced by the corresponding values.",
-    "User content credits": "User content credits",
+    "User content credits": "Kredado\u00f9 evit danvez an implijer",
     "User interface options": "Dibarzhio\u00f9 etrefas an implijer",
     "Versions": "Stummo\u00f9",
     "View Fullscreen": "Mont e mod skramm a-bezh",
-    "Where do we go from here?": "Where do we go from here?",
-    "Whether to display or not polygons paths.": "Whether to display or not polygons paths.",
-    "Whether to fill polygons with color.": "Whether to fill polygons with color.",
+    "Where do we go from here?": "Dre belec'h ez eomp adalek ama\u00f1?",
+    "Whether to display or not polygons paths.": "Diskouez trolinenno\u00f9 al lieskorno\u00f9",
+    "Whether to fill polygons with color.": "Leunia\u00f1 al lieskorno\u00f9 gant liv",
     "Who can edit": "Piv a c'hall aoza\u00f1",
     "Who can view": "Piv a c'hall gwelet",
-    "Will be displayed in the bottom right corner of the map": "Will be displayed in the bottom right corner of the map",
-    "Will be permanently visible in the bottom left corner of the map": "Will be permanently visible in the bottom left corner of the map",
-    "Will be visible in the caption of the map": "Will be visible in the caption of the map",
+    "Will be displayed in the bottom right corner of the map": "Diskwelet e vo e trao\u00f1 a-zeho\u00f9 ar gartenn",
+    "Will be permanently visible in the bottom left corner of the map": "Diskwel dalc'hmat e trao\u00f1 a-gleiz ar gartenn",
+    "Will be visible in the caption of the map": "Gwelus e vo en alc'hwez ar gartenn",
     "Woops! Someone else seems to have edited the data. You can save anyway, but this will erase the changes made by others.": "Chaous! Seblant a ra ez eus bet kemmet ar gartenn gant unan bennak all. Gallout a rit enrolla\u00f1 koulskoude, kollet e vo e roadenno\u00f9 avat.",
     "You have unsaved changes.": "N'ho peus ket enrollet ho kemmo\u00f9.",
-    "Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:": "Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:",
+    "Your map has been created! As you are not logged in, here is your secret link to edit the map, please keep it safe:": "Krouet eo bet ho kartenn! Peogwir n'oc'h ket kevreet, setu al liamm kuzh evit aoza\u00f1 ar gartenn diwezhatoc'h, diwallit mat anezha\u00f1 !",
     "Zoom in": "Zouma\u00f1",
-    "Zoom level for automatic zooms": "Zoom level for automatic zooms",
+    "Zoom level for automatic zooms": "Live ar zoum emgefreek",
     "Zoom out": "Dizouma\u00f1",
-    "Zoom to layer extent": "Zoom to layer extent",
+    "Zoom to layer extent": "Zouma\u00f1 evit gwelet ar gwiskad en e bezh",
     "Zoom to the next": "War-lerc'h",
     "Zoom to the previous": "Kent",
-    "Zoom to this feature": "Zoom to this feature",
+    "Zoom to this feature": "Zouma\u00f1 war an elfenn-ma\u00f1",
     "Zoom to this place": "Zouma\u00f1 war al lec'h-ma\u00f1",
     "always": "bepred",
     "attribution": "attribution",
     "by": "gant",
     "clear": "skarzha\u00f1",
-    "collapsed": "collapsed",
+    "collapsed": "serret",
     "color": "liv",
-    "dash array": "dash array",
+    "dash array": "Barrenno\u00f9igo\u00f9",
     "define": "termena\u00f1",
     "description": "deskrivadur",
     "display name": "anv diskwel",
-    "expanded": "expanded",
+    "expanded": "digor",
     "fill": "leunia\u00f1",
     "fill color": "liv leunia\u00f1",
-    "fill opacity": "fill opacity",
+    "fill opacity": "demerez al leunia\u00f1",
     "height": "uhelder",
     "hidden": "kuzhet",
     "icon opacity": "Demerez an ikon",
     "iframe": "iframe",
-    "inherit": "inherit",
+    "inherit": "herita\u00f1",
     "kilometers": "kilometro\u00f9",
     "km": "km",
     "licence": "aotre-implijout",
     "max East": "bevenn retera\u00f1",
     "max North": "bevenn norzha\u00f1",
     "max South": "bevenn sua\u00f1",
     "max West": "bevenn gorn\u00f4ga\u00f1",
-    "max zoom": "max zoom",
+    "max zoom": "zoum brasa\u00f1",
     "mi": "mi",
     "miles": "miltirio\u00f9",
-    "min zoom": "min zoom",
+    "min zoom": "zoum bihana\u00f1",
     "name": "anv",
-    "nautical miles": "milmor",
+    "nautical miles": "milmorio\u00f9",
     "never": "morse",
     "new window": "prenestr nevez",
     "next": "war-lerc'h",
     "no": "ket",
     "on hover": "on hover",
     "opacity": "demerez",
     "parent window": "prenestr kar",
     "previous": "kent",
-    "stroke": "stroke",
+    "stroke": "tres",
     "weight": "tevder",
     "width": "ledander",
     "yes": "ya",
     "{area}&#8239;acres": "{area} erv",
     "{area}&#8239;ha": "{area} ha",
     "{area}&#8239;m&sup2;": "{area} m&sup2;",
     "{area}&#8239;mi&sup2;": "{area} mi&sup2;",
```

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ca.js` & `umap_project-1.4.4/umap/static/umap/locale/ca.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ca.json` & `umap_project-1.4.4/umap/static/umap/locale/ca.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/cs_CZ.js` & `umap_project-1.4.4/umap/static/umap/locale/cs_CZ.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/cs_CZ.json` & `umap_project-1.4.4/umap/static/umap/locale/cs_CZ.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/da.js` & `umap_project-1.4.4/umap/static/umap/locale/da.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/da.json` & `umap_project-1.4.4/umap/static/umap/locale/da.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/de.js` & `umap_project-1.4.4/umap/static/umap/locale/de.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/de.json` & `umap_project-1.4.4/umap/static/umap/locale/de.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/el.js` & `umap_project-1.4.4/umap/static/umap/locale/el.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/el.json` & `umap_project-1.4.4/umap/static/umap/locale/el.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/en.js` & `umap_project-1.4.4/umap/static/umap/locale/en.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/en.json` & `umap_project-1.4.4/umap/static/umap/locale/en.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/en_US.json` & `umap_project-1.4.4/umap/static/umap/locale/en_US.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/es.js` & `umap_project-1.4.4/umap/static/umap/locale/es.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/es.json` & `umap_project-1.4.4/umap/static/umap/locale/es.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/et.js` & `umap_project-1.4.4/umap/static/umap/locale/et.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/et.json` & `umap_project-1.4.4/umap/static/umap/locale/et.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/eu.js` & `umap_project-1.4.4/umap/static/umap/locale/eu.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/eu.json` & `umap_project-1.4.4/umap/static/umap/locale/eu.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/fa_IR.js` & `umap_project-1.4.4/umap/static/umap/locale/fa_IR.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/fa_IR.json` & `umap_project-1.4.4/umap/static/umap/locale/fa_IR.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/fi.js` & `umap_project-1.4.4/umap/static/umap/locale/fi.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/fi.json` & `umap_project-1.4.4/umap/static/umap/locale/fi.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/fr.js` & `umap_project-1.4.4/umap/static/umap/locale/fr.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/fr.json` & `umap_project-1.4.4/umap/static/umap/locale/fr.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/gl.js` & `umap_project-1.4.4/umap/static/umap/locale/gl.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/gl.json` & `umap_project-1.4.4/umap/static/umap/locale/gl.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/he.js` & `umap_project-1.4.4/umap/static/umap/locale/he.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/he.json` & `umap_project-1.4.4/umap/static/umap/locale/he.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/hr.js` & `umap_project-1.4.4/umap/static/umap/locale/hr.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/hr.json` & `umap_project-1.4.4/umap/static/umap/locale/hr.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/hu.js` & `umap_project-1.4.4/umap/static/umap/locale/hu.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/hu.json` & `umap_project-1.4.4/umap/static/umap/locale/hu.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/id.js` & `umap_project-1.4.4/umap/static/umap/locale/id.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/id.json` & `umap_project-1.4.4/umap/static/umap/locale/id.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/is.js` & `umap_project-1.4.4/umap/static/umap/locale/is.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/is.json` & `umap_project-1.4.4/umap/static/umap/locale/is.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/it.js` & `umap_project-1.4.4/umap/static/umap/locale/it.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/it.json` & `umap_project-1.4.4/umap/static/umap/locale/it.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ja.js` & `umap_project-1.4.4/umap/static/umap/locale/ja.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ja.json` & `umap_project-1.4.4/umap/static/umap/locale/ja.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ko.js` & `umap_project-1.4.4/umap/static/umap/locale/ko.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ko.json` & `umap_project-1.4.4/umap/static/umap/locale/ko.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/lt.js` & `umap_project-1.4.4/umap/static/umap/locale/lt.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/lt.json` & `umap_project-1.4.4/umap/static/umap/locale/lt.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ms.js` & `umap_project-1.4.4/umap/static/umap/locale/ms.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ms.json` & `umap_project-1.4.4/umap/static/umap/locale/ms.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/nl.js` & `umap_project-1.4.4/umap/static/umap/locale/nl.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/nl.json` & `umap_project-1.4.4/umap/static/umap/locale/nl.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/no.js` & `umap_project-1.4.4/umap/static/umap/locale/no.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/no.json` & `umap_project-1.4.4/umap/static/umap/locale/no.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pl.js` & `umap_project-1.4.4/umap/static/umap/locale/pl.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pl.json` & `umap_project-1.4.4/umap/static/umap/locale/pl.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pl_PL.json` & `umap_project-1.4.4/umap/static/umap/locale/pl_PL.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pt.js` & `umap_project-1.4.4/umap/static/umap/locale/pt.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pt.json` & `umap_project-1.4.4/umap/static/umap/locale/pt.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pt_BR.js` & `umap_project-1.4.4/umap/static/umap/locale/pt_BR.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pt_BR.json` & `umap_project-1.4.4/umap/static/umap/locale/pt_BR.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pt_PT.js` & `umap_project-1.4.4/umap/static/umap/locale/pt_PT.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/pt_PT.json` & `umap_project-1.4.4/umap/static/umap/locale/pt_PT.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ro.js` & `umap_project-1.4.4/umap/static/umap/locale/ro.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ro.json` & `umap_project-1.4.4/umap/static/umap/locale/ro.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ru.js` & `umap_project-1.4.4/umap/static/umap/locale/ru.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/ru.json` & `umap_project-1.4.4/umap/static/umap/locale/ru.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/si.js` & `umap_project-1.4.4/umap/static/umap/locale/si.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/si.json` & `umap_project-1.4.4/umap/static/umap/locale/si.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sk_SK.js` & `umap_project-1.4.4/umap/static/umap/locale/sk_SK.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sk_SK.json` & `umap_project-1.4.4/umap/static/umap/locale/sk_SK.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sl.js` & `umap_project-1.4.4/umap/static/umap/locale/sl.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sl.json` & `umap_project-1.4.4/umap/static/umap/locale/sl.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sr.js` & `umap_project-1.4.4/umap/static/umap/locale/sr.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sr.json` & `umap_project-1.4.4/umap/static/umap/locale/sr.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sv.js` & `umap_project-1.4.4/umap/static/umap/locale/sv.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/sv.json` & `umap_project-1.4.4/umap/static/umap/locale/sv.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/th_TH.js` & `umap_project-1.4.4/umap/static/umap/locale/th_TH.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/th_TH.json` & `umap_project-1.4.4/umap/static/umap/locale/th_TH.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/tr.js` & `umap_project-1.4.4/umap/static/umap/locale/tr.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/tr.json` & `umap_project-1.4.4/umap/static/umap/locale/tr.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/uk_UA.js` & `umap_project-1.4.4/umap/static/umap/locale/uk_UA.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/uk_UA.json` & `umap_project-1.4.4/umap/static/umap/locale/uk_UA.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/vi.js` & `umap_project-1.4.4/umap/static/umap/locale/vi.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/vi.json` & `umap_project-1.4.4/umap/static/umap/locale/vi.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/vi_VN.json` & `umap_project-1.4.4/umap/static/umap/locale/vi_VN.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/zh.js` & `umap_project-1.4.4/umap/static/umap/locale/zh.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/zh.json` & `umap_project-1.4.4/umap/static/umap/locale/zh.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/zh_CN.json` & `umap_project-1.4.4/umap/static/umap/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/zh_TW.Big5.json` & `umap_project-1.4.4/umap/static/umap/locale/zh_TW.Big5.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/zh_TW.js` & `umap_project-1.4.4/umap/static/umap/locale/zh_TW.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/locale/zh_TW.json` & `umap_project-1.4.4/umap/static/umap/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Controls.js` & `umap_project-1.4.4/umap/static/umap/test/Controls.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/DataLayer.js` & `umap_project-1.4.4/umap/static/umap/test/DataLayer.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Feature.js` & `umap_project-1.4.4/umap/static/umap/test/Feature.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Map.js` & `umap_project-1.4.4/umap/static/umap/test/Map.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Marker.js` & `umap_project-1.4.4/umap/static/umap/test/Marker.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Permissions.js` & `umap_project-1.4.4/umap/static/umap/test/Permissions.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -46,15 +46,15 @@
         })
     })
 
     describe('#editor', function() {
         var button
 
         it('should only allow editors', function() {
-            this.map.options.permissions.owner = {
+            this.map.permissions.options.owner = {
                 id: 1,
                 url: '/url',
                 name: 'jojo'
             }
             button = qs('a.update-map-permissions')
             happen.click(button)
             expect(qs('select[name="edit_status"]')).not.to.be.ok
@@ -64,15 +64,15 @@
         })
     })
 
     describe('#owner', function() {
         var button
 
         it('should allow everything', function() {
-            this.map.options.permissions.owner = {
+            this.map.permissions.options.owner = {
                 id: 1,
                 url: '/url',
                 name: 'jojo'
             }
             this.map.options.user = {
                 id: 1,
                 url: '/url',
```

### Comparing `umap_project-1.4.3/umap/static/umap/test/Polygon.js` & `umap_project-1.4.4/umap/static/umap/test/Polygon.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Polyline.js` & `umap_project-1.4.4/umap/static/umap/test/Polyline.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/TableEditor.js` & `umap_project-1.4.4/umap/static/umap/test/TableEditor.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/Util.js` & `umap_project-1.4.4/umap/static/umap/test/Util.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -249,14 +249,33 @@
                 L.Util.greedyTemplate('A phrase with a {@variable}.', {
                     '@variable': 'value',
                 }),
                 'A phrase with a value.'
             )
         })
 
+        it('should accept space', function() {
+            assert.equal(
+                L.Util.greedyTemplate('A phrase with a {var iable}.', {
+                    'var iable': 'value',
+                }),
+                'A phrase with a value.'
+            )
+        })
+
+        it('should accept non ascii chars', function() {
+            assert.equal(
+                L.Util.greedyTemplate('A phrase with a {Accessibilité} and {переменная}.', {
+                    'Accessibilité': 'value',
+                    'переменная': 'another',
+                }),
+                'A phrase with a value and another.'
+            )
+        })
+
         it('should replace even with ignore if key is found', function() {
             assert.equal(
                 L.Util.greedyTemplate(
                     'A phrase with a {variable:fr}.', {
                         'variable:fr': 'value'
                     },
                     true
```

### Comparing `umap_project-1.4.3/umap/static/umap/test/_pre.js` & `umap_project-1.4.4/umap/static/umap/test/_pre.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/test/index.html` & `umap_project-1.4.4/umap/static/umap/test/index.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/choropleth/choropleth.js` & `umap_project-1.4.4/umap/static/umap/vendors/choropleth/choropleth.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/chroma/chroma.min.js` & `umap_project-1.4.4/umap/static/umap/vendors/chroma/chroma.min.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css` & `umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js` & `umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css` & `umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js` & `umap_project-1.4.4/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/csv2geojson/csv2geojson.js` & `umap_project-1.4.4/umap/static/umap/vendors/csv2geojson/csv2geojson.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/csv2geojson/index.js` & `umap_project-1.4.4/umap/static/umap/vendors/csv2geojson/index.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/dompurify/purify.js` & `umap_project-1.4.4/umap/static/umap/vendors/dompurify/purify.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/editable/Leaflet.Editable.js` & `umap_project-1.4.4/umap/static/umap/vendors/editable/Leaflet.Editable.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/editable/Path.Drag.js` & `umap_project-1.4.4/umap/static/umap/vendors/editable/Path.Drag.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css` & `umap_project-1.4.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js` & `umap_project-1.4.4/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/editinosm/edit-in-osm.png` & `umap_project-1.4.4/umap/static/umap/vendors/editinosm/edit-in-osm.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js` & `umap_project-1.4.4/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js` & `umap_project-1.4.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js` & `umap_project-1.4.4/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css` & `umap_project-1.4.4/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js` & `umap_project-1.4.4/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/hash/leaflet-hash.js` & `umap_project-1.4.4/umap/static/umap/vendors/hash/leaflet-hash.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/heat/leaflet-heat.js` & `umap_project-1.4.4/umap/static/umap/vendors/heat/leaflet-heat.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/i18n/Leaflet.i18n.js` & `umap_project-1.4.4/umap/static/umap/vendors/i18n/Leaflet.i18n.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.esm.js` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.js` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet-src.js.map` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet.css` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet.js` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/leaflet.js.map` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/layers-2x.png` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/layers.png` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/marker-icon.png` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/leaflet/images/marker-shadow.png` & `umap_project-1.4.4/umap/static/umap/vendors/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/loading/Control.Loading.css` & `umap_project-1.4.4/umap/static/umap/vendors/loading/Control.Loading.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/loading/Control.Loading.js` & `umap_project-1.4.4/umap/static/umap/vendors/loading/Control.Loading.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css` & `umap_project-1.4.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js` & `umap_project-1.4.4/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css` & `umap_project-1.4.4/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/markercluster/MarkerCluster.css` & `umap_project-1.4.4/umap/static/umap/vendors/markercluster/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js` & `umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map` & `umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster.js` & `umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map` & `umap_project-1.4.4/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/measurable/Leaflet.Measurable.css` & `umap_project-1.4.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/measurable/Leaflet.Measurable.js` & `umap_project-1.4.4/umap/static/umap/vendors/measurable/Leaflet.Measurable.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/minimap/Control.MiniMap.css` & `umap_project-1.4.4/umap/static/umap/vendors/minimap/Control.MiniMap.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/minimap/Control.MiniMap.js` & `umap_project-1.4.4/umap/static/umap/vendors/minimap/Control.MiniMap.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/minimap/images/toggle.svg` & `umap_project-1.4.4/umap/static/umap/vendors/minimap/images/toggle.svg`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js` & `umap_project-1.4.4/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/photon/leaflet.photon.js` & `umap_project-1.4.4/umap/static/umap/vendors/photon/leaflet.photon.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/print/leaflet.browser.print.js` & `umap_project-1.4.4/umap/static/umap/vendors/print/leaflet.browser.print.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/print/leaflet.browser.print.min.js` & `umap_project-1.4.4/umap/static/umap/vendors/print/leaflet.browser.print.min.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/togeojson/togeojson.js` & `umap_project-1.4.4/umap/static/umap/vendors/togeojson/togeojson.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/togpx/togpx.js` & `umap_project-1.4.4/umap/static/umap/vendors/togpx/togpx.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/tokml/tokml.js` & `umap_project-1.4.4/umap/static/umap/vendors/tokml/tokml.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css` & `umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js` & `umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar.css` & `umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.css`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/static/umap/vendors/toolbar/leaflet.toolbar.js` & `umap_project-1.4.4/umap/static/umap/vendors/toolbar/leaflet.toolbar.js`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/500.html` & `umap_project-1.4.4/umap/templates/500.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/base.html` & `umap_project-1.4.4/umap/templates/base.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/registration/login.html` & `umap_project-1.4.4/umap/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/about_summary.html` & `umap_project-1.4.4/umap/templates/umap/about_summary.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/content.html` & `umap_project-1.4.4/umap/templates/umap/content.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/content_footer.html` & `umap_project-1.4.4/umap/templates/umap/content_footer.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/css.html` & `umap_project-1.4.4/umap/templates/umap/css.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/home.html` & `umap_project-1.4.4/umap/templates/umap/home.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/js.html` & `umap_project-1.4.4/umap/templates/umap/js.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/login_popup_end.html` & `umap_project-1.4.4/umap/templates/umap/login_popup_end.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/map_detail.html` & `umap_project-1.4.4/umap/templates/umap/map_detail.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/map_list.html` & `umap_project-1.4.4/umap/templates/umap/map_list.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/map_table.html` & `umap_project-1.4.4/umap/templates/umap/map_table.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/navigation.html` & `umap_project-1.4.4/umap/templates/umap/navigation.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/password_change.html` & `umap_project-1.4.4/umap/templates/umap/password_change.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/search.html` & `umap_project-1.4.4/umap/templates/umap/search.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/search_bar.html` & `umap_project-1.4.4/umap/templates/umap/search_bar.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templates/umap/user_dashboard.html` & `umap_project-1.4.4/umap/templates/umap/user_dashboard.html`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/templatetags/umap_tags.py` & `umap_project-1.4.4/umap/templatetags/umap_tags.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/base.py` & `umap_project-1.4.4/umap/tests/base.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/conftest.py` & `umap_project-1.4.4/umap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/test_datalayer.py` & `umap_project-1.4.4/umap/tests/test_datalayer.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/test_datalayer_views.py` & `umap_project-1.4.4/umap/tests/test_datalayer_views.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/test_map.py` & `umap_project-1.4.4/umap/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/test_map_views.py` & `umap_project-1.4.4/umap/tests/test_map_views.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/test_tilelayer.py` & `umap_project-1.4.4/umap/tests/test_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/test_views.py` & `umap_project-1.4.4/umap/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/fixtures/test_upload_data.gpx` & `umap_project-1.4.4/umap/tests/fixtures/test_upload_data.gpx`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/fixtures/test_upload_data.json` & `umap_project-1.4.4/umap/tests/fixtures/test_upload_data.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/fixtures/test_upload_data.kml` & `umap_project-1.4.4/umap/tests/fixtures/test_upload_data.kml`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/fixtures/test_upload_empty_coordinates.json` & `umap_project-1.4.4/umap/tests/fixtures/test_upload_empty_coordinates.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/fixtures/test_upload_missing_name.json` & `umap_project-1.4.4/umap/tests/fixtures/test_upload_missing_name.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/umap/tests/fixtures/test_upload_non_linear_ring.json` & `umap_project-1.4.4/umap/tests/fixtures/test_upload_non_linear_ring.json`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/README.md` & `umap_project-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/pyproject.toml` & `umap_project-1.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `umap_project-1.4.3/PKG-INFO` & `umap_project-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.4.3
+Version: 1.4.4
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
 Author-email: Yohan Boniface <yb@enix.org>
 Maintainer-email: David Larlet <david@larlet.fr>
 License-File: LICENSE
 Keywords: django,geodjango,leaflet,map,openstreetmap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

