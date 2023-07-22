# Comparing `tmp/ihatemoney-6.0.0.tar.gz` & `tmp/ihatemoney-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ihatemoney-6.0.0.tar", last modified: Thu Jul 13 14:11:49 2023, max compression
+gzip compressed data, was "ihatemoney-6.0.1.tar", last modified: Sat Jul 22 18:02:18 2023, max compression
```

## Comparing `ihatemoney-6.0.0.tar` & `ihatemoney-6.0.1.tar`

### file list

```diff
@@ -1,319 +1,319 @@
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      945 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/CONTRIBUTORS
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1781 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/LICENSE
--rw-r--r--   0 zorun     (1000) zorun     (1000)      205 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/MANIFEST.in
--rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/PKG-INFO
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2183 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/README.md
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/__init__.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/api/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6122 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/common.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/api/v1/
--rw-r--r--   0 zorun     (1000) zorun     (1000)       53 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/v1/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1115 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/api/v1/resources.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)       97 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/babel.cfg
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/conf-templates/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      641 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/apache-vhost.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      192 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/gunicorn.conf.py.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2170 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/ihatemoney.cfg.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      752 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/nginx.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      186 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/conf-templates/supervisord.conf.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1844 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/currency_convertor.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      845 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/default_settings.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      544 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/emails.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15851 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/forms.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6041 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/history.py
--rwxr-xr-x   0 zorun     (1000) zorun     (1000)     2406 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/manage.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/migrations/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      790 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/alembic.ini
--rwxr-xr-x   0 zorun     (1000) zorun     (1000)     3014 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/env.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/migrations/versions/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      614 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/26d6a218c329_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8427 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      627 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2002 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      963 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      625 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1085 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1629 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      977 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26923 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/models.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3498 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/monkeypath_continuum.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8632 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/run.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/static/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/static/css/
--rw-r--r--   0 zorun     (1000) zorun     (1000)   155758 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/bootstrap.min.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14225 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/datatables.min.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/download_mobile_app.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9387 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/main.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2185 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/css/tagsinput.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6742 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/favicon.ico
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.738748 ihatemoney-6.0.0/ihatemoney/static/fonts/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4582 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/OFL.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)    40370 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot
--rw-r--r--   0 zorun     (1000) zorun     (1000)    81869 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20920 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff
--rw-r--r--   0 zorun     (1000) zorun     (1000)      777 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/fontfaces.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    63744 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.eot
--rw-r--r--   0 zorun     (1000) zorun     (1000)    77893 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    33380 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.woff
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/images/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      155 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/add.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)    12353 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/app-store.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5634 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/bill.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      518 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/book.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      890 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/cog.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/delete.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      143 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/deleter.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      167 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/edit.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6681 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/f-droid.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      557 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/file-alt.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1272 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/file-csv-solid.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      692 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/git.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1458 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/globe.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    69751 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/google-play.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5814 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/indicate.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1304 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/legal.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      356 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/mobile-alt.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      293 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/paper-plane.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      319 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/plus.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      183 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/reactivate.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3505 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/read.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)     7325 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/share.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      259 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/show.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      158 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_asc.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      146 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_asc_disabled.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      199 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_both.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      157 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_desc.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/sort_desc_disabled.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)      291 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/images/x.svg
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/js/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    58072 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/bootstrap.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    84649 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/datatables.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)      326 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/ihatemoney.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    89501 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21004 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/popper.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    10060 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/tagsinput.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24989 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/js/tether.min.js
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/photoswipe/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11607 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)      547 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.png
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1554 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      866 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/preloader.gif
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9878 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4137 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.css
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31904 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.min.js
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.742748 ihatemoney-6.0.0/ihatemoney/static/showcase/
--rw-r--r--   0 zorun     (1000) zorun     (1000)   110452 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/1.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    80684 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/2.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    79206 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/3.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    74018 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/4.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    85550 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/5.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)   116502 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/6.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    91376 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/7.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)    93966 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/8.webp
--rw-r--r--   0 zorun     (1000) zorun     (1000)   132986 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/static/showcase/9.webp
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/templates/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      508 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/404.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      381 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/add_bill.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      266 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/add_member.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      340 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/admin.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      456 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/authenticate.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      195 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/create_project.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2047 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/dashboard.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      253 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/display_errors.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1274 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/download_mobile_app.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      384 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/edit_member.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3183 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/edit_project.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8805 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/forms.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      819 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/helpers.js
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14239 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/history.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3242 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/home.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      628 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      663 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9363 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/layout.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     8094 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/list_bills.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      308 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      189 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      296 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/password_reminder_sent.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      240 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/recent_projects.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      458 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/reminder_mail.en.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      462 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/reminder_mail.fr.j2
--rw-r--r--   0 zorun     (1000) zorun     (1000)      278 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/reset_password.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2188 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/send_invites.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)      649 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/settle_bills.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3333 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/showcase.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/sidebar_table_layout.html
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1323 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/templates/statistics.html
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/tests/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31635 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/api_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    61406 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/budget_test.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/tests/common/
--rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/common/__init__.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      455 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/common/help_functions.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3642 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/common/ihatemoney_testcase.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24616 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/history_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)      247 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/ihatemoney.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)      243 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/ihatemoney_envvar.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23512 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/import_test.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15296 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/tests/main_test.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/bn/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3752 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16617 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2301 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17660 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/ca/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24065 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24506 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/cs/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4843 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    18430 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/de/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22234 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26149 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/el/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11957 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24682 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/eo/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16894 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23526 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/es/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    10759 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20609 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/es_419/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23847 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    26146 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/fa/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     5193 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17711 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/fr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24071 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    32655 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/he/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    10940 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19036 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/hi/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24585 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    34005 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.730748 ihatemoney-6.0.0/ihatemoney/translations/hu/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.746748 ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6439 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17198 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/id/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21642 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24706 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/it/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17631 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24667 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ja/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17381 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25107 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/kn/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6978 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19687 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ms/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1784 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    16363 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14524 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    28725 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/nl/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14078 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22967 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/pl/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23425 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25665 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/pt/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22033 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25016 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    21501 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    24893 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ru/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    27299 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    31641 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/sr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3671 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17512 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/sv/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    19864 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23702 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ta/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9168 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23154 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/te/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    11737 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    22790 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/th/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     4044 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    17480 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/tr/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23498 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    25984 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/uk/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     6939 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20672 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/ur/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)     1266 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    15034 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/vi/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/vi/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      471 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/vi/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14545 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/vi/LC_MESSAGES/messages.po
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 zorun     (1000) zorun     (1000)    20113 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 zorun     (1000) zorun     (1000)    23264 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
--rw-r--r--   0 zorun     (1000) zorun     (1000)    14648 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/utils.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)     3596 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/versioning.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)    30464 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/web.py
--rw-r--r--   0 zorun     (1000) zorun     (1000)       66 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney/wsgi.py
-drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-13 14:11:49.734748 ihatemoney-6.0.0/ihatemoney.egg-info/
--rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/PKG-INFO
--rw-r--r--   0 zorun     (1000) zorun     (1000)     9525 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/SOURCES.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/dependency_links.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)      229 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/entry_points.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/not-zip-safe
--rw-r--r--   0 zorun     (1000) zorun     (1000)      708 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/requires.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)       11 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/ihatemoney.egg-info/top_level.txt
--rw-r--r--   0 zorun     (1000) zorun     (1000)     2038 2023-07-13 14:11:49.750748 ihatemoney-6.0.0/setup.cfg
--rw-r--r--   0 zorun     (1000) zorun     (1000)       38 2023-07-13 14:11:49.000000 ihatemoney-6.0.0/setup.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      945 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/CONTRIBUTORS
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1781 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/LICENSE
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      205 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/MANIFEST.in
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/PKG-INFO
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2183 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/README.md
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/__init__.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/api/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6122 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/common.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/api/v1/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       53 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/v1/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1115 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/api/v1/resources.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       97 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/babel.cfg
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/conf-templates/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      641 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/apache-vhost.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      192 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/gunicorn.conf.py.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2277 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/ihatemoney.cfg.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      752 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/nginx.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      186 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/conf-templates/supervisord.conf.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1844 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/currency_convertor.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      868 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/default_settings.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      544 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/emails.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    15859 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/forms.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6041 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/history.py
+-rwxr-xr-x   0 zorun     (1000) zorun     (1000)     2406 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/manage.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/migrations/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      790 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/alembic.ini
+-rwxr-xr-x   0 zorun     (1000) zorun     (1000)     3014 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/env.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/migrations/versions/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      614 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/26d6a218c329_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8427 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      627 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/6c6fb2b7f229_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2002 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      963 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      625 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1085 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/b9a10d5d63ce_.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1629 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      977 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26923 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/models.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3498 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/monkeypath_continuum.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8632 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/run.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/static/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/static/css/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   155758 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/bootstrap.min.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14225 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/datatables.min.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/download_mobile_app.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9387 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/main.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2185 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/css/tagsinput.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6742 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/favicon.ico
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.415235 ihatemoney-6.0.1/ihatemoney/static/fonts/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4582 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/OFL.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    40370 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.eot
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    81869 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20920 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.woff
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      777 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/fontfaces.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    63744 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.eot
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    77893 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    33380 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.woff
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/images/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      155 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/add.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12353 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/app-store.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5634 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/bill.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      518 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/book.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      890 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/cog.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/delete.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      143 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/deleter.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      167 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/edit.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6681 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/f-droid.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      557 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/file-alt.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1272 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/file-csv-solid.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      692 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/git.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1458 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/globe.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    69751 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/google-play.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5814 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/indicate.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1304 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/legal.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      356 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/mobile-alt.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      293 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/paper-plane.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      319 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/plus.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      183 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/reactivate.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3505 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/read.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     7325 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/share.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      259 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/show.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      158 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_asc.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      146 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_asc_disabled.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      199 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_both.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      157 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_desc.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      144 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/sort_desc_disabled.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      291 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/images/x.svg
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/js/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    58072 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/bootstrap.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    84649 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/datatables.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      326 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/ihatemoney.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    89501 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21004 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/popper.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    10060 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/tagsinput.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24989 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/js/tether.min.js
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/photoswipe/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11607 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      547 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.png
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1554 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.svg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      866 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/preloader.gif
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9878 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4137 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.css
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31904 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.min.js
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.419235 ihatemoney-6.0.1/ihatemoney/static/showcase/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   110452 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/1.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    80684 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/2.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    79206 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/3.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    74018 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/4.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    85550 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/5.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   116502 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/6.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    91376 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/7.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    93966 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/8.webp
+-rw-r--r--   0 zorun     (1000) zorun     (1000)   132986 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/static/showcase/9.webp
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/templates/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      508 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/404.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      381 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/add_bill.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      266 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/add_member.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      340 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/admin.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      456 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/authenticate.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      195 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/create_project.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2047 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/dashboard.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      253 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/display_errors.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1274 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/download_mobile_app.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      384 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/edit_member.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3183 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/edit_project.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8800 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/forms.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      819 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/helpers.js
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14207 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/history.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3242 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/home.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      628 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      663 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9363 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/layout.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8094 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/list_bills.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      298 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      308 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      189 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      296 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/password_reminder_sent.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      240 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/recent_projects.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      458 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/reminder_mail.en.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      462 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/reminder_mail.fr.j2
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      278 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/reset_password.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2132 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/send_invites.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      649 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/settle_bills.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3333 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/showcase.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2537 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/sidebar_table_layout.html
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1323 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/templates/statistics.html
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/tests/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    31635 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/api_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    62720 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/budget_test.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/tests/common/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/common/__init__.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      455 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/common/help_functions.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3642 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/common/ihatemoney_testcase.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24612 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/history_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      247 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/ihatemoney.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      243 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/ihatemoney_envvar.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    23512 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/import_test.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    15296 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/tests/main_test.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/bn/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3626 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18252 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2105 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19243 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/ca/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20292 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26010 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/cs/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3806 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19876 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/de/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21148 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27611 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/el/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    11152 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26286 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/eo/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14668 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24947 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/es/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     8803 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21878 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/es_419/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    20099 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27588 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/fa/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     4871 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19283 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/fr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24032 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    34440 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.407235 ihatemoney-6.0.1/ihatemoney/translations/he/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    13498 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21847 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/hi/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21207 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    35887 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/hu/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6025 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18680 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/id/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18123 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26079 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/it/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14297 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26112 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ja/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14961 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26614 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/kn/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6873 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    21364 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ms/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.423235 ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1711 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    17896 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12943 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    30034 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/nl/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    12418 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24311 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/pl/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19768 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27083 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/pt/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19649 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26437 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19135 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    26311 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ru/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24769 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    33304 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/sr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3599 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19114 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/sv/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    18537 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    25233 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ta/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     6917 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24755 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/te/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9177 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24405 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/th/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3702 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19037 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/tr/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    19795 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    27394 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/uk/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     5936 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    22133 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/ur/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     1190 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16608 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/vi/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      411 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16154 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/messages.po
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    16680 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    24563 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    14648 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/utils.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     3596 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/versioning.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)    30734 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/web.py
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       66 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney/wsgi.py
+drwxr-xr-x   0 zorun     (1000) zorun     (1000)        0 2023-07-22 18:02:18.411235 ihatemoney-6.0.1/ihatemoney.egg-info/
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      847 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/PKG-INFO
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     9525 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      229 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/entry_points.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)        1 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/not-zip-safe
+-rw-r--r--   0 zorun     (1000) zorun     (1000)      708 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/requires.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       11 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/ihatemoney.egg-info/top_level.txt
+-rw-r--r--   0 zorun     (1000) zorun     (1000)     2038 2023-07-22 18:02:18.427235 ihatemoney-6.0.1/setup.cfg
+-rw-r--r--   0 zorun     (1000) zorun     (1000)       38 2023-07-22 18:02:18.000000 ihatemoney-6.0.1/setup.py
```

### Comparing `ihatemoney-6.0.0/CONTRIBUTORS` & `ihatemoney-6.0.1/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/LICENSE` & `ihatemoney-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/PKG-INFO` & `ihatemoney-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihatemoney
-Version: 6.0.0
+Version: 6.0.1
 Summary: A simple shared budget manager web application.
 Home-page: https://github.com/spiral-project/ihatemoney
 Author: Alexis Métaireau & contributors
 Author-email: alexis@notmyidea.org
 License: Custom BSD Beerware
 Description: UNKNOWN
 Keywords: web,budget
```

### Comparing `ihatemoney-6.0.0/README.md` & `ihatemoney-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/api/common.py` & `ihatemoney-6.0.1/ihatemoney/api/common.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/api/v1/resources.py` & `ihatemoney-6.0.1/ihatemoney/api/v1/resources.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/conf-templates/apache-vhost.conf.j2` & `ihatemoney-6.0.1/ihatemoney/conf-templates/apache-vhost.conf.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/conf-templates/ihatemoney.cfg.j2` & `ihatemoney-6.0.1/ihatemoney/conf-templates/ihatemoney.cfg.j2`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,18 @@
 #derived from the server OS.
 #BABEL_DEFAULT_TIMEZONE = "Europe/Paris"
 
 # Enable secure cookies. Requires HTTPS. Disable if you run your ihatemoney
 # service over plain HTTP.
 SESSION_COOKIE_SECURE = True
 
+# Set this to a URL path under which the application will be served.  Defaults to "/"
+APPLICATION_ROOT = "/"
+
 # You can activate an optional CAPTCHA if you want to. It can be helpful
 # to filter spammer bots.
-# ENABLE_CAPTCHA = True
+ENABLE_CAPTCHA = False
 
 # You may want to point to a special legal page, for instance to give information
 # about GDPR, or how you handle the data of your users.
 # Set this variable to the URL you want.
-# LEGAL_LINK = ""
+LEGAL_LINK = ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/conf-templates/nginx.conf.j2` & `ihatemoney-6.0.1/ihatemoney/conf-templates/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/currency_convertor.py` & `ihatemoney-6.0.1/ihatemoney/currency_convertor.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/default_settings.py` & `ihatemoney-6.0.1/ihatemoney/default_settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 DEBUG = SQLACHEMY_ECHO = False
 SQLALCHEMY_DATABASE_URI = "sqlite:////tmp/ihatemoney.db"
 SQLALCHEMY_TRACK_MODIFICATIONS = False
 SECRET_KEY = "tralala"
 MAIL_DEFAULT_SENDER = "Budget manager <admin@example.com>"
 SHOW_ADMIN_EMAIL = True
 ACTIVATE_DEMO_PROJECT = True
+ACTIVATE_ADMIN_DASHBOARD = False
 ADMIN_PASSWORD = ""
 ALLOW_PUBLIC_PROJECT_CREATION = True
-ACTIVATE_ADMIN_DASHBOARD = False
 SESSION_COOKIE_SECURE = True
+APPLICATION_ROOT = "/"
+ENABLE_CAPTCHA = False
+LEGAL_LINK = ""
 SUPPORTED_LANGUAGES = [
     "ca",
     "cs",
     "de",
     "el",
     "en",
     "eo",
@@ -39,9 +42,7 @@
     "ta",
     "te",
     "th",
     "tr",
     "uk",
     "zh_Hans",
 ]
-ENABLE_CAPTCHA = False
-LEGAL_LINK = ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/emails.py` & `ihatemoney-6.0.1/ihatemoney/emails.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/forms.py` & `ihatemoney-6.0.1/ihatemoney/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,15 @@
     def fill(self, member):
         self.name.data = member.name
         self.weight.data = member.weight
 
 
 class InviteForm(FlaskForm):
     emails = StringField(_("People to notify"), render_kw={"class": "tag"})
-    submit = SubmitField(_("Send invites"))
+    submit = SubmitField(_("Send the invitations"))
 
     def validate_emails(self, field):
         for email in [email.strip() for email in self.emails.data.split(",")]:
             try:
                 email_validator.validate_email(email)
             except email_validator.EmailNotValidError:
                 raise ValidationError(
```

### Comparing `ihatemoney-6.0.0/ihatemoney/history.py` & `ihatemoney-6.0.1/ihatemoney/history.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/manage.py` & `ihatemoney-6.0.1/ihatemoney/manage.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/alembic.ini` & `ihatemoney-6.0.1/ihatemoney/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/env.py` & `ihatemoney-6.0.1/ihatemoney/migrations/env.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/26d6a218c329_.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/26d6a218c329_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/2dcb0c0048dc_autologger.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/6c6fb2b7f229_.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/6c6fb2b7f229_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/927ed575acbd_add_currencies.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/a67119aa3ee5_migrate_negative_weights.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/afbf27e6ef20_add_bill_import_date_field.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/b78f8a8bdb16_hash_project_passwords.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/b9a10d5d63ce_.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/b9a10d5d63ce_.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/cb038f79982e_sqlite_autoincrement.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py` & `ihatemoney-6.0.1/ihatemoney/migrations/versions/f629c8ef4ab0_initialize_all_members_weights_to_1.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/models.py` & `ihatemoney-6.0.1/ihatemoney/models.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/monkeypath_continuum.py` & `ihatemoney-6.0.1/ihatemoney/monkeypath_continuum.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/run.py` & `ihatemoney-6.0.1/ihatemoney/run.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/css/bootstrap.min.css` & `ihatemoney-6.0.1/ihatemoney/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/css/datatables.min.css` & `ihatemoney-6.0.1/ihatemoney/static/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/css/main.css` & `ihatemoney-6.0.1/ihatemoney/static/css/main.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/css/tagsinput.css` & `ihatemoney-6.0.1/ihatemoney/static/css/tagsinput.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/favicon.ico` & `ihatemoney-6.0.1/ihatemoney/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/OFL.txt` & `ihatemoney-6.0.1/ihatemoney/static/fonts/OFL.txt`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.eot` & `ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.svg` & `ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/comfortaa-regular-webfont.woff` & `ihatemoney-6.0.1/ihatemoney/static/fonts/comfortaa-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/fontfaces.css` & `ihatemoney-6.0.1/ihatemoney/static/fonts/fontfaces.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.eot` & `ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.eot`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.svg` & `ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/fonts/lobster-webfont.woff` & `ihatemoney-6.0.1/ihatemoney/static/fonts/lobster-webfont.woff`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/app-store.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/app-store.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/bill.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/bill.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/book.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/book.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/cog.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/cog.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/f-droid.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/f-droid.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/file-alt.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/file-alt.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/file-csv-solid.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/file-csv-solid.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/git.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/git.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/globe.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/globe.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/google-play.png` & `ihatemoney-6.0.1/ihatemoney/static/images/google-play.png`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/indicate.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/indicate.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/legal.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/legal.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/read.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/read.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/images/share.svg` & `ihatemoney-6.0.1/ihatemoney/static/images/share.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/js/bootstrap.min.js` & `ihatemoney-6.0.1/ihatemoney/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/js/datatables.min.js` & `ihatemoney-6.0.1/ihatemoney/static/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/js/jquery-3.6.0.min.js` & `ihatemoney-6.0.1/ihatemoney/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/js/popper.min.js` & `ihatemoney-6.0.1/ihatemoney/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/js/tagsinput.js` & `ihatemoney-6.0.1/ihatemoney/static/js/tagsinput.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/js/tether.min.js` & `ihatemoney-6.0.1/ihatemoney/static/js/tether.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.css` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.png` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.png`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/default-skin.svg` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/default-skin.svg`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/default-skin/preloader.gif` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/default-skin/preloader.gif`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe-ui-default.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.css` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.css`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/photoswipe/photoswipe.min.js` & `ihatemoney-6.0.1/ihatemoney/static/photoswipe/photoswipe.min.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/1.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/1.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/2.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/2.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/3.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/3.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/4.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/4.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/5.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/5.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/6.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/6.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/7.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/7.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/8.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/8.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/static/showcase/9.webp` & `ihatemoney-6.0.1/ihatemoney/static/showcase/9.webp`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/dashboard.html` & `ihatemoney-6.0.1/ihatemoney/templates/dashboard.html`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
                     _('edit') }}</a>
 
                 <form id="delete-project" class="form-horizontal" action="{{ url_for('.dashboard_delete_project',
                     project_id=project.id) }}" method="post">
 
                     <button class="delete">{{ _("Delete project") }}</button>
                 </form>
-                <a class="show" href="{{ url_for('.list_bills', project_id=project.id) }}" title="{{ _(" show") }}">{{
+                <a class="show" href="{{ url_for('.list_bills', project_id=project.id) }}" title="{{ _("show") }}">{{
                     _('show') }}</a>
             </td>
         </tr>
         {% endfor %}
     </tbody>
 </table>
 <script language="JavaScript">
@@ -47,8 +47,8 @@
             paging: true
         });
     })
 </script>
 {% else %}
 <div class="alert alert-danger">{{ _("The Dashboard is currently deactivated.") }}</div>
 {% endif %}
-{% endblock %}
+{% endblock %}
```

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/download_mobile_app.html` & `ihatemoney-6.0.1/ihatemoney/templates/download_mobile_app.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/edit_project.html` & `ihatemoney-6.0.1/ihatemoney/templates/edit_project.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/forms.html` & `ihatemoney-6.0.1/ihatemoney/templates/forms.html`

 * *Files 2% similar despite different names*

```diff
@@ -97,27 +97,27 @@
         {{ checkbox(form.project_history) }}
         {{ checkbox(form.ip_recording) }}
         </div>
     </div>
 
     {{ input(form.default_currency) }}
     <div class="actions">
-        <button class="btn btn-primary">{{ _("Edit the project") }}</button>
+        <button class="btn btn-primary">{{ _("Save changes") }}</button>
     </div>
 
 {% endmacro %}
 
 {% macro delete_project(form) %}
 
     {% include "display_errors.html" %}
     <p><strong>{{ _("This will remove all bills and participants in this project!") }}</strong></p>
     {{ form.hidden_tag() }}
     {{ input(form.password) }}
     <div class="actions">
-        <button class="btn btn-primary">{{ _("Delete project") }}</button>
+        <button class="btn btn-danger">{{ _("Delete project") }}</button>
     </div>
 
 {% endmacro %}
 
 {% macro import_project(form) %}
 
     {% include "display_errors.html" %}
```

#### html2text {}

```diff
@@ -27,15 +27,15 @@
 { submit(form.submit, home=True) }} {% endif %} {% endmacro %} {% macro
 edit_project(form) %} {% include "display_errors.html" %} {{ form.hidden_tag()
 }} {{ input(form.name) }} {{ input(form.password) }} {{ input
 (form.contact_email) }}
 {{ _("Privacy Settings") }}
 {{ checkbox(form.project_history) }} {{ checkbox(form.ip_recording) }}
 {{ input(form.default_currency) }}
-{{ _("Edit the project") }}
+{{ _("Save changes") }}
 {% endmacro %} {% macro delete_project(form) %} {% include
 "display_errors.html" %}
 {{ _("This will remove all bills and participants in this project!") }}
 {{ form.hidden_tag() }} {{ input(form.password) }}
 {{ _("Delete project") }}
 {% endmacro %} {% macro import_project(form) %} {% include
 "display_errors.html" %} {{ form.hidden_tag() }}
```

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/helpers.js` & `ihatemoney-6.0.1/ihatemoney/templates/helpers.js`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/history.html` & `ihatemoney-6.0.1/ihatemoney/templates/history.html`

 * *Files 2% similar despite different names*

```diff
@@ -99,26 +99,25 @@
 
 
 
 {% block content %}
     {% if current_log_pref == LoggingMode.DISABLED  or (current_log_pref != LoggingMode.RECORD_IP and any_ip_addresses) %}
     <div id="history_warnings" class="card card-body bg-light">
     {% if current_log_pref == LoggingMode.DISABLED  %}
-        <p>{% set url = url_for(".edit_project") %}
-            {% trans %}
-            <i>This project has history disabled. New actions won't appear below. You can enable history on the</i>
-            <a href="{{ url }}">settings page</a>
-            {% endtrans %}
+        <p>
+            <i>{{ _("This project has history disabled. New actions won't appear below.") }}
+               <a href="{{ url_for(".edit_project") }}">{{ _("You can enable history on the settings page.") }}</a>
+            </i>
         </p>
         {% if history %}
         <p>
-            {% trans %}
-            <i>The table below reflects actions recorded prior to disabling project history. You can
-            <a href="#" data-toggle="modal" data-keyboard="false" data-target="#confirm-erase">clear project history</a> to remove them.</i></p>
-            {% endtrans %}
+            <i>{{ _("The table below reflects actions recorded prior to disabling project history.") }}
+              <a href="#" data-toggle="modal" data-keyboard="false" data-target="#confirm-erase">{{ _("You can clear the project history to remove them.") }}</a>
+            </i>
+        </p>
         {% endif %}
     {% endif %}
     {% if current_log_pref != LoggingMode.RECORD_IP and any_ip_addresses %}
         <p>
             <i>{{ _("Some entries below contain IP addresses, even though this project has IP recording disabled. ") }}
             <a href="#" data-toggle="modal" data-keyboard="false" data-target="#confirm-ip-delete">{{ _("Delete stored IP addresses") }}</a></i>
         </p>
```

#### html2text {}

```diff
@@ -41,22 +41,21 @@
 else %} {% trans %}Bill {{ name }}: removed {{ owers_list_str }} from owers
 list{% endtrans %} {% endif %} {% endmacro %} {% block sidebar %}
 {{ balance_table(show_weight=False, show_header=True) }}
 {% endblock %} {% block content %} {% if current_log_pref ==
 LoggingMode.DISABLED or (current_log_pref != LoggingMode.RECORD_IP and
 any_ip_addresses) %}
 {% if current_log_pref == LoggingMode.DISABLED %}
-{% set url = url_for(".edit_project") %} {% trans %} This project has history
-disabled. New actions won't appear below. You can enable history on the
-settings_page {% endtrans %}
+{{ _("This project has history disabled. New actions won't appear below.") }}
+edit_project") }}">{{ _("You can enable history on the settings page.") }}
 {% if history %}
-{% trans %} The table below reflects actions recorded prior to disabling
-project history. You can clear_project_history to remove them.
-{% endtrans %} {% endif %} {% endif %} {% if current_log_pref !=
-LoggingMode.RECORD_IP and any_ip_addresses %}
+{{ _("The table below reflects actions recorded prior to disabling project
+history.") }} {{__("You_can_clear_the_project_history_to_remove_them.")_}}
+{% endif %} {% endif %} {% if current_log_pref != LoggingMode.RECORD_IP and
+any_ip_addresses %}
 {{ _("Some entries below contain IP addresses, even though this project has IP
 recording disabled. ") }} {{__("Delete_stored_IP_addresses")_}}
 {% endif %}
 {% endif %} {{ clear_history_modals() }}
 % if not any_ip_addresses %}data-placement="top" data-toggle="tooltip" title="{
 {_('No IP Addresses to erase')}}" {% endif %}> {{_static_include("images/
 x.svg")_|_safe_}}_{{__("Delete_Stored_IP_Addresses")_}}
```

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/home.html` & `ihatemoney-6.0.1/ihatemoney/templates/home.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.en.j2` & `ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.en.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/invitation_mail.fr.j2` & `ihatemoney-6.0.1/ihatemoney/templates/invitation_mail.fr.j2`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/layout.html` & `ihatemoney-6.0.1/ihatemoney/templates/layout.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/list_bills.html` & `ihatemoney-6.0.1/ihatemoney/templates/list_bills.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/send_invites.html` & `ihatemoney-6.0.1/ihatemoney/templates/send_invites.html`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                     {{ url_for(".join_project", _external=True, project_id=g.project.id, token=g.project.generate_token()) }}
                 </a>
             </td>
         </tr>
         <tr>
             <td>
                 <h3>{{ _('Scan QR code') }}</h3>
-                <p><small>{% trans download_mobile=url_for(".mobile") %}On a mobile device, with <a href="{{ download_mobile }}">a compatible app installed</a>.{% endtrans %}</small></p>
+                <p><small><a href="{{ url_for(".mobile") }}">{{ _("Use a mobile device with a compatible app.") }}</a></small></p>
             </td>
             <td>
                 {{ qrcode | safe }}
             </td>
         </tr>
         <tr>
             <td>
```

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/settle_bills.html` & `ihatemoney-6.0.1/ihatemoney/templates/settle_bills.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/showcase.html` & `ihatemoney-6.0.1/ihatemoney/templates/showcase.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/sidebar_table_layout.html` & `ihatemoney-6.0.1/ihatemoney/templates/sidebar_table_layout.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/templates/statistics.html` & `ihatemoney-6.0.1/ihatemoney/templates/statistics.html`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/tests/api_test.py` & `ihatemoney-6.0.1/ihatemoney/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/tests/budget_test.py` & `ihatemoney-6.0.1/ihatemoney/tests/budget_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,24 @@
         )
         self.assertIn("Create a new project", resp.data.decode("utf-8"))
 
         # A token MUST have a point between payload and signature
         resp = self.client.get("/raclette/join/token.invalid", follow_redirects=True)
         self.assertIn("Provided token is invalid", resp.data.decode("utf-8"))
 
+    def test_create_should_remember_project(self):
+        """Test that creating a project adds it to the "logged in project" list,
+        as it does for authentication
+        """
+        self.login("raclette")
+        self.post_project("raclette")
+        self.post_project("tartiflette")
+        data = self.client.get("/raclette/").data.decode("utf-8")
+        self.assertEqual(data.count('href="/tartiflette/"'), 1)
+
     def test_multiple_join(self):
         """Test that joining multiple times a project
         doesn't add it multiple times in the session"""
         self.login("raclette")
         self.post_project("raclette")
         project = self.get_project("raclette")
         invite_link = url_for(
@@ -1651,10 +1661,30 @@
         self.assertIn('<p class="alert alert-danger">', resp.data.decode("utf-8"))
 
         # Without any check, the following request will fail.
         resp = self.client.get("/raclette/")
         # No bills, the previous one was not added
         self.assertIn("No bills", resp.data.decode("utf-8"))
 
+    def test_session_projects_migration_to_list(self):
+        """In https://github.com/spiral-project/ihatemoney/pull/1082, session["projects"]
+        was migrated from a list to a dict. We need to handle this.
+        """
+        self.post_project("raclette")
+        self.client.get("/exit")
+
+        with self.client as c:
+            c.post("/authenticate", data={"id": "raclette", "password": "raclette"})
+            self.assertTrue(session["raclette"])
+            # New behavior
+            self.assertIsInstance(session["projects"], dict)
+            # Now, go back to the past
+            with c.session_transaction() as sess:
+                sess["projects"] = [("raclette", "raclette")]
+            # It should convert entry to dict
+            c.get("/")
+            self.assertIsInstance(session["projects"], dict)
+            self.assertIn("raclette", session["projects"])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `ihatemoney-6.0.0/ihatemoney/tests/common/ihatemoney_testcase.py` & `ihatemoney-6.0.1/ihatemoney/tests/common/ihatemoney_testcase.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/tests/history_test.py` & `ihatemoney-6.0.1/ihatemoney/tests/history_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             self.assertIn('<input checked id="ip_recording"', resp.data.decode("utf-8"))
         else:
             self.assertIn('<input id="ip_recording"', resp.data.decode("utf-8"))
 
     def assert_empty_history_logging_disabled(self):
         resp = self.client.get("/demo/history")
         self.assertIn(
-            "This project has history disabled. New actions won't appear below. ",
+            "This project has history disabled. New actions won't appear below.",
             resp.data.decode("utf-8"),
         )
         self.assertIn("Nothing to list", resp.data.decode("utf-8"))
         self.assertNotIn(
             "The table below reflects actions recorded prior to disabling project history.",
             resp.data.decode("utf-8"),
         )
@@ -244,15 +244,15 @@
             resp.data.decode("utf-8"),
         )
 
         # List history
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertIn(
-            "This project has history disabled. New actions won't appear below. ",
+            "This project has history disabled. New actions won't appear below.",
             resp.data.decode("utf-8"),
         )
         self.assertIn(
             "The table below reflects actions recorded prior to disabling project history.",
             resp.data.decode("utf-8"),
         )
         self.assertNotIn("Nothing to list", resp.data.decode("utf-8"))
@@ -283,15 +283,15 @@
 
         # Disable IP Recording
         self.change_privacy_to(LoggingMode.ENABLED)
 
         resp = self.client.get("/demo/history")
         self.assertEqual(resp.status_code, 200)
         self.assertNotIn(
-            "This project has history disabled. New actions won't appear below. ",
+            "This project has history disabled. New actions won't appear below.",
             resp.data.decode("utf-8"),
         )
         self.assertNotIn(
             "The table below reflects actions recorded prior to disabling project history.",
             resp.data.decode("utf-8"),
         )
         self.assertNotIn("Nothing to list", resp.data.decode("utf-8"))
@@ -328,15 +328,15 @@
             "/demo/strip_ip_addresses",
             data={"password": "123456"},
             follow_redirects=True,
         )
 
         self.assertEqual(resp.status_code, 200)
         self.assertNotIn(
-            "This project has history disabled. New actions won't appear below. ",
+            "This project has history disabled. New actions won't appear below.",
             resp.data.decode("utf-8"),
         )
         self.assertNotIn(
             "The table below reflects actions recorded prior to disabling project history.",
             resp.data.decode("utf-8"),
         )
         self.assertNotIn("Nothing to list", resp.data.decode("utf-8"))
```

### Comparing `ihatemoney-6.0.0/ihatemoney/tests/import_test.py` & `ihatemoney-6.0.1/ihatemoney/tests/import_test.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/tests/main_test.py` & `ihatemoney-6.0.1/ihatemoney/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/bn/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Bengali (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-04-14 21:10+0000\n"
+"Last-Translator: Hasidul Islam <ihasidul@gmail.com>\n"
+"Language: bn\n"
 "Language-Team: Bengali <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/bn/>\n"
-"Language: bn\n"
+"Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 "এই শনাক্তকারী(\"%(project)s\")সহ একটি প্রজেক্ট ইতিমধ্যেই বিদ্যমান৷ একটি নতুন "
 "শনাক্তকারী ঠিক করুন"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/bn/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/ms/LC_MESSAGES/messages.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,189 +1,210 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-04-13 21:42+0200\n"
-"PO-Revision-Date: 2022-04-14 21:10+0000\n"
-"Last-Translator: Hasidul Islam <ihasidul@gmail.com>\n"
-"Language-Team: Bengali <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/bn/>\n"
-"Language: bn\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2021-07-18 12:32+0000\n"
+"Last-Translator: Kemystra <izzmin97@gmail.com>\n"
+"Language: ms\n"
+"Language-Team: Malay <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/ms/>\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.12-dev\n"
+"Generated-By: Babel 2.9.0\n"
+
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
-msgstr ""
+msgstr "Nilai atau ungkapan yang sah. Hanya nombor dan operasi + - * / diterima."
 
 msgid "Project name"
-msgstr "প্রজেক্টের নাম"
+msgstr "Nama projek"
 
 msgid "New private code"
-msgstr "নতুন ব্যক্তিগত কোড"
+msgstr "Kod peribadi baharu"
 
 msgid "Enter a new code if you want to change it"
-msgstr "আপনি যদি এটি পরিবর্তন করতে চান তবে একটি নতুন কোড লিখুন"
+msgstr "Masukkan kod baharu jika kamu mahu mengubahnya"
 
 msgid "Email"
-msgstr "ইমেইল"
+msgstr "E-mel"
 
+#, fuzzy
 msgid "Enable project history"
-msgstr "প্রজেক্টের ইতিহাস সক্ষম করুন"
+msgstr "Aktifkan sejarah projek"
 
+#, fuzzy
 msgid "Use IP tracking for project history"
-msgstr "প্রজেক্ট ইতিহাসের জন্য আইপি ট্র্যাকিং ব্যবহার করুন"
+msgstr "Gunakan penjejakan IP untuk sejarah projek"
 
+#, fuzzy
 msgid "Default Currency"
-msgstr "ডিফল্ট মুদ্রা"
+msgstr "Mata wang asal"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
+#, fuzzy
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"এই প্রজেক্টটি 'নো কারেন্সি' সেট করা যাবে না কারণ এতে একাধিক মুদ্রার বিল "
-"রয়েছে৷"
-
-msgid "Import previously exported JSON file"
-msgstr ""
+"Projek ini tidak boleh disetkan kepada 'tiada mata wang' kerana projek "
+"ini mempunyai wang dalam beberapa bentuk mata wang"
 
-msgid "Import"
+msgid "Compatible with Cospend"
 msgstr ""
 
 msgid "Project identifier"
-msgstr "প্রজেক্ট শনাক্তকারী"
+msgstr ""
 
 msgid "Private code"
-msgstr "ব্যক্তিগত কোড"
+msgstr "Kod peribadi"
 
 msgid "Create the project"
-msgstr "প্রজেক্ট তৈরি করুন"
+msgstr "Cipta projek ini"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"এই শনাক্তকারী(\"%(project)s\")সহ একটি প্রজেক্ট ইতিমধ্যেই বিদ্যমান৷ একটি নতুন "
-"শনাক্তকারী ঠিক করুন"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr "কোনটি আসল মুদ্রা: ইউরো না পেট্রো ডলার?"
+msgstr ""
 
 msgid "euro"
-msgstr "ইউরো"
+msgstr ""
 
 msgid "Please, validate the captcha to proceed."
-msgstr "অনুগ্রহ করে, এগিয়ে যেতে ক্যাপচা যাচাই করুন।"
+msgstr ""
 
 msgid "Enter private code to confirm deletion"
-msgstr "মুছে ফেলা নিশ্চিত করতে ব্যক্তিগত কোড লিখুন"
+msgstr "Masukkan kod peribadi untuk mengesahkan penghapusan"
 
+#, fuzzy
 msgid "Unknown error"
-msgstr "অজানা ত্রুটি"
+msgstr "Ralat yang tidak dikenalpasti"
 
 msgid "Invalid private code."
-msgstr "অবৈধ ব্যক্তিগত কোড."
+msgstr "Kod peribadi tidak sah."
 
 msgid "Get in"
-msgstr "প্রবেশ করুন"
+msgstr "Masuk"
 
 msgid "Admin password"
-msgstr "অ্যাডমিন পাসওয়ার্ড"
+msgstr "Kata laluan pentadbir"
 
 msgid "Send me the code by email"
-msgstr "আমাকে ইমেল দ্বারা কোড পাঠান"
+msgstr "Hantar kod saya melalui e-mel"
 
 msgid "This project does not exists"
-msgstr ""
+msgstr "Projek ini tidak wujud"
 
+#, fuzzy
 msgid "Password mismatch"
-msgstr "পাসওয়ার্ড মেলেনি"
+msgstr "Kata laluan tidak sama"
 
 msgid "Password"
-msgstr "পাসওয়ার্ড"
+msgstr "Kata laluan"
 
 msgid "Password confirmation"
-msgstr "পাসওয়ার্ড নিশ্চিতকরণ"
+msgstr "Pengesahan kata laluan"
 
+#, fuzzy
 msgid "Reset password"
-msgstr "পাসওয়ার্ড রিসেট করুন"
+msgstr "Tetapkan semula kata laluan"
 
-msgid "Date"
-msgstr "তারিখ"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
-msgstr "কি?"
+msgstr "Apa?"
 
-msgid "Payer"
-msgstr "প্রদানকারী"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
+msgid "How much?"
 msgstr ""
 
 msgid "Currency"
-msgstr "মুদ্রা"
+msgstr "Mata wang"
 
+#, fuzzy
 msgid "External link"
-msgstr ""
+msgstr "pautan luar"
 
 msgid "A link to an external document, related to this bill"
 msgstr ""
 
 msgid "For whom?"
-msgstr ""
+msgstr "Untuk siapa?"
 
 msgid "Submit"
-msgstr ""
+msgstr "Hantar"
 
+#, fuzzy
 msgid "Submit and add a new one"
-msgstr ""
+msgstr "Hantar dan tambah yang baharu"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr ""
 
-msgid "Bills can't be null"
-msgstr ""
-
 msgid "Name"
-msgstr ""
+msgstr "Nama"
 
+#, fuzzy
 msgid "Weights should be positive"
-msgstr ""
+msgstr "Berat perlulah positif"
 
+#, fuzzy
 msgid "Weight"
-msgstr ""
+msgstr "Berat"
 
 msgid "Add"
-msgstr ""
+msgstr "Tambah"
 
 msgid "The participant name is invalid"
 msgstr ""
 
+#, fuzzy
 msgid "This project already have this participant"
-msgstr ""
+msgstr "Projek ini sudah mempunyai ahli"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr ""
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -203,89 +224,84 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+msgid "Too many failed login attempts."
 msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
 msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -320,14 +336,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr ""
 
 msgid "Deleted project history."
 msgstr ""
 
 msgid "Error deleting recorded IP addresses"
@@ -380,43 +400,35 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "Cipta projek ini"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -434,26 +446,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Import fail JSON yang telah dieksport sebelum ini"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -464,17 +486,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -531,51 +550,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -631,17 +645,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Pembayar"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "Tarikh"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -743,15 +763,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -777,46 +798,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -861,14 +876,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -900,7 +921,115 @@
 msgstr ""
 
 msgid "Expenses by Month"
 msgstr ""
 
 msgid "Period"
 msgstr ""
+
+#~ msgid "You either provided a bad token or no project identifier."
+#~ msgstr ""
+
+#~ msgid "User name incorrect"
+#~ msgstr "Nama pengguna tidak tepat"
+
+#~ msgid "People to notify"
+#~ msgstr ""
+
+#~ msgid "Error activating member"
+#~ msgstr ""
+
+#~ msgid "Error removing member"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "User '%(name)s' has been deactivated. It"
+#~ " will still appear in the users "
+#~ "list until its balance becomes zero."
+#~ msgstr ""
+
+#~ msgid "User '%(name)s' has been removed"
+#~ msgstr ""
+
+#~ msgid "User '%(name)s' has been edited"
+#~ msgstr ""
+
+#~ msgid "Number of members"
+#~ msgstr ""
+
+#~ msgid "Edit this member"
+#~ msgstr ""
+
+#~ msgid "Participants to notify"
+#~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "Import"
+
+#~ msgid "Amount paid"
+#~ msgstr "Jumlah dibayar"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Bil tidak boleh kosong"
+
+#~ msgid "Too many failed login attempts, please retry later."
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr ""
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2020-08-01 10:41+0000\n"
 "Last-Translator: Oymate <dhruboadittya96@gmail.com>\n"
 "Language: bn_BD\n"
 "Language-Team: Bengali (Bangladesh) <https://hosted.weblate.org/projects/i-"
 "hate-money/i-hate-money/bn_BD/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "Admin password"
 msgstr "অ্যাডমিন পাসওয়ার্ড"
 
 msgid "Create the project"
 msgstr "প্রকল্প তৈরি করুন"
 
@@ -34,20 +34,14 @@
 
 msgid "Enter private code to confirm deletion"
 msgstr "মুছে ফেলার জন্য ব্যক্তিগত কোড লিখুন"
 
 msgid "Get in"
 msgstr "ভিতরে আস"
 
-msgid "Import"
-msgstr "আমদানি"
-
-msgid "Import previously exported JSON file"
-msgstr "পূর্বে রপ্তানি করা JSON ফাইল আমদানি করুন"
-
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "কোন বৈধ পরিমাণ বা অভিব্যক্তি নয়। শুধুমাত্র সংখ্যা এবং + - * / অপারেটর গ্রহণ করা হয়।"
 
 msgid "Private code"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/bn_BD/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2020-08-01 10:41+0000\n"
 "Last-Translator: Oymate <dhruboadittya96@gmail.com>\n"
 "Language: bn_BD\n"
 "Language-Team: Bengali (Bangladesh) "
 "<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/bn_BD/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "কোন বৈধ পরিমাণ বা অভিব্যক্তি নয়। শুধুমাত্র সংখ্যা এবং + - * / অপারেটর "
 "গ্রহণ করা হয়।"
 
@@ -48,19 +52,16 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
-msgstr "পূর্বে রপ্তানি করা JSON ফাইল আমদানি করুন"
-
-msgid "Import"
-msgstr "আমদানি"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "প্রকল্প শনাক্তকারী"
 
 msgid "Private code"
 msgstr "ব্যক্তিগত কোড"
 
@@ -112,24 +113,24 @@
 
 msgid "Password confirmation"
 msgstr ""
 
 msgid "Reset password"
 msgstr ""
 
-msgid "Date"
+msgid "When?"
 msgstr ""
 
 msgid "What?"
 msgstr ""
 
-msgid "Payer"
+msgid "Who paid?"
 msgstr ""
 
-msgid "Amount paid"
+msgid "How much?"
 msgstr ""
 
 msgid "Currency"
 msgstr ""
 
 msgid "External link"
 msgstr ""
@@ -146,17 +147,14 @@
 msgid "Submit and add a new one"
 msgstr ""
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr ""
 
-msgid "Bills can't be null"
-msgstr ""
-
 msgid "Name"
 msgstr ""
 
 msgid "Weights should be positive"
 msgstr ""
 
 msgid "Weight"
@@ -170,21 +168,33 @@
 
 msgid "This project already have this participant"
 msgstr ""
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr ""
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -204,89 +214,84 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+msgid "Too many failed login attempts."
 msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
 msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -321,14 +326,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "প্রকল্পের ইতিহাস সক্রিয় করো"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "প্রকল্পের ইতিহাস সক্রিয় করো"
@@ -383,43 +392,35 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "প্রকল্প তৈরি করুন"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -437,26 +438,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "পূর্বে রপ্তানি করা JSON ফাইল আমদানি করুন"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -467,17 +478,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -534,51 +542,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -634,17 +637,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr ""
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr ""
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -746,15 +755,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -780,46 +790,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -864,14 +868,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1008,7 +1018,79 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "আমদানি"
+
+#~ msgid "Amount paid"
+#~ msgstr ""
+
+#~ msgid "Bills can't be null"
+#~ msgstr ""
+
+#~ msgid "Too many failed login attempts, please retry later."
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr ""
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Catalan (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-09-12 15:25+0000\n"
+"Last-Translator: Maite Guix <maite.guix@gmail.com>\n"
+"Language: ca\n"
 "Language-Team: Catalan <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/ca/>\n"
-"Language: ca\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>La taula següent reflecteix les accions enregistrades abans "
-"de deshabilitar l'historial de projectes. Pots \n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\"> netejar l'historial del projecte</a> per a "
-"eliminar-les.</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Aquest projecte té l'historial deshabilitat. Les accions "
-"noves no apareixeran a continuació. Pots habilitar l'historial a la </i>\n"
-"            <a href=\"%(url)s\">pàgina de configuració</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "«I hate money» és programari lliure"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s cadascun"
 
@@ -108,17 +80,14 @@
 
 msgid "Amount"
 msgstr "Import"
 
 msgid "Amount in %(currency)s"
 msgstr "Import en %(currency)s"
 
-msgid "Amount paid"
-msgstr "Import pagat"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Estàs segur que vols suprimir totes les adreces IP enregistrades d'aquest "
@@ -129,17 +98,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Estàs segur que vols esborrar tot l'historial d'aquest projecte? Aquesta "
 "acció no es pot desfer."
 
-msgid "Are you sure?"
-msgstr "N'estàs segur?"
-
 msgid "Authentication"
 msgstr "Autenticació"
 
 msgid "Back to the list"
 msgstr "Tornar a la llista"
 
 msgid "Balance"
@@ -177,17 +143,14 @@
 
 msgid "Bill items"
 msgstr "Elements de factura"
 
 msgid "Bills"
 msgstr "Factures"
 
-msgid "Bills can't be null"
-msgstr "Les factures no poden ser nul·les"
-
 msgid "Can't remember the password?"
 msgstr "No recordes la contrasenya?"
 
 msgid "Cancel"
 msgstr "Cancel·lar"
 
 msgid ""
@@ -390,26 +353,14 @@
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
 "L'enregistrament d'adreces IP es pot habilitar a la pàgina de configuració"
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
-msgid "Import"
-msgstr "Importar"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Importar el fitxer JSON anteriorment exportat"
-
-msgid "Invalid JSON"
-msgstr "JSON no vàlid"
-
 msgid "Invalid private code."
 msgstr "Codi privat no vàlid."
 
 msgid "Invalid token"
 msgstr "Testimoni no vàlid"
 
 msgid "Invite people"
@@ -668,31 +619,14 @@
 msgstr ""
 "Algunes de les entrades següents contenen adreces IP, tot i que aquest "
 "projecte té l'enregistrament IP deshabilitat. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Probablement algú ha netejat l'historial del projecte."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Ho sentim, s'ha produït un error en enviar-te un correu electrònic amb "
-"instruccions de restabliment de la contrasenya. Comprova la configuració de "
-"correu electrònic del servidor o posa't en contacte amb l'administrador."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Ho sentim, s'ha produït un error en intentar enviar els correus electrònics "
-"d'invitació. Comprova la configuració de correu electrònic del servidor o "
-"posa't en contacte amb l'administrador."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Ho sentim, no hem pogut trobar la pàgina que has demanat."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -735,17 +669,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "El correu electrònic %(email)s no és vàlid"
 
 msgid "The participant name is invalid"
 msgstr "El nom del participant no és vàlid"
 
-msgid "The project identifier is %(project)s"
-msgstr "L'identificador del projecte és %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "El projecte al qual estàs intentant accedir no existeix, vols"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Aquesta contrasenya d'administrador no és la correcta. Només queden %(num)d "
 "intents."
@@ -772,17 +703,14 @@
 
 msgid "Time"
 msgstr "Hora"
 
 msgid "To whom?"
 msgstr "A qui?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Massa intents d'inici de sessió fallits, torna-ho a provar més tard."
-
 msgid "Try out the demo"
 msgstr "Prova la demo"
 
 msgid "Unknown error"
 msgstr "Error desconegut"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ca/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/ca/LC_MESSAGES/messages.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-29 18:51+0200\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-09-12 15:25+0000\n"
 "Last-Translator: Maite Guix <maite.guix@gmail.com>\n"
-"Language-Team: Catalan <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/ca/>\n"
 "Language: ca\n"
+"Language-Team: Catalan <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/ca/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
+"Generated-By: Babel 2.9.0\n"
+
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Acabes de crear '%(project)s' per a compartir les teves despeses"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
-"No és un import o expressió vàlida. Només s'accepten números i els operadors "
-"+ - * /."
+"No és un import o expressió vàlida. Només s'accepten números i els "
+"operadors + - * /."
 
 msgid "Project name"
 msgstr "Nom del projecte"
 
 msgid "New private code"
 msgstr "Codi privat nou"
 
@@ -47,22 +52,19 @@
 "L'establiment d'una moneda predeterminada permet la conversió de moneda "
 "entre factures"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Aquest projecte no es pot definir com a «cap moneda» perquè conté factures "
-"en diverses monedes."
+"Aquest projecte no es pot definir com a «cap moneda» perquè conté "
+"factures en diverses monedes."
 
-msgid "Import previously exported JSON file"
-msgstr "Importar el fitxer JSON anteriorment exportat"
-
-msgid "Import"
-msgstr "Importar"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identificador del projecte"
 
 msgid "Private code"
 msgstr "Codi privat"
 
@@ -70,16 +72,16 @@
 msgstr "Crear projecte"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Ja existeix un projecte amb aquest identificador (\"%(project)s\"). Si us "
-"plau, tria un identificador nou"
+"Ja existeix un projecte amb aquest identificador (\"%(project)s\"). Si us"
+" plau, tria un identificador nou"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr "En quina moneda: euro o petrodòlar?"
 
 msgid "euro"
 msgstr "euro"
 
@@ -115,25 +117,25 @@
 
 msgid "Password confirmation"
 msgstr "Confirmació de contrasenya"
 
 msgid "Reset password"
 msgstr "Restablir la contrasenya"
 
-msgid "Date"
-msgstr "Data"
+msgid "When?"
+msgstr "Quan?"
 
 msgid "What?"
 msgstr "Què?"
 
-msgid "Payer"
-msgstr "Pagador"
+msgid "Who paid?"
+msgstr "Qui va pagar?"
 
-msgid "Amount paid"
-msgstr "Import pagat"
+msgid "How much?"
+msgstr "Quant?"
 
 msgid "Currency"
 msgstr "Moneda"
 
 msgid "External link"
 msgstr "Enllaç extern"
 
@@ -149,17 +151,14 @@
 msgid "Submit and add a new one"
 msgstr "Enviar i afegir-ne un de nou"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Moneda predeterminada del projecte: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Les factures no poden ser nul·les"
-
 msgid "Name"
 msgstr "Nom"
 
 msgid "Weights should be positive"
 msgstr "Els pesos han de ser positius"
 
 msgid "Weight"
@@ -173,21 +172,36 @@
 
 msgid "This project already have this participant"
 msgstr "Aquest projecte ja compta amb aquest participant"
 
 msgid "People to notify"
 msgstr "Gent a notificar"
 
-msgid "Send invites"
-msgstr "Enviar invitacions"
+msgid "Send the invitations"
+msgstr "Enviar les invitacions"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "El correu electrònic %(email)s no és vàlid"
 
+msgid "Logout"
+msgstr "Tancar sessió"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Ho sentim, s'ha produït un error en intentar enviar els correus "
+"electrònics d'invitació. Comprova la configuració de correu electrònic "
+"del servidor o posa't en contacte amb l'administrador."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} i {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, i {end_object}"
@@ -207,102 +221,101 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Massa intents d'inici de sessió fallits, torna-ho a provar més tard."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"Aquesta contrasenya d'administrador no és la correcta. Només queden %(num)d "
-"intents."
+"Aquesta contrasenya d'administrador no és la correcta. Només queden "
+"%(num)d intents."
 
 msgid "Provided token is invalid"
 msgstr "El testimoni proporcionat no és vàlid"
 
 msgid "This private code is not the right one"
 msgstr "Aquest codi privat no és el correcte"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Acabes de crear '%(project)s' per a compartir les teves despeses"
-
 msgid "A reminder email has just been sent to you"
 msgstr "T'acaben d'enviar un correu electrònic de recordatori"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Hem intentat enviar-vos un correu electrònic de recordatori, però s'ha "
 "produït un error. Encara podeu utilitzar el projecte amb normalitat."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "L'identificador del projecte és %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Ho sentim, s'ha produït un error en enviar-te un correu electrònic amb "
-"instruccions de restabliment de la contrasenya. Comprova la configuració de "
-"correu electrònic del servidor o posa't en contacte amb l'administrador."
+"instruccions de restabliment de la contrasenya. Comprova la configuració "
+"de correu electrònic del servidor o posa't en contacte amb "
+"l'administrador."
 
 msgid "No token provided"
 msgstr "No s'ha proporcionat cap testimoni"
 
 msgid "Invalid token"
 msgstr "Testimoni no vàlid"
 
 msgid "Unknown project"
 msgstr "Projecte desconegut"
 
 msgid "Password successfully reset."
 msgstr "La contrasenya s'ha restablert correctament."
 
-msgid "Project successfully uploaded"
-msgstr "El projecte s'ha penjat correctament"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON no vàlid"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"No es poden afegir factures en diverses monedes a un projecte sense moneda "
-"predeterminada"
+"No es poden afegir factures en diverses monedes a un projecte sense "
+"moneda predeterminada"
+
+msgid "Project successfully uploaded"
+msgstr "El projecte s'ha penjat correctament"
 
 msgid "Project successfully deleted"
 msgstr "El projecte s'ha suprimit correctament"
 
 msgid "Error deleting project"
 msgstr "S'ha produït un error en suprimir el projecte"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "T'han convidat a compartir les teves despeses per a %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "S'han enviat les teves invitacions"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
-"Ho sentim, s'ha produït un error en intentar enviar els correus electrònics "
-"d'invitació. Comprova la configuració de correu electrònic del servidor o "
-"posa't en contacte amb l'administrador."
+"Ho sentim, s'ha produït un error en intentar enviar els correus "
+"electrònics d'invitació. Comprova la configuració de correu electrònic "
+"del servidor o posa't en contacte amb l'administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "S'ha afegit %(member)s"
 
 msgid "Error activating participant"
 msgstr "S'ha produït un error en activar el participant"
@@ -315,16 +328,16 @@
 msgstr "S'ha produït un error en eliminar el participant"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"El participant «%(name)s» ha estat desactivat. Continuarà apareixent a la "
-"llista fins que el seu saldo arribi a zero."
+"El participant «%(name)s» ha estat desactivat. Continuarà apareixent a la"
+" llista fins que el seu saldo arribi a zero."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "S'ha eliminat el participant '%(name)s'"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -338,14 +351,18 @@
 
 msgid "The bill has been deleted"
 msgstr "La factura s'ha suprimit"
 
 msgid "The bill has been modified"
 msgstr "La factura ha estat modificada"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "S'ha produït un error en suprimir l'historial del projecte"
 
 msgid "Deleted project history."
 msgstr "S'ha suprimit l'historial del projecte."
 
 msgid "Error deleting recorded IP addresses"
@@ -398,43 +415,35 @@
 
 msgid "Actions"
 msgstr "Accions"
 
 msgid "edit"
 msgstr "editar"
 
-msgid "delete"
-msgstr "suprimir"
+msgid "Delete project"
+msgstr "Suprimir el projecte"
 
 msgid "show"
 msgstr "mostrar"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "El panell està desactivat actualment."
 
 msgid "Download Mobile Application"
 msgstr "Descarregar l'aplicació mòbil"
 
 msgid "Get it on"
 msgstr "Aconsegueix-ho"
 
-msgid "Are you sure?"
-msgstr "N'estàs segur?"
-
 msgid "Edit project"
 msgstr "Editar el projecte"
 
-msgid "Delete project"
-msgstr "Suprimir el projecte"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Choose file"
-msgstr "Triar fitxer"
+#, fuzzy
+msgid "Import project"
+msgstr "Editar el projecte"
 
 msgid "Download project's data"
 msgstr "Descarregar les dades del projecte"
 
 msgid "Bill items"
 msgstr "Elements de factura"
 
@@ -442,39 +451,50 @@
 msgstr "Descarregar la llista de factures amb propietari, import, motiu,... "
 
 msgid "Settle plans"
 msgstr "Plans de liquidació"
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
-"Descarregar la llista transaccions necessàries per a liquidar les factures "
-"actuals."
+"Descarregar la llista transaccions necessàries per a liquidar les "
+"factures actuals."
 
 msgid "Can't remember the password?"
 msgstr "No recordes la contrasenya?"
 
 msgid "Cancel"
 msgstr "Cancel·lar"
 
 msgid "Privacy Settings"
 msgstr "Configuració de la privacitat"
 
-msgid "Edit the project"
-msgstr "Editar el projecte"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
-"Això eliminarà totes les factures i tots els participants en aquest projecte!"
+"Això eliminarà totes les factures i tots els participants en aquest "
+"projecte!"
+
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importar el fitxer JSON anteriorment exportat"
+
+msgid "Choose file"
+msgstr "Triar fitxer"
 
 msgid "Edit this bill"
 msgstr "Editar aquesta factura"
 
 msgid "Add a bill"
 msgstr "Afegir una factura"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Tothom"
 
 msgid "No one"
 msgstr "Ningú"
 
 msgid "More options"
@@ -485,17 +505,14 @@
 
 msgid "Edit this participant"
 msgstr "Editar aquest participant"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "eloi.serra@exemple.cat, maria.canut@lloc.com"
 
-msgid "Send the invitations"
-msgstr "Enviar les invitacions"
-
 msgid "Download"
 msgstr "Descarregar"
 
 msgid "Disabled Project History"
 msgstr "Historial del projecte deshabilitat"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -514,34 +531,33 @@
 msgstr "Enregistrament d'adreces IP habilitat"
 
 msgid "History Settings Changed"
 msgstr "S'ha canviat la configuració de l'historial"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr ""
-"Factura %(name)s: %(property_name)s ha canviat de %(before)s a %(after)s"
+msgstr "Factura %(name)s: %(property_name)s ha canviat de %(before)s a %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
 msgstr "Factura %(name)s: %(property_name)s ha canviat a %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirma l'eliminació d'adreces IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
-"Estàs segur que vols suprimir totes les adreces IP enregistrades d'aquest "
-"projecte?\n"
-"                La resta de l'historial del projecte no es veurà afectat. "
-"Aquesta acció no es pot desfer."
+"Estàs segur que vols suprimir totes les adreces IP enregistrades d'aquest"
+" projecte?\n"
+"                La resta de l'historial del projecte no es veurà afectat."
+" Aquesta acció no es pot desfer."
 
 msgid "Confirm deletion"
 msgstr "Confirmar la supressió"
 
 msgid "Close"
 msgstr "Tancar"
 
@@ -557,83 +573,67 @@
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Factura %(name)s: afegida a la llista de propietaris %(owers_list_str)s"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
+msgstr "Factura %(name)s: eliminada de la llista de propietaris %(owers_list_str)s"
+
+msgid "This project has history disabled. New actions won't appear below."
 msgstr ""
-"Factura %(name)s: eliminada de la llista de propietaris %(owers_list_str)s"
 
-#, python-format
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "L'enregistrament d'adreces IP es pot habilitar a la pàgina de configuració"
+
 msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Aquest projecte té l'historial deshabilitat. Les accions "
-"noves no apareixeran a continuació. Pots habilitar l'historial a la </i>\n"
-"            <a href=\"%(url)s\">pàgina de configuració</a>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>La taula següent reflecteix les accions enregistrades abans "
-"de deshabilitar l'historial de projectes. Pots \n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\"> netejar l'historial del projecte</a> per a "
-"eliminar-les.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Probablement algú ha netejat l'historial del projecte."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Algunes de les entrades següents contenen adreces IP, tot i que aquest "
 "projecte té l'enregistrament IP deshabilitat. "
 
 msgid "Delete stored IP addresses"
 msgstr "Suprimir les adreces IP emmagatzemades"
 
-msgid "No history to erase"
-msgstr "No hi ha historial a esborrar"
-
-msgid "Clear Project History"
-msgstr "Netejar l'historial del projecte"
-
 msgid "No IP Addresses to erase"
 msgstr "No hi ha adreces IP a esborrar"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Suprimir les adreces IP emmagatzemades"
 
+msgid "No history to erase"
+msgstr "No hi ha historial a esborrar"
+
+msgid "Clear Project History"
+msgstr "Netejar l'historial del projecte"
+
 msgid "Time"
 msgstr "Hora"
 
 msgid "Event"
 msgstr "Esdeveniment"
 
 msgid "IP address recording can be enabled on the settings page"
-msgstr ""
-"L'enregistrament d'adreces IP es pot habilitar a la pàgina de configuració"
+msgstr "L'enregistrament d'adreces IP es pot habilitar a la pàgina de configuració"
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
-"L'enregistrament d'adreces IP es pot deshabilitar a la pàgina de configuració"
+"L'enregistrament d'adreces IP es pot deshabilitar a la pàgina de "
+"configuració"
 
 msgid "From IP"
 msgstr "Des d'IP"
 
 #, python-format
 msgid "Project %(name)s added"
 msgstr "S'ha afegit el projecte %(name)s"
@@ -651,16 +651,15 @@
 
 #, python-format
 msgid "Project renamed to %(new_project_name)s"
 msgstr "S'ha canviat el nom del projecte a %(new_project_name)s"
 
 #, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr ""
-"El correu electrònic de contacte del projecte ha canviat a %(new_email)s"
+msgstr "El correu electrònic de contacte del projecte ha canviat a %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "S'ha modificat la configuració del projecte"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
 msgstr "S'ha desactivat el participant %(name)s"
@@ -675,20 +674,25 @@
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Factura %(name)s ha canviat el nom a %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr ""
-"Participant %(name)s: el pes ha canviat de %(old_weight)s a %(new_weight)s"
+msgstr "Participant %(name)s: el pes ha canviat de %(old_weight)s a %(new_weight)s"
+
+msgid "Payer"
+msgstr "Pagador"
 
 msgid "Amount"
 msgstr "Import"
 
+msgid "Date"
+msgstr "Data"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Import en %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Factura %(name)s modificada"
@@ -753,16 +757,16 @@
 msgid "Create"
 msgstr "Crear"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
-"No reutilitzis una contrasenya personal. Tria un codi privat i envia'l als "
-"teus amics"
+"No reutilitzis una contrasenya personal. Tria un codi privat i envia'l "
+"als teus amics"
 
 msgid "Account manager"
 msgstr "Gestor de comptes"
 
 msgid "Bills"
 msgstr "Factures"
 
@@ -792,16 +796,17 @@
 
 msgid "switch to"
 msgstr "commutar a"
 
 msgid "Dashboard"
 msgstr "Panell"
 
-msgid "Logout"
-msgstr "Tancar sessió"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Codi"
 
 msgid "Mobile Application"
 msgstr "Aplicació mòbil"
 
@@ -826,46 +831,40 @@
 
 msgid "you sure?"
 msgstr "n'estàs segur?"
 
 msgid "Invite people"
 msgstr "Convidar gent"
 
-msgid "You should start by adding participants"
-msgstr "Hauries de començar afegint participants"
-
-msgid "Add a new bill"
-msgstr "Afegir una factura nova"
-
 msgid "Newer bills"
 msgstr "Factures més noves"
 
 msgid "Older bills"
 msgstr "Factures més antigues"
 
-msgid "When?"
-msgstr "Quan?"
+msgid "You should start by adding participants"
+msgstr "Hauries de començar afegint participants"
 
-msgid "Who paid?"
-msgstr "Qui va pagar?"
+msgid "Add a new bill"
+msgstr "Afegir una factura nova"
 
 msgid "For what?"
 msgstr "Què va pagar?"
 
-msgid "How much?"
-msgstr "Quant?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Afegida el %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Tothom menys %(excluded)s"
 
+msgid "delete"
+msgstr "suprimir"
+
 msgid "No bills"
 msgstr "Sense factures"
 
 msgid "Nothing to list yet."
 msgstr "Res a enumerar encara."
 
 msgid "You probably want to"
@@ -880,16 +879,16 @@
 msgid "Password reminder"
 msgstr "Recordatori de contrasenya"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
-"Se t'ha enviat un enllaç per a restablir la vostra contrasenya, comprova els "
-"teus correus electrònics."
+"Se t'ha enviat un enllaç per a restablir la vostra contrasenya, comprova "
+"els teus correus electrònics."
 
 msgid "Return to home page"
 msgstr "Tornar a la pàgina d'inici"
 
 msgid "Your projects"
 msgstr "Els teus projectes"
 
@@ -902,40 +901,47 @@
 msgid "Share Identifier & code"
 msgstr "Compartir l'identificador i el codi"
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
-"Pots compartir l'identificador del projecte i el codi privat per qualsevol "
-"mitjà de comunicació."
+"Pots compartir l'identificador del projecte i el codi privat per "
+"qualsevol mitjà de comunicació."
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
 msgid "Share the Link"
 msgstr "Compartir l'enllaç"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
-"Pots compartir directament l'enllaç següent a través del teu mitjà preferit"
+"Pots compartir directament l'enllaç següent a través del teu mitjà "
+"preferit"
+
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
 
 msgid "Send via Emails"
 msgstr "Enviar per correu electrònic"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
-"Especifica una llista (separada per comes) dels correus electrònic als que "
-"vols notificar la\n"
-"                creació d'aquest projecte de gestió pressupostària i els hi "
-"enviarem un correu electrònic."
+"Especifica una llista (separada per comes) dels correus electrònic als "
+"que vols notificar la\n"
+"                creació d'aquest projecte de gestió pressupostària i els "
+"hi enviarem un correu electrònic."
 
 msgid "Who pays?"
 msgstr "Qui ha de pagar?"
 
 msgid "To whom?"
 msgstr "A qui?"
 
@@ -958,7 +964,78 @@
 msgstr "Gastat"
 
 msgid "Expenses by Month"
 msgstr "Despeses per mes"
 
 msgid "Period"
 msgstr "Període"
+
+#~ msgid "Import"
+#~ msgstr "Importar"
+
+#~ msgid "Amount paid"
+#~ msgstr "Import pagat"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Les factures no poden ser nul·les"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "L'identificador del projecte és %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON no vàlid"
+
+#~ msgid "Are you sure?"
+#~ msgstr "N'estàs segur?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importar JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Aquest projecte té l'historial"
+#~ " deshabilitat. Les accions noves no "
+#~ "apareixeran a continuació. Pots habilitar "
+#~ "l'historial a la </i>\n"
+#~ "            <a href=\"%(url)s\">pàgina de configuració</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>La taula següent reflecteix "
+#~ "les accions enregistrades abans de "
+#~ "deshabilitar l'historial de projectes. Pots"
+#~ " \n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\"> netejar l'historial "
+#~ "del projecte</a> per a eliminar-"
+#~ "les.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Enviar invitacions"
+
+#~ msgid " show"
+#~ msgstr "mostrar"
+
+#~ msgid "Edit the project"
+#~ msgstr "Editar el projecte"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Czech (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-11-07 10:07+0000\n"
+"Last-Translator: Moshi Moshi <ifeeltiredboss@gmail.com>\n"
+"Language: cs\n"
 "Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/cs/>\n"
-"Language: cs\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.2\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "A link to an external document, related to this bill"
 msgstr "Externí odkaz k této účtence"
 
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
@@ -25,20 +26,14 @@
 
 msgid "Add"
 msgstr "Přidat"
 
 msgid "Admin password"
 msgstr "Administrátorské heslo"
 
-msgid "Amount paid"
-msgstr "Zaplacená částka"
-
-msgid "Bills can't be null"
-msgstr "Účtenka nemůže být nulová"
-
 msgid "Create the project"
 msgstr "Vytvořit projekt"
 
 msgid "Currency"
 msgstr "Měna"
 
 msgid "Date"
@@ -67,23 +62,14 @@
 
 msgid "For whom?"
 msgstr "Od koho?"
 
 msgid "Get in"
 msgstr "Vstoupit"
 
-msgid "Import"
-msgstr "Import"
-
-msgid "Import previously exported JSON file"
-msgstr "Import exportovaného JSON souboru"
-
-msgid "Invalid JSON"
-msgstr "Neplatný JSON"
-
 msgid "Invalid private code."
 msgstr "Neplatný soukromý přístupový kód."
 
 msgid "Name"
 msgstr "Jméno"
 
 msgid "New private code"
@@ -139,23 +125,14 @@
 
 msgid "Send invites"
 msgstr "Poslat pozvánky"
 
 msgid "Send me the code by email"
 msgstr "Poslat kód na e-mail"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Omlouváme se, během odesílání emailu s instrukcemi pro obnovení hesla se "
-"vyskytla chyba. Zkontrolujte si prosím nastavení vašeho emailového serveru "
-"nebo kontaktujte administrátora."
-
 msgid "Submit"
 msgstr "Odeslat"
 
 msgid "Submit and add a new one"
 msgstr "Odeslat a přidat nový"
 
 msgid "The email %(email)s is not valid"
@@ -167,17 +144,14 @@
 msgstr ""
 "Tento projekt nemůže být nastaven na 'bez měny' protože obsahuje účty v "
 "různých měnáh."
 
 msgid "This project does not exists"
 msgstr "Tento projekt neexistuje"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Příliš mnoho pokusů, zkuste to později."
-
 msgid "Unknown error"
 msgstr "Neznámá chyba"
 
 msgid "Unknown project"
 msgstr "Neznámý projekt"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/cs/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/sr/LC_MESSAGES/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,298 +1,296 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2022-11-07 10:07+0000\n"
-"Last-Translator: Moshi Moshi <ifeeltiredboss@gmail.com>\n"
-"Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/cs/>\n"
-"Language: cs\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2021-04-09 13:26+0000\n"
+"Last-Translator: Rastko Sarcevic <ralesarcevic@gmail.com>\n"
+"Language: sr\n"
+"Language-Team: Serbian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/sr/>\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.2\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
-msgstr "Neplatná částka nebo výraz. Pouze čísla a operátory + - * / jsou přípustná"
+msgstr ""
 
 msgid "Project name"
-msgstr "Název projektu"
+msgstr ""
 
 msgid "New private code"
-msgstr "Nový soukromý kód"
+msgstr ""
 
 msgid "Enter a new code if you want to change it"
-msgstr "Pokud chcete provést změnu vložte nový kód"
+msgstr ""
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Enable project history"
-msgstr "Povolit historii projektu"
+msgstr ""
 
 msgid "Use IP tracking for project history"
-msgstr "Záznam IP adres pro historii projektu"
+msgstr ""
 
 msgid "Default Currency"
-msgstr "Výchozí měna"
+msgstr "Podrazumevana Valuta"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Tento projekt nemůže být nastaven na 'bez měny' protože obsahuje účty v "
-"různých měnáh."
-
-msgid "Import previously exported JSON file"
-msgstr "Import exportovaného JSON souboru"
 
-msgid "Import"
-msgstr "Import"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
-msgstr "Identifikátor projektu"
+msgstr ""
 
 msgid "Private code"
-msgstr "Přístupový kód"
+msgstr ""
 
 msgid "Create the project"
-msgstr "Vytvořit projekt"
+msgstr ""
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Projekt s tímto identifikátorem (\"%(project)s\") již existuje, zvolte "
-"nový identifikátor"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr ""
 
+#, fuzzy
 msgid "euro"
-msgstr ""
+msgstr "Period"
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
-msgstr "Potvrďte smazání vložením soukromého kódu"
+msgstr ""
 
 msgid "Unknown error"
-msgstr "Neznámá chyba"
+msgstr ""
 
 msgid "Invalid private code."
-msgstr "Neplatný soukromý přístupový kód."
+msgstr ""
 
 msgid "Get in"
-msgstr "Vstoupit"
+msgstr ""
 
 msgid "Admin password"
-msgstr "Administrátorské heslo"
+msgstr "Administratorska lozinka"
 
 msgid "Send me the code by email"
-msgstr "Poslat kód na e-mail"
+msgstr "Pošalji mi kod putem email-a"
 
 msgid "This project does not exists"
-msgstr "Tento projekt neexistuje"
+msgstr ""
 
 msgid "Password mismatch"
-msgstr "Heslo nesouhlasí"
+msgstr "Lozinke se ne slažu"
 
 msgid "Password"
-msgstr "Heslo"
+msgstr "Lozinka"
 
 msgid "Password confirmation"
-msgstr "Potvrzení hesla"
+msgstr "Potvrda lozinke"
 
 msgid "Reset password"
-msgstr "Obnova hesla"
+msgstr "Resetuj lozinku"
 
-msgid "Date"
-msgstr "Datum"
+msgid "When?"
+msgstr "Kada?"
 
 msgid "What?"
-msgstr "Co?"
+msgstr ""
 
-msgid "Payer"
-msgstr "Platící"
+msgid "Who paid?"
+msgstr "Ko je platio?"
 
-msgid "Amount paid"
-msgstr "Zaplacená částka"
+msgid "How much?"
+msgstr "Koliko?"
 
 msgid "Currency"
-msgstr "Měna"
+msgstr "Valuta"
 
 msgid "External link"
-msgstr "Externí odkaz"
+msgstr ""
 
 msgid "A link to an external document, related to this bill"
-msgstr "Externí odkaz k této účtence"
+msgstr ""
 
 msgid "For whom?"
-msgstr "Od koho?"
+msgstr "Za koga?"
 
 msgid "Submit"
-msgstr "Odeslat"
+msgstr "Unesi"
 
 msgid "Submit and add a new one"
-msgstr "Odeslat a přidat nový"
+msgstr ""
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr "Výchozí měna projektu: %(currency)s"
-
-msgid "Bills can't be null"
-msgstr "Účtenka nemůže být nulová"
+msgstr ""
 
 msgid "Name"
-msgstr "Jméno"
+msgstr "Ime"
 
 msgid "Weights should be positive"
-msgstr "Váhy musí být kladné"
+msgstr "Težine moraju biti pozitivne"
 
 msgid "Weight"
-msgstr "Váha"
+msgstr "Težina"
 
 msgid "Add"
-msgstr "Přidat"
+msgstr "Dodaj"
 
+#, fuzzy
 msgid "The participant name is invalid"
-msgstr ""
+msgstr "Korisnik %(name)s je uklonjen"
 
-#, fuzzy
 msgid "This project already have this participant"
-msgstr "Projekt již obsahuje tohoto člena"
+msgstr ""
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "Poslat pozvánky"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
-msgstr "Toto (%(email)s) není validní e-mail"
+msgstr "Email %(email)s nije validan"
+
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr "{dual_object_0} a {dual_object_1}"
+msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr "{previous_object}, a {end_object}"
+msgstr ""
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
 msgstr ""
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
 msgstr ""
 
 msgid "No Currency"
-msgstr "Žádná měna"
+msgstr ""
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Příliš mnoho pokusů, zkuste to později."
+msgid "Too many failed login attempts."
+msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
-"Omlouváme se, během odesílání emailu s instrukcemi pro obnovení hesla se "
-"vyskytla chyba. Zkontrolujte si prosím nastavení vašeho emailového "
-"serveru nebo kontaktujte administrátora."
 
-#, fuzzy
 msgid "No token provided"
-msgstr "Nebyl vložen klíč"
+msgstr ""
 
-#, fuzzy
 msgid "Invalid token"
-msgstr "Neplatná klíč"
+msgstr ""
 
 msgid "Unknown project"
-msgstr "Neznámý projekt"
+msgstr ""
 
 msgid "Password successfully reset."
-msgstr "Heslo bylo úspěšné obnoveno."
+msgstr "Lozinka uspešno resetovana."
 
-msgid "Project successfully uploaded"
-msgstr "Projekt byl úspěšně nahrán."
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Neplatný JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
-msgstr "Projekt byl úspěšně smazán"
+msgstr ""
 
 msgid "Error deleting project"
-msgstr "Nastala chyba při mazání projektu"
+msgstr ""
+
+msgid "Unable to logout"
+msgstr ""
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
-msgstr "Vaše pozvánka byla odeslána"
+msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -307,166 +305,170 @@
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
 
-#, python-format
+#, fuzzy, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr ""
+msgstr "Korisnik %(name)s je uklonjen"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr ""
+msgstr "Korisnik %(name)s je uklonjen"
 
 msgid "The bill has been added"
-msgstr ""
+msgstr "Račun je dodat"
 
 msgid "Error deleting bill"
 msgstr ""
 
 msgid "The bill has been deleted"
-msgstr ""
+msgstr "Račun je uklonjen"
 
 msgid "The bill has been modified"
+msgstr "Račun je izmenjen"
+
+#, python-format
+msgid "%(lang)s is not a supported language"
 msgstr ""
 
-#, fuzzy
 msgid "Error deleting project history"
-msgstr "Povolit historii projektu"
+msgstr ""
 
-#, fuzzy
 msgid "Deleted project history."
-msgstr "Povolit historii projektu"
+msgstr ""
 
 msgid "Error deleting recorded IP addresses"
 msgstr ""
 
 msgid "Deleted recorded IP addresses in project history."
 msgstr ""
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr ""
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr ""
 
 msgid "Back to the list"
-msgstr ""
+msgstr "Nazad na listu"
 
 msgid "Administration tasks are currently disabled."
 msgstr ""
 
+#, fuzzy
 msgid "Authentication"
-msgstr ""
+msgstr "Dokumentacija"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 
 msgid "create it"
 msgstr ""
 
 msgid "?"
-msgstr ""
+msgstr "?"
 
 msgid "Create a new project"
 msgstr ""
 
 msgid "Project"
-msgstr "Projekt"
+msgstr "Projekat"
 
 msgid "Number of participants"
 msgstr ""
 
 msgid "Number of bills"
-msgstr ""
+msgstr "Broj računa"
 
 msgid "Newest bill"
-msgstr ""
+msgstr "Najnoviji račun"
 
 msgid "Oldest bill"
-msgstr ""
+msgstr "Najstariji račun"
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
-msgstr ""
+msgstr "izmeni"
 
-msgid "delete"
-msgstr ""
+#, fuzzy
+msgid "Delete project"
+msgstr "ukloni"
 
 msgid "show"
-msgstr ""
+msgstr "prikaži"
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
+#, fuzzy
 msgid "Download Mobile Application"
-msgstr ""
+msgstr "Mobilna Aplikacija"
 
-#, fuzzy
 msgid "Get it on"
-msgstr "Vstoupit"
-
-msgid "Are you sure?"
 msgstr ""
 
 msgid "Edit project"
 msgstr ""
 
 #, fuzzy
-msgid "Delete project"
-msgstr "Vytvořit projekt"
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+msgid "Import project"
+msgstr "ukloni"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
-msgstr ""
+msgstr "Stavke računa"
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr ""
 
 msgid "Settle plans"
 msgstr ""
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
 
 msgid "Can't remember the password?"
 msgstr ""
 
 msgid "Cancel"
-msgstr ""
+msgstr "Otkaži"
 
 msgid "Privacy Settings"
-msgstr ""
+msgstr "Podešavanja Privatnosti"
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
-msgid "Edit this bill"
+msgid "Import previously exported project"
 msgstr ""
 
+msgid "Choose file"
+msgstr "Izaberi fajl"
+
+msgid "Edit this bill"
+msgstr "Izmeni ovaj račun"
+
 msgid "Add a bill"
+msgstr "Dodaj račun"
+
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
 msgstr ""
 
 msgid "Everyone"
-msgstr ""
+msgstr "Svi"
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
 msgstr ""
 
@@ -475,19 +477,16 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
-msgstr ""
+msgstr "Preuzmi"
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr ""
 
@@ -542,75 +541,70 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
-msgstr ""
+msgstr "Vreme"
 
 msgid "Event"
-msgstr ""
+msgstr "Događaj"
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 
 msgid "From IP"
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Project %(name)s added"
-msgstr "Název projektu"
+msgstr ""
 
-#, python-format
+#, fuzzy, python-format
 msgid "Bill %(name)s added"
-msgstr ""
+msgstr "Račun je dodat"
 
 #, python-format
 msgid "Participant %(name)s added"
 msgstr ""
 
 msgid "Project private code changed"
 msgstr ""
@@ -642,36 +636,42 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
-msgid "Amount"
+msgid "Payer"
 msgstr ""
 
+msgid "Amount"
+msgstr "Iznos"
+
+msgid "Date"
+msgstr "Datum"
+
 #, python-format
 msgid "Amount in %(currency)s"
-msgstr ""
+msgstr "Iznos u %(currency)s"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Bill %(name)s modified"
-msgstr ""
+msgstr "Račun je izmenjen"
 
 #, python-format
 msgid "Participant %(name)s modified"
 msgstr ""
 
-#, python-format
+#, fuzzy, python-format
 msgid "Bill %(name)s removed"
-msgstr ""
+msgstr "Korisnik %(name)s je uklonjen"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Participant %(name)s removed"
-msgstr ""
+msgstr "Korisnik %(name)s je uklonjen"
 
 #, python-format
 msgid "Project %(name)s changed in an unknown way"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s changed in an unknown way"
@@ -687,15 +687,15 @@
 msgid "Someone probably cleared the project history."
 msgstr ""
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr ""
 
 msgid "Try out the demo"
-msgstr ""
+msgstr "Isprobaj demo verziju"
 
 msgid "You're sharing a house?"
 msgstr ""
 
 msgid "Going on holidays with friends?"
 msgstr ""
 
@@ -722,57 +722,58 @@
 "your friends"
 msgstr ""
 
 msgid "Account manager"
 msgstr ""
 
 msgid "Bills"
-msgstr ""
+msgstr "Računi"
 
 msgid "Settle"
 msgstr ""
 
 msgid "Statistics"
-msgstr ""
+msgstr "Statistika"
 
 msgid "Languages"
-msgstr ""
+msgstr "Jezici"
 
 msgid "Projects"
 msgstr ""
 
 msgid "Start a new project"
 msgstr ""
 
 msgid "History"
-msgstr ""
+msgstr "Istorija"
 
 msgid "Settings"
-msgstr ""
+msgstr "Podešavanja"
 
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
-msgstr ""
+msgstr "Kod"
 
 msgid "Mobile Application"
-msgstr ""
+msgstr "Mobilna Aplikacija"
 
 msgid "Documentation"
-msgstr ""
+msgstr "Dokumentacija"
 
 msgid "Administation Dashboard"
 msgstr ""
 
 msgid "Legal information"
 msgstr ""
 
@@ -780,53 +781,47 @@
 msgstr ""
 
 msgid "you can contribute and improve it!"
 msgstr ""
 
 #, python-format
 msgid "%(amount)s each"
-msgstr ""
+msgstr "%(amount)s svako"
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
-msgstr ""
+msgstr "Noviji računi"
 
 msgid "Older bills"
-msgstr ""
+msgstr "Stariji računi"
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
-msgstr ""
+msgid "Add a new bill"
+msgstr "Dodaj novi račun"
 
 msgid "For what?"
-msgstr ""
-
-msgid "How much?"
-msgstr ""
+msgstr "Za šta?"
 
 #, python-format
 msgid "Added on %(date)s"
-msgstr ""
+msgstr "Dodato %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
-msgstr ""
+msgstr "Svi osim %(excluded)s"
+
+msgid "delete"
+msgstr "ukloni"
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
@@ -844,21 +839,21 @@
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
 
 msgid "Return to home page"
-msgstr ""
+msgstr "Vrati se na početnu stranu"
 
 msgid "Your projects"
 msgstr ""
 
 msgid "Reset your password"
-msgstr ""
+msgstr "Resetuj lozinku"
 
 msgid "Invite people to join this project"
 msgstr ""
 
 msgid "Share Identifier & code"
 msgstr ""
 
@@ -867,83 +862,73 @@
 "communication means."
 msgstr ""
 
 msgid "Identifier:"
 msgstr ""
 
 msgid "Share the Link"
-msgstr ""
+msgstr "Podelite link"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
 
 msgid "Who pays?"
-msgstr ""
+msgstr "Ko plaća?"
 
 msgid "To whom?"
-msgstr ""
+msgstr "Kome?"
 
 msgid "Who?"
-msgstr ""
+msgstr "Ko?"
 
 msgid "Balance"
-msgstr ""
+msgstr "Stanje"
 
 msgid "deactivate"
 msgstr ""
 
 msgid "reactivate"
 msgstr ""
 
 msgid "Paid"
-msgstr ""
+msgstr "Plaćeno"
 
 msgid "Spent"
-msgstr ""
+msgstr "Potrošeno"
 
 msgid "Expenses by Month"
-msgstr ""
+msgstr "Mesečni troškovi"
 
 msgid "Period"
-msgstr ""
-
-#~ msgid "%(msg_compl)sThe project identifier is %(project)s"
-#~ msgstr ""
-
-#~ msgid "each"
-#~ msgstr ""
-
-#~ msgid "Error while sending reminder email"
-#~ msgstr ""
-
-#~ msgid ""
-#~ "This access code will be sent to"
-#~ " your friends. It is stored as-"
-#~ "is by the server, so don\\'t reuse"
-#~ " a personal password!"
-#~ msgstr ""
+msgstr "Period"
 
 #~ msgid "Participant"
-#~ msgstr "Účastník"
+#~ msgstr "Učesnik"
 
 #~ msgid "Bill"
-#~ msgstr "Účet"
+#~ msgstr "Račun"
 
 #~ msgid "Select all"
-#~ msgstr ""
+#~ msgstr "Izaberi sve"
 
 #~ msgid "Select none"
 #~ msgstr ""
 
 #~ msgid "changed"
 #~ msgstr ""
 
@@ -953,21 +938,21 @@
 #~ msgid "to"
 #~ msgstr ""
 
 #~ msgid "Confirm Delete"
 #~ msgstr ""
 
 #~ msgid "Added"
-#~ msgstr ""
+#~ msgstr "Dodato"
 
 #~ msgid "Removed"
-#~ msgstr ""
+#~ msgstr "Uklonjeno"
 
 #~ msgid "and"
-#~ msgstr ""
+#~ msgstr "i"
 
 #~ msgid "owers list"
 #~ msgstr ""
 
 #~ msgid "added"
 #~ msgstr ""
 
@@ -986,50 +971,125 @@
 #~ msgid "renamed to"
 #~ msgstr ""
 
 #~ msgid "External link changed to"
 #~ msgstr ""
 
 #~ msgid "modified"
-#~ msgstr ""
+#~ msgstr "izmenjeno"
 
 #~ msgid "removed"
-#~ msgstr ""
+#~ msgstr "uklonjeno"
 
 #~ msgid "changed in a unknown way"
 #~ msgstr ""
 
 #~ msgid "You either provided a bad token or no project identifier."
 #~ msgstr ""
 
 #~ msgid "User name incorrect"
-#~ msgstr "Nesprávné uživatelské jméno"
+#~ msgstr ""
+
+#~ msgid "This project already have this member"
+#~ msgstr ""
 
 #~ msgid "People to notify"
-#~ msgstr "Osoby k informování"
+#~ msgstr ""
 
 #~ msgid "Error activating member"
 #~ msgstr ""
 
 #~ msgid "Error removing member"
 #~ msgstr ""
 
 #~ msgid ""
 #~ "User '%(name)s' has been deactivated. It"
 #~ " will still appear in the users "
 #~ "list until its balance becomes zero."
 #~ msgstr ""
 
-#~ msgid "User '%(name)s' has been removed"
-#~ msgstr ""
-
 #~ msgid "User '%(name)s' has been edited"
 #~ msgstr ""
 
 #~ msgid "Number of members"
-#~ msgstr ""
+#~ msgstr "Broj korisnika"
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
+
+#~ msgid "Import previously exported JSON file"
+#~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "Uvezi"
+
+#~ msgid "Amount paid"
+#~ msgstr "Plaćeni iznos"
+
+#~ msgid "Bills can't be null"
+#~ msgstr ""
+
+#~ msgid "Too many failed login attempts, please retry later."
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr ""
+
+#~ msgid " show"
+#~ msgstr "prikaži"
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -9,43 +9,14 @@
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.0-dev\n"
 
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <I>Die folgende Tabelle zeigt alle aufgezeichneten Aktionen "
-"bevor der Projektverlauf deaktiviert wurde. Du kannst den\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">Projektverlauf löschen</a>, um sie zu entfernen.</"
-"i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Der Verlauf dieses Projekts ist deaktiviert. Neue Aktionen "
-"werden nicht im Folgenden auftauchen. Du kannst den Verlauf auf der\n"
-"<a href=\"%(url)s\">Einstellungsseite</a> aktivieren.</i>\n"
-"            "
-
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" ist freie Software"
 
 msgid "%(amount)s each"
 msgstr "jeweils %(amount)s"
 
 msgid "%(member)s has been added"
@@ -171,17 +142,14 @@
 
 msgid "Bill items"
 msgstr "Rechungsposition"
 
 msgid "Bills"
 msgstr "Ausgaben"
 
-msgid "Bills can't be null"
-msgstr "Der Betrag darf nicht null sein"
-
 msgid "Can't remember the password?"
 msgstr "Passwort vergessen?"
 
 msgid "Cancel"
 msgstr "Abbrechen"
 
 msgid ""
@@ -280,17 +248,14 @@
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr "Bilanzübersicht herunterladen."
 
 msgid "Edit project"
 msgstr "Projekt bearbeiten"
 
-msgid "Edit the project"
-msgstr "Projekt bearbeiten"
-
 msgid "Edit this bill"
 msgstr "Ausgabe bearbeiten"
 
 msgid "Edit this participant"
 msgstr "Diesen Benutzer bearbeiten"
 
 msgid "Email"
@@ -335,15 +300,15 @@
 msgid "Event"
 msgstr "Ereignis"
 
 msgid "Everyone"
 msgstr "Jeder"
 
 msgid "Everyone but %(excluded)s"
-msgstr "Jeder außer %(excluded)s"
+msgstr "Alle außer %(excluded)s"
 
 msgid "Expenses by Month"
 msgstr "Ausgaben je Monat"
 
 msgid "External link"
 msgstr "Externer Link"
 
@@ -379,14 +344,17 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "IP-Adresserfassung kann in den Einstellungen aktiviert werden"
 
 msgid "Identifier:"
 msgstr "ID:"
 
+msgid "Import project"
+msgstr "Projekt importieren"
+
 msgid "Invalid private code."
 msgstr "ungültiger privater Code."
 
 msgid "Invalid token"
 msgstr "Ungültiger Token"
 
 msgid "Invite people"
@@ -599,16 +567,16 @@
 
 msgid "Reset your password"
 msgstr "Setze dein Passwort zurück"
 
 msgid "Return to home page"
 msgstr "Zurück zur Hauptseite"
 
-msgid "Send invites"
-msgstr "Einladungen senden"
+msgid "Save changes"
+msgstr "Änderungen speichern"
 
 msgid "Send me the code by email"
 msgstr "Sende mir den Code per E-Mail"
 
 msgid "Send the invitations"
 msgstr "Einladung versenden"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/de/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/de/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2023-07-09 19:50+0000\n"
-"Last-Translator: Sebastian Lay <mail@sebastian-lay.de>\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2023-07-16 14:04+0000\n"
+"Last-Translator: Luke <luke@luporr.de>\n"
 "Language-Team: German <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 5.0-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+"Du hast gerade das Projekt '%(project)s' erstellt, um deine Ausgaben zu "
+"teilen"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Kein gültiger Betrag oder Ausdruck. Es werden nur Zahlen und die "
 "Operatoren + - * / akzeptiert."
 
@@ -51,19 +57,16 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Dieses Projekt kann nicht auf \"ohne Währung\" eingestellt werden, weil "
 "es Rechnungen unterschiedlicher Währungen enthält."
 
-msgid "Import previously exported JSON file"
-msgstr "Zuvor exportierte JSON-Datei importieren"
-
-msgid "Import"
-msgstr "Importieren"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Projektkennung"
 
 msgid "Private code"
 msgstr "Privater Code"
 
@@ -116,25 +119,25 @@
 
 msgid "Password confirmation"
 msgstr "Passwort bestätigen"
 
 msgid "Reset password"
 msgstr "Passwort zurücksetzen"
 
-msgid "Date"
-msgstr "Datum"
+msgid "When?"
+msgstr "Wann?"
 
 msgid "What?"
 msgstr "Was?"
 
-msgid "Payer"
-msgstr "Von"
+msgid "Who paid?"
+msgstr "Wer hat bezahlt?"
 
-msgid "Amount paid"
-msgstr "Betrag"
+msgid "How much?"
+msgstr "Wieviel?"
 
 msgid "Currency"
 msgstr "Währung"
 
 msgid "External link"
 msgstr "Externer Link"
 
@@ -152,17 +155,14 @@
 msgid "Submit and add a new one"
 msgstr "Hinzufügen und neuen erstellen"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Projekt Standardwährung: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Der Betrag darf nicht null sein"
-
 msgid "Name"
 msgstr "Name"
 
 msgid "Weights should be positive"
 msgstr "Die Gewichtungen sollten positiv sein"
 
 msgid "Weight"
@@ -176,21 +176,36 @@
 
 msgid "This project already have this participant"
 msgstr "Der Benutzer ist bereits diesem Projekt zugeordnet"
 
 msgid "People to notify"
 msgstr "Personen, die informiert werden sollen"
 
-msgid "Send invites"
-msgstr "Einladungen senden"
+msgid "Send the invitations"
+msgstr "Einladung versenden"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Die E-Mail-Adresse(n) %(email)s ist/sind nicht gültig"
 
+msgid "Logout"
+msgstr "Ausloggen"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Entschuldigung, es trat ein Fehler beim Versenden der Einladungsmails "
+"auf. Bitte überprüfe die E-Mail Konfiguration des Servers oder "
+"kontaktiere einen Administrator."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} und {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object} und {end_object}"
@@ -210,54 +225,46 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr ""
-"Zu viele fehlgeschlagene Anmeldeversuche, bitte versuche es später nochmal."
+"Zu viele fehlgeschlagene Anmeldeversuche, bitte versuche es später "
+"nochmal."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Das Administrator-Passwort ist nicht korrekt. Noch %(num)d Versuch(e) "
 "verbleibend."
 
 msgid "Provided token is invalid"
 msgstr "Bereitgestelltes Token ist ungültig"
 
 msgid "This private code is not the right one"
 msgstr "Der private Code ist nicht korrekt"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-"Du hast gerade das Projekt '%(project)s' erstellt, um deine Ausgaben zu "
-"teilen"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Dir wurde soeben eine Erinnerungsmail gesendet"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Wir haben versucht dir eine Erinnerungsmail zu senden, aber das hat nicht"
 " geklappt. Du kannst das Projekt weiterhin wie gewohnt nutzen."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Die Projektkennung ist %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Entschuldigung, es trat ein Fehler beim Senden der E-Mail zur Passwort "
 "Zurücksetzung auf. Bitte überprüfe die E-Mail Konfiguration des Servers "
 "oder kontaktiere einen Administrator."
 
 msgid "No token provided"
 msgstr "Kein Token zur Verfügung gestellt"
@@ -267,44 +274,49 @@
 
 msgid "Unknown project"
 msgstr "Unbekanntes Projekt"
 
 msgid "Password successfully reset."
 msgstr "Passwort erfolgreich zurückgesetzt."
 
-msgid "Project successfully uploaded"
-msgstr "Projekt erfolgreich hochgeladen"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Ungültiges JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"Rechnungen in mehreren Währungen können einem Projekt ohne Standardwährung "
-"nicht hinzugefügt werden"
+"Rechnungen in mehreren Währungen können einem Projekt ohne "
+"Standardwährung nicht hinzugefügt werden"
+
+msgid "Project successfully uploaded"
+msgstr "Projekt erfolgreich hochgeladen"
 
 msgid "Project successfully deleted"
 msgstr "Projekt erfolgreich gelöscht"
 
 msgid "Error deleting project"
 msgstr "Fehler bei Projektlöschung"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Du wurdest eingeladen, deine Ausgaben für %(project)s zu teilen"
 
 msgid "Your invitations have been sent"
 msgstr "Deine Einladungen wurden versendet"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Entschuldigung, es trat ein Fehler beim Versenden der Einladungsmails "
 "auf. Bitte überprüfe die E-Mail Konfiguration des Servers oder "
 "kontaktiere einen Administrator."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -344,14 +356,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Die Ausgabe wurde entfernt"
 
 msgid "The bill has been modified"
 msgstr "Die Ausgabe wurde bearbeitet"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Projekthistorie konnte nicht gelöscht werden"
 
 msgid "Deleted project history."
 msgstr "Projekthistorie gelöscht."
 
 msgid "Error deleting recorded IP addresses"
@@ -404,43 +420,34 @@
 
 msgid "Actions"
 msgstr "Aktionen"
 
 msgid "edit"
 msgstr "Bearbeiten"
 
-msgid "delete"
-msgstr "Löschen"
+msgid "Delete project"
+msgstr "Projekt löschen"
 
 msgid "show"
 msgstr "Zeigen"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Das Dashboard ist aktuell deaktiviert."
 
 msgid "Download Mobile Application"
 msgstr "Handy-Applikation herunterladen"
 
 msgid "Get it on"
 msgstr "Mach mit"
 
-msgid "Are you sure?"
-msgstr "Bist du sicher?"
-
 msgid "Edit project"
 msgstr "Projekt bearbeiten"
 
-msgid "Delete project"
-msgstr "Projekt löschen"
-
-msgid "Import JSON"
-msgstr "JSON importieren"
-
-msgid "Choose file"
-msgstr "Datei auswählen"
+msgid "Import project"
+msgstr "Projekt importieren"
 
 msgid "Download project's data"
 msgstr "Projektdaten herunterladen"
 
 msgid "Bill items"
 msgstr "Rechungsposition"
 
@@ -458,26 +465,36 @@
 
 msgid "Cancel"
 msgstr "Abbrechen"
 
 msgid "Privacy Settings"
 msgstr "Datenschutzeinstellungen"
 
-msgid "Edit the project"
-msgstr "Projekt bearbeiten"
+msgid "Save changes"
+msgstr "Änderungen speichern"
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "Dies wird alle Ausgaben und Mitglieder dieses Projektes löschen!"
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Zuvor exportierte JSON-Datei importieren"
+
+msgid "Choose file"
+msgstr "Datei auswählen"
+
 msgid "Edit this bill"
 msgstr "Ausgabe bearbeiten"
 
 msgid "Add a bill"
 msgstr "Ausgabe hinzufügen"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Jeder"
 
 msgid "No one"
 msgstr "Keiner"
 
 msgid "More options"
@@ -488,17 +505,14 @@
 
 msgid "Edit this participant"
 msgstr "Diesen Benutzer bearbeiten"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "max.mustermann@beispiel.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "Einladung versenden"
-
 msgid "Download"
 msgstr "Herunterladen"
 
 msgid "Disabled Project History"
 msgstr "Projektverlauf deaktivieren"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -563,67 +577,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Rechnung %(name)s: %(owers_list_str)s zur Eigentümerliste hinzugefügt"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Rechnung %(name)s: %(owers_list_str)s von der Eigentümerliste entfernt"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Der Verlauf dieses Projekts ist deaktiviert. Neue Aktionen"
-" werden nicht im Folgenden auftauchen. Du kannst den Verlauf auf der\n"
-"<a href=\"%(url)s\">Einstellungsseite</a> aktivieren.</i>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "IP-Adresserfassung kann in den Einstellungen aktiviert werden"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <I>Die folgende Tabelle zeigt alle aufgezeichneten Aktionen "
-"bevor der Projektverlauf deaktiviert wurde. Du kannst den\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">Projektverlauf löschen</a>, um sie zu "
-"entfernen.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Wahrscheinlich hat jemand den Projektverlauf gelöscht."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Einige der folgenden Einträge enthalten IP-Adressen, wenngleich die IP-"
 "Erfassung dieses Projekts deaktiviert ist. "
 
 msgid "Delete stored IP addresses"
 msgstr "Gespeicherte IP-Adressen löschen"
 
-msgid "No history to erase"
-msgstr "Kein Verlauf zu löschen"
-
-msgid "Clear Project History"
-msgstr "Projektverlauf löschen"
-
 msgid "No IP Addresses to erase"
 msgstr "Keine IP-Adressen zu löschen"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Gespeicherte IP-Adressen löschen"
 
+msgid "No history to erase"
+msgstr "Kein Verlauf zu löschen"
+
+msgid "Clear Project History"
+msgstr "Projektverlauf löschen"
+
 msgid "Time"
 msgstr "Zeit"
 
 msgid "Event"
 msgstr "Ereignis"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -679,17 +678,23 @@
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 "Teinehmer %(name)s: Gewichtung von %(old_weight)s auf %(new_weight)s "
 "geändert"
 
+msgid "Payer"
+msgstr "Von"
+
 msgid "Amount"
 msgstr "Betrag"
 
+msgid "Date"
+msgstr "Datum"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Betrag in %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Ausgabe %(name)s wurde bearbeitet"
@@ -793,16 +798,17 @@
 
 msgid "switch to"
 msgstr "wechseln zu"
 
 msgid "Dashboard"
 msgstr "Dashboard"
 
-msgid "Logout"
-msgstr "Ausloggen"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Code"
 
 msgid "Mobile Application"
 msgstr "Handy-Applikation"
 
@@ -827,45 +833,39 @@
 
 msgid "you sure?"
 msgstr "Bist du sicher?"
 
 msgid "Invite people"
 msgstr "Leute einladen"
 
-msgid "You should start by adding participants"
-msgstr "Du kannst anfangen, Teilnehmer hinzuzufügen"
-
-msgid "Add a new bill"
-msgstr "Neue Ausgabe"
-
 msgid "Newer bills"
 msgstr "Aktuellere Rechnungen"
 
 msgid "Older bills"
 msgstr "Ältere Rechnungen"
 
-msgid "When?"
-msgstr "Wann?"
+msgid "You should start by adding participants"
+msgstr "Du kannst anfangen, Teilnehmer hinzuzufügen"
 
-msgid "Who paid?"
-msgstr "Wer hat bezahlt?"
+msgid "Add a new bill"
+msgstr "Neue Ausgabe"
 
 msgid "For what?"
 msgstr "Wofür?"
 
-msgid "How much?"
-msgstr "Wieviel?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Hinzugefügt am %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
-msgstr "Jeder außer %(excluded)s"
+msgstr "Alle außer %(excluded)s"
+
+msgid "delete"
+msgstr "Löschen"
 
 msgid "No bills"
 msgstr "Keine Ausgaben"
 
 msgid "Nothing to list yet."
 msgstr "Noch nichts aufzulisten."
 
@@ -915,14 +915,20 @@
 
 msgid "Share the Link"
 msgstr "Link teilen"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Du kannst den folgenden Link direkt über dein bevorzugtes Medium teilen"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Per E-Mail versenden"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1064,7 +1070,76 @@
 #~ msgstr "Anzahl der Teilnehmer"
 
 #~ msgid "Edit this member"
 #~ msgstr "Teilnehmer bearbeiten"
 
 #~ msgid "Participants to notify"
 #~ msgstr "Teilnehmer hinzufügen"
+
+#~ msgid "Import"
+#~ msgstr "Importieren"
+
+#~ msgid "Amount paid"
+#~ msgstr "Betrag"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Der Betrag darf nicht null sein"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Die Projektkennung ist %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Ungültiges JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Bist du sicher?"
+
+#~ msgid "Import JSON"
+#~ msgstr "JSON importieren"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Der Verlauf dieses Projekts "
+#~ "ist deaktiviert. Neue Aktionen werden "
+#~ "nicht im Folgenden auftauchen. Du kannst"
+#~ " den Verlauf auf der\n"
+#~ "<a href=\"%(url)s\">Einstellungsseite</a> aktivieren.</i>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <I>Die folgende Tabelle zeigt "
+#~ "alle aufgezeichneten Aktionen bevor der "
+#~ "Projektverlauf deaktiviert wurde. Du kannst"
+#~ " den\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">Projektverlauf löschen</a>, "
+#~ "um sie zu entfernen.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Einladungen senden"
+
+#~ msgid " show"
+#~ msgstr "Zeigen"
+
+#~ msgid "Edit the project"
+#~ msgstr "Projekt bearbeiten"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2021-08-01 08:34+0000\n"
 "Last-Translator: Eugenia Russell <eugenia.russell2019@gmail.com>\n"
 "Language: el\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/el/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s έχει προστεθεί"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s είναι και πάλι μέρος αυτού του έργου"
 
@@ -58,26 +58,20 @@
 
 msgid "Amount"
 msgstr "Ποσό"
 
 msgid "Amount in %(currency)s"
 msgstr "Ποσό σε %(currency)s"
 
-msgid "Amount paid"
-msgstr "Καταβληθέν ποσό"
-
 msgid "Back to the list"
 msgstr "Επιστροφή στη λίστα"
 
 msgid "Bill items"
 msgstr "Στοιχεία λογαριασμού"
 
-msgid "Bills can't be null"
-msgstr "Οι λογαριασμοί δεν μπορούν να είναι μηδενικοί"
-
 msgid "Can't remember the password?"
 msgstr "Δεν μπορείτε να θυμηθείτε τον κωδικό πρόσβασης;"
 
 msgid "Cancel"
 msgstr "Ακύρωση"
 
 msgid "Choose file"
@@ -175,26 +169,14 @@
 
 msgid "Get in"
 msgstr "Συνδεθείτε"
 
 msgid "History Settings Changed"
 msgstr "Αλλαγή ρυθμίσεων ιστορικού"
 
-msgid "Import"
-msgstr "Εισαγωγή"
-
-msgid "Import JSON"
-msgstr "Εισαγωγή JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Εισαγωγή αρχείου JSON που έχει εξαχθεί προηγουμένως"
-
-msgid "Invalid JSON"
-msgstr "Η JSON δεν είναι έγκυρη"
-
 msgid "Invalid token"
 msgstr "Το διακριτικό δεν είναι έγκυρο"
 
 msgid "Name"
 msgstr "Όνομα"
 
 msgid "Newest bill"
@@ -317,17 +299,14 @@
 
 msgid "The bill has been modified"
 msgstr "Ο λογαριασμός έχει τροποποιηθεί"
 
 msgid "The email %(email)s is not valid"
 msgstr "Το μήνυμα ηλεκτρονικού ταχυδρομείου %(email)s δεν είναι έγκυρο"
 
-msgid "The project identifier is %(project)s"
-msgstr "Το αναγνωριστικό έργου είναι %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 "Το έργο στο οποίο προσπαθείτε να αποκτήσετε πρόσβαση δεν υπάρχει, θέλετε να"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Αυτός ο κωδικός διαχειριστή δεν είναι σωστός. Μένουν μόνο %(num)d "
@@ -345,18 +324,14 @@
 
 msgid "This project does not exists"
 msgstr "Το έργο αυτό δεν υφίσταται"
 
 msgid "Time"
 msgstr "Ώρα"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Πάρα πολλές αποτυχημένες προσπάθειες σύνδεσης, δοκιμάστε ξανά αργότερα."
-
 msgid "Unknown project"
 msgstr "Άγνωστο πρότζεκτ"
 
 msgid "Use IP tracking for project history"
 msgstr "Χρήση παρακολούθησης IP για ιστορικό έργων"
 
 msgid ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/el/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/el/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2021-08-01 08:34+0000\n"
 "Last-Translator: Eugenia Russell <eugenia.russell2019@gmail.com>\n"
 "Language: el\n"
 "Language-Team: Greek <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/el/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr "Τίτλος εργασίας"
@@ -48,19 +52,16 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Αυτό το έργο δεν μπορεί να οριστεί σε \"χωρίς νόμισμα\" επειδή περιέχει "
 "λογαριασμούς σε πολλαπλά νομίσματα."
 
-msgid "Import previously exported JSON file"
-msgstr "Εισαγωγή αρχείου JSON που έχει εξαχθεί προηγουμένως"
-
-msgid "Import"
-msgstr "Εισαγωγή"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Αναγνωριστικό έργου"
 
 msgid "Private code"
 msgstr "Ιδιωτικός κωδικός"
 
@@ -116,25 +117,25 @@
 
 msgid "Password confirmation"
 msgstr "Επιβεβαίωση κωδικού πρόσβασης"
 
 msgid "Reset password"
 msgstr "Επαναφορά κωδικού πρόσβασης"
 
-msgid "Date"
-msgstr "Ημερομηνία"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "Τι?"
 
-msgid "Payer"
-msgstr "Φορέας πληρωμής"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "Καταβληθέν ποσό"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "Νόμισμα"
 
 msgid "External link"
 msgstr "Εξωτερική σύνδεση"
 
@@ -152,17 +153,14 @@
 msgid "Submit and add a new one"
 msgstr "Υποβολή και προσθήκη νέου"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Προεπιλογή έργου: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Οι λογαριασμοί δεν μπορούν να είναι μηδενικοί"
-
 msgid "Name"
 msgstr "Όνομα"
 
 msgid "Weights should be positive"
 msgstr "Τα βάρη πρέπει να είναι θετικά"
 
 msgid "Weight"
@@ -178,21 +176,33 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "Αυτό το έργο έχει ήδη αυτό το μέλος"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "Αποστολή προσκλήσεων"
+msgid "Send the invitations"
+msgstr "Αποστολή των προσκλήσεων"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Το μήνυμα ηλεκτρονικού ταχυδρομείου %(email)s δεν είναι έγκυρο"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -212,93 +222,89 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Πάρα πολλές αποτυχημένες προσπάθειες σύνδεσης, δοκιμάστε ξανά αργότερα."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Αυτός ο κωδικός διαχειριστή δεν είναι σωστός. Μένουν μόνο %(num)d "
 "προσπάθειες."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "Αυτός ο ιδιωτικός κωδικός δεν είναι ο σωστός"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr "Ένα εμάιλ υπενθύμισης μόλις σας στάλθηκε"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Προσπαθήσαμε να σας στείλουμε ένα εμάιλ υπενθύμισης, αλλά υπήρξε ένα "
 "λάθος. Μπορείτε ακόμα να χρησιμοποιήσετε το πρότζεκτ κανονικά."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Το αναγνωριστικό έργου είναι %(project)s"
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr "Δεν παρέχεται διακριτικό"
 
 msgid "Invalid token"
 msgstr "Το διακριτικό δεν είναι έγκυρο"
 
 msgid "Unknown project"
 msgstr "Άγνωστο πρότζεκτ"
 
 msgid "Password successfully reset."
 msgstr "Επαναφορά του κωδικού επιτυχώς."
 
-msgid "Project successfully uploaded"
-msgstr "Έργο που φορτώθηκε επιτυχώς"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Η JSON δεν είναι έγκυρη"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Έργο που φορτώθηκε επιτυχώς"
+
 msgid "Project successfully deleted"
 msgstr "Το πρότζεκτ διαγράφηκε επιτυχώς"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Έχετε κληθεί να μοιραστείτε τα έξοδά σας για %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Οι προσκλήσεις έχουν σταλθεί"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s έχει προστεθεί"
 
 msgid "Error activating participant"
@@ -333,14 +339,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Ο λογαριασμός έχει διαγραφεί"
 
 msgid "The bill has been modified"
 msgstr "Ο λογαριασμός έχει τροποποιηθεί"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Ενεργοποίηση ιστορικού έργων"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Ενεργοποίηση ιστορικού έργων"
@@ -399,47 +409,38 @@
 
 msgid "Actions"
 msgstr "Ενέργειες"
 
 msgid "edit"
 msgstr "επιμελειθήτε"
 
-msgid "delete"
-msgstr "διαγραφή"
+#, fuzzy
+msgid "Delete project"
+msgstr "Επεξεργασία έργου"
 
 msgid "show"
 msgstr "εμφάνιση"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Ο πίνακας ελέγχου είναι προς το παρόν απενεργοποιημένος."
 
 msgid "Download Mobile Application"
 msgstr ""
 
 #, fuzzy
 msgid "Get it on"
 msgstr "Συνδεθείτε"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "Είστε σίγουρος;"
-
 msgid "Edit project"
 msgstr "Επεξεργασία έργου"
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "Επεξεργασία έργου"
 
-msgid "Import JSON"
-msgstr "Εισαγωγή JSON"
-
-msgid "Choose file"
-msgstr "Επιλογή αρχείου"
-
 msgid "Download project's data"
 msgstr "Κατεβάστε τα δεδομένα του έργου"
 
 msgid "Bill items"
 msgstr "Στοιχεία λογαριασμού"
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -460,26 +461,36 @@
 
 msgid "Cancel"
 msgstr "Ακύρωση"
 
 msgid "Privacy Settings"
 msgstr "Ρυθμίσεις απορρήτου"
 
-msgid "Edit the project"
-msgstr "Επεξεργαστείτε το έργο"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Εισαγωγή αρχείου JSON που έχει εξαχθεί προηγουμένως"
+
+msgid "Choose file"
+msgstr "Επιλογή αρχείου"
+
 msgid "Edit this bill"
 msgstr "Επεξεργαστείτε αυτόν τον λογαριασμό"
 
 msgid "Add a bill"
 msgstr "Προσθήκη λογαριασμού"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -491,17 +502,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "Προσθήκη συμμετέχοντος"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr "Αποστολή των προσκλήσεων"
-
 msgid "Download"
 msgstr "Κατεβάστε"
 
 msgid "Disabled Project History"
 msgstr "Απενεργοποιημένο ιστορικό έργου"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -559,53 +567,49 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
 msgstr ""
 
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Κάποιος πιθανώς διέγραψε το ιστορικό του έργου."
+
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr "Διαγραφή αποθηκευμένων διευθύνσεων IP"
 
-msgid "No history to erase"
-msgstr "Δεν υπάρχει ιστορία για διαγραφή"
-
-msgid "Clear Project History"
-msgstr "Απαλοιφή ιστορικού έργου"
-
 msgid "No IP Addresses to erase"
 msgstr "Δεν υπάρχουν διευθύνσεις IP προς διαγραφή"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Διαγραφή αποθηκευμένων διευθύνσεων IP"
 
+msgid "No history to erase"
+msgstr "Δεν υπάρχει ιστορία για διαγραφή"
+
+msgid "Clear Project History"
+msgstr "Απαλοιφή ιστορικού έργου"
+
 msgid "Time"
 msgstr "Ώρα"
 
 msgid "Event"
 msgstr "Εκδήλωση"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -659,17 +663,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Φορέας πληρωμής"
+
 msgid "Amount"
 msgstr "Ποσό"
 
+msgid "Date"
+msgstr "Ημερομηνία"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Ποσό σε %(currency)s"
 
 #, fuzzy, python-format
 msgid "Bill %(name)s modified"
 msgstr "Ο λογαριασμός έχει τροποποιηθεί"
@@ -771,15 +781,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -806,46 +817,40 @@
 
 msgid "you sure?"
 msgstr "Είστε σίγουρος;"
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr "διαγραφή"
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -890,14 +895,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1013,7 +1024,76 @@
 #~ "είτε δεν δώσατε αναγνωριστικό έργου."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Λανθασμένο όνομα χρήστη"
 
 #~ msgid "People to notify"
 #~ msgstr "Πρόσωπα προς ενημέρωση"
+
+#~ msgid "Import"
+#~ msgstr "Εισαγωγή"
+
+#~ msgid "Amount paid"
+#~ msgstr "Καταβληθέν ποσό"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Οι λογαριασμοί δεν μπορούν να είναι μηδενικοί"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Το αναγνωριστικό έργου είναι %(project)s"
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Η JSON δεν είναι έγκυρη"
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr "Είστε σίγουρος;"
+
+#~ msgid "Import JSON"
+#~ msgstr "Εισαγωγή JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Αποστολή προσκλήσεων"
+
+#~ msgid " show"
+#~ msgstr "εμφάνιση"
+
+#~ msgid "Edit the project"
+#~ msgstr "Επεξεργαστείτε το έργο"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2021-10-01 20:35+0000\n"
 "Last-Translator: phlostically <phlostically@mailinator.com>\n"
 "Language: eo\n"
 "Language-Team: Esperanto <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/eo/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>La ĉi-suba tabelo montras agojn registritajn antaŭ malŝalto "
-"de la projekta historio. Vi povas\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">forviŝi la projektan historion</a> por forigi ilin."
-"</i></ p >\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Historio estis malŝaltita por ĉi tiu projekto. Novaj agoj ne "
-"aperos ĉi-sube. Vi povas ŝalti historion ĉe la</i>\n"
-"            <a href=\"%(url)s\">paĝo pri agordoj</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "«I hate money» estas libera programo"
 
 msgid "%(amount)s each"
 msgstr "po %(amount)s"
 
@@ -109,17 +80,14 @@
 
 msgid "Amount"
 msgstr "Kvanto"
 
 msgid "Amount in %(currency)s"
 msgstr "Kvanto en %(currency)s"
 
-msgid "Amount paid"
-msgstr "Kvanto pagita"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Ĉu vi certe volas forigi ĉiujn registritajn IP-adresojn de ĉi tiu projekto?\n"
@@ -129,32 +97,26 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Ĉu vi certe volas forviŝi ĉiom da historio de ĉi tiu projekto? Ĉi tiu ago "
 "estas malfarebla."
 
-msgid "Are you sure?"
-msgstr "Ĉu vi certas?"
-
 msgid "Back to the list"
 msgstr "Reen al la listo"
 
 msgid "Balance"
 msgstr "Saldo"
 
 msgid "Bill items"
 msgstr "Elementoj de fakturo"
 
 msgid "Bills"
 msgstr "Fakturoj"
 
-msgid "Bills can't be null"
-msgstr "Fakturoj ne povas esti nulaj"
-
 msgid "Can't remember the password?"
 msgstr "Ĉu vi ne memoras la pasvorton?"
 
 msgid "Cancel"
 msgstr "Nuligi"
 
 msgid "Choose file"
@@ -311,26 +273,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "Registrado de IP-adresoj estas ŝaltebla per la agorda paĝo"
 
 msgid "Identifier:"
 msgstr "Identigilo:"
 
-msgid "Import"
-msgstr "Enporti"
-
-msgid "Import JSON"
-msgstr "Enporti JSON-dosieron"
-
-msgid "Import previously exported JSON file"
-msgstr "Importi antaŭe elportitan JSON-dosieron"
-
-msgid "Invalid JSON"
-msgstr "Nevalida JSON"
-
 msgid "Invalid private code."
 msgstr "Nevalida privata kodo."
 
 msgid "Invalid token"
 msgstr "Nevalida ĵetono"
 
 msgid "Invite people"
@@ -514,30 +464,14 @@
 msgstr ""
 "Iuj ĉi-subaj eroj enhavas IP-adresojn, kvankam registrado de IP-adresoj "
 "estis malŝaltita por ĉi tiu projekto. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Iu verŝajne forviŝis la historion de la projekto."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Pardonu, okazis eraro dum sendado al vi de retpoŝta mesaĝo de instrukcioj "
-"pri restarigo de pasvorto. Bonvolu kontroli la retpoŝtan agordon de la "
-"servilo aŭ kontakti la administranton."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Pardonu, okazis eraro dum sendado de la invitoj. Bonvolu kontroli la "
-"retpoŝtan agordon de la servilo aŭ kontakti la administranton."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Pardonu, ni ne povis trovi tiun paĝon, kiun vi petis."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -577,17 +511,14 @@
 
 msgid "The bill has been modified"
 msgstr "La fakturo estis modifita"
 
 msgid "The email %(email)s is not valid"
 msgstr "La retpoŝta adreso %(email)s ne validas"
 
-msgid "The project identifier is %(project)s"
-msgstr "La identigilo de la projekto estas %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Ne ekzistas la projekto, al kiu vi provas aliri. Ĉu vi volas"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Ĉi tiu administra pasvorto ne estas ĝusta. Restas nur %(num)d provoj."
 
 msgid "This private code is not the right one"
@@ -605,17 +536,14 @@
 
 msgid "Time"
 msgstr "Tempo"
 
 msgid "To whom?"
 msgstr "Al kiu?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Tro da malsukcesaj provoj de salutado; bonvolu reprovi poste."
-
 msgid "Try out the demo"
 msgstr "Provu la demonstraĵon"
 
 msgid "Unknown error"
 msgstr "Nekonata eraro"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/eo/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/eo/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2021-10-01 20:35+0000\n"
 "Last-Translator: phlostically <phlostically@mailinator.com>\n"
 "Language: eo\n"
 "Language-Team: Esperanto <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/eo/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Vi ĵus kreis la projekton «%(project)s» por dividi viajn elspezojn"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Ne valida kvanto aŭ esprimo. Nur nombroj kaj la operatoroj + - * / estas "
 "akceptataj."
 
@@ -49,19 +53,16 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Ĉi tiu projekto ne povas esti agordita al «neniu valuto», ĉar ĝi enhavas "
 "fakturojn en pluraj valutoj."
 
-msgid "Import previously exported JSON file"
-msgstr "Importi antaŭe elportitan JSON-dosieron"
-
-msgid "Import"
-msgstr "Enporti"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identigilo de projekto"
 
 msgid "Private code"
 msgstr "Privata kodo"
 
@@ -115,25 +116,25 @@
 
 msgid "Password confirmation"
 msgstr "Konfirmo de pasvorto"
 
 msgid "Reset password"
 msgstr "Restarigi pasvorton"
 
-msgid "Date"
-msgstr "Dato"
+msgid "When?"
+msgstr "Kiam?"
 
 msgid "What?"
 msgstr "Kio?"
 
-msgid "Payer"
-msgstr "Paganto"
+msgid "Who paid?"
+msgstr "Kiu pagis?"
 
-msgid "Amount paid"
-msgstr "Kvanto pagita"
+msgid "How much?"
+msgstr "Kiom?"
 
 msgid "Currency"
 msgstr "Valuto"
 
 msgid "External link"
 msgstr "Ekstera ligo"
 
@@ -149,17 +150,14 @@
 msgid "Submit and add a new one"
 msgstr "Submeti kaj aldoni novan"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Implicita valuto de la projekto: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Fakturoj ne povas esti nulaj"
-
 msgid "Name"
 msgstr "Nomo"
 
 msgid "Weights should be positive"
 msgstr "Pondoj devas esti pozitivaj"
 
 msgid "Weight"
@@ -175,21 +173,35 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "Ĉi tiu projekto jam havas ĉi tiun anon"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "Sendi invitojn"
+msgid "Send the invitations"
+msgstr "Sendi la invitojn"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "La retpoŝta adreso %(email)s ne validas"
 
+msgid "Logout"
+msgstr "Adiaŭi"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Pardonu, okazis eraro dum sendado de la invitoj. Bonvolu kontroli la "
+"retpoŝtan agordon de la servilo aŭ kontakti la administranton."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} kaj {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object} kaj {end_object}"
@@ -209,49 +221,42 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Tro da malsukcesaj provoj de salutado; bonvolu reprovi poste."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Ĉi tiu administra pasvorto ne estas ĝusta. Restas nur %(num)d provoj."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "Ĉi tiu privata kodo ne ĝustas"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Vi ĵus kreis la projekton «%(project)s» por dividi viajn elspezojn"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Rememoriga retpoŝta mesaĝo ĵus estis sendita al vi"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Ni provis sendi al vi rememorigan retpoŝtan mesaĝon, sed okazis eraro. Vi"
 " ankoraŭ povas uzi la projekton normale."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "La identigilo de la projekto estas %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Pardonu, okazis eraro dum sendado al vi de retpoŝta mesaĝo de instrukcioj"
 " pri restarigo de pasvorto. Bonvolu kontroli la retpoŝtan agordon de la "
 "servilo aŭ kontakti la administranton."
 
 msgid "No token provided"
 msgstr "Neniu ĵetono estis provizita"
@@ -261,42 +266,47 @@
 
 msgid "Unknown project"
 msgstr "Nekonata projekto"
 
 msgid "Password successfully reset."
 msgstr "Pasvorto sukcese restarigita."
 
-msgid "Project successfully uploaded"
-msgstr "Projekto sukcese alŝutita"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Nevalida JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Projekto sukcese alŝutita"
+
 msgid "Project successfully deleted"
 msgstr "La projekto estis sukcese forigitaj"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Vi estis invitita dividi viajn elspezojn por %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Viaj invitoj estis senditaj"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Pardonu, okazis eraro dum sendado de la invitoj. Bonvolu kontroli la "
 "retpoŝtan agordon de la servilo aŭ kontakti la administranton."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s estis aldonita"
@@ -335,14 +345,18 @@
 
 msgid "The bill has been deleted"
 msgstr "La fakturo estis forigita"
 
 msgid "The bill has been modified"
 msgstr "La fakturo estis modifita"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Ŝalti projektan historion"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Ŝalti projektan historion"
@@ -400,43 +414,35 @@
 
 msgid "Actions"
 msgstr "Agoj"
 
 msgid "edit"
 msgstr "redakti"
 
-msgid "delete"
-msgstr "forigi"
+msgid "Delete project"
+msgstr "Forviŝi projekton"
 
 msgid "show"
 msgstr "montri"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "La panelo estas nuntempe malaktivigita."
 
 msgid "Download Mobile Application"
 msgstr "Elŝuti programon por poŝaparato"
 
 msgid "Get it on"
 msgstr "Elŝuti ĝin ĉe"
 
-msgid "Are you sure?"
-msgstr "Ĉu vi certas?"
-
 msgid "Edit project"
 msgstr "Redakti projekton"
 
-msgid "Delete project"
-msgstr "Forviŝi projekton"
-
-msgid "Import JSON"
-msgstr "Enporti JSON-dosieron"
-
-msgid "Choose file"
-msgstr "Elekti dosieron"
+#, fuzzy
+msgid "Import project"
+msgstr "Redakti projekton"
 
 msgid "Download project's data"
 msgstr "Elŝuti projektajn datenojn"
 
 msgid "Bill items"
 msgstr "Elementoj de fakturo"
 
@@ -454,26 +460,36 @@
 
 msgid "Cancel"
 msgstr "Nuligi"
 
 msgid "Privacy Settings"
 msgstr "Agordoj pri privateco"
 
-msgid "Edit the project"
-msgstr "Redakti la projekton"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importi antaŭe elportitan JSON-dosieron"
+
+msgid "Choose file"
+msgstr "Elekti dosieron"
+
 msgid "Edit this bill"
 msgstr "Redakti ĉi tiun fakturon"
 
 msgid "Add a bill"
 msgstr "Aldoni fakturon"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Ĉiuj"
 
 msgid "No one"
 msgstr "Neniu"
 
 msgid "More options"
@@ -485,17 +501,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "Aldono partoprenanton"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "johano.zamenhof@example.com, maria.baghy@example.net"
 
-msgid "Send the invitations"
-msgstr "Sendi la invitojn"
-
 msgid "Download"
 msgstr "Elŝuti"
 
 msgid "Disabled Project History"
 msgstr "Projekta historio estas malŝaltita"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -559,67 +572,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "Registrado de IP-adresoj estas ŝaltebla per la agorda paĝo"
+
 msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Historio estis malŝaltita por ĉi tiu projekto. Novaj agoj "
-"ne aperos ĉi-sube. Vi povas ŝalti historion ĉe la</i>\n"
-"            <a href=\"%(url)s\">paĝo pri agordoj</a>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>La ĉi-suba tabelo montras agojn registritajn antaŭ "
-"malŝalto de la projekta historio. Vi povas\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">forviŝi la projektan historion</a> por "
-"forigi ilin.</i></ p >\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Iu verŝajne forviŝis la historion de la projekto."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Iuj ĉi-subaj eroj enhavas IP-adresojn, kvankam registrado de IP-adresoj "
 "estis malŝaltita por ĉi tiu projekto. "
 
 msgid "Delete stored IP addresses"
 msgstr "Forviŝi konservitajn IP-adresojn"
 
-msgid "No history to erase"
-msgstr "Neniom da forviŝebla historio"
-
-msgid "Clear Project History"
-msgstr "Forviŝi historion de projekto"
-
 msgid "No IP Addresses to erase"
 msgstr "Neniom da forviŝeblaj IP-adresoj"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Forviŝi konservitajn IP-adresojn"
 
+msgid "No history to erase"
+msgstr "Neniom da forviŝebla historio"
+
+msgid "Clear Project History"
+msgstr "Forviŝi historion de projekto"
+
 msgid "Time"
 msgstr "Tempo"
 
 msgid "Event"
 msgstr "Evento"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -673,17 +671,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Paganto"
+
 msgid "Amount"
 msgstr "Kvanto"
 
+msgid "Date"
+msgstr "Dato"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Kvanto en %(currency)s"
 
 #, fuzzy, python-format
 msgid "Bill %(name)s modified"
 msgstr "La fakturo estis modifita"
@@ -787,16 +791,17 @@
 
 msgid "switch to"
 msgstr "salti al"
 
 msgid "Dashboard"
 msgstr "Panelo"
 
-msgid "Logout"
-msgstr "Adiaŭi"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Kodo"
 
 msgid "Mobile Application"
 msgstr "Poŝaparata programo"
 
@@ -822,46 +827,40 @@
 
 msgid "you sure?"
 msgstr "ĉu vi certas?"
 
 msgid "Invite people"
 msgstr "Inviti homojn"
 
-msgid "You should start by adding participants"
-msgstr "Vi komencu aldonante partoprenantojn"
-
-msgid "Add a new bill"
-msgstr "Aldoni novan fakturon"
-
 msgid "Newer bills"
 msgstr "Pli novaj fakturoj"
 
 msgid "Older bills"
 msgstr "Pli malnovaj fakturoj"
 
-msgid "When?"
-msgstr "Kiam?"
+msgid "You should start by adding participants"
+msgstr "Vi komencu aldonante partoprenantojn"
 
-msgid "Who paid?"
-msgstr "Kiu pagis?"
+msgid "Add a new bill"
+msgstr "Aldoni novan fakturon"
 
 msgid "For what?"
 msgstr "Por kio?"
 
-msgid "How much?"
-msgstr "Kiom?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Aldonita en %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Ĉiuj krom %(excluded)s"
 
+msgid "delete"
+msgstr "forigi"
+
 msgid "No bills"
 msgstr "Neniu fakturo"
 
 msgid "Nothing to list yet."
 msgstr "Nenio listigebla ankoraŭ."
 
 msgid "You probably want to"
@@ -908,14 +907,20 @@
 
 msgid "Share the Link"
 msgstr "Sendi la ligon"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Vi povas rekte sendi la jenan hiperligon per via preferata komunikilo"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Sendi retpoŝte"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1017,7 +1022,77 @@
 #~ msgstr "Vi donis aŭ nevalidan ĵetonon aŭ neniun identigilon de projekto."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Salutnomo ne ĝustas"
 
 #~ msgid "People to notify"
 #~ msgstr "Sciigotaj homoj"
+
+#~ msgid "Import"
+#~ msgstr "Enporti"
+
+#~ msgid "Amount paid"
+#~ msgstr "Kvanto pagita"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Fakturoj ne povas esti nulaj"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "La identigilo de la projekto estas %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Nevalida JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Ĉu vi certas?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Enporti JSON-dosieron"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Historio estis malŝaltita por"
+#~ " ĉi tiu projekto. Novaj agoj ne "
+#~ "aperos ĉi-sube. Vi povas ŝalti "
+#~ "historion ĉe la</i>\n"
+#~ "            <a href=\"%(url)s\">paĝo pri agordoj</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>La ĉi-suba tabelo montras"
+#~ " agojn registritajn antaŭ malŝalto de "
+#~ "la projekta historio. Vi povas\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">forviŝi la projektan "
+#~ "historion</a> por forigi ilin.</i></ p >"
+#~ "\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Sendi invitojn"
+
+#~ msgid " show"
+#~ msgstr "montri"
+
+#~ msgid "Edit the project"
+#~ msgstr "Redakti la projekton"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Spanish (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-11-14 05:48+0000\n"
+"Last-Translator: Sabtag3 <dioni1984@yahoo.com>\n"
+"Language: es\n"
 "Language-Team: Spanish <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/es/>\n"
-"Language: es\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "A link to an external document, related to this bill"
 msgstr ""
 "Un enlace para un documento externo relacionado con esta cuenta/factura"
 
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
@@ -47,17 +48,14 @@
 
 msgid "Amount"
 msgstr "Cantidad"
 
 msgid "Amount in %(currency)s"
 msgstr "Cantidad en %(currency)s"
 
-msgid "Amount paid"
-msgstr "Cantidad pagada"
-
 msgid "Bills"
 msgstr "Facturas"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid ""
@@ -144,23 +142,14 @@
 
 msgid "History"
 msgstr "Historia"
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
-msgid "Import"
-msgstr "Importar"
-
-msgid "Import previously exported JSON file"
-msgstr "Importar .JSON previamente exportado"
-
-msgid "Invalid JSON"
-msgstr "JSON invalido"
-
 msgid "Invalid private code."
 msgstr "Código privado no válido."
 
 msgid "Invalid token"
 msgstr "Token invalido"
 
 msgid "Languages"
@@ -233,15 +222,15 @@
 msgid "Private code"
 msgstr "Código privado"
 
 msgid "Project"
 msgstr "Proyecto"
 
 msgid "Project default: %(currency)s"
-msgstr "Valor predeterminado del proyecto: %(currency)s%(divisa)s"
+msgstr "Valor predeterminado del proyecto: %(currency)s"
 
 msgid "Project identifier"
 msgstr "Identificador del proyecto"
 
 msgid "Project name"
 msgstr "Nombre del proyecto"
 
@@ -285,31 +274,14 @@
 
 msgid "Share Identifier & code"
 msgstr "Compartir identificador i código"
 
 msgid "Share the Link"
 msgstr "Compartir el enlace"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Lo sentimos, se ha producido un error al enviarle un correo electrónico con "
-"instrucciones para restablecer la contraseña. Compruebe la configuración de "
-"correo electrónico del servidor o póngase en contacto con el administrador."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Lo sentimos, se ha producido un error al intentar enviar los correos "
-"electrónicos de invitación. Compruebe la configuración de correo electrónico "
-"del servidor o póngase en contacto con el administrador."
-
 msgid "Spent"
 msgstr "Gastado"
 
 msgid "Statistics"
 msgstr "Estadísticas"
 
 msgid "Submit"
@@ -320,17 +292,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "El correo %(email)s no es válido"
 
 msgid "The participant name is invalid"
 msgstr "El nombre del participante es invalido"
 
-msgid "The project identifier is %(project)s"
-msgstr "El identificador del proyecto es %(proyecto)s"
-
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta contraseña de administrador no es la correcta. Solo %(num)d intentos "
 "restantes."
 
 msgid "This private code is not the right one"
 msgstr "Este código privado no es el correcto"
@@ -350,19 +319,14 @@
 
 msgid "Time"
 msgstr "Hora"
 
 msgid "To whom?"
 msgstr "¿Para quién?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Demasiados intentos de inicio de sesión fallidos, por favor reinténtelo más "
-"tarde"
-
 msgid "Unknown error"
 msgstr "Error desconocido"
 
 msgid "Unknown project"
 msgstr "Proyecto desconocido"
 
 msgid "Use IP tracking for project history"
@@ -393,18 +357,18 @@
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr "¿Cuál es una moneda real: el euro o el petrodólar?"
 
 msgid "Who?"
 msgstr "¿Quién?"
 
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr "Ha sido invitado a compartir sus gastos para %(proyecto)s"
+msgstr "Ha sido invitado a compartir sus gastos para %(project)s"
 
 msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Acabas de crear '%(proyect)s' para compartir tus gastos"
+msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
 
 msgid "You probably want to"
 msgstr "Probablemente quieras"
 
 msgid "Your invitations have been sent"
 msgstr "Sus invitaciones han sido enviadas"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/es/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/es/LC_MESSAGES/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-11-14 05:48+0000\n"
 "Last-Translator: Sabtag3 <dioni1984@yahoo.com>\n"
-"Language-Team: Spanish <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/es/>\n"
 "Language: es\n"
+"Language-Team: Spanish <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/es/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.15-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Cantidad o expresión no válida. Solo se aceptan números y los operadores "
 "+ - * /."
 
@@ -41,29 +45,26 @@
 msgstr "Usar trackeo IP para historial de proyecto"
 
 msgid "Default Currency"
 msgstr "Moneda por defecto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"Establecer una moneda predeterminada permite la conversión de moneda entre "
-"facturas"
+"Establecer una moneda predeterminada permite la conversión de moneda "
+"entre facturas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Este proyecto no se puede configurar como \"sin moneda\" porque contiene "
 "facturas en varias monedas."
 
-msgid "Import previously exported JSON file"
-msgstr "Importar .JSON previamente exportado"
-
-msgid "Import"
-msgstr "Importar"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identificador del proyecto"
 
 msgid "Private code"
 msgstr "Código privado"
 
@@ -116,25 +117,25 @@
 
 msgid "Password confirmation"
 msgstr "Confirmar contraseña"
 
 msgid "Reset password"
 msgstr "Reestablecer contraseña"
 
-msgid "Date"
-msgstr "Fecha"
+msgid "When?"
+msgstr "¿Cuándo?"
 
 msgid "What?"
 msgstr "¿Qué?"
 
-msgid "Payer"
-msgstr "Pagador"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "Cantidad pagada"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "Divisa"
 
 msgid "External link"
 msgstr "Enlace externo"
 
@@ -150,17 +151,14 @@
 msgid "Submit and add a new one"
 msgstr "Enviar y agregar uno nuevo"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Valor predeterminado del proyecto: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr ""
-
 msgid "Name"
 msgstr "Nombre"
 
 msgid "Weights should be positive"
 msgstr "Los pesos deben ser positivos"
 
 msgid "Weight"
@@ -174,21 +172,36 @@
 
 msgid "This project already have this participant"
 msgstr "Este proyecto ya tiene a este participante"
 
 msgid "People to notify"
 msgstr "Personas a las que notificar"
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "Enviar invitaciones"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "El correo %(email)s no es válido"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Lo sentimos, se ha producido un error al intentar enviar los correos "
+"electrónicos de invitación. Compruebe la configuración de correo "
+"electrónico del servidor o póngase en contacto con el administrador."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{doble_objecto_0} y {doble_objecto_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{objecto_previo}, and {fin_objecto}"
@@ -208,104 +221,103 @@
 msgid "{prefix}: {error}"
 msgstr "{prefijo}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefijo}:<br />{errores}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr ""
-"Demasiados intentos de inicio de sesión fallidos, por favor reinténtelo más "
-"tarde"
+"Demasiados intentos de inicio de sesión fallidos, por favor reinténtelo "
+"más tarde"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"Esta contraseña de administrador no es la correcta. Solo %(num)d intentos "
-"restantes."
+"Esta contraseña de administrador no es la correcta. Solo %(num)d intentos"
+" restantes."
 
 msgid "Provided token is invalid"
 msgstr "El token proporcionado no es válido"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado no es el correcto"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Se te acaba de enviar un email recordatorio"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"Intentamos enviarte un email recordatorio, pero se produjo un error. Puedes "
-"continuar usando el proyecto normalmente"
-
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "El identificador del proyecto es %(project)s"
+"Intentamos enviarte un email recordatorio, pero se produjo un error. "
+"Puedes continuar usando el proyecto normalmente"
 
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
-"Lo sentimos, se ha producido un error al enviarle un correo electrónico con "
-"instrucciones para restablecer la contraseña. Compruebe la configuración de "
-"correo electrónico del servidor o póngase en contacto con el administrador."
+"Lo sentimos, se ha producido un error al enviarle un correo electrónico "
+"con instrucciones para restablecer la contraseña. Compruebe la "
+"configuración de correo electrónico del servidor o póngase en contacto "
+"con el administrador."
 
 msgid "No token provided"
 msgstr "No se proporciona ningún token"
 
 msgid "Invalid token"
 msgstr "Token invalido"
 
 msgid "Unknown project"
 msgstr "Proyecto desconocido"
 
 msgid "Password successfully reset."
 msgstr "La contraseña se restableció correctamente."
 
-msgid "Project successfully uploaded"
-msgstr "Proyecto cargado correctamente"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON invalido"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"No se pueden agregar billetes en varias monedas a un proyecto sin la moneda "
-"predeterminada"
+"No se pueden agregar billetes en varias monedas a un proyecto sin la "
+"moneda predeterminada"
+
+msgid "Project successfully uploaded"
+msgstr "Proyecto cargado correctamente"
 
 msgid "Project successfully deleted"
 msgstr "Proyecto eliminado correctamente"
 
 msgid "Error deleting project"
 msgstr "Error al eliminar el proyecto"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Ha sido invitado a compartir sus gastos para %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Sus invitaciones han sido enviadas"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Lo sentimos, se ha producido un error al intentar enviar los correos "
-"electrónicos de invitación. Compruebe la configuración de correo electrónico "
-"del servidor o póngase en contacto con el administrador."
+"electrónicos de invitación. Compruebe la configuración de correo "
+"electrónico del servidor o póngase en contacto con el administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
 msgstr ""
@@ -339,14 +351,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Habilitar historial del proyecto"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Habilitar historial del proyecto"
@@ -403,45 +419,37 @@
 
 msgid "Actions"
 msgstr "Acciones"
 
 msgid "edit"
 msgstr "editar"
 
-msgid "delete"
-msgstr "eliminar"
+#, fuzzy
+msgid "Delete project"
+msgstr "Editar el proyecto"
 
 msgid "show"
 msgstr "mostrar"
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 #, fuzzy
 msgid "Download Mobile Application"
 msgstr "Aplicación móvil"
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
 #, fuzzy
-msgid "Delete project"
-msgstr "Editar el proyecto"
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+msgid "Import project"
+msgstr "Tus proyectos"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -459,26 +467,36 @@
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Privacy Settings"
 msgstr "Ajustes de privacidad"
 
-msgid "Edit the project"
-msgstr "Editar el proyecto"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importar .JSON previamente exportado"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr "Editar esta factura"
 
 msgid "Add a bill"
 msgstr "Añadir una factura"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -490,17 +508,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "Añadir participante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr "Enviar invitaciones"
-
 msgid "Download"
 msgstr "Descargar"
 
 msgid "Disabled Project History"
 msgstr "Historial del proyecto desactivado"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -557,51 +572,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr "Hora"
 
 msgid "Event"
 msgstr "Evento"
@@ -657,17 +667,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Pagador"
+
 msgid "Amount"
 msgstr "Cantidad"
 
+msgid "Date"
+msgstr "Fecha"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Cantidad en %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -771,15 +787,16 @@
 
 msgid "switch to"
 msgstr "cambiar a"
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Mobile Application"
 msgstr "Aplicación móvil"
@@ -805,46 +822,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
-msgstr "¿Cuándo?"
-
-msgid "Who paid?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "For what?"
+msgid "Add a new bill"
 msgstr ""
 
-msgid "How much?"
+msgid "For what?"
 msgstr ""
 
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr "eliminar"
+
 msgid "No bills"
 msgstr "Sin facturas"
 
 msgid "Nothing to list yet."
 msgstr "No hay nada que mostrar todavía."
 
 msgid "You probably want to"
@@ -889,14 +900,20 @@
 
 msgid "Share the Link"
 msgstr "Compartir el enlace"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1033,7 +1050,60 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr "Editar miembro"
 
 #~ msgid "Participants to notify"
 #~ msgstr "añadir participantes"
+
+#~ msgid "Import"
+#~ msgstr "Importar"
+
+#~ msgid "Amount paid"
+#~ msgstr "Cantidad pagada"
+
+#~ msgid "Bills can't be null"
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "El identificador del proyecto es %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON invalido"
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Enviar invitaciones"
+
+#~ msgid " show"
+#~ msgstr "mostrar"
+
+#~ msgid "Edit the project"
+#~ msgstr "Editar el proyecto"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,23 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Spanish (Latin America) (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-04-11 17:12+0000\n"
+"Last-Translator: Santiago José Gutiérrez Llanos <gutierrezapata17@gmail."
+"com>\n"
+"Language: es_419\n"
 "Language-Team: Spanish (Latin America) <https://hosted.weblate.org/projects/"
 "i-hate-money/i-hate-money/es_419/>\n"
-"Language: es_419\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.12-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Este registro muestra la actividad previa a la desactivación "
-"del historial del proyecto. Use la opción \n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">Eliminar historial del proyecto</a> para borrarlo."
-"</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>El historial de este proyecto ha sido desactivado. Nuevas "
-"operaciones no apareceran a continuacion. El historial se puede agregar</"
-"i> \n"
-"            <a href=\"%(url)s\">en la página de ajustes</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" es un software libre"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s cada uno"
 
@@ -109,17 +81,14 @@
 
 msgid "Amount"
 msgstr "Cantidad"
 
 msgid "Amount in %(currency)s"
 msgstr "Cantidad en %(currency)s"
 
-msgid "Amount paid"
-msgstr "Cantidad pagada"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Por favor confirme la eliminación completa del registro de direcciones IP "
@@ -130,17 +99,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Por favor confirme la eliminación completa del historial del proyecto. Esta "
 "acción es irreversible."
 
-msgid "Are you sure?"
-msgstr "¿Estás segura?"
-
 msgid "Authentication"
 msgstr "Autenticación"
 
 msgid "Back to the list"
 msgstr "Volver a la lista"
 
 msgid "Balance"
@@ -176,17 +142,14 @@
 
 msgid "Bill items"
 msgstr "Elementos de factura"
 
 msgid "Bills"
 msgstr "Facturas"
 
-msgid "Bills can't be null"
-msgstr "Las facturas no pueden ser nulas"
-
 msgid "Can't remember the password?"
 msgstr "¿No recuerdas la contraseña?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid ""
@@ -388,26 +351,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "El registro de direcciones IP se puede activar en la página de ajustes"
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
-msgid "Import"
-msgstr "Importar"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Importar archivo JSON previamente exportado"
-
-msgid "Invalid JSON"
-msgstr "JSON inválido"
-
 msgid "Invalid private code."
 msgstr "Código privado inválido."
 
 msgid "Invalid token"
 msgstr "Token no válido"
 
 msgid "Invite people"
@@ -665,32 +616,14 @@
 msgstr ""
 "Algunos registros contienen direcciones IP, a pesar de que el registro de "
 "direcciones IP del proyecto no está activo. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Es probable que alguien borrara el historial del proyecto."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Lo sentimos, hubo un error al enviarle un correo electrónico con las "
-"instrucciones de restablecimiento de contraseña. Compruebe la configuración "
-"de correo electrónico del servidor o póngase en contacto con el "
-"administrador."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Lo sentimos, hubo un error cuando intentamos enviarle correos de invitación. "
-"Por favor, revise la configuración de correo en el servidor o contactese con "
-"el administrador."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Lo sentimos, no hemos encontrado la página que has solicitado."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -733,17 +666,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "El correo electrónico %(email)s no es válido"
 
 msgid "The participant name is invalid"
 msgstr "El nombre del participante no es válido"
 
-msgid "The project identifier is %(project)s"
-msgstr "El identificador del proyecto es %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "El proyecto al que intentas acceder no existe, ¿quieres"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Esta contraseña de administrador no es la correcta. Solo quedan %(num)d "
 "intentos."
@@ -769,19 +699,14 @@
 
 msgid "Time"
 msgstr "Hora"
 
 msgid "To whom?"
 msgstr "¿A quién?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Demasiados intentos fallidos de inicio de sesión, vuelva a intentarlo más "
-"tarde."
-
 msgid "Try out the demo"
 msgstr "Prueba la demo"
 
 msgid "Unknown error"
 msgstr "Error desconocido"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/es_419/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/es_419/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-04-11 17:12+0000\n"
-"Last-Translator: Santiago José Gutiérrez Llanos <gutierrezapata17@gmail.com>"
-"\n"
-"Language-Team: Spanish (Latin America) <https://hosted.weblate.org/projects/"
-"i-hate-money/i-hate-money/es_419/>\n"
+"Last-Translator: Santiago José Gutiérrez Llanos "
+"<gutierrezapata17@gmail.com>\n"
 "Language: es_419\n"
+"Language-Team: Spanish (Latin America) "
+"<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/es_419/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.12-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "No es una cantidad o expresión válida. Solo se aceptan números y los "
 "operadores + - * /."
 
@@ -42,29 +46,26 @@
 msgstr "Registrar la IPs para el historial del proyecto"
 
 msgid "Default Currency"
 msgstr "Moneda por defecto"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"Establecer una moneda predeterminada permite la conversión de divisas entre "
-"facturas"
+"Establecer una moneda predeterminada permite la conversión de divisas "
+"entre facturas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Este proyecto no se puede establecer en 'ninguna moneda' porque contiene "
 "facturas en varias monedas."
 
-msgid "Import previously exported JSON file"
-msgstr "Importar archivo JSON previamente exportado"
-
-msgid "Import"
-msgstr "Importar"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identificador de proyecto"
 
 msgid "Private code"
 msgstr "Código privado"
 
@@ -117,25 +118,25 @@
 
 msgid "Password confirmation"
 msgstr "Confirmar contraseña"
 
 msgid "Reset password"
 msgstr "Restablecer contraseña"
 
-msgid "Date"
-msgstr "Fecha"
+msgid "When?"
+msgstr "¿Cuando?"
 
 msgid "What?"
 msgstr "¿Qué?"
 
-msgid "Payer"
-msgstr "Paga"
+msgid "Who paid?"
+msgstr "¿Quién pagó?"
 
-msgid "Amount paid"
-msgstr "Cantidad pagada"
+msgid "How much?"
+msgstr "¿Cuánto?"
 
 msgid "Currency"
 msgstr "Moneda"
 
 msgid "External link"
 msgstr "Enlace externo"
 
@@ -151,17 +152,14 @@
 msgid "Submit and add a new one"
 msgstr "Enviar y agregar uno nuevo"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "moneda predeterminada del projecto: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Las facturas no pueden ser nulas"
-
 msgid "Name"
 msgstr "Nombre"
 
 msgid "Weights should be positive"
 msgstr "Los pesos deben ser positivos"
 
 msgid "Weight"
@@ -175,21 +173,36 @@
 
 msgid "This project already have this participant"
 msgstr "Este proyecto ya tiene a este participante"
 
 msgid "People to notify"
 msgstr "Personas para notificar"
 
-msgid "Send invites"
-msgstr "Enviar invitaciones"
+msgid "Send the invitations"
+msgstr "Enviar las invitaciones"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "El correo electrónico %(email)s no es válido"
 
+msgid "Logout"
+msgstr "Cerrar sesión"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Lo sentimos, hubo un error cuando intentamos enviarle correos de "
+"invitación. Por favor, revise la configuración de correo en el servidor o"
+" contactese con el administrador."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} y {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, y {end_object}"
@@ -209,15 +222,16 @@
 msgid "{prefix}: {error}"
 msgstr "{prefijo}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefijo}:<br />{errores}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr ""
 "Demasiados intentos fallidos de inicio de sesión, vuelva a intentarlo más"
 " tarde."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
@@ -226,84 +240,81 @@
 
 msgid "Provided token is invalid"
 msgstr "La muestra proporcionada no es válida"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado no es el correcto"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Acabas de crear '%(project)s' para compartir tus gastos"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Acabamos de enviarte un email de recordatorio"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Te hemos intentado enviar un correo electrónico recordatorio pero ha "
 "habido un error. Todavía puedes usar el proyecto habitualmente."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "El identificador del proyecto es %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Lo sentimos, hubo un error al enviarle un correo electrónico con las "
-"instrucciones de restablecimiento de contraseña. Compruebe la configuración "
-"de correo electrónico del servidor o póngase en contacto con el "
-"administrador."
+"instrucciones de restablecimiento de contraseña. Compruebe la "
+"configuración de correo electrónico del servidor o póngase en contacto "
+"con el administrador."
 
 msgid "No token provided"
 msgstr "No se proporciono ningún token"
 
 msgid "Invalid token"
 msgstr "Token no válido"
 
 msgid "Unknown project"
 msgstr "Proyecto desconocido"
 
 msgid "Password successfully reset."
 msgstr "Contraseña restablecida con éxito."
 
-msgid "Project successfully uploaded"
-msgstr "El proyecto se subió exitosamente"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON inválido"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"No se pueden agregar facturas en varias monedas a un proyecto sin la moneda "
-"predeterminada"
+"No se pueden agregar facturas en varias monedas a un proyecto sin la "
+"moneda predeterminada"
+
+msgid "Project successfully uploaded"
+msgstr "El proyecto se subió exitosamente"
 
 msgid "Project successfully deleted"
 msgstr "Proyecto eliminado correctamente"
 
 msgid "Error deleting project"
 msgstr "Error al borrar poryecto"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Usted ha sido invitado a compartir sus gastos para %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Sus invitaciones han sido enviadas"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Lo sentimos, hubo un error cuando intentamos enviarle correos de "
 "invitación. Por favor, revise la configuración de correo en el servidor o"
 " contactese con el administrador."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -320,16 +331,16 @@
 msgstr "Error eliminando participante"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"El participante '%(name)s' ha sido desactivado. Seguirá apareciendo en la "
-"lista hasta que su saldo llegue a cero."
+"El participante '%(name)s' ha sido desactivado. Seguirá apareciendo en la"
+" lista hasta que su saldo llegue a cero."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "Se ha eliminado al participante '%(name)s'"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -343,14 +354,18 @@
 
 msgid "The bill has been deleted"
 msgstr "La factura ha sido eliminada"
 
 msgid "The bill has been modified"
 msgstr "La factura ha sido modificada"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Error al eliminar el historial del proyecto"
 
 msgid "Deleted project history."
 msgstr "Historial del proyecto eliminada."
 
 msgid "Error deleting recorded IP addresses"
@@ -403,43 +418,35 @@
 
 msgid "Actions"
 msgstr "Acciones"
 
 msgid "edit"
 msgstr "Editar"
 
-msgid "delete"
-msgstr "Eliminar"
+msgid "Delete project"
+msgstr "Borrar proyecto"
 
 msgid "show"
 msgstr "enseñar"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "El panel está desactivado actualmente."
 
 msgid "Download Mobile Application"
 msgstr "Instalar aplicación móvil"
 
 msgid "Get it on"
 msgstr "Conseguir en"
 
-msgid "Are you sure?"
-msgstr "¿Estás segura?"
-
 msgid "Edit project"
 msgstr "Editar proyecto"
 
-msgid "Delete project"
-msgstr "Borrar proyecto"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Choose file"
-msgstr "Escoger un archivo"
+#, fuzzy
+msgid "Import project"
+msgstr "Editar proyecto"
 
 msgid "Download project's data"
 msgstr "Descargar datos del proyecto"
 
 msgid "Bill items"
 msgstr "Elementos de factura"
 
@@ -459,26 +466,36 @@
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Privacy Settings"
 msgstr "Ajustes de privacidad"
 
-msgid "Edit the project"
-msgstr "Editar el proyecto"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "Esto va a remover todas las facturas y participantes en este proyecto!"
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importar archivo JSON previamente exportado"
+
+msgid "Choose file"
+msgstr "Escoger un archivo"
+
 msgid "Edit this bill"
 msgstr "Editar esta factura"
 
 msgid "Add a bill"
 msgstr "Agregar una factura"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "No one"
 msgstr "Ninguno"
 
 msgid "More options"
@@ -489,17 +506,14 @@
 
 msgid "Edit this participant"
 msgstr "Editar este participante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "Enviar las invitaciones"
-
 msgid "Download"
 msgstr "Descargar"
 
 msgid "Disabled Project History"
 msgstr "Historial de proyecto activo"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -518,16 +532,15 @@
 msgstr "Se activó el registros de dirección IP"
 
 msgid "History Settings Changed"
 msgstr "Se cambiaron los ajustes del historial"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr ""
-"Factura %(name)s: %(property_name)s ha cambiado de %(before)s a %(after)s"
+msgstr "Factura %(name)s: %(property_name)s ha cambiado de %(before)s a %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
 msgstr "Factura %(name)s:%(property_name)s ha cambiado a %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar eliminación de direcciones IP"
@@ -563,68 +576,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Factura%(name)s: añadida %(owers_list_str)s a la lista de dueños"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Factura %(name)s: removida %(owers_list_str)s de la lista de dueños"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>El historial de este proyecto ha sido desactivado. Nuevas "
-"operaciones no apareceran a continuacion. El historial se puede "
-"agregar</i> \n"
-"            <a href=\"%(url)s\">en la página de ajustes</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "El registro de direcciones IP se puede activar en la página de ajustes"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Este registro muestra la actividad previa a la "
-"desactivación del historial del proyecto. Use la opción \n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">Eliminar historial del proyecto</a> para "
-"borrarlo.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Es probable que alguien borrara el historial del proyecto."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Algunos registros contienen direcciones IP, a pesar de que el registro de"
 " direcciones IP del proyecto no está activo. "
 
 msgid "Delete stored IP addresses"
 msgstr "Borrar las direcciones IP registradas"
 
-msgid "No history to erase"
-msgstr "No hay historial para borrar"
-
-msgid "Clear Project History"
-msgstr "Borrar el historial del proyecto"
-
 msgid "No IP Addresses to erase"
 msgstr "No hay direcciones IP para borrar"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Borrar direcciones IP registradas"
 
+msgid "No history to erase"
+msgstr "No hay historial para borrar"
+
+msgid "Clear Project History"
+msgstr "Borrar el historial del proyecto"
+
 msgid "Time"
 msgstr "Hora"
 
 msgid "Event"
 msgstr "Evento"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -678,17 +675,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Factura %(name)s renombrada a %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr "Participante %(name)s: peso cambiado de %(old_weight)s a %(new_weight)s"
 
+msgid "Payer"
+msgstr "Paga"
+
 msgid "Amount"
 msgstr "Cantidad"
 
+msgid "Date"
+msgstr "Fecha"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Cantidad en %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "La factura %(name)s ha sido modificada"
@@ -753,16 +756,16 @@
 msgid "Create"
 msgstr "Crear"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
-"No reutilice una contraseña personal. Elija un código privado y envíelo a "
-"sus amigos"
+"No reutilice una contraseña personal. Elija un código privado y envíelo a"
+" sus amigos"
 
 msgid "Account manager"
 msgstr "Gestor de cuentas"
 
 msgid "Bills"
 msgstr "Facturas"
 
@@ -792,16 +795,17 @@
 
 msgid "switch to"
 msgstr "cambiar a"
 
 msgid "Dashboard"
 msgstr "Tablero"
 
-msgid "Logout"
-msgstr "Cerrar sesión"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Mobile Application"
 msgstr "Aplicación móvil"
 
@@ -826,46 +830,40 @@
 
 msgid "you sure?"
 msgstr "¿Estás seguro?"
 
 msgid "Invite people"
 msgstr "Invitar personas"
 
-msgid "You should start by adding participants"
-msgstr "Deberías comenzar agregando participantes"
-
-msgid "Add a new bill"
-msgstr "Añadir una nueva factura"
-
 msgid "Newer bills"
 msgstr "Nuevas facturas"
 
 msgid "Older bills"
 msgstr "Facturas anteriores"
 
-msgid "When?"
-msgstr "¿Cuando?"
+msgid "You should start by adding participants"
+msgstr "Deberías comenzar agregando participantes"
 
-msgid "Who paid?"
-msgstr "¿Quién pagó?"
+msgid "Add a new bill"
+msgstr "Añadir una nueva factura"
 
 msgid "For what?"
 msgstr "¿Para qué?"
 
-msgid "How much?"
-msgstr "¿Cuánto?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Agregado el %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Todo el mundo menos %(excluded)s"
 
+msgid "delete"
+msgstr "Eliminar"
+
 msgid "No bills"
 msgstr "Sin facturas"
 
 msgid "Nothing to list yet."
 msgstr "Aún no hay nada que listar."
 
 msgid "You probably want to"
@@ -916,14 +914,20 @@
 msgstr "Comparte el enlace"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 "Puedes compartir directamente el siguiente enlace a través de tu medio "
 "preferido"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Enviar por correo electrónico"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1048,7 +1052,77 @@
 #~ msgstr "Usted proporcionó un token incorrecto o no identificó el proyecto."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Nombre de usuario incorrecto"
 
 #~ msgid "People to notify"
 #~ msgstr "Personas a notificar"
+
+#~ msgid "Import"
+#~ msgstr "Importar"
+
+#~ msgid "Amount paid"
+#~ msgstr "Cantidad pagada"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Las facturas no pueden ser nulas"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "El identificador del proyecto es %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON inválido"
+
+#~ msgid "Are you sure?"
+#~ msgstr "¿Estás segura?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importar JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>El historial de este "
+#~ "proyecto ha sido desactivado. Nuevas "
+#~ "operaciones no apareceran a continuacion. "
+#~ "El historial se puede agregar</i> \n"
+#~ "            <a href=\"%(url)s\">en la página de ajustes</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Este registro muestra la "
+#~ "actividad previa a la desactivación del"
+#~ " historial del proyecto. Use la "
+#~ "opción \n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">Eliminar historial del "
+#~ "proyecto</a> para borrarlo.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Enviar invitaciones"
+
+#~ msgid " show"
+#~ msgstr "enseñar"
+
+#~ msgid "Edit the project"
+#~ msgstr "Editar el proyecto"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Persian (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2023-03-19 21:40+0000\n"
+"Last-Translator: Sai Mohammad-Hossein Emami <emami@outlook.com>\n"
+"Language: fa\n"
 "Language-Team: Persian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/fa/>\n"
-"Language: fa\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "A link to an external document, related to this bill"
 msgstr "یه لینک به سند خارجی به این قبض مربوطه"
 
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
@@ -25,17 +26,14 @@
 
 msgid "Add"
 msgstr "اضافه"
 
 msgid "Admin password"
 msgstr "گذرواژه‌ی مدیر"
 
-msgid "Bills can't be null"
-msgstr "قبض‌ها نمی‌تونند تهی باشن"
-
 msgid "Create the project"
 msgstr "ساخت پروژه"
 
 msgid "Currency"
 msgstr "واحد پولی"
 
 msgid "Date"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/fa/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/fa/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2023-03-19 21:40+0000\n"
 "Last-Translator: Sai Mohammad-Hossein Emami <emami@outlook.com>\n"
-"Language-Team: Persian <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/fa/>\n"
 "Language: fa\n"
+"Language-Team: Persian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/fa/>\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.16.2-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "مقدار یا عبارت نامعتبر. فقط اعداد و عملیات‌های + - * / مجاز هستند."
 
 msgid "Project name"
 msgstr "نام پروژه"
@@ -47,18 +51,15 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "این پروژه نمی‌تونه به صورت «بدون واحد پولی» تنظیم بشه چون شامل قبوض با "
 "ارزهای مختلفه."
 
-msgid "Import previously exported JSON file"
-msgstr ""
-
-msgid "Import"
+msgid "Compatible with Cospend"
 msgstr ""
 
 msgid "Project identifier"
 msgstr "شناسه پروژه"
 
 msgid "Private code"
 msgstr "کد خصوصی"
@@ -67,16 +68,16 @@
 msgstr "ساخت پروژه"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"پروژه‌ای با شناسه‌ی (\"%(project)s\") از قبل وجود داره. لطفا یه شناسه‌ی جدید "
-"وارد کن"
+"پروژه‌ای با شناسه‌ی (\"%(project)s\") از قبل وجود داره. لطفا یه شناسه‌ی "
+"جدید وارد کن"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr "کدوم یکی واقعا واحد پولیه: یورو یا دلار نفتی؟"
 
 msgid "euro"
 msgstr "یورو"
 
@@ -112,24 +113,24 @@
 
 msgid "Password confirmation"
 msgstr "تایید گذرواژه"
 
 msgid "Reset password"
 msgstr "بازنشانی گذرواژه"
 
-msgid "Date"
-msgstr "تاریخ"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "چی؟"
 
-msgid "Payer"
-msgstr "پرداخت کننده"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
+msgid "How much?"
 msgstr ""
 
 msgid "Currency"
 msgstr "واحد پولی"
 
 msgid "External link"
 msgstr "لینک خارجی"
@@ -146,17 +147,14 @@
 msgid "Submit and add a new one"
 msgstr "ثبت و اضافه کردن جدید"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "پیش فرض پروژه: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "قبض‌ها نمی‌تونند تهی باشن"
-
 msgid "Name"
 msgstr "نام"
 
 msgid "Weights should be positive"
 msgstr "وزن باید مثبت باشه"
 
 msgid "Weight"
@@ -170,21 +168,33 @@
 
 msgid "This project already have this participant"
 msgstr "این شرکت کننده از قبل عضو پروژه هست"
 
 msgid "People to notify"
 msgstr "افرادی که براشون نوتیفیکیشن ارسال میشه"
 
-msgid "Send invites"
-msgstr "فرستادن دعوت نامه"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "ایمیل %(email)s نامعتبره"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -204,89 +214,84 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+msgid "Too many failed login attempts."
 msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "گذرواژه‌ی مدیر صحیح نیست. فقط %(num)d بار دیگه میشه سعی کنی."
 
 msgid "Provided token is invalid"
 msgstr "توکن وارد شده نامعتبره"
 
 msgid "This private code is not the right one"
 msgstr "این کد خصوصی اون کد خصوصی درست نیست"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
 msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -321,14 +326,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr ""
 
 msgid "Deleted project history."
 msgstr ""
 
 msgid "Error deleting recorded IP addresses"
@@ -381,43 +390,35 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "ساخت پروژه"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -435,26 +436,35 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+msgid "Import previously exported project"
+msgstr ""
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -465,17 +475,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -532,51 +539,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -632,17 +634,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "پرداخت کننده"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "تاریخ"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -744,15 +752,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -778,46 +787,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -862,14 +865,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -943,7 +952,82 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
+
+#~ msgid "Import previously exported JSON file"
+#~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr ""
+
+#~ msgid "Amount paid"
+#~ msgstr ""
+
+#~ msgid "Bills can't be null"
+#~ msgstr "قبض‌ها نمی‌تونند تهی باشن"
+
+#~ msgid "Too many failed login attempts, please retry later."
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "فرستادن دعوت نامه"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,52 +7,25 @@
 "Language-Team: French <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Le tableau ci-dessous liste les actions enregistrées avant la "
-"désactivation de l'historique du projet. Vous pouvez\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">supprimer l'historique du projet</a> pour les "
-"supprimer.</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>L'historique de ce projet a été désactivé. Les nouvelles "
-"actions n'apparaîtront pas ci-dessous. Vous pouvez réactiver l'historique du "
-"projet dans les </i>\n"
-"            <a href=\"%(url)s\">paramètres du projet</a>\n"
-"            "
+"X-Generator: Weblate 5.0-dev\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "« I hate money » est un logiciel libre"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s chacun⋅e"
 
+msgid "%(lang)s is not a supported language"
+msgstr "La langue %(lang)s n'est pas prise en charge"
+
 msgid "%(member)s has been added"
 msgstr "%(member)s a été ajouté⋅e"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s a rejoint le projet"
 
 msgid "?"
@@ -109,17 +82,14 @@
 
 msgid "Amount"
 msgstr "Montant"
 
 msgid "Amount in %(currency)s"
 msgstr "Montant en %(currency)s"
 
-msgid "Amount paid"
-msgstr "Montant"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Êtes-vous sûr⋅e de vouloir supprimer toutes les adresses IP enregistrées "
@@ -130,17 +100,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Êtes-vous sur de vouloir supprimer tout l'historique du projet ? Cette "
 "action n'est pas réversible."
 
-msgid "Are you sure?"
-msgstr "Êtes-vous sûr⋅e ?"
-
 msgid "Authentication"
 msgstr "Authentification"
 
 msgid "Back to the list"
 msgstr "Retourner à la liste"
 
 msgid "Balance"
@@ -177,17 +144,14 @@
 
 msgid "Bill items"
 msgstr "Factures"
 
 msgid "Bills"
 msgstr "Factures"
 
-msgid "Bills can't be null"
-msgstr "Le montant d’une facture ne peut pas être vide"
-
 msgid "Can't remember the password?"
 msgstr "Vous avez oublié le code d’accès ?"
 
 msgid "Cancel"
 msgstr "Annuler"
 
 msgid ""
@@ -203,14 +167,17 @@
 
 msgid "Close"
 msgstr "Fermer"
 
 msgid "Code"
 msgstr "Code"
 
+msgid "Compatible with Cospend"
+msgstr "Compatible avec Cospend"
+
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmer la suppression des adresses IP"
 
 msgid "Confirm deletion"
 msgstr "Confirmer la suppression"
 
 msgid "Create"
@@ -286,22 +253,19 @@
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
 "Télécharger la liste des transactions nécessaires pour les remboursements."
 
 msgid "Edit project"
 msgstr "Éditer le projet"
 
-msgid "Edit the project"
-msgstr "Éditer le projet"
-
 msgid "Edit this bill"
 msgstr "Éditer cette facture"
 
 msgid "Edit this participant"
-msgstr "Ajouter un⋅e participant⋅e"
+msgstr "Modifier un⋅e participant⋅e"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Enable project history"
 msgstr "Activer l'historique de projet"
 
@@ -389,25 +353,19 @@
 msgstr ""
 "Vous pouvez activer l'enregistrement des adresses IP dans les paramètres de "
 "la page"
 
 msgid "Identifier:"
 msgstr "Identifiant :"
 
-msgid "Import"
-msgstr "Importer"
-
-msgid "Import JSON"
-msgstr "Importer le fichier JSON"
+msgid "Import previously exported project"
+msgstr "Importer un projet précédemment exporté"
 
-msgid "Import previously exported JSON file"
-msgstr "Importer un fichier JSON précédemment exporté"
-
-msgid "Invalid JSON"
-msgstr "Le fichier JSON est invalide"
+msgid "Import project"
+msgstr "Importer le projet"
 
 msgid "Invalid private code."
 msgstr "Code d’accès invalide."
 
 msgid "Invalid token"
 msgstr "Jeton invalide"
 
@@ -431,14 +389,17 @@
 
 msgid "Logout"
 msgstr "Se déconnecter"
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Gérez facilement <br />vos dépenses partagées"
 
+msgid "Missing attribute: %(attribute)s"
+msgstr "Attribut manquant : %(attribute)s"
+
 msgid "Mobile Application"
 msgstr "Application mobile"
 
 msgid "More options"
 msgstr "Plus d'options"
 
 msgid "Name"
@@ -562,14 +523,27 @@
 
 msgid "People to notify"
 msgstr "Personnes à inviter"
 
 msgid "Period"
 msgstr "Période"
 
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Veuillez vérifier la configuration email du serveur ou contacter "
+"l’administrateur⋅ice : %(admin_email)s"
+
+msgid "Please check the email configuration of the server."
+msgstr "Veuillez vérifier la configuration email du serveur."
+
+msgid "Please retry after %(date)s."
+msgstr "Veuillez réessayer après %(date)s."
+
 msgid "Please, validate the captcha to proceed."
 msgstr "Merci de valider le captcha avant de continuer."
 
 msgid "Privacy Settings"
 msgstr "Vie privée"
 
 msgid "Private code"
@@ -622,16 +596,19 @@
 
 msgid "Reset your password"
 msgstr "Changez votre code d'accès"
 
 msgid "Return to home page"
 msgstr "Retourner à la page d'accueil"
 
-msgid "Send invites"
-msgstr "Envoyer les invitations"
+msgid "Save changes"
+msgstr "Sauvegarder les modifications"
+
+msgid "Scan QR code"
+msgstr "Scannez le QR code"
 
 msgid "Send me the code by email"
 msgstr "Envoyez moi le code par email"
 
 msgid "Send the invitations"
 msgstr "Envoyer les invitations"
 
@@ -654,14 +631,17 @@
 
 msgid "Share Identifier & code"
 msgstr "Partager l'identifiant et le code"
 
 msgid "Share the Link"
 msgstr "Partagez le lien"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr "Les opérations simples sont possibles, par exemple (18+36.2)/3"
+
 msgid "Simply sharing money with others?"
 msgstr "Ça vous arrive de partager de l’argent avec d’autres ?"
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
@@ -669,28 +649,22 @@
 "projet ait désactivé l'enregistrement des adresses IP. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Quelqu'un a probablement vidé l'historique du projet."
 
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
+"instructions."
 msgstr ""
 "Désolé, une erreur s’est produite lors de l’envoi du courriel contenant les "
-"instructions de réinitialisation de mot de passe. Veuillez vérifier la "
-"configuration des courriels du serveur ou contacter l’administrateur⋅ice."
+"instructions de réinitialisation de mot de passe."
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
-"Désolé, une erreur s’est produite lors de l’envoi du courriel d’invitation. "
-"Veuillez vérifier la configuration des courriels du serveur ou contacter "
-"l’administrateur⋅ice."
+"Désolé, une erreur s’est produite lors de l’envoi du courriel d’invitation."
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Désolé, nous ne trouvons pas la page demandée."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
@@ -730,22 +704,25 @@
 msgid "The bill has been modified"
 msgstr "La facture a été modifiée"
 
 msgid "The email %(email)s is not valid"
 msgstr "L’email %(email)s est invalide"
 
 msgid "The participant name is invalid"
-msgstr "Participant⋅e %(name)s réactivé⋅e"
-
-msgid "The project identifier is %(project)s"
-msgstr "L’identifiant de ce projet est %(project)s"
+msgstr "Le nom du participant est incorrect"
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Le projet auquel vous essayez d’accéder n’existe pas, souhaitez vous"
 
+msgid ""
+"The table below reflects actions recorded prior to disabling project history."
+msgstr ""
+"Le tableau ci-dessous affiche uniquement les actions enregistrées avant que "
+"l'historique n'ait été désactivé pour ce projet."
+
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Le mot de passe administrateur⋅ice que vous avez entré n’est pas correct. "
 "Plus que %(num)d tentatives."
 
 msgid "This private code is not the right one"
 msgstr "Le code d'accès n’est pas correct"
@@ -759,39 +736,52 @@
 msgstr ""
 "Ce projet ne peut pas être sans devise car il contient des factures "
 "utilisant des devises différentes."
 
 msgid "This project does not exists"
 msgstr "Ce projet n’existe pas"
 
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+"L'historique de ce projet est désactivé. Les nouvelles actions "
+"n'apparaîtront pas ci-dessous."
+
 msgid "This will remove all bills and participants in this project!"
 msgstr "Cela supprimera toutes les factures et participant⋅es du projet !"
 
 msgid "Time"
 msgstr "Heure"
 
 msgid "To whom?"
 msgstr "Pour qui ?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Trop d'échecs d’authentification successifs, veuillez réessayer plus tard."
+msgid "Too many failed login attempts."
+msgstr "Trop d'échecs d’authentification successifs."
 
 msgid "Try out the demo"
 msgstr "Essayez la démo"
 
+msgid "Unable to logout"
+msgstr "Impossible de se déconnecter"
+
+msgid "Unable to parse CSV"
+msgstr "Erreur lors de la lecture du fichier CSV"
+
 msgid "Unknown error"
 msgstr "Erreur inconnue"
 
 msgid "Unknown project"
 msgstr "Projet inconnu"
 
 msgid "Use IP tracking for project history"
 msgstr "Collecter les adresses IP dans l'historique de projet"
 
+msgid "Use a mobile device with a compatible app."
+msgstr "Utilisez un appareil mobile avec une application compatible."
+
 msgid "We can help!"
 msgstr "On peut vous aider !"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
@@ -807,28 +797,34 @@
 msgid "What?"
 msgstr "Quoi ?"
 
 msgid "When?"
 msgstr "Quand ?"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr "Euro ou Petrodollar ?"
+msgstr "Quelle est la vraie monnaie : Euro ou Petrodollar ?"
 
 msgid "Who paid?"
 msgstr "Qui a payé ?"
 
 msgid "Who pays?"
 msgstr "Qui doit payer ?"
 
 msgid "Who?"
 msgstr "Qui ?"
 
+msgid "You can clear the project history to remove them."
+msgstr "Vous pouvez supprimer l'historique du projet pour les enlever."
+
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Vous pouvez directement partager le lien suivant"
 
+msgid "You can enable history on the settings page."
+msgstr "Vous pouvez activer l'historique dans les paramètres."
+
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
 "Vous pouvez partager l'identifiant de ce projet et le code d'accès par "
 "d'autres moyens."
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/fr/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/fr/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 # This file is distributed under the same license as the PROJECT project.
 # Alexis Métaireau <alexis@notmyidea.org>, 2011.
 # Adrien CLERC, 2018.
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2023-01-29 15:17+0000\n"
-"Last-Translator: Glandos <bugs-github@antipoul.fr>\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2023-07-15 08:51+0000\n"
+"Last-Translator: Baptiste <weblate@bitsofnetworks.org>\n"
 "Language-Team: French <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"X-Generator: Weblate 5.0-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Vous venez de créer « %(project)s » pour partager vos dépenses"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Ceci n'est pas un montant ou une expression valide. Seuls les nombres et "
 "les opérateurs + - * / sont acceptés."
 
@@ -56,19 +60,16 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Ce projet ne peut pas être sans devise car il contient des factures "
 "utilisant des devises différentes."
 
-msgid "Import previously exported JSON file"
-msgstr "Importer un fichier JSON précédemment exporté"
-
-msgid "Import"
-msgstr "Importer"
+msgid "Compatible with Cospend"
+msgstr "Compatible avec Cospend"
 
 msgid "Project identifier"
 msgstr "Identifiant du projet"
 
 msgid "Private code"
 msgstr "Code d’accès"
 
@@ -76,19 +77,19 @@
 msgstr "Créer le projet"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Il existe déjà un projet avec l'identifiant (\"%(project)s\"). Merci d'en "
-"choisir un autre"
+"Il existe déjà un projet avec l'identifiant (\"%(project)s\"). Merci d'en"
+" choisir un autre"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr "Euro ou Petrodollar ?"
+msgstr "Quelle est la vraie monnaie : Euro ou Petrodollar ?"
 
 msgid "euro"
 msgstr "euro"
 
 msgid "Please, validate the captcha to proceed."
 msgstr "Merci de valider le captcha avant de continuer."
 
@@ -121,25 +122,25 @@
 
 msgid "Password confirmation"
 msgstr "Confirmation du mot de passe"
 
 msgid "Reset password"
 msgstr "Réinitialiser le mot de passe"
 
-msgid "Date"
-msgstr "Date"
+msgid "When?"
+msgstr "Quand ?"
 
 msgid "What?"
 msgstr "Quoi ?"
 
-msgid "Payer"
-msgstr "Payeur"
+msgid "Who paid?"
+msgstr "Qui a payé ?"
 
-msgid "Amount paid"
-msgstr "Montant"
+msgid "How much?"
+msgstr "Combien ?"
 
 msgid "Currency"
 msgstr "Devise"
 
 msgid "External link"
 msgstr "Lien externe"
 
@@ -155,45 +156,56 @@
 msgid "Submit and add a new one"
 msgstr "Valider et ajouter une autre facture"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Devise du projet : %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Le montant d’une facture ne peut pas être vide"
-
 msgid "Name"
 msgstr "Nom"
 
 msgid "Weights should be positive"
 msgstr "Les parts doivent être positives"
 
 msgid "Weight"
 msgstr "Parts"
 
 msgid "Add"
 msgstr "Ajouter"
 
 msgid "The participant name is invalid"
-msgstr "Participant⋅e %(name)s réactivé⋅e"
+msgstr "Le nom du participant est incorrect"
 
 msgid "This project already have this participant"
 msgstr "Ce⋅tte membre existe déjà pour ce projet"
 
 msgid "People to notify"
 msgstr "Personnes à inviter"
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "Envoyer les invitations"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "L’email %(email)s est invalide"
 
+msgid "Logout"
+msgstr "Se déconnecter"
+
+msgid "Please check the email configuration of the server."
+msgstr "Veuillez vérifier la configuration email du serveur."
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Veuillez vérifier la configuration email du serveur ou contacter "
+"l’administrateur⋅ice : %(admin_email)s"
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} et {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object} et {end_object}"
@@ -213,101 +225,94 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix} : {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix} :<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Trop d'échecs d’authentification successifs, veuillez réessayer plus tard."
+msgid "Too many failed login attempts."
+msgstr "Trop d'échecs d’authentification successifs."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"Le mot de passe administrateur⋅ice que vous avez entré n’est pas correct. "
-"Plus que %(num)d tentatives."
+"Le mot de passe administrateur⋅ice que vous avez entré n’est pas correct."
+" Plus que %(num)d tentatives."
 
 msgid "Provided token is invalid"
 msgstr "Ce jeton est invalide"
 
 msgid "This private code is not the right one"
 msgstr "Le code d'accès n’est pas correct"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Vous venez de créer « %(project)s » pour partager vos dépenses"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Un courriel de rappel vient de vous être envoyé"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Nous avons essayé de vous envoyer un courriel de rappel, mais une erreur "
 "s’est produite. Il est toujours possible d’utiliser le projet "
 "normalement."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "L’identifiant de ce projet est %(project)s"
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
-"Désolé, une erreur s’est produite lors de l’envoi du courriel contenant les "
-"instructions de réinitialisation de mot de passe. Veuillez vérifier la "
-"configuration des courriels du serveur ou contacter l’administrateur⋅ice."
+"Désolé, une erreur s’est produite lors de l’envoi du courriel contenant "
+"les instructions de réinitialisation de mot de passe."
 
 msgid "No token provided"
 msgstr "Aucun jeton n’a été fourni"
 
 msgid "Invalid token"
 msgstr "Jeton invalide"
 
 msgid "Unknown project"
 msgstr "Projet inconnu"
 
 msgid "Password successfully reset."
 msgstr "Le mot de passe a été changé avec succès."
 
-msgid "Project successfully uploaded"
-msgstr "Le projet a été correctement importé"
+msgid "Unable to parse CSV"
+msgstr "Erreur lors de la lecture du fichier CSV"
 
-msgid "Invalid JSON"
-msgstr "Le fichier JSON est invalide"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr "Attribut manquant : %(attribute)s"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr "Impossible d'ajouter plusieurs devises à un projet sans devise par défaut"
 
+msgid "Project successfully uploaded"
+msgstr "Le projet a été correctement importé"
+
 msgid "Project successfully deleted"
 msgstr "Projet supprimé"
 
 msgid "Error deleting project"
 msgstr "Erreur lors de la suppression du projet"
 
+msgid "Unable to logout"
+msgstr "Impossible de se déconnecter"
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Vous avez été invité⋅e à partager vos dépenses pour %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Vos invitations ont bien été envoyées"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
-"Désolé, une erreur s’est produite lors de l’envoi du courriel d’invitation. "
-"Veuillez vérifier la configuration des courriels du serveur ou contacter "
-"l’administrateur⋅ice."
+"Désolé, une erreur s’est produite lors de l’envoi du courriel "
+"d’invitation."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s a été ajouté⋅e"
 
 msgid "Error activating participant"
 msgstr "Erreur lors de l'activation de ce⋅tte participant⋅e"
@@ -320,16 +325,16 @@
 msgstr "Erreur lors de la suppression d'un⋅e participant⋅e"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"« %(name)s » a été désactivé⋅e. Il⋅elle continuera d’apparaître jusqu'à ce "
-"que son solde soit nul."
+"« %(name)s » a été désactivé⋅e. Il⋅elle continuera d’apparaître jusqu'à "
+"ce que son solde soit nul."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "« %(name)s » a été supprimé⋅e"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -343,14 +348,18 @@
 
 msgid "The bill has been deleted"
 msgstr "La facture a été supprimée"
 
 msgid "The bill has been modified"
 msgstr "La facture a été modifiée"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr "La langue %(lang)s n'est pas prise en charge"
+
 msgid "Error deleting project history"
 msgstr "Erreur lors de la suppression de l'historique du projet"
 
 msgid "Deleted project history."
 msgstr "Historique de projet supprimé."
 
 msgid "Error deleting recorded IP addresses"
@@ -403,43 +412,34 @@
 
 msgid "Actions"
 msgstr "Actions"
 
 msgid "edit"
 msgstr "éditer"
 
-msgid "delete"
-msgstr "supprimer"
+msgid "Delete project"
+msgstr "Supprimer le projet"
 
 msgid "show"
 msgstr "voir"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Le tableau de bord est actuellement désactivé."
 
 msgid "Download Mobile Application"
 msgstr "Télécharger l’application mobile"
 
 msgid "Get it on"
 msgstr "Télécharger depuis"
 
-msgid "Are you sure?"
-msgstr "Êtes-vous sûr⋅e ?"
-
 msgid "Edit project"
 msgstr "Éditer le projet"
 
-msgid "Delete project"
-msgstr "Supprimer le projet"
-
-msgid "Import JSON"
-msgstr "Importer le fichier JSON"
-
-msgid "Choose file"
-msgstr "Choisir un fichier"
+msgid "Import project"
+msgstr "Importer le projet"
 
 msgid "Download project's data"
 msgstr "Télécharger les données du projet"
 
 msgid "Bill items"
 msgstr "Factures"
 
@@ -457,47 +457,53 @@
 
 msgid "Cancel"
 msgstr "Annuler"
 
 msgid "Privacy Settings"
 msgstr "Vie privée"
 
-msgid "Edit the project"
-msgstr "Éditer le projet"
+msgid "Save changes"
+msgstr "Sauvegarder les modifications"
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "Cela supprimera toutes les factures et participant⋅es du projet !"
 
+msgid "Import previously exported project"
+msgstr "Importer un projet précédemment exporté"
+
+msgid "Choose file"
+msgstr "Choisir un fichier"
+
 msgid "Edit this bill"
 msgstr "Éditer cette facture"
 
 msgid "Add a bill"
 msgstr "Ajouter une facture"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr "Les opérations simples sont possibles, par exemple (18+36.2)/3"
+
 msgid "Everyone"
 msgstr "Tout le monde"
 
 msgid "No one"
 msgstr "Personne"
 
 msgid "More options"
 msgstr "Plus d'options"
 
 msgid "Add participant"
 msgstr "Ajouter un⋅e participant⋅e"
 
 msgid "Edit this participant"
-msgstr "Ajouter un⋅e participant⋅e"
+msgstr "Modifier un⋅e participant⋅e"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "marie@site.com, jean.dupont@exemple.com"
 
-msgid "Send the invitations"
-msgstr "Envoyer les invitations"
-
 msgid "Download"
 msgstr "Télécharger"
 
 msgid "Disabled Project History"
 msgstr "Désactiver l'historique du projet"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -554,86 +560,72 @@
 "cannot be undone."
 msgstr ""
 "Êtes-vous sur de vouloir supprimer tout l'historique du projet ? Cette "
 "action n'est pas réversible."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr ""
-"Facture %(name)s : %(owers_list_str)s ajouté à la liste des débiteur⋅ices"
+msgstr "Facture %(name)s : %(owers_list_str)s ajouté à la liste des débiteur⋅ices"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
-"Facture %(name)s : %(owers_list_str)s supprimé de la liste des débiteur⋅ices"
+"Facture %(name)s : %(owers_list_str)s supprimé de la liste des "
+"débiteur⋅ices"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>L'historique de ce projet a été désactivé. Les nouvelles "
-"actions n'apparaîtront pas ci-dessous. Vous pouvez réactiver l'historique"
-" du projet dans les </i>\n"
-"            <a href=\"%(url)s\">paramètres du projet</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+"L'historique de ce projet est désactivé. Les nouvelles actions "
+"n'apparaîtront pas ci-dessous."
+
+msgid "You can enable history on the settings page."
+msgstr "Vous pouvez activer l'historique dans les paramètres."
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Le tableau ci-dessous liste les actions enregistrées avant la "
-"désactivation de l'historique du projet. Vous pouvez\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">supprimer l'historique du projet</a> pour les "
-"supprimer.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+"Le tableau ci-dessous affiche uniquement les actions enregistrées avant "
+"que l'historique n'ait été désactivé pour ce projet."
+
+msgid "You can clear the project history to remove them."
+msgstr "Vous pouvez supprimer l'historique du projet pour les enlever."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Certaines entrées de l'historique contiennent une adresse IP, bien que ce"
 " projet ait désactivé l'enregistrement des adresses IP. "
 
 msgid "Delete stored IP addresses"
 msgstr "Supprimer toutes les adresses IP enregistrées"
 
-msgid "No history to erase"
-msgstr "Aucun historique à supprimer"
-
-msgid "Clear Project History"
-msgstr "Supprimer les entrées de l'historique du projet"
-
 msgid "No IP Addresses to erase"
 msgstr "Aucune adresse IP à supprimer"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Supprimer les adresses IP enregistrées"
 
+msgid "No history to erase"
+msgstr "Aucun historique à supprimer"
+
+msgid "Clear Project History"
+msgstr "Supprimer les entrées de l'historique du projet"
+
 msgid "Time"
 msgstr "Heure"
 
 msgid "Event"
 msgstr "Évènement"
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
-"Vous pouvez activer l'enregistrement des adresses IP dans les paramètres de "
-"la page"
+"Vous pouvez activer l'enregistrement des adresses IP dans les paramètres "
+"de la page"
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 "L'enregistrement des adresses IP peut-être désactivé dans les paramètres "
 "de la page"
 
 msgid "From IP"
@@ -683,17 +675,23 @@
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 "Participant⋅e %(name)s : nombre de parts changé de %(old_weight)s en "
 "%(new_weight)s"
 
+msgid "Payer"
+msgstr "Payeur"
+
 msgid "Amount"
 msgstr "Montant"
 
+msgid "Date"
+msgstr "Date"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Montant en %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Facture %(name)s modifiée"
@@ -797,16 +795,17 @@
 
 msgid "switch to"
 msgstr "aller à"
 
 msgid "Dashboard"
 msgstr "Tableau de bord"
 
-msgid "Logout"
-msgstr "Se déconnecter"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr "Veuillez réessayer après %(date)s."
 
 msgid "Code"
 msgstr "Code"
 
 msgid "Mobile Application"
 msgstr "Application mobile"
 
@@ -831,46 +830,40 @@
 
 msgid "you sure?"
 msgstr "vous confirmez ?"
 
 msgid "Invite people"
 msgstr "Inviter des gens"
 
-msgid "You should start by adding participants"
-msgstr "Vous devriez commencer par ajouter des participant⋅es"
-
-msgid "Add a new bill"
-msgstr "Nouvelle facture"
-
 msgid "Newer bills"
 msgstr "Factures suivantes"
 
 msgid "Older bills"
 msgstr "Factures précédentes"
 
-msgid "When?"
-msgstr "Quand ?"
+msgid "You should start by adding participants"
+msgstr "Vous devriez commencer par ajouter des participant⋅es"
 
-msgid "Who paid?"
-msgstr "Qui a payé ?"
+msgid "Add a new bill"
+msgstr "Nouvelle facture"
 
 msgid "For what?"
 msgstr "Pour quoi ?"
 
-msgid "How much?"
-msgstr "Combien ?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Ajouté le %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Tout le monde sauf %(excluded)s"
 
+msgid "delete"
+msgstr "supprimer"
+
 msgid "No bills"
 msgstr "Pas encore de factures"
 
 msgid "Nothing to list yet."
 msgstr "Rien à lister pour le moment."
 
 msgid "You probably want to"
@@ -919,25 +912,31 @@
 
 msgid "Share the Link"
 msgstr "Partagez le lien"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Vous pouvez directement partager le lien suivant"
 
+msgid "Scan QR code"
+msgstr "Scannez le QR code"
+
+msgid "Use a mobile device with a compatible app."
+msgstr "Utilisez un appareil mobile avec une application compatible."
+
 msgid "Send via Emails"
 msgstr "Envoyer par email(s)"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
-"Entrez les emails des personnes avec qui vous souhaitez partager ce projet, "
-"nous leur enverrons un lien d'invitation."
+"Entrez les emails des personnes avec qui vous souhaitez partager ce "
+"projet, nous leur enverrons un lien d'invitation."
 
 msgid "Who pays?"
 msgstr "Qui doit payer ?"
 
 msgid "To whom?"
 msgstr "Pour qui ?"
 
@@ -1265,7 +1264,77 @@
 #~ msgstr "Nombre de membres"
 
 #~ msgid "Edit this member"
 #~ msgstr "Éditer ce⋅tte participant⋅e"
 
 #~ msgid "Participants to notify"
 #~ msgstr "ajouter des participant⋅e⋅s"
+
+#~ msgid "Import"
+#~ msgstr "Importer"
+
+#~ msgid "Amount paid"
+#~ msgstr "Montant"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Le montant d’une facture ne peut pas être vide"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "L’identifiant de ce projet est %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Le fichier JSON est invalide"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Êtes-vous sûr⋅e ?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importer le fichier JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>L'historique de ce projet "
+#~ "a été désactivé. Les nouvelles actions"
+#~ " n'apparaîtront pas ci-dessous. Vous "
+#~ "pouvez réactiver l'historique du projet "
+#~ "dans les </i>\n"
+#~ "            <a href=\"%(url)s\">paramètres du projet</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Le tableau ci-dessous "
+#~ "liste les actions enregistrées avant la"
+#~ " désactivation de l'historique du projet."
+#~ " Vous pouvez\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">supprimer l'historique du"
+#~ " projet</a> pour les supprimer.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Envoyer les invitations"
+
+#~ msgid " show"
+#~ msgstr "voir"
+
+#~ msgid "Edit the project"
+#~ msgstr "Éditer le projet"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/he/LC_MESSAGES/messages.mo`

 * *Files 21% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,29 +8,36 @@
 "hate-money/he/>\n"
 "Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1) ? 0 : ((n == 2) ? 1 : ((n > 10 && "
 "n % 10 == 0) ? 2 : 3));\n"
-"X-Generator: Weblate 4.14.2\n"
+"X-Generator: Weblate 5.0-dev\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"אני שונא כסף\" היא תוכנה חינמית"
 
+msgid "%(lang)s is not a supported language"
+msgstr "%(lang)s אינה שפה נתמכת"
+
 msgid "%(member)s has been added"
 msgstr "%(member)s נוסף"
 
 msgid "?"
 msgstr "?"
 
 msgid "A link to an external document, related to this bill"
 msgstr "קישור למסמך חיצוני, בקשר לחשבון הזה"
 
 msgid ""
+"A link to reset your password has been sent to you, please check your emails."
+msgstr "נשלח לחשבונך לינק לאיפוס הסיסמה, אנא בדוק את תיבת הדוא\"ל שלך."
+
+msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr "פרויקט עם המזהה (\"%(project)s\") כבר קיים. אנא בחרו מזהה חדש"
 
 msgid "A reminder email has just been sent to you"
 msgstr "דוא\"ל תזכורת נשלח אליך כעת"
 
@@ -39,50 +46,50 @@
 
 msgid "Actions"
 msgstr "פעולות"
 
 msgid "Add"
 msgstr "הוסף"
 
+msgid "Add a new bill"
+msgstr "הוסף הוצאה חדשה"
+
 msgid "Added on %(date)s"
 msgstr "נוסף בתאריך %(date)s"
 
 msgid "Admin password"
 msgstr "סיסמת מנהל"
 
 msgid "Administration tasks are currently disabled."
 msgstr "פעולות ניהול מבוטלות לעת עתה."
 
 msgid "Amount"
 msgstr "סכום"
 
-msgid "Amount paid"
-msgstr "כמות ששולמה"
-
 msgid "Authentication"
 msgstr "הזדהות"
 
 msgid "Back to the list"
 msgstr "חזרה לרשימה"
 
-msgid "Bills can't be null"
-msgstr "חשבונות לא יכולים להיות ריקים"
+msgid "Balance"
+msgstr "מאזן"
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default currency"
 msgstr "לא ניתן להוסיף חשבונות במספר מטבעות לפרויקט ללא מטבע ברירת מחדל"
 
 msgid "Choose file"
 msgstr "בחר קובץ"
 
 msgid "Code"
 msgstr "קוד"
 
 msgid "Create a new project"
-msgstr "צור פרויקט"
+msgstr "צור פרויקט חדש"
 
 msgid "Create the project"
 msgstr "צור את הפרויקט"
 
 msgid "Currency"
 msgstr "מטבע"
 
@@ -112,23 +119,29 @@
 
 msgid "Enter a new code if you want to change it"
 msgstr "הזן.י קוד חדש אם תרצה.י לשנות את הקוד"
 
 msgid "Enter private code to confirm deletion"
 msgstr "הזן את הקוד הפרטי כדי לאשר מחיקה"
 
+msgid "Error deleting bill"
+msgstr "שגיאה בעת מחיקת החשבון"
+
 msgid "Error deleting project"
 msgstr "שגיאה במחיקת הפרויקט"
 
 msgid "Error deleting project history"
 msgstr "שגיאה במחיקת הסטוריית הפרויקט"
 
 msgid "Event"
 msgstr "אירוע"
 
+msgid "Expenses by Month"
+msgstr "הוצאות לפי חודש"
+
 msgid "External link"
 msgstr "קישור חיצוני"
 
 msgid "For what?"
 msgstr "עבור מה?"
 
 msgid "For whom?"
@@ -145,56 +158,68 @@
 
 msgid "How much?"
 msgstr "כמה?"
 
 msgid "Identifier:"
 msgstr "מזהה:"
 
-msgid "Import"
-msgstr "ייבא"
-
-msgid "Import JSON"
-msgstr "ייבא JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "ייבא קובץ JSON מיוצא"
+msgid "Import previously exported project"
+msgstr "ייבא פרוייקט קודם מיוצא"
 
-msgid "Invalid JSON"
-msgstr "פורמט JSON לא תקין"
+msgid "Import project"
+msgstr "ייבא פרוייקטים"
 
 msgid "Invalid private code."
 msgstr "קוד פרטי לא תקין."
 
 msgid "Invalid token"
 msgstr "טוקן לא תקין"
 
+msgid "Invite people"
+msgstr "הזמן אנשים"
+
+msgid "Invite people to join this project"
+msgstr "הזמן אנשים להצטרף לפרויקט"
+
 msgid "Languages"
 msgstr "שפות"
 
 msgid "Legal information"
 msgstr "מידע משפטי"
 
 msgid "Log in"
 msgstr "התחבר"
 
 msgid "Log in to an existing project"
 msgstr "התחבר לפרויקט קיים"
 
+msgid "Logout"
+msgstr "להתנתק"
+
+msgid "Missing attribute: %(attribute)s"
+msgstr "תכונה חסרה:%(attribute)s"
+
+msgid "Mobile Application"
+msgstr "יישום לנייד"
+
 msgid "Name"
 msgstr "שם"
 
 msgid "New private code"
 msgstr "קוד פרטי חדש"
 
 msgid "Newest bill"
 msgstr "החשבון החדש ביותר"
 
 msgid "No Currency"
 msgstr "ללא מטבע"
 
+msgid "No bills"
+msgstr "אין הוצאות"
+
 msgid "No token provided"
 msgstr "טוקן לא הוזן"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "כמות או ביטוי לא תקין. יש להזין רק מספרים וסימני הפעולה + - * /."
@@ -204,17 +229,23 @@
 
 msgid "Number of bills"
 msgstr "מספר חשבונות"
 
 msgid "Number of participants"
 msgstr "מספר משתתפים"
 
+msgid "Older bills"
+msgstr "הוצאות ישנות"
+
 msgid "Oldest bill"
 msgstr "החשבון הישן ביותר"
 
+msgid "Other projects :"
+msgstr "פרויקטים אחרים:"
+
 msgid "Paid"
 msgstr "שולם"
 
 msgid "Password"
 msgstr "סיסמה"
 
 msgid "Password confirmation"
@@ -234,14 +265,21 @@
 
 msgid "People to notify"
 msgstr "אנשים להתריע להם"
 
 msgid "Period"
 msgstr "תקופה"
 
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"מצטערים, אך אירעה שגיאה בעת ששלחנו לכם את המייל עם הוראות איפוס הסיסמה. אנא "
+"בדקו את הגדרות המייל בשרת או פנו למנהל השרת:%(admin_email)s"
+
 msgid "Please, validate the captcha to proceed."
 msgstr "אנא אמת את ה-Captcha כדי להמשיך."
 
 msgid "Private code"
 msgstr "קוד פרטי"
 
 msgid "Project"
@@ -267,55 +305,71 @@
 
 msgid "Provided token is invalid"
 msgstr "הטוקן שהוזן אינו תקין"
 
 msgid "Reset password"
 msgstr "איפוס סיסמה"
 
+msgid "Reset your password"
+msgstr "אפס את סיסמתך"
+
 msgid "Return to home page"
 msgstr "חזור לעמוד הבית"
 
-msgid "Send invites"
-msgstr "שלח הזמנות"
+msgid "Scan QR code"
+msgstr "סרוק את הברקוד"
 
 msgid "Send me the code by email"
 msgstr "שלח לי את הקוד בדוא\"ל"
 
+msgid "Send the invitations"
+msgstr "שלח את ההזמנות"
+
+msgid "Send via Emails"
+msgstr "שלח באמצעות דוא\"ל"
+
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "בחירת מטבע ברירת מחדל מאפשרת המרת מטבע בין חשבונות"
 
 msgid "Settings"
 msgstr "הגדרות"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"מצטערים, אך אירעה שגיאה בעת ששלחנו לכם את המייל עם הוראות איפוס הסיסמה. "
-"בבקשה תבדקו את הגדרות המייל בשרת או פנו למנהל השרת."
+msgid "Share Identifier & code"
+msgstr "שתף מזהה וקוד"
+
+msgid "Share the Link"
+msgstr "שתף את הלינק"
+
+msgid "Sorry, there was an error while trying to send the invitation emails."
+msgstr "מצטערים, אך אירעה שגיאה בעת שליחת ההזמנות."
+
+msgid "Sorry, we were unable to find the page you've asked for."
+msgstr "מצטערים, לא הצלחנו לגשת לדף שחיפשת."
+
+msgid "Start a new project"
+msgstr "התחל פרוייקט חדש"
 
 msgid "Submit"
 msgstr "הזן"
 
 msgid "Submit and add a new one"
 msgstr "הזן והוסף אחד חדש"
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "כנראה שהדבר הטוב ביותר לעשות הוא לחזור לעמוד הראשי."
 
+msgid "The bill has been added"
+msgstr "החשבון נוסף"
+
 msgid "The email %(email)s is not valid"
 msgstr "כתובת הדוא\"ל %(email)s אינה תקינה"
 
 msgid "The participant name is invalid"
 msgstr "שם המשתתף אינו תקין"
 
-msgid "The project identifier is %(project)s"
-msgstr "מזהה הפרויקט הוא %(project)s"
-
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "סיסמת המנהל הזו שגויה. נותרו %(num)d ניסיונות."
 
 msgid "This private code is not the right one"
 msgstr "קוד פרטי זה שגוי"
 
 msgid "This project already have this participant"
@@ -332,29 +386,35 @@
 
 msgid "Time"
 msgstr "זמן"
 
 msgid "To whom?"
 msgstr "למי?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "יותר מדי ניסיון התחברות כושלים, אנא נסו שם מאוחר יותר."
+msgid "Too many failed login attempts."
+msgstr "יותר מדי ניסיון התחברות כושלים."
 
 msgid "Try out the demo"
 msgstr "נסו את הדמו"
 
+msgid "Unable to logout"
+msgstr "לא ניתן להתנתק"
+
 msgid "Unknown error"
 msgstr "שגיאה לא ידועה"
 
 msgid "Unknown project"
 msgstr "פרויקט לא ידוע"
 
 msgid "Use IP tracking for project history"
 msgstr "השתמש במעקב IP עבור היסטוריית פרויקט"
 
+msgid "Use a mobile device with a compatible app."
+msgstr "השתמש במכשיר נייד עם יישום תואם."
+
 msgid "We can help!"
 msgstr "אנחנו יכולים לעזור!"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
@@ -381,32 +441,64 @@
 
 msgid "Who pays?"
 msgstr "מי משלם?"
 
 msgid "Who?"
 msgstr "מי?"
 
+msgid "You can directly share the following link via your prefered medium"
+msgstr "אתה יכול לשתף ישירות את הלינק באמצעי המועדף עליך"
+
+msgid ""
+"You can share the project identifier and the private code by any "
+"communication means."
+msgstr "אתה יכול לשתף את מזהה הפרויקט והקוד הפרטי באמצעות כל אמצעי תקשורת."
+
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "הוזמנת לשתף הוצאות בפרויקט %(project)s"
 
 msgid "You have just created '%(project)s' to share your expenses"
 msgstr "יצרת את פרויקט '%(project)s' כדי לחלוק את הוצאותיך"
 
+msgid "You probably want to"
+msgstr "אתה כנראה רוצה"
+
+msgid "You should start by adding participants"
+msgstr "כדאי להתחיל בהוספת משתמשים"
+
 msgid "Your invitations have been sent"
 msgstr "ההזמנות שלך נשלחו"
 
 msgid "Your projects"
 msgstr "הפרויקטים שלך"
 
+msgid "add participants"
+msgstr "הוסף משתמשים"
+
 msgid "can't remember your password?"
 msgstr "לא זוכרים את הסיסמה?"
 
+msgid "delete"
+msgstr "מחק"
+
+msgid "edit"
+msgstr "ערוך"
+
 msgid "euro"
 msgstr "אירו"
 
+msgid "switch to"
+msgstr "שנה ל"
+
+msgid "you can contribute and improve it!"
+msgstr "אתה יכול לתרום ולשפר אותו!"
+
+msgid "you sure?"
+msgstr "האם אתה בטוח?"
+
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} ו- {dual_object_1}"
 
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 msgid "{prefix}:<br />{errors}"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/he/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.po`

 * *Files 18% similar despite different names*

```diff
@@ -1,301 +1,313 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-05-22 20:21+0200\n"
-"PO-Revision-Date: 2022-11-07 10:07+0000\n"
-"Last-Translator: Raanan Katz <raakatz97@gmail.com>\n"
-"Language-Team: Hebrew <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/he/>\n"
-"Language: he\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2023-04-19 11:51+0000\n"
+"Last-Translator: Gergely Kocsis <koger23@gmail.com>\n"
+"Language: hu\n"
+"Language-Team: Hungarian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/hu/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1) ? 0 : ((n == 2) ? 1 : ((n > 10 && "
-"n % 10 == 0) ? 2 : 3));\n"
-"X-Generator: Weblate 4.14.2\n"
+"Generated-By: Babel 2.9.0\n"
+
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Létrehoztál egy projektet '%(project)s' a kiadásaid megosztására"
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
-msgstr "כמות או ביטוי לא תקין. יש להזין רק מספרים וסימני הפעולה + - * /."
+msgstr ""
+"Érvénytelen mennyiség vagy kifejezés. Csak számok és műveleti jelek ( + -"
+" * /) megengedettek."
 
 msgid "Project name"
-msgstr "שם הפרויקט"
+msgstr "A projekt neve"
 
 msgid "New private code"
-msgstr "קוד פרטי חדש"
+msgstr "Új titkos kód"
 
 msgid "Enter a new code if you want to change it"
-msgstr "הזן.י קוד חדש אם תרצה.י לשנות את הקוד"
+msgstr "Adj meg egy új kódot, ha meg akarod változtatni"
 
 msgid "Email"
-msgstr "דוא\"ל"
+msgstr "Email"
 
 msgid "Enable project history"
-msgstr "אפשר היסטוריית פרויקט"
+msgstr "Projekt történet bekapcsolása"
 
 msgid "Use IP tracking for project history"
-msgstr "השתמש במעקב IP עבור היסטוריית פרויקט"
+msgstr "IP nyomkövetés használata a projekt előzményekhez"
 
 msgid "Default Currency"
-msgstr "מטבע ברירת המחדל"
+msgstr "Alapértelmezett Pénznem"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr "בחירת מטבע ברירת מחדל מאפשרת המרת מטבע בין חשבונות"
+msgstr ""
+"Alapértelmezett pénznem beállítása lehetővé teszi a számlák közötti "
+"pénzváltást"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"בפרויקט זה לא ניתן להגדיר 'ללא מטבע' מכיוון שהוא כולל חשבונות במספר מטבעות."
+"A projekt nem állítható pénznem nélkülire, mert számlákat és több "
+"pénznemet is tartalmaz."
 
-msgid "Import previously exported JSON file"
-msgstr "ייבא קובץ JSON מיוצא"
-
-msgid "Import"
-msgstr "ייבא"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
-msgstr "מזהה פרויקט"
+msgstr "Projekt azonosító"
 
 msgid "Private code"
-msgstr "קוד פרטי"
+msgstr "Titkos kód"
 
 msgid "Create the project"
-msgstr "צור את הפרויקט"
+msgstr "Projekt létrehozása"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
-msgstr "פרויקט עם המזהה (\"%(project)s\") כבר קיים. אנא בחרו מזהה חדש"
+msgstr ""
+"Már létezik egy projekt ezzel az azonosítóval (\"%(project)s\"). Kérjük, "
+"válasszon más azonosítót"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr "איזה מהם הוא מטבע אמיתי: אירו או דולר פטרו?"
+msgstr "Melyik valódi pénznem, az euró vagy a petrodollár?"
 
 msgid "euro"
-msgstr "אירו"
+msgstr "euró"
 
 msgid "Please, validate the captcha to proceed."
-msgstr "אנא אמת את ה-Captcha כדי להמשיך."
+msgstr "Kérlek validáld a captcha-t a folytatáshoz."
 
 msgid "Enter private code to confirm deletion"
-msgstr "הזן את הקוד הפרטי כדי לאשר מחיקה"
+msgstr "Add meg a titkos kódot a törlés megerősítéséhez"
 
 msgid "Unknown error"
-msgstr "שגיאה לא ידועה"
+msgstr "Ismeretlen hiba"
 
 msgid "Invalid private code."
-msgstr "קוד פרטי לא תקין."
+msgstr "Érvénytelen titkos kód."
 
+#, fuzzy
 msgid "Get in"
-msgstr "היכנס"
+msgstr "Szállj be"
 
 msgid "Admin password"
-msgstr "סיסמת מנהל"
+msgstr "Adminisztrátori jelszó"
 
 msgid "Send me the code by email"
-msgstr "שלח לי את הקוד בדוא\"ל"
+msgstr "Kód küldése e-mailben"
 
 msgid "This project does not exists"
-msgstr "פרויקט זה לא קיים"
+msgstr "Ez a projekt nem létezik"
 
 msgid "Password mismatch"
-msgstr "חוסר התאמה בסיסמה"
+msgstr "A jelszavak nem egyeznek"
 
 msgid "Password"
-msgstr "סיסמה"
+msgstr "Jelszó"
 
 msgid "Password confirmation"
-msgstr "אימות סיסמה"
+msgstr "Jelszó megerősítése"
 
 msgid "Reset password"
-msgstr "איפוס סיסמה"
+msgstr "Jelszó visszaállítása"
 
-msgid "Date"
-msgstr "תאריך"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
-msgstr "מה?"
+msgstr "Mi?"
 
-msgid "Payer"
-msgstr "משלם"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "כמות ששולמה"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
-msgstr "מטבע"
+msgstr "Pénznem"
 
 msgid "External link"
-msgstr "קישור חיצוני"
+msgstr "Külső hivatkozás"
 
 msgid "A link to an external document, related to this bill"
-msgstr "קישור למסמך חיצוני, בקשר לחשבון הזה"
+msgstr "A számlához kapcsolódó külső dokumentum linkje"
 
 msgid "For whom?"
-msgstr "עבור מי?"
+msgstr "Kinek?"
 
 msgid "Submit"
-msgstr "הזן"
+msgstr "Mentés"
 
 msgid "Submit and add a new one"
-msgstr "הזן והוסף אחד חדש"
+msgstr "Mentés és új hozzáadása"
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr "ברירת המחדל בפרויקט: %(currency)s"
-
-msgid "Bills can't be null"
-msgstr "חשבונות לא יכולים להיות ריקים"
+msgstr "Projekt alapértelmezés: %(currency)s"
 
 msgid "Name"
-msgstr "שם"
+msgstr "Név"
 
 msgid "Weights should be positive"
-msgstr "משקלים צריכים להיות חיוביים"
+msgstr "A súlyoknak pozitív értékűnek kell lenni"
 
 msgid "Weight"
-msgstr "משקל"
+msgstr "Súly"
 
 msgid "Add"
-msgstr "הוסף"
+msgstr "Hozzáadás"
 
 msgid "The participant name is invalid"
-msgstr "שם המשתתף אינו תקין"
+msgstr "A résztvevő neve érvénytelen"
 
 msgid "This project already have this participant"
-msgstr "המשתתף כבר נמצא בפרויקט זה"
+msgstr "Ez a résztvevő már szerepel ebben a projektben"
 
 msgid "People to notify"
-msgstr "אנשים להתריע להם"
+msgstr "Értesítendő személyek"
 
-msgid "Send invites"
-msgstr "שלח הזמנות"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
-msgstr "כתובת הדוא\"ל %(email)s אינה תקינה"
+msgstr "Érvénytelen e-mail cím: %(email)s"
+
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr "{dual_object_0} ו- {dual_object_1}"
+msgstr "{dual_object_0} és {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr "{previous_object}, ו- {end_object}"
+msgstr "{previous_object} és {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
 msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
 msgstr "{start_object}, {next_object}"
 
 msgid "No Currency"
-msgstr "ללא מטבע"
+msgstr "Nincs pénznem"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "יותר מדי ניסיון התחברות כושלים, אנא נסו שם מאוחר יותר."
+#, fuzzy
+msgid "Too many failed login attempts."
+msgstr "Túl sok sikertelen bejelentkezési kísérlet, kérlek, próbáld újra később."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
-msgstr "סיסמת המנהל הזו שגויה. נותרו %(num)d ניסיונות."
+msgstr "Az admin jelszó érvénytelen. Csak %(num)d próbálkozásod maradt."
 
 msgid "Provided token is invalid"
-msgstr "הטוקן שהוזן אינו תקין"
+msgstr "A megadott token érvénytelen"
 
 msgid "This private code is not the right one"
-msgstr "קוד פרטי זה שגוי"
-
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "יצרת את פרויקט '%(project)s' כדי לחלוק את הוצאותיך"
+msgstr "Ez a titkos kód nem megfelelő"
 
 msgid "A reminder email has just been sent to you"
-msgstr "דוא\"ל תזכורת נשלח אליך כעת"
+msgstr "Az emlékeztető e-mailt kiküldtük"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"ניסינו לשלוח לך דוא\"ל תזכורת, אבל הייתה שגיאה. תוכל.י להמשיך להשתמש בפרויקט "
-"כרגיל."
-
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "מזהה הפרויקט הוא %(project)s"
+"Megpróbáltuk az emlékeztető e-mailt kiküldeni, de hiba történt. Ettől még"
+" használhatod a megszokott módon a projektet."
 
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
-"מצטערים, אך אירעה שגיאה בעת ששלחנו לכם את המייל עם הוראות איפוס הסיסמה. "
-"בבקשה תבדקו את הגדרות המייל בשרת או פנו למנהל השרת."
 
 msgid "No token provided"
-msgstr "טוקן לא הוזן"
+msgstr "Nincs token megadva"
 
 msgid "Invalid token"
-msgstr "טוקן לא תקין"
+msgstr "Érvénytelen token"
 
 msgid "Unknown project"
-msgstr "פרויקט לא ידוע"
+msgstr "Ismeretlen projekt"
 
 msgid "Password successfully reset."
-msgstr "הסיסמה אופסה בהצלחה."
+msgstr "Jelszó sikeresen visszaállítva."
 
-msgid "Project successfully uploaded"
-msgstr "הפרויקט הועלה בהצלחה"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "פורמט JSON לא תקין"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
-msgstr "לא ניתן להוסיף חשבונות במספר מטבעות לפרויקט ללא מטבע ברירת מחדל"
+msgstr ""
+
+msgid "Project successfully uploaded"
+msgstr "Projekt sikeresen feltöltve"
 
 msgid "Project successfully deleted"
-msgstr "הפרויקט נמחק בהצלחה"
+msgstr "Projekt sikeresen törölve"
 
 msgid "Error deleting project"
-msgstr "שגיאה במחיקת הפרויקט"
+msgstr "Hiba történt a projekt törlésekor"
+
+msgid "Unable to logout"
+msgstr ""
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr "הוזמנת לשתף הוצאות בפרויקט %(project)s"
+msgstr "Meghívtak a következő projektbe %(project)s a kiadásaid megosztására"
 
 msgid "Your invitations have been sent"
-msgstr "ההזמנות שלך נשלחו"
+msgstr "A meghívóid sikeresen kiküldve"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
-msgstr "%(member)s נוסף"
+msgstr "%(member)s hozzáadva"
 
 msgid "Error activating participant"
-msgstr ""
+msgstr "Hiba történt a résztvevő aktiválása közben"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr ""
 
 msgid "Error removing participant"
 msgstr ""
@@ -322,103 +334,99 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
-msgstr "שגיאה במחיקת הסטוריית הפרויקט"
+msgstr ""
 
 msgid "Deleted project history."
-msgstr "הסטוריית הפרויקט נמחקה."
+msgstr ""
 
 msgid "Error deleting recorded IP addresses"
 msgstr ""
 
 msgid "Deleted recorded IP addresses in project history."
 msgstr ""
 
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr ""
 
 msgid "The best thing to do is probably to get back to the main page."
-msgstr "כנראה שהדבר הטוב ביותר לעשות הוא לחזור לעמוד הראשי."
+msgstr ""
 
 msgid "Back to the list"
-msgstr "חזרה לרשימה"
+msgstr ""
 
 msgid "Administration tasks are currently disabled."
-msgstr "פעולות ניהול מבוטלות לעת עתה."
+msgstr ""
 
 msgid "Authentication"
-msgstr "הזדהות"
+msgstr ""
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 
 msgid "create it"
 msgstr ""
 
 msgid "?"
-msgstr "?"
+msgstr ""
 
 msgid "Create a new project"
-msgstr "צור פרויקט"
+msgstr ""
 
 msgid "Project"
-msgstr "פרויקט"
+msgstr ""
 
 msgid "Number of participants"
-msgstr "מספר משתתפים"
+msgstr ""
 
 msgid "Number of bills"
-msgstr "מספר חשבונות"
+msgstr ""
 
 msgid "Newest bill"
-msgstr "החשבון החדש ביותר"
+msgstr ""
 
 msgid "Oldest bill"
-msgstr "החשבון הישן ביותר"
+msgstr ""
 
 msgid "Actions"
-msgstr "פעולות"
+msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
-msgstr "הורד אפליקציית מובייל"
-
-msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
+msgid "Get it on"
 msgstr ""
 
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr "מחק פרויקט"
-
-msgid "Import JSON"
-msgstr "ייבא JSON"
-
-msgid "Choose file"
-msgstr "בחר קובץ"
+#, fuzzy
+msgid "Import project"
+msgstr "Projekt létrehozása"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -436,26 +444,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Korábban exportált JSON fájl importálása"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -466,17 +484,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -533,67 +548,62 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
-msgstr "זמן"
+msgstr ""
 
 msgid "Event"
-msgstr "אירוע"
+msgstr ""
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 
 msgid "From IP"
-msgstr "מכתובת IP"
+msgstr ""
 
 #, python-format
 msgid "Project %(name)s added"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s added"
@@ -633,16 +643,22 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Fizető"
+
 msgid "Amount"
-msgstr "סכום"
+msgstr ""
+
+msgid "Date"
+msgstr "Dátum"
 
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
@@ -669,156 +685,151 @@
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s changed in an unknown way"
 msgstr ""
 
 msgid "Nothing to list"
-msgstr "אין מה להציג"
+msgstr ""
 
 msgid "Someone probably cleared the project history."
 msgstr ""
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr ""
 
 msgid "Try out the demo"
-msgstr "נסו את הדמו"
+msgstr ""
 
 msgid "You're sharing a house?"
 msgstr ""
 
 msgid "Going on holidays with friends?"
 msgstr ""
 
 msgid "Simply sharing money with others?"
 msgstr ""
 
 msgid "We can help!"
-msgstr "אנחנו יכולים לעזור!"
+msgstr ""
 
 msgid "Log in to an existing project"
-msgstr "התחבר לפרויקט קיים"
+msgstr ""
 
 msgid "Log in"
-msgstr "התחבר"
+msgstr ""
 
 msgid "can't remember your password?"
-msgstr "לא זוכרים את הסיסמה?"
+msgstr ""
 
 msgid "Create"
 msgstr ""
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
 
 msgid "Account manager"
-msgstr "מנהל החשבון"
+msgstr ""
 
 msgid "Bills"
 msgstr ""
 
 msgid "Settle"
 msgstr ""
 
 msgid "Statistics"
 msgstr ""
 
 msgid "Languages"
-msgstr "שפות"
+msgstr ""
 
 msgid "Projects"
-msgstr "פרויקטים"
+msgstr ""
 
 msgid "Start a new project"
 msgstr ""
 
 msgid "History"
-msgstr "הסטוריה"
+msgstr ""
 
 msgid "Settings"
-msgstr "הגדרות"
+msgstr ""
 
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
-msgstr "קוד"
+msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
 
 msgid "Documentation"
-msgstr "דוקומנטציה"
+msgstr ""
 
 msgid "Administation Dashboard"
 msgstr ""
 
 msgid "Legal information"
-msgstr "מידע משפטי"
+msgstr ""
 
 msgid "\"I hate money\" is free software"
-msgstr "\"אני שונא כסף\" היא תוכנה חינמית"
+msgstr ""
 
 msgid "you can contribute and improve it!"
 msgstr ""
 
 #, python-format
 msgid "%(amount)s each"
 msgstr ""
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
-msgstr "מתי?"
+msgid "You should start by adding participants"
+msgstr ""
 
-msgid "Who paid?"
-msgstr "מי שילם?"
+msgid "Add a new bill"
+msgstr ""
 
 msgid "For what?"
-msgstr "עבור מה?"
-
-msgid "How much?"
-msgstr "כמה?"
+msgstr ""
 
 #, python-format
 msgid "Added on %(date)s"
-msgstr "נוסף בתאריך %(date)s"
+msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -827,26 +838,26 @@
 msgid "add a bill"
 msgstr ""
 
 msgid "add participants"
 msgstr ""
 
 msgid "Password reminder"
-msgstr "תזכורת סיסמה"
+msgstr ""
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
 
 msgid "Return to home page"
-msgstr "חזור לעמוד הבית"
+msgstr ""
 
 msgid "Your projects"
-msgstr "הפרויקטים שלך"
+msgstr ""
 
 msgid "Reset your password"
 msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
@@ -855,54 +866,129 @@
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
 
 msgid "Identifier:"
-msgstr "מזהה:"
+msgstr ""
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
 
 msgid "Who pays?"
-msgstr "מי משלם?"
+msgstr ""
 
 msgid "To whom?"
-msgstr "למי?"
+msgstr ""
 
 msgid "Who?"
-msgstr "מי?"
+msgstr ""
 
 msgid "Balance"
 msgstr ""
 
 msgid "deactivate"
 msgstr ""
 
 msgid "reactivate"
 msgstr ""
 
 msgid "Paid"
-msgstr "שולם"
+msgstr ""
 
 msgid "Spent"
 msgstr ""
 
 msgid "Expenses by Month"
 msgstr ""
 
 msgid "Period"
-msgstr "תקופה"
+msgstr ""
+
+#~ msgid "Import"
+#~ msgstr ""
+
+#~ msgid "Amount paid"
+#~ msgstr "Kifizetett összeg"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "A számla nem lehet üres"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Meghívók küldése"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2020-06-14 14:41+0000\n"
 "Last-Translator: raghupalash <singhpalash0@gmail.com>\n"
 "Language: hi\n"
 "Language-Team: Hindi <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/hi/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>नीचे दी गई तालिका परियोजना इतिहास को अक्षम करने से पहले दर्ज की गई "
-"कार्रवाइयों को दर्शाती है। आप उन्हें हटाने के लिए\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">प्रोजेक्ट इतिहास हटा</a>सकते हैं।</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>इस प्रोजेक्ट में इतिहास अक्षम है। नई कार्रवाइयां नीचे दिखाई नहीं देंगी। आप "
-"इतिहास को यहाँ से सक्षम कर सकते हैं</i>\n"
-"              <a href=\"%(url)s\">सेटिंग्स पृष्ठ</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" एक मुफ्त सॉफ्टवेयर है"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s प्रत्येक"
 
@@ -106,17 +78,14 @@
 
 msgid "Amount"
 msgstr "रकम"
 
 msgid "Amount in %(currency)s"
 msgstr "%(currency)s में राशि"
 
-msgid "Amount paid"
-msgstr "भुगतान की गई राशि"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "क्या आप वाकई इस प्रोजेक्ट के सभी रिकॉर्ड किए गए IP पतों को हटाना चाहते हैं?\n"
@@ -138,17 +107,14 @@
 
 msgid "Bill items"
 msgstr "बिल आइटम"
 
 msgid "Bills"
 msgstr "बिल"
 
-msgid "Bills can't be null"
-msgstr "बिल शून्य नहीं हो सकते"
-
 msgid "Can't remember the password?"
 msgstr "पासवर्ड याद नहीं?"
 
 msgid "Cancel"
 msgstr "रद्द करें"
 
 msgid "Choose file"
@@ -293,26 +259,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "आईपी पता रिकॉर्डिंग को सेटिंग पेज पर सक्षम किया जा सकता है"
 
 msgid "Identifier:"
 msgstr "पहचानकर्ता:"
 
-msgid "Import"
-msgstr "आयात"
-
-msgid "Import JSON"
-msgstr "JSON को आयात करे"
-
-msgid "Import previously exported JSON file"
-msgstr "पूर्व में निर्यात की गई JSON फ़ाइल आयात करें"
-
-msgid "Invalid JSON"
-msgstr "अमान्य JSON"
-
 msgid "Invalid token"
 msgstr "अमान्य टोकन"
 
 msgid "Invite people"
 msgstr "लोगों को निमंत्रण भेजें"
 
 msgid "Invite people to join this project"
@@ -483,29 +437,14 @@
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr "नीचे कुछ प्रविष्टियों में IP पते हैं, भले ही इस परियोजना में IP रिकॉर्डिंग अक्षम है। "
 
 msgid "Someone probably cleared the project history."
 msgstr "किसी ने शायद परियोजना के इतिहास को हटा दिया है।"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"क्षमा करें, पासवर्ड रीसेट निर्देशों के साथ आपको एक ईमेल भेजते समय कोई त्रुटि हुई थी। कृपया "
-"सर्वर के ईमेल कॉन्फ़िगरेशन की जाँच करें या व्यवस्थापक से संपर्क करें।"
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"क्षमा करें, आमंत्रण ईमेल भेजने का प्रयास करते समय कोई त्रुटि हुई। कृपया सर्वर के ईमेल "
-"कॉन्फ़िगरेशन की जाँच करें या व्यवस्थापक से संपर्क करें।"
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "क्षमा करें, हम आपके द्वारा मांगे गए पृष्ठ को खोजने में असमर्थ थे।"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -544,17 +483,14 @@
 
 msgid "The bill has been modified"
 msgstr "बिल को संशोधित कर दिया गया है"
 
 msgid "The email %(email)s is not valid"
 msgstr "ईमेल %(email)s मान्य नहीं है"
 
-msgid "The project identifier is %(project)s"
-msgstr "प्रोजेक्ट पहचानकर्ता %(project)s है"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 "जिस प्रोजेक्ट पर आप पहुचने की कोशिश कर रहे हैं, वह मौजूद नहीं है, क्या आप यह करना चाहते हैं"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "यह व्यवस्थापक पासवर्ड सही नहीं है। केवल %(num)d प्रयास बचे हैं।"
 
@@ -566,17 +502,14 @@
 
 msgid "Time"
 msgstr "समय"
 
 msgid "To whom?"
 msgstr "किसको?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "बहुत से विफल लॉगिन प्रयास, कृपया बाद में पुनः प्रयास करें।"
-
 msgid "Try out the demo"
 msgstr "डेमो आज़माएं"
 
 msgid "Unknown project"
 msgstr "अज्ञात परियोजना"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/hi/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/hi/LC_MESSAGES/messages.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2020-06-14 14:41+0000\n"
 "Last-Translator: raghupalash <singhpalash0@gmail.com>\n"
 "Language: hi\n"
 "Language-Team: Hindi <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/hi/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "आपने अभी अभी अपने खर्चों को साझा करने के लिए '%(project)s' बनाया है"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "वैध राशि या चिह्न नहीं। केवल संख्या और + - * / ऑपरेटरों को स्वीकार किया "
 "जाता है।"
 
@@ -48,19 +52,16 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
-msgstr "पूर्व में निर्यात की गई JSON फ़ाइल आयात करें"
-
-msgid "Import"
-msgstr "आयात"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "परियोजना पहचानकर्ता"
 
 msgid "Private code"
 msgstr "निजी कोड"
 
@@ -116,25 +117,25 @@
 
 msgid "Password confirmation"
 msgstr "पासवर्ड पुष्टीकरण"
 
 msgid "Reset password"
 msgstr "पासवर्ड रीसेट"
 
-msgid "Date"
-msgstr "तारीख"
+msgid "When?"
+msgstr "कब?"
 
 msgid "What?"
 msgstr "क्या?"
 
-msgid "Payer"
-msgstr "भुगतानकर्ता"
+msgid "Who paid?"
+msgstr "किसने भुगतान किया?"
 
-msgid "Amount paid"
-msgstr "भुगतान की गई राशि"
+msgid "How much?"
+msgstr "कितना?"
 
 msgid "Currency"
 msgstr "मुद्रा"
 
 msgid "External link"
 msgstr "बाहरी लिंक"
 
@@ -150,17 +151,14 @@
 msgid "Submit and add a new one"
 msgstr "जमा करें और एक नया जोड़ें"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "प्रोजेक्ट डिफ़ॉल्ट:%(currency)s"
 
-msgid "Bills can't be null"
-msgstr "बिल शून्य नहीं हो सकते"
-
 msgid "Name"
 msgstr "नाम"
 
 msgid "Weights should be positive"
 msgstr "वज़न सकारात्मक होना चाहिए"
 
 msgid "Weight"
@@ -176,21 +174,35 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "इस परियोजना में पहले से ही यह सदस्य है"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "आमंत्रण भेजें"
+msgid "Send the invitations"
+msgstr "निमंत्रण भेजें"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "ईमेल %(email)s मान्य नहीं है"
 
+msgid "Logout"
+msgstr "लॉग आउट"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"क्षमा करें, आमंत्रण ईमेल भेजने का प्रयास करते समय कोई त्रुटि हुई। कृपया "
+"सर्वर के ईमेल कॉन्फ़िगरेशन की जाँच करें या व्यवस्थापक से संपर्क करें।"
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -210,49 +222,42 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "बहुत से विफल लॉगिन प्रयास, कृपया बाद में पुनः प्रयास करें।"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "यह व्यवस्थापक पासवर्ड सही नहीं है। केवल %(num)d प्रयास बचे हैं।"
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "यह निजी कोड सही नहीं है"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "आपने अभी अभी अपने खर्चों को साझा करने के लिए '%(project)s' बनाया है"
-
 msgid "A reminder email has just been sent to you"
 msgstr "आपको अभी एक अनुस्मारक ईमेल भेजा गया है"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "हमने आपको एक अनुस्मारक ईमेल भेजने की कोशिश की, लेकिन कोई त्रुटि थी। आप "
 "अभी भी सामान्य रूप से प्रोजेक्ट का उपयोग कर सकते हैं।"
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "प्रोजेक्ट पहचानकर्ता %(project)s है"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "क्षमा करें, पासवर्ड रीसेट निर्देशों के साथ आपको एक ईमेल भेजते समय कोई "
 "त्रुटि हुई थी। कृपया सर्वर के ईमेल कॉन्फ़िगरेशन की जाँच करें या "
 "व्यवस्थापक से संपर्क करें।"
 
 msgid "No token provided"
 msgstr "कोई टोकन प्रदान नहीं किया गया"
@@ -262,44 +267,49 @@
 
 msgid "Unknown project"
 msgstr "अज्ञात परियोजना"
 
 msgid "Password successfully reset."
 msgstr "पासवर्ड सफलतापूर्वक रीसेट हो गया है।"
 
-msgid "Project successfully uploaded"
-msgstr "प्रोजेक्ट सफलतापूर्वक अपलोड किया गया"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "अमान्य JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "प्रोजेक्ट सफलतापूर्वक अपलोड किया गया"
+
 msgid "Project successfully deleted"
 msgstr "प्रोजेक्ट सफलतापूर्वक हटा दिया गया"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 "आपको %(project)s के लिए अपने खर्चों को साझा करने के लिए आमंत्रित किया गया"
 " है"
 
 msgid "Your invitations have been sent"
 msgstr "आपके निमंत्रण भेज दिए गए हैं"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "क्षमा करें, आमंत्रण ईमेल भेजने का प्रयास करते समय कोई त्रुटि हुई। कृपया "
 "सर्वर के ईमेल कॉन्फ़िगरेशन की जाँच करें या व्यवस्थापक से संपर्क करें।"
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s को जोड़ लिया गया है"
@@ -338,14 +348,18 @@
 
 msgid "The bill has been deleted"
 msgstr "बिल को हटा दिया गया है"
 
 msgid "The bill has been modified"
 msgstr "बिल को संशोधित कर दिया गया है"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "प्रोजेक्ट इतिहास सक्षम करें"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "प्रोजेक्ट इतिहास सक्षम करें"
@@ -405,16 +419,17 @@
 
 msgid "Actions"
 msgstr "कार्य"
 
 msgid "edit"
 msgstr "संपादित करें"
 
-msgid "delete"
-msgstr "हटाइये"
+#, fuzzy
+msgid "Delete project"
+msgstr "परियोजना संपादित करें"
 
 msgid "show"
 msgstr "प्रदर्शन"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "डैशबोर्ड वर्तमान में निष्क्रिय है।"
 
@@ -422,31 +437,21 @@
 msgid "Download Mobile Application"
 msgstr "मोबाइल एप्लीकेशन"
 
 #, fuzzy
 msgid "Get it on"
 msgstr "अंदर जाइये"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "आपको यकीन है?"
-
 msgid "Edit project"
 msgstr "परियोजना संपादित करें"
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "परियोजना संपादित करें"
 
-msgid "Import JSON"
-msgstr "JSON को आयात करे"
-
-msgid "Choose file"
-msgstr "फ़ाइल चुनें"
-
 msgid "Download project's data"
 msgstr "प्रोजेक्ट का डेटा डाउनलोड करें"
 
 msgid "Bill items"
 msgstr "बिल आइटम"
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -463,26 +468,36 @@
 
 msgid "Cancel"
 msgstr "रद्द करें"
 
 msgid "Privacy Settings"
 msgstr "प्राइवेसी सेटिंग्स"
 
-msgid "Edit the project"
-msgstr "प्रोजेक्ट संपादित करें"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "पूर्व में निर्यात की गई JSON फ़ाइल आयात करें"
+
+msgid "Choose file"
+msgstr "फ़ाइल चुनें"
+
 msgid "Edit this bill"
 msgstr "इस बिल को संपादित करें"
 
 msgid "Add a bill"
 msgstr "बिल जोड़ें"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "सब"
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -494,17 +509,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "प्रतिभागी जोड़ें"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "निमंत्रण भेजें"
-
 msgid "Download"
 msgstr "डाउनलोड"
 
 msgid "Disabled Project History"
 msgstr "प्रोजेक्ट इतिहास अक्षम किया गया"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -568,67 +580,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>इस प्रोजेक्ट में इतिहास अक्षम है। नई कार्रवाइयां नीचे "
-"दिखाई नहीं देंगी। आप इतिहास को यहाँ से सक्षम कर सकते हैं</i>\n"
-"              <a href=\"%(url)s\">सेटिंग्स पृष्ठ</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "आईपी पता रिकॉर्डिंग को सेटिंग पेज पर सक्षम किया जा सकता है"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>नीचे दी गई तालिका परियोजना इतिहास को अक्षम करने से पहले "
-"दर्ज की गई कार्रवाइयों को दर्शाती है। आप उन्हें हटाने के लिए\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">प्रोजेक्ट इतिहास हटा</a>सकते हैं।</i></p>"
-"\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "किसी ने शायद परियोजना के इतिहास को हटा दिया है।"
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "नीचे कुछ प्रविष्टियों में IP पते हैं, भले ही इस परियोजना में IP "
 "रिकॉर्डिंग अक्षम है। "
 
 msgid "Delete stored IP addresses"
 msgstr "संग्रहीत IP पते हटाएं"
 
-msgid "No history to erase"
-msgstr "मिटाने के लिए कोई इतिहास नहीं है"
-
-msgid "Clear Project History"
-msgstr "प्रोजेक्ट इतिहास हटाएं"
-
 msgid "No IP Addresses to erase"
 msgstr "मिटाने के लिए कोई IP पते नहीं हैं"
 
 msgid "Delete Stored IP Addresses"
 msgstr "संग्रहीत IP पते हटाएं"
 
+msgid "No history to erase"
+msgstr "मिटाने के लिए कोई इतिहास नहीं है"
+
+msgid "Clear Project History"
+msgstr "प्रोजेक्ट इतिहास हटाएं"
+
 msgid "Time"
 msgstr "समय"
 
 msgid "Event"
 msgstr "घटना"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -682,17 +679,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "भुगतानकर्ता"
+
 msgid "Amount"
 msgstr "रकम"
 
+msgid "Date"
+msgstr "तारीख"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "%(currency)s में राशि"
 
 #, fuzzy, python-format
 msgid "Bill %(name)s modified"
 msgstr "बिल को संशोधित कर दिया गया है"
@@ -796,16 +799,17 @@
 
 msgid "switch to"
 msgstr "पर स्विच करें"
 
 msgid "Dashboard"
 msgstr "डैशबोर्ड"
 
-msgid "Logout"
-msgstr "लॉग आउट"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "कोड"
 
 msgid "Mobile Application"
 msgstr "मोबाइल एप्लीकेशन"
 
@@ -831,46 +835,40 @@
 
 msgid "you sure?"
 msgstr "आपको यकीन है?"
 
 msgid "Invite people"
 msgstr "लोगों को निमंत्रण भेजें"
 
-msgid "You should start by adding participants"
-msgstr "शुरू करने के लिए प्रतिभागियों को जोड़ें"
-
-msgid "Add a new bill"
-msgstr "नया बिल जोड़ें"
-
 msgid "Newer bills"
 msgstr "नए बिल"
 
 msgid "Older bills"
 msgstr "पुराने बिल"
 
-msgid "When?"
-msgstr "कब?"
+msgid "You should start by adding participants"
+msgstr "शुरू करने के लिए प्रतिभागियों को जोड़ें"
 
-msgid "Who paid?"
-msgstr "किसने भुगतान किया?"
+msgid "Add a new bill"
+msgstr "नया बिल जोड़ें"
 
 msgid "For what?"
 msgstr "किस लिए?"
 
-msgid "How much?"
-msgstr "कितना?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "%(date)s पर जोड़ा गया"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "%(excluded)s को छोड़ के बाकी सब"
 
+msgid "delete"
+msgstr "हटाइये"
+
 msgid "No bills"
 msgstr "कोई बिल नहीं"
 
 msgid "Nothing to list yet."
 msgstr "सूचि बनाने के लिए कुछ नहीं।"
 
 msgid "You probably want to"
@@ -919,14 +917,20 @@
 
 msgid "Share the Link"
 msgstr "लिंक साझा करें"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "आप नीचे दिए गए लिंक को सीधे अपने पसंदीदा माध्यम से साझा कर सकते हैं"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "ईमेल के माध्यम से भेजें"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1031,7 +1035,78 @@
 #~ "नहीं है।"
 
 #~ msgid "User name incorrect"
 #~ msgstr "उपयोगकर्ता नाम गलत है"
 
 #~ msgid "People to notify"
 #~ msgstr "सूचित किये जाने वाले लोग"
+
+#~ msgid "Import"
+#~ msgstr "आयात"
+
+#~ msgid "Amount paid"
+#~ msgstr "भुगतान की गई राशि"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "बिल शून्य नहीं हो सकते"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "प्रोजेक्ट पहचानकर्ता %(project)s है"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "अमान्य JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "आपको यकीन है?"
+
+#~ msgid "Import JSON"
+#~ msgstr "JSON को आयात करे"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>इस प्रोजेक्ट में इतिहास "
+#~ "अक्षम है। नई कार्रवाइयां नीचे दिखाई "
+#~ "नहीं देंगी। आप इतिहास को यहाँ से"
+#~ " सक्षम कर सकते हैं</i>\n"
+#~ "              <a href=\"%(url)s\">सेटिंग्स पृष्ठ</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>नीचे दी गई तालिका "
+#~ "परियोजना इतिहास को अक्षम करने से "
+#~ "पहले दर्ज की गई कार्रवाइयों को "
+#~ "दर्शाती है। आप उन्हें हटाने के लिए"
+#~ "\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">प्रोजेक्ट इतिहास "
+#~ "हटा</a>सकते हैं।</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "आमंत्रण भेजें"
+
+#~ msgid " show"
+#~ msgstr "प्रदर्शन"
+
+#~ msgid "Edit the project"
+#~ msgstr "प्रोजेक्ट संपादित करें"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/hu/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Hungarian (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2023-04-19 11:51+0000\n"
+"Last-Translator: Gergely Kocsis <koger23@gmail.com>\n"
+"Language: hu\n"
 "Language-Team: Hungarian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/hu/>\n"
-"Language: hu\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s hozzáadva"
 
 msgid "A link to an external document, related to this bill"
 msgstr "A számlához kapcsolódó külső dokumentum linkje"
 
@@ -31,17 +32,14 @@
 
 msgid "Add"
 msgstr "Hozzáadás"
 
 msgid "Admin password"
 msgstr "Adminisztrátori jelszó"
 
-msgid "Bills can't be null"
-msgstr "A számla nem lehet üres"
-
 msgid "Create the project"
 msgstr "Projekt létrehozása"
 
 msgid "Currency"
 msgstr "Pénznem"
 
 msgid "Date"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/hu/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/cs/LC_MESSAGES/messages.po`

 * *Files 17% similar despite different names*

```diff
@@ -1,307 +1,316 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-01-22 21:15+0200\n"
-"PO-Revision-Date: 2023-04-19 11:51+0000\n"
-"Last-Translator: Gergely Kocsis <koger23@gmail.com>\n"
-"Language-Team: Hungarian <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/hu/>\n"
-"Language: hu\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2022-11-07 10:07+0000\n"
+"Last-Translator: Moshi Moshi <ifeeltiredboss@gmail.com>\n"
+"Language: cs\n"
+"Language-Team: Czech <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/cs/>\n"
+"Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
+"Generated-By: Babel 2.9.0\n"
+
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
 
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
-msgstr ""
-"Érvénytelen mennyiség vagy kifejezés. Csak számok és műveleti jelek ( + - * "
-"/) megengedettek."
+msgstr "Neplatná částka nebo výraz. Pouze čísla a operátory + - * / jsou přípustná"
 
 msgid "Project name"
-msgstr "A projekt neve"
+msgstr "Název projektu"
 
 msgid "New private code"
-msgstr "Új titkos kód"
+msgstr "Nový soukromý kód"
 
 msgid "Enter a new code if you want to change it"
-msgstr "Adj meg egy új kódot, ha meg akarod változtatni"
+msgstr "Pokud chcete provést změnu vložte nový kód"
 
 msgid "Email"
 msgstr "Email"
 
 msgid "Enable project history"
-msgstr "Projekt történet bekapcsolása"
+msgstr "Povolit historii projektu"
 
 msgid "Use IP tracking for project history"
-msgstr "IP nyomkövetés használata a projekt előzményekhez"
+msgstr "Záznam IP adres pro historii projektu"
 
 msgid "Default Currency"
-msgstr "Alapértelmezett Pénznem"
+msgstr "Výchozí měna"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"Alapértelmezett pénznem beállítása lehetővé teszi a számlák közötti "
-"pénzváltást"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"A projekt nem állítható pénznem nélkülire, mert számlákat és több pénznemet "
-"is tartalmaz."
+"Tento projekt nemůže být nastaven na 'bez měny' protože obsahuje účty v "
+"různých měnáh."
 
-msgid "Import previously exported JSON file"
-msgstr "Korábban exportált JSON fájl importálása"
-
-msgid "Import"
+msgid "Compatible with Cospend"
 msgstr ""
 
 msgid "Project identifier"
-msgstr "Projekt azonosító"
+msgstr "Identifikátor projektu"
 
 msgid "Private code"
-msgstr "Titkos kód"
+msgstr "Přístupový kód"
 
 msgid "Create the project"
-msgstr "Projekt létrehozása"
+msgstr "Vytvořit projekt"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Már létezik egy projekt ezzel az azonosítóval (\"%(project)s\"). Kérjük, "
-"válasszon más azonosítót"
+"Projekt s tímto identifikátorem (\"%(project)s\") již existuje, zvolte "
+"nový identifikátor"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
-msgstr "Melyik valódi pénznem, az euró vagy a petrodollár?"
+msgstr ""
 
 msgid "euro"
-msgstr "euró"
+msgstr ""
 
 msgid "Please, validate the captcha to proceed."
-msgstr "Kérlek validáld a captcha-t a folytatáshoz."
+msgstr ""
 
 msgid "Enter private code to confirm deletion"
-msgstr "Add meg a titkos kódot a törlés megerősítéséhez"
+msgstr "Potvrďte smazání vložením soukromého kódu"
 
 msgid "Unknown error"
-msgstr "Ismeretlen hiba"
+msgstr "Neznámá chyba"
 
 msgid "Invalid private code."
-msgstr "Érvénytelen titkos kód."
+msgstr "Neplatný soukromý přístupový kód."
 
-#, fuzzy
 msgid "Get in"
-msgstr "Szállj be"
+msgstr "Vstoupit"
 
 msgid "Admin password"
-msgstr "Adminisztrátori jelszó"
+msgstr "Administrátorské heslo"
 
 msgid "Send me the code by email"
-msgstr "Kód küldése e-mailben"
+msgstr "Poslat kód na e-mail"
 
 msgid "This project does not exists"
-msgstr "Ez a projekt nem létezik"
+msgstr "Tento projekt neexistuje"
 
 msgid "Password mismatch"
-msgstr "A jelszavak nem egyeznek"
+msgstr "Heslo nesouhlasí"
 
 msgid "Password"
-msgstr "Jelszó"
+msgstr "Heslo"
 
 msgid "Password confirmation"
-msgstr "Jelszó megerősítése"
+msgstr "Potvrzení hesla"
 
 msgid "Reset password"
-msgstr "Jelszó visszaállítása"
+msgstr "Obnova hesla"
 
-msgid "Date"
-msgstr "Dátum"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
-msgstr "Mi?"
+msgstr "Co?"
 
-msgid "Payer"
-msgstr "Fizető"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "Kifizetett összeg"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
-msgstr "Pénznem"
+msgstr "Měna"
 
 msgid "External link"
-msgstr "Külső hivatkozás"
+msgstr "Externí odkaz"
 
 msgid "A link to an external document, related to this bill"
-msgstr "A számlához kapcsolódó külső dokumentum linkje"
+msgstr "Externí odkaz k této účtence"
 
 msgid "For whom?"
-msgstr "Kinek?"
+msgstr "Od koho?"
 
 msgid "Submit"
-msgstr "Mentés"
+msgstr "Odeslat"
 
 msgid "Submit and add a new one"
-msgstr "Mentés és új hozzáadása"
+msgstr "Odeslat a přidat nový"
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr "Projekt alapértelmezés: %(currency)s"
-
-msgid "Bills can't be null"
-msgstr "A számla nem lehet üres"
+msgstr "Výchozí měna projektu: %(currency)s"
 
 msgid "Name"
-msgstr "Név"
+msgstr "Jméno"
 
 msgid "Weights should be positive"
-msgstr "A súlyoknak pozitív értékűnek kell lenni"
+msgstr "Váhy musí být kladné"
 
 msgid "Weight"
-msgstr "Súly"
+msgstr "Váha"
 
 msgid "Add"
-msgstr "Hozzáadás"
+msgstr "Přidat"
 
 msgid "The participant name is invalid"
-msgstr "A résztvevő neve érvénytelen"
+msgstr ""
 
+#, fuzzy
 msgid "This project already have this participant"
-msgstr "Ez a résztvevő már szerepel ebben a projektben"
+msgstr "Projekt již obsahuje tohoto člena"
 
 msgid "People to notify"
-msgstr "Értesítendő személyek"
+msgstr ""
 
-msgid "Send invites"
-msgstr "Meghívók küldése"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
-msgstr "Érvénytelen e-mail cím: %(email)s"
+msgstr "Toto (%(email)s) není validní e-mail"
+
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Omlouváme se, během odesílání emailu s instrukcemi pro obnovení hesla se "
+"vyskytla chyba. Zkontrolujte si prosím nastavení vašeho emailového "
+"serveru nebo kontaktujte administrátora."
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr "{dual_object_0} és {dual_object_1}"
+msgstr "{dual_object_0} a {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr "{previous_object} és {end_object}"
+msgstr "{previous_object}, a {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
-msgstr "{previous_object}, {next_object}"
+msgstr ""
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
-msgstr "{start_object}, {next_object}"
+msgstr ""
 
 msgid "No Currency"
-msgstr "Nincs pénznem"
+msgstr "Žádná měna"
 
 #. Form error with only one error
 msgid "{prefix}: {error}"
-msgstr "{prefix}: {error}"
+msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
-msgstr "{prefix}:<br />{errors}"
-
-msgid "Too many failed login attempts, please retry later."
 msgstr ""
-"Túl sok sikertelen bejelentkezési kísérlet, kérlek, próbáld újra később."
+
+#, fuzzy
+msgid "Too many failed login attempts."
+msgstr "Příliš mnoho pokusů, zkuste to později."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
-msgstr "Az admin jelszó érvénytelen. Csak %(num)d próbálkozásod maradt."
+msgstr ""
 
 msgid "Provided token is invalid"
-msgstr "A megadott token érvénytelen"
+msgstr ""
 
 msgid "This private code is not the right one"
-msgstr "Ez a titkos kód nem megfelelő"
-
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Létrehoztál egy projektet '%(project)s' a kiadásaid megosztására"
+msgstr ""
 
 msgid "A reminder email has just been sent to you"
-msgstr "Az emlékeztető e-mailt kiküldtük"
+msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"Megpróbáltuk az emlékeztető e-mailt kiküldeni, de hiba történt. Ettől még "
-"használhatod a megszokott módon a projektet."
-
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
 
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
+"Omlouváme se, během odesílání emailu s instrukcemi pro obnovení hesla se "
+"vyskytla chyba. Zkontrolujte si prosím nastavení vašeho emailového "
+"serveru nebo kontaktujte administrátora."
 
+#, fuzzy
 msgid "No token provided"
-msgstr "Nincs token megadva"
+msgstr "Nebyl vložen klíč"
 
+#, fuzzy
 msgid "Invalid token"
-msgstr "Érvénytelen token"
+msgstr "Neplatná klíč"
 
 msgid "Unknown project"
-msgstr "Ismeretlen projekt"
+msgstr "Neznámý projekt"
 
 msgid "Password successfully reset."
-msgstr "Jelszó sikeresen visszaállítva."
+msgstr "Heslo bylo úspěšné obnoveno."
 
-msgid "Project successfully uploaded"
-msgstr "Projekt sikeresen feltöltve"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Projekt byl úspěšně nahrán."
+
 msgid "Project successfully deleted"
-msgstr "Projekt sikeresen törölve"
+msgstr "Projekt byl úspěšně smazán"
 
 msgid "Error deleting project"
-msgstr "Hiba történt a projekt törlésekor"
+msgstr "Nastala chyba při mazání projektu"
+
+msgid "Unable to logout"
+msgstr ""
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr "Meghívtak a következő projektbe %(project)s a kiadásaid megosztására"
+msgstr ""
 
 msgid "Your invitations have been sent"
-msgstr "A meghívóid sikeresen kiküldve"
+msgstr "Vaše pozvánka byla odeslána"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
-msgstr "%(member)s hozzáadva"
+msgstr ""
 
 msgid "Error activating participant"
-msgstr "Hiba történt a résztvevő aktiválása közben"
+msgstr ""
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr ""
 
 msgid "Error removing participant"
 msgstr ""
@@ -328,19 +337,25 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
-msgid "Error deleting project history"
+#, python-format
+msgid "%(lang)s is not a supported language"
 msgstr ""
 
+#, fuzzy
+msgid "Error deleting project history"
+msgstr "Povolit historii projektu"
+
+#, fuzzy
 msgid "Deleted project history."
-msgstr ""
+msgstr "Povolit historii projektu"
 
 msgid "Error deleting recorded IP addresses"
 msgstr ""
 
 msgid "Deleted recorded IP addresses in project history."
 msgstr ""
 
@@ -368,15 +383,15 @@
 msgid "?"
 msgstr ""
 
 msgid "Create a new project"
 msgstr ""
 
 msgid "Project"
-msgstr ""
+msgstr "Projekt"
 
 msgid "Number of participants"
 msgstr ""
 
 msgid "Number of bills"
 msgstr ""
 
@@ -388,43 +403,37 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
-msgstr ""
+#, fuzzy
+msgid "Delete project"
+msgstr "Vytvořit projekt"
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
+#, fuzzy
 msgid "Get it on"
-msgstr ""
-
-msgid "Are you sure?"
-msgstr ""
+msgstr "Vstoupit"
 
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "Vytvořit projekt"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -442,26 +451,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Import exportovaného JSON souboru"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -472,17 +491,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -539,51 +555,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -593,17 +604,17 @@
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 
 msgid "From IP"
 msgstr ""
 
-#, python-format
+#, fuzzy, python-format
 msgid "Project %(name)s added"
-msgstr ""
+msgstr "Název projektu"
 
 #, python-format
 msgid "Bill %(name)s added"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s added"
@@ -639,17 +650,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Platící"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "Datum"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -751,15 +768,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -785,46 +803,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -869,14 +881,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -908,7 +926,186 @@
 msgstr ""
 
 msgid "Expenses by Month"
 msgstr ""
 
 msgid "Period"
 msgstr ""
+
+#~ msgid "%(msg_compl)sThe project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid "each"
+#~ msgstr ""
+
+#~ msgid "Error while sending reminder email"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "This access code will be sent to"
+#~ " your friends. It is stored as-"
+#~ "is by the server, so don\\'t reuse"
+#~ " a personal password!"
+#~ msgstr ""
+
+#~ msgid "Participant"
+#~ msgstr "Účastník"
+
+#~ msgid "Bill"
+#~ msgstr "Účet"
+
+#~ msgid "Select all"
+#~ msgstr ""
+
+#~ msgid "Select none"
+#~ msgstr ""
+
+#~ msgid "changed"
+#~ msgstr ""
+
+#~ msgid "from"
+#~ msgstr ""
+
+#~ msgid "to"
+#~ msgstr ""
+
+#~ msgid "Confirm Delete"
+#~ msgstr ""
+
+#~ msgid "Added"
+#~ msgstr ""
+
+#~ msgid "Removed"
+#~ msgstr ""
+
+#~ msgid "and"
+#~ msgstr ""
+
+#~ msgid "owers list"
+#~ msgstr ""
+
+#~ msgid "added"
+#~ msgstr ""
+
+#~ msgid "Project renamed to"
+#~ msgstr ""
+
+#~ msgid "Project contact email changed to"
+#~ msgstr ""
+
+#~ msgid "deactivated"
+#~ msgstr ""
+
+#~ msgid "reactivated"
+#~ msgstr ""
+
+#~ msgid "renamed to"
+#~ msgstr ""
+
+#~ msgid "External link changed to"
+#~ msgstr ""
+
+#~ msgid "modified"
+#~ msgstr ""
+
+#~ msgid "removed"
+#~ msgstr ""
+
+#~ msgid "changed in a unknown way"
+#~ msgstr ""
+
+#~ msgid "You either provided a bad token or no project identifier."
+#~ msgstr ""
+
+#~ msgid "User name incorrect"
+#~ msgstr "Nesprávné uživatelské jméno"
+
+#~ msgid "People to notify"
+#~ msgstr "Osoby k informování"
+
+#~ msgid "Error activating member"
+#~ msgstr ""
+
+#~ msgid "Error removing member"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "User '%(name)s' has been deactivated. It"
+#~ " will still appear in the users "
+#~ "list until its balance becomes zero."
+#~ msgstr ""
+
+#~ msgid "User '%(name)s' has been removed"
+#~ msgstr ""
+
+#~ msgid "User '%(name)s' has been edited"
+#~ msgstr ""
+
+#~ msgid "Number of members"
+#~ msgstr ""
+
+#~ msgid "Edit this member"
+#~ msgstr ""
+
+#~ msgid "Participants to notify"
+#~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "Import"
+
+#~ msgid "Amount paid"
+#~ msgstr "Zaplacená částka"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Účtenka nemůže být nulová"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Neplatný JSON"
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Poslat pozvánky"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,23 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Indonesian (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-04-11 17:12+0000\n"
+"Last-Translator: Santiago José Gutiérrez Llanos <gutierrezapata17@gmail."
+"com>\n"
+"Language: id\n"
 "Language-Team: Indonesian <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/id/>\n"
-"Language: id\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.12-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i> Tabel di bawah mencerminkan tindakan yang direkam sebelum "
-"menonaktifkan riwayat proyek. Anda bisa\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\"> membersihkan riwayat proyek </a> untuk "
-"menghapusnya. </i> </ p >\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i> Proyek ini memiliki riwayat yang dinonaktifkan. Tindakan "
-"baru tidak akan muncul di bawah ini. Anda dapat mengaktifkan riwayat pada</"
-"i>\n"
-"            <a href=\"%(url)s\">halaman pengaturan</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" adalah perangkat lunak gratis"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s masing-masing"
 
@@ -110,17 +82,14 @@
 
 msgid "Amount"
 msgstr "Jumlah"
 
 msgid "Amount in %(currency)s"
 msgstr "Jumlah dalam %(currency)s"
 
-msgid "Amount paid"
-msgstr "Jumlah bayar"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Anda yakin ingin menghapus semua alamat IP yang direkam dari proyek ini?\n"
@@ -130,17 +99,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Anda yakin ingin menghapus semua riwayat untuk proyek ini? Tindakan ini "
 "tidak bisa dibatalkan."
 
-msgid "Are you sure?"
-msgstr "Apakah Anda yakin?"
-
 msgid "Authentication"
 msgstr "Otentikasi"
 
 msgid "Back to the list"
 msgstr "Kembali ke daftar"
 
 msgid "Balance"
@@ -163,17 +129,14 @@
 
 msgid "Bill items"
 msgstr "Item tagihan"
 
 msgid "Bills"
 msgstr "Tagihan"
 
-msgid "Bills can't be null"
-msgstr "Tagihan tidak boleh kosong"
-
 msgid "Can't remember the password?"
 msgstr "Tidak bisa mengingat kata sandi?"
 
 msgid "Cancel"
 msgstr "Batalkan"
 
 msgid "Choose file"
@@ -354,26 +317,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "Perekaman alamat IP dapat diaktifkan di halaman pengaturan"
 
 msgid "Identifier:"
 msgstr "ID:"
 
-msgid "Import"
-msgstr "Impor"
-
-msgid "Import JSON"
-msgstr "Impor JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Impor file JSON yang sudah diekspor sebelumnya"
-
-msgid "Invalid JSON"
-msgstr "JSON tidak valid"
-
 msgid "Invalid private code."
 msgstr "Kode pribadi tidak valid."
 
 msgid "Invalid token"
 msgstr "Token tidak benar"
 
 msgid "Invite people"
@@ -629,29 +580,14 @@
 msgstr ""
 "Beberapa entri dibawah mengandung alamat IP, walaupun proyek ini "
 "menonaktifkan rekaman alamat IP. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Seseorang mungkin membersihkan riwayat proyek."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Maaf, ada galat saat mengirim email berisi instruksi pengaturan ulang kata "
-"sandi. Silakan periksa konfigurasi email peladen atau hubungi administrator."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Maaf, ada galat saat mencoba mengirim email undangan. Silakan periksa "
-"konfigurasi email peladen atau hubungi administrator."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Maaf, kami tidak bisa menemukan halaman yang Anda minta."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -694,17 +630,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "Surel %(email)s tidak valid"
 
 msgid "The participant name is invalid"
 msgstr "Nama pengguna tidak valid"
 
-msgid "The project identifier is %(project)s"
-msgstr "Pengidentifikasi proyek adalah %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Anda mencoba mengakses proyek yang tidak ada, apakah Anda ingin"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Kata sandi admin ini tidak cocok. Hanya tinggal %(num)d percobaan lagi."
 
@@ -726,17 +659,14 @@
 
 msgid "Time"
 msgstr "Waktu"
 
 msgid "To whom?"
 msgstr "Kepada siapa?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Terlalu banyak percobaan masuk, silakan coba lagi nanti."
-
 msgid "Try out the demo"
 msgstr "Coba demo"
 
 msgid "Unknown error"
 msgstr "Kesalahan tidak diketahui"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/id/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/id/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-04-11 17:12+0000\n"
-"Last-Translator: Santiago José Gutiérrez Llanos <gutierrezapata17@gmail.com>"
-"\n"
-"Language-Team: Indonesian <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/id/>\n"
+"Last-Translator: Santiago José Gutiérrez Llanos "
+"<gutierrezapata17@gmail.com>\n"
 "Language: id\n"
+"Language-Team: Indonesian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/id/>\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.12-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Anda baru saja membuat %(project)s untuk membagikan harga Anda"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Bukan jumlah atau operator yang valid. Hanya angka dan operator + -* / "
 "yang diterima."
 
@@ -41,29 +45,25 @@
 msgid "Use IP tracking for project history"
 msgstr "Gunakan pelacakan IP untuk riwayat proyek"
 
 msgid "Default Currency"
 msgstr "Mata Uang Standar"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr ""
-"Menetapkan mata uang default memungkinkan konversi mata uang antar tagihan"
+msgstr "Menetapkan mata uang default memungkinkan konversi mata uang antar tagihan"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Proyek ini tidak dapat disetel ke 'tanpa mata uang' karena berisi tagihan"
 " dalam berbagai mata uang."
 
-msgid "Import previously exported JSON file"
-msgstr "Impor file JSON yang sudah diekspor sebelumnya"
-
-msgid "Import"
-msgstr "Impor"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Pengidentifikasi proyek"
 
 msgid "Private code"
 msgstr "Kode pribadi"
 
@@ -116,25 +116,25 @@
 
 msgid "Password confirmation"
 msgstr "Konfirmasi kata sandi"
 
 msgid "Reset password"
 msgstr "Atur ulang kata sandi"
 
-msgid "Date"
-msgstr "Tanggal"
+msgid "When?"
+msgstr "Kapan?"
 
 msgid "What?"
 msgstr "Apa?"
 
-msgid "Payer"
-msgstr "Pembayar"
+msgid "Who paid?"
+msgstr "Siapa yang bayar?"
 
-msgid "Amount paid"
-msgstr "Jumlah bayar"
+msgid "How much?"
+msgstr "Berapa banyak?"
 
 msgid "Currency"
 msgstr "Mata Uang"
 
 msgid "External link"
 msgstr "Tautan luar"
 
@@ -150,17 +150,14 @@
 msgid "Submit and add a new one"
 msgstr "Ajukan dan tambah yang baru"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Default proyek: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Tagihan tidak boleh kosong"
-
 msgid "Name"
 msgstr "Nama"
 
 msgid "Weights should be positive"
 msgstr "Bobot harus positif"
 
 msgid "Weight"
@@ -174,21 +171,35 @@
 
 msgid "This project already have this participant"
 msgstr "Proyek ini sudah mempunyai /ada anggota ini"
 
 msgid "People to notify"
 msgstr "Orang yang akan dinotifikasi"
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "Kirim undangan"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Surel %(email)s tidak valid"
 
+msgid "Logout"
+msgstr "Keluar"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Maaf, ada galat saat mencoba mengirim email undangan. Silakan periksa "
+"konfigurasi email peladen atau hubungi administrator."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} dan {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, dan {end_object}"
@@ -208,49 +219,42 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:1<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Terlalu banyak percobaan masuk, silakan coba lagi nanti."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Kata sandi admin ini tidak cocok. Hanya tinggal %(num)d percobaan lagi."
 
 msgid "Provided token is invalid"
 msgstr "Token yang disediakan tidak valid"
 
 msgid "This private code is not the right one"
 msgstr "Kode pribadi ini tidak benar"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Anda baru saja membuat %(project)s untuk membagikan harga Anda"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Email pengingat baru saja dikirimkan kepada Anda"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Kami telah mengirimi Anda email pengingat, tetapi ada kesalahan. Anda "
 "masih dapat menggunakan proyek secara normal."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Pengidentifikasi proyek adalah %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Maaf, ada galat saat mengirim email berisi instruksi pengaturan ulang "
 "kata sandi. Silakan periksa konfigurasi email peladen atau hubungi "
 "administrator."
 
 msgid "No token provided"
 msgstr "Belum ada token diberikan"
@@ -260,42 +264,47 @@
 
 msgid "Unknown project"
 msgstr "Proyek tidak diketahui"
 
 msgid "Password successfully reset."
 msgstr "Kata sandi berhasil diatur ulang."
 
-msgid "Project successfully uploaded"
-msgstr "Proyek berhasil diunggah"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON tidak valid"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Proyek berhasil diunggah"
+
 msgid "Project successfully deleted"
 msgstr "Proyek berhasil dihapus"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Anda telah diundang untuk membagikan harga Anda untuk %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Undangan Anda telah dikirim"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Maaf, ada galat saat mencoba mengirim email undangan. Silakan periksa "
 "konfigurasi email peladen atau hubungi administrator."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s telah ditambahkan"
@@ -334,14 +343,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Tagihan telah dihapus"
 
 msgid "The bill has been modified"
 msgstr "Tagihan telah diperbarui"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Kesalahan saat menghapus riwayat proyek"
 
 msgid "Deleted project history."
 msgstr "Rriwayat proyek terhapus."
 
 msgid "Error deleting recorded IP addresses"
@@ -394,43 +407,35 @@
 
 msgid "Actions"
 msgstr "Aksi"
 
 msgid "edit"
 msgstr "ubah"
 
-msgid "delete"
-msgstr "hapus"
+msgid "Delete project"
+msgstr "Hapus proyek"
 
 msgid "show"
 msgstr "tampilkan"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Dasbor sekarang ini sedang dinonaktifkan."
 
 msgid "Download Mobile Application"
 msgstr "Unduh Aplikasi Seluler"
 
 msgid "Get it on"
 msgstr "Dapatkan di"
 
-msgid "Are you sure?"
-msgstr "Apakah Anda yakin?"
-
 msgid "Edit project"
 msgstr "Ubah proyek"
 
-msgid "Delete project"
-msgstr "Hapus proyek"
-
-msgid "Import JSON"
-msgstr "Impor JSON"
-
-msgid "Choose file"
-msgstr "Pilih berkas"
+#, fuzzy
+msgid "Import project"
+msgstr "Ubah proyek"
 
 msgid "Download project's data"
 msgstr "Unduh data proyek"
 
 msgid "Bill items"
 msgstr "Item tagihan"
 
@@ -448,26 +453,36 @@
 
 msgid "Cancel"
 msgstr "Batalkan"
 
 msgid "Privacy Settings"
 msgstr "Pengaturan Privasi"
 
-msgid "Edit the project"
-msgstr "Ubah proyek"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Impor file JSON yang sudah diekspor sebelumnya"
+
+msgid "Choose file"
+msgstr "Pilih berkas"
+
 msgid "Edit this bill"
 msgstr "Ubah tagihan ini"
 
 msgid "Add a bill"
 msgstr "Tambah tagihan"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Semua orang"
 
 msgid "No one"
 msgstr "Tidak ada"
 
 msgid "More options"
@@ -478,17 +493,14 @@
 
 msgid "Edit this participant"
 msgstr "Sunting anggota ini"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "Kirim undangan"
-
 msgid "Download"
 msgstr "Unduh"
 
 msgid "Disabled Project History"
 msgstr "Nonaktifkan riwayat proyek"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -551,68 +563,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i> Proyek ini memiliki riwayat yang dinonaktifkan. Tindakan "
-"baru tidak akan muncul di bawah ini. Anda dapat mengaktifkan riwayat "
-"pada</i>\n"
-"            <a href=\"%(url)s\">halaman pengaturan</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "Perekaman alamat IP dapat diaktifkan di halaman pengaturan"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i> Tabel di bawah mencerminkan tindakan yang direkam sebelum"
-" menonaktifkan riwayat proyek. Anda bisa\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\"> membersihkan riwayat proyek </a> untuk "
-"menghapusnya. </i> </ p >\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Seseorang mungkin membersihkan riwayat proyek."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Beberapa entri dibawah mengandung alamat IP, walaupun proyek ini "
 "menonaktifkan rekaman alamat IP. "
 
 msgid "Delete stored IP addresses"
 msgstr "Hapus alamat IP yang disimpan"
 
-msgid "No history to erase"
-msgstr "Tidak ada riwayat untuk dihapus"
-
-msgid "Clear Project History"
-msgstr "Bersihkan Riwayat Proyek"
-
 msgid "No IP Addresses to erase"
 msgstr "Tidak ada Alamat IP untuk dihapus"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Hapus alamat IP yang disimpan"
 
+msgid "No history to erase"
+msgstr "Tidak ada riwayat untuk dihapus"
+
+msgid "Clear Project History"
+msgstr "Bersihkan Riwayat Proyek"
+
 msgid "Time"
 msgstr "Waktu"
 
 msgid "Event"
 msgstr "Peristiwa"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -666,17 +662,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Tagihan %(name)s diganti ke %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr "Pengguna %(name)s: berat berubah dari %(old_weight)s ke %(new_weight)s"
 
+msgid "Payer"
+msgstr "Pembayar"
+
 msgid "Amount"
 msgstr "Jumlah"
 
+msgid "Date"
+msgstr "Tanggal"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Jumlah dalam %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Tagihan %(name)s telah dimodifikasi"
@@ -780,16 +782,17 @@
 
 msgid "switch to"
 msgstr "ganti ke"
 
 msgid "Dashboard"
 msgstr "Dasbor"
 
-msgid "Logout"
-msgstr "Keluar"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Kode"
 
 msgid "Mobile Application"
 msgstr "Aplikasi Gawai"
 
@@ -814,46 +817,40 @@
 
 msgid "you sure?"
 msgstr "Anda yakin?"
 
 msgid "Invite people"
 msgstr "Undang orang"
 
-msgid "You should start by adding participants"
-msgstr "Anda harus mulai dengan menambahkan partisipan"
-
-msgid "Add a new bill"
-msgstr "Tambah tagihan baru"
-
 msgid "Newer bills"
 msgstr "Tagihan terbaru"
 
 msgid "Older bills"
 msgstr "Tagihan terdahulu"
 
-msgid "When?"
-msgstr "Kapan?"
+msgid "You should start by adding participants"
+msgstr "Anda harus mulai dengan menambahkan partisipan"
 
-msgid "Who paid?"
-msgstr "Siapa yang bayar?"
+msgid "Add a new bill"
+msgstr "Tambah tagihan baru"
 
 msgid "For what?"
 msgstr "Untuk apa?"
 
-msgid "How much?"
-msgstr "Berapa banyak?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Ditambahkan pada %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Semua orang kecuali %(excluded)s"
 
+msgid "delete"
+msgstr "hapus"
+
 msgid "No bills"
 msgstr "Tidak ada tagihan"
 
 msgid "Nothing to list yet."
 msgstr "Belum ada untuk didaftarkan."
 
 msgid "You probably want to"
@@ -904,14 +901,20 @@
 msgstr "Bagikan tautan"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 "Anda bisa membagikan tautan secara langsung melalui media yang Anda "
 "inginkan"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Kirim melalui surel"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1042,7 +1045,79 @@
 #~ msgstr "Anda memasukkan token yang salah atau tidak memiliki ID proyek."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Nama pengguna tidak benar"
 
 #~ msgid "People to notify"
 #~ msgstr "Orang yang akan diberi pemberitahuan"
+
+#~ msgid "Import"
+#~ msgstr "Impor"
+
+#~ msgid "Amount paid"
+#~ msgstr "Jumlah bayar"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Tagihan tidak boleh kosong"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Pengidentifikasi proyek adalah %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON tidak valid"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Apakah Anda yakin?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Impor JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i> Proyek ini memiliki "
+#~ "riwayat yang dinonaktifkan. Tindakan baru "
+#~ "tidak akan muncul di bawah ini. "
+#~ "Anda dapat mengaktifkan riwayat pada</i>\n"
+#~ ""
+#~ "            <a href=\"%(url)s\">halaman pengaturan</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i> Tabel di bawah "
+#~ "mencerminkan tindakan yang direkam sebelum "
+#~ "menonaktifkan riwayat proyek. Anda bisa\n"
+#~ ""
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\"> membersihkan riwayat "
+#~ "proyek </a> untuk menghapusnya. </i> </"
+#~ " p >\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Kirim undangan"
+
+#~ msgid " show"
+#~ msgstr "tampilkan"
+
+#~ msgid "Edit the project"
+#~ msgstr "Ubah proyek"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Italian (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-07-12 15:18+0000\n"
+"Last-Translator: Matteo Piotto <piotto@gmail.com>\n"
+"Language: it\n"
 "Language-Team: Italian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/it/>\n"
-"Language: it\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>La tabella seguente riporta le azioni registrate prima della "
-"disabilitazione della cronologia del progetto. È possibile\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">ripulire la cronologia del progetto</a> per "
-"rimuoverle.</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Questo progetto ha la cronologia disattivata. Le nuove azioni "
-"non appariranno qui sotto. È possibile abilitare la cronologia sulla</i>\n"
-"            <a href=\"%(url)s\">pagina delle impostazioni</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" è un software libero"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s ciascuno"
 
@@ -108,17 +80,14 @@
 
 msgid "Amount"
 msgstr "Importo"
 
 msgid "Amount in %(currency)s"
 msgstr "Importo in %(currency)s"
 
-msgid "Amount paid"
-msgstr "Importo pagato"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Sei sicuro di voler cancellare tutti gli indirizzi IP registrati per questo "
@@ -141,17 +110,14 @@
 
 msgid "Bill items"
 msgstr "Addebiti"
 
 msgid "Bills"
 msgstr "Spese"
 
-msgid "Bills can't be null"
-msgstr "L'addebito non può essere nullo"
-
 msgid "Can't remember the password?"
 msgstr "Non ricordi la password?"
 
 msgid "Cancel"
 msgstr "Annulla"
 
 msgid "Choose file"
@@ -306,26 +272,14 @@
 msgstr ""
 "La registrazione degli indirizzi IP può essere attivata nella pagina delle "
 "impostazioni"
 
 msgid "Identifier:"
 msgstr "Identificatore:"
 
-msgid "Import"
-msgstr "Importare"
-
-msgid "Import JSON"
-msgstr "Importa JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Importare il file JSON esportato precedentemente"
-
-msgid "Invalid JSON"
-msgstr "JSON non valido"
-
 msgid "Invalid token"
 msgstr "Token invalido"
 
 msgid "Invite people"
 msgstr "Invita persone"
 
 msgid "Invite people to join this project"
@@ -500,30 +454,14 @@
 
 msgid "Simply sharing money with others?"
 msgstr "Condividi spese con altre persone?"
 
 msgid "Someone probably cleared the project history."
 msgstr "Probabilmente qualcuno ha svuotato lo storico del progetto."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Spiacenti, si è verificato un errore durante l'invio dell'email con le "
-"istruzioni per il reset della password. Verifica la configurazione "
-"dell'email del server o contatta l'amministratore."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Spiacenti, si è verificato un errore durante l'invio delle email di invito. "
-"Verifica la configurazione dell'email sul server o contatta l'amministratore."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Spiacenti, non abbiamo trovato la pagina che cerchi."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -564,17 +502,14 @@
 
 msgid "The bill has been modified"
 msgstr "L'addebito è stato aggiornato"
 
 msgid "The email %(email)s is not valid"
 msgstr "L'email %(email)s non è valida"
 
-msgid "The project identifier is %(project)s"
-msgstr "L'identificatore del progetto è %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Il progetto cui stai provando ad accedere non esiste, vuoi"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Questa password di amministrazione non è quella corretta. Solo %(num)d "
 "tentativi rimasti."
@@ -594,17 +529,14 @@
 
 msgid "Time"
 msgstr "Ora"
 
 msgid "To whom?"
 msgstr "A chi?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Troppi tentativi di accesso non riusciti. Riprova più tardi."
-
 msgid "Try out the demo"
 msgstr "Prova la demo"
 
 msgid "Unknown project"
 msgstr "Progetto non conosciuto"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/it/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/it/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-07-12 15:18+0000\n"
 "Last-Translator: Matteo Piotto <piotto@gmail.com>\n"
-"Language-Team: Italian <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/it/>\n"
 "Language: it\n"
+"Language-Team: Italian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/it/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Hai appena creato '%(project)s' per condividere le tue spese"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Quantità o espressione non valida. Solo numeri e operatori + - * / "
 "accettati."
 
@@ -42,29 +46,26 @@
 msgstr "Utilizzare la localizzazione IP per lo storico del progetto"
 
 msgid "Default Currency"
 msgstr "Valuta predefinita"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"Impostando una valuta predefinita abilita la conversione della valuta tra le "
-"fatture"
+"Impostando una valuta predefinita abilita la conversione della valuta tra"
+" le fatture"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Questo progetto non può essere impostato come 'nessuna valuta' perché "
 "contiene fatture in più valute."
 
-msgid "Import previously exported JSON file"
-msgstr "Importare il file JSON esportato precedentemente"
-
-msgid "Import"
-msgstr "Importare"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identificatore del progetto"
 
 msgid "Private code"
 msgstr "Codice privato"
 
@@ -120,25 +121,25 @@
 
 msgid "Password confirmation"
 msgstr "Conferma password"
 
 msgid "Reset password"
 msgstr "Reset della password"
 
-msgid "Date"
-msgstr "Data"
+msgid "When?"
+msgstr "Quando?"
 
 msgid "What?"
 msgstr "Cosa?"
 
-msgid "Payer"
-msgstr "Pagatore"
+msgid "Who paid?"
+msgstr "Chi ha pagato?"
 
-msgid "Amount paid"
-msgstr "Importo pagato"
+msgid "How much?"
+msgstr "Quanto?"
 
 msgid "Currency"
 msgstr "Valuta"
 
 msgid "External link"
 msgstr "Link esterno"
 
@@ -154,17 +155,14 @@
 msgid "Submit and add a new one"
 msgstr "Invia ed aggiungine uno nuovo"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Impostazione predefinita per il progetto: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "L'addebito non può essere nullo"
-
 msgid "Name"
 msgstr "Nome"
 
 msgid "Weights should be positive"
 msgstr "I pesi dovrebbero essere positivi"
 
 msgid "Weight"
@@ -181,21 +179,36 @@
 msgid "This project already have this participant"
 msgstr "Membro già presente in questo progetto"
 
 #, fuzzy
 msgid "People to notify"
 msgstr "Persone da avvisare"
 
-msgid "Send invites"
-msgstr "Invia inviti"
+msgid "Send the invitations"
+msgstr "Spedisci gli inviti"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "L'email %(email)s non è valida"
 
+msgid "Logout"
+msgstr "Esci"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Spiacenti, si è verificato un errore durante l'invio delle email di "
+"invito. Verifica la configurazione dell'email sul server o contatta "
+"l'amministratore."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -215,51 +228,44 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Troppi tentativi di accesso non riusciti. Riprova più tardi."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Questa password di amministrazione non è quella corretta. Solo %(num)d "
 "tentativi rimasti."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "Questo codice privato non è quello corretto"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Hai appena creato '%(project)s' per condividere le tue spese"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Ti è stato inviato un promemoria per email"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Abbiamo provato a inviarti un promemoria per email, ma si è verificato un"
 " errore. Puoi comunque utilizzare normalmente il progetto."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "L'identificatore del progetto è %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Spiacenti, si è verificato un errore durante l'invio dell'email con le "
 "istruzioni per il reset della password. Verifica la configurazione "
 "dell'email del server o contatta l'amministratore."
 
 msgid "No token provided"
 msgstr "Nessun token fornito"
@@ -269,42 +275,47 @@
 
 msgid "Unknown project"
 msgstr "Progetto non conosciuto"
 
 msgid "Password successfully reset."
 msgstr "Reset della password effettuato."
 
-msgid "Project successfully uploaded"
-msgstr "Progetto caricato con successo"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON non valido"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Progetto caricato con successo"
+
 msgid "Project successfully deleted"
 msgstr "Progetto rimosso con successo"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Sei stato invitato a condividere le tue spese per %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "I tuoi inviti sono stati spediti"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Spiacenti, si è verificato un errore durante l'invio delle email di "
 "invito. Verifica la configurazione dell'email sul server o contatta "
 "l'amministratore."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -344,14 +355,18 @@
 
 msgid "The bill has been deleted"
 msgstr "La spesa è stata cancellata"
 
 msgid "The bill has been modified"
 msgstr "L'addebito è stato aggiornato"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Attivare la cronologia del progetto"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Cronologia del progetto cancellata."
@@ -409,16 +424,17 @@
 
 msgid "Actions"
 msgstr "Azioni"
 
 msgid "edit"
 msgstr "modifica"
 
-msgid "delete"
-msgstr "rimuovi"
+#, fuzzy
+msgid "Delete project"
+msgstr "Modifica progetto"
 
 msgid "show"
 msgstr "visualizza"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Il Cruscotto è attualmente disabilitato."
 
@@ -426,31 +442,21 @@
 msgid "Download Mobile Application"
 msgstr "Applicazione mobile"
 
 #, fuzzy
 msgid "Get it on"
 msgstr "Entra"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "sei sicuro?"
-
 msgid "Edit project"
 msgstr "Modifica progetto"
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "Modifica progetto"
 
-msgid "Import JSON"
-msgstr "Importa JSON"
-
-msgid "Choose file"
-msgstr "Scegli file"
-
 msgid "Download project's data"
 msgstr "Scarica i dati del progetto"
 
 msgid "Bill items"
 msgstr "Addebiti"
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -469,26 +475,36 @@
 
 msgid "Cancel"
 msgstr "Annulla"
 
 msgid "Privacy Settings"
 msgstr "Impostazioni Privacy"
 
-msgid "Edit the project"
-msgstr "Modifica il progetto"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importare il file JSON esportato precedentemente"
+
+msgid "Choose file"
+msgstr "Scegli file"
+
 msgid "Edit this bill"
 msgstr "Modifica questa spesa"
 
 msgid "Add a bill"
 msgstr "Aggiungi un addebito"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Tutti"
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -500,17 +516,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "Aggiungi partecipante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "mario.rossi@example.com, maria.bianchi@site.com"
 
-msgid "Send the invitations"
-msgstr "Spedisci gli inviti"
-
 msgid "Download"
 msgstr "Scarica"
 
 msgid "Disabled Project History"
 msgstr "Cronologia Progetto Disabilitata"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -574,70 +587,56 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Questo progetto ha la cronologia disattivata. Le nuove "
-"azioni non appariranno qui sotto. È possibile abilitare la cronologia "
-"sulla</i>\n"
-"            <a href=\"%(url)s\">pagina delle impostazioni</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr ""
+"La registrazione degli indirizzi IP può essere attivata nella pagina "
+"delle impostazioni"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>La tabella seguente riporta le azioni registrate prima "
-"della disabilitazione della cronologia del progetto. È possibile\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">ripulire la cronologia del progetto</a> "
-"per rimuoverle.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Probabilmente qualcuno ha svuotato lo storico del progetto."
 
 #, fuzzy
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
-"Alcune voci qui sotto contengono indirizzi IP, anche se in questo progetto "
-"la registrazione degli IP è disabilitata. "
+"Alcune voci qui sotto contengono indirizzi IP, anche se in questo "
+"progetto la registrazione degli IP è disabilitata. "
 
 msgid "Delete stored IP addresses"
 msgstr "Cancella indirizzi IP conservati"
 
+msgid "No IP Addresses to erase"
+msgstr "Nessun indirizzo IP da cancellare"
+
+msgid "Delete Stored IP Addresses"
+msgstr "Cancella Indirizzi IP Conservati"
+
 #, fuzzy
 msgid "No history to erase"
 msgstr "Nessuna cronologia da cancellare"
 
 msgid "Clear Project History"
 msgstr "Cancella Cronologia Progetto"
 
-msgid "No IP Addresses to erase"
-msgstr "Nessun indirizzo IP da cancellare"
-
-msgid "Delete Stored IP Addresses"
-msgstr "Cancella Indirizzi IP Conservati"
-
 msgid "Time"
 msgstr "Ora"
 
 msgid "Event"
 msgstr "Evento"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -695,17 +694,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Pagatore"
+
 msgid "Amount"
 msgstr "Importo"
 
+msgid "Date"
+msgstr "Data"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Importo in %(currency)s"
 
 #, fuzzy, python-format
 msgid "Bill %(name)s modified"
 msgstr "L'addebito è stato aggiornato"
@@ -809,16 +814,17 @@
 
 msgid "switch to"
 msgstr "passa a"
 
 msgid "Dashboard"
 msgstr "Cruscotto"
 
-msgid "Logout"
-msgstr "Esci"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Codice"
 
 msgid "Mobile Application"
 msgstr "Applicazione mobile"
 
@@ -844,46 +850,40 @@
 
 msgid "you sure?"
 msgstr "sei sicuro?"
 
 msgid "Invite people"
 msgstr "Invita persone"
 
-msgid "You should start by adding participants"
-msgstr "Dovresti cominciare aggiungendo partecipanti"
-
-msgid "Add a new bill"
-msgstr "Aggiungi una nuova spesa"
-
 msgid "Newer bills"
 msgstr "Addebiti recenti"
 
 msgid "Older bills"
 msgstr "Prime spese"
 
-msgid "When?"
-msgstr "Quando?"
+msgid "You should start by adding participants"
+msgstr "Dovresti cominciare aggiungendo partecipanti"
 
-msgid "Who paid?"
-msgstr "Chi ha pagato?"
+msgid "Add a new bill"
+msgstr "Aggiungi una nuova spesa"
 
 msgid "For what?"
 msgstr "Per cosa?"
 
-msgid "How much?"
-msgstr "Quanto?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Aggiunto il %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Tutti tranne %(excluded)s"
 
+msgid "delete"
+msgstr "rimuovi"
+
 msgid "No bills"
 msgstr "Nessun addebito"
 
 msgid "Nothing to list yet."
 msgstr "Ancora niente da mostrare."
 
 msgid "You probably want to"
@@ -934,14 +934,20 @@
 msgstr "Condividi il Link"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 "Puoi condividere direttamente il seguente link attraverso il tuo canale "
 "preferito"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Inviare via Email"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1066,7 +1072,77 @@
 #~ "valido."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Nome utente non valido"
 
 #~ msgid "People to notify"
 #~ msgstr "Persone da informare"
+
+#~ msgid "Import"
+#~ msgstr "Importare"
+
+#~ msgid "Amount paid"
+#~ msgstr "Importo pagato"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "L'addebito non può essere nullo"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "L'identificatore del progetto è %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON non valido"
+
+#~ msgid "Are you sure?"
+#~ msgstr "sei sicuro?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importa JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Questo progetto ha la "
+#~ "cronologia disattivata. Le nuove azioni "
+#~ "non appariranno qui sotto. È possibile"
+#~ " abilitare la cronologia sulla</i>\n"
+#~ "            <a href=\"%(url)s\">pagina delle impostazioni</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>La tabella seguente riporta "
+#~ "le azioni registrate prima della "
+#~ "disabilitazione della cronologia del progetto."
+#~ " È possibile\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">ripulire la cronologia "
+#~ "del progetto</a> per rimuoverle.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Invia inviti"
+
+#~ msgid " show"
+#~ msgstr "visualizza"
+
+#~ msgid "Edit the project"
+#~ msgstr "Modifica il progetto"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2020-11-11 16:28+0000\n"
 "Last-Translator: Jwen921 <yangjingwen0921@gmail.com>\n"
 "Language: ja\n"
 "Language-Team: Japanese <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/ja/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>下の表では操作不可になる前に、プロジェクトの歴史に対して記録さ"
-"れた操作が反映されています。…できます。\n"
-"<a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">プロジェクトの歴史を取り除く</a> で取り除きます.</"
-"i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>このプロジェクトの歴史は操作できません。新しい操作は下に出ませ"
-"ん。</i>で歴史を操作可能にすることができます。\n"
-"<a href=\"%(url)s\">設定ページ</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\"は無料のソフトウェアです"
 
 msgid "%(amount)s each"
 msgstr "各自に%(amount)s"
 
@@ -107,17 +78,14 @@
 
 msgid "Amount"
 msgstr "金額"
 
 msgid "Amount in %(currency)s"
 msgstr "%(currency)sでの金額"
 
-msgid "Amount paid"
-msgstr "支払額"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "本当にこのプロジェクトから記録されたIPアドレスを全部削除したいですか。\n"
@@ -137,17 +105,14 @@
 
 msgid "Bill items"
 msgstr "明細項目"
 
 msgid "Bills"
 msgstr "明細書"
 
-msgid "Bills can't be null"
-msgstr "数値を空値にしてはいけません"
-
 msgid "Can't remember the password?"
 msgstr "パスワードを覚えていないです？"
 
 msgid "Cancel"
 msgstr "キャンセル"
 
 msgid "Choose file"
@@ -293,26 +258,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "設定ページでIPアドレス記録を編集可能にすることができる"
 
 msgid "Identifier:"
 msgstr "名前："
 
-msgid "Import"
-msgstr "インポート"
-
-msgid "Import JSON"
-msgstr "JSONを導入する"
-
-msgid "Import previously exported JSON file"
-msgstr "以前のJSONファイルをインポートする"
-
-msgid "Invalid JSON"
-msgstr "無効なJSON"
-
 msgid "Invalid token"
 msgstr "無効な印"
 
 msgid "Invite people"
 msgstr "人を誘う"
 
 msgid "Invite people to join this project"
@@ -485,29 +438,14 @@
 msgstr ""
 "このプロジェクトのIP記録が操作できない一方、下の入り口の一部がIPアドレスを含"
 "めています。 "
 
 msgid "Someone probably cleared the project history."
 msgstr "プロジェクトの歴史が誰かに取り除かれたかもしれません。"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"申し訳ございませんが、パスワード再設定の説明メールを送った時、エラーが発生し"
-"ました。メールアドレスを一度確認してまたは管理者に連絡してください。"
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"申し訳ございませんが、招待メールを送ったとき、エラーが発生しました。メールア"
-"ドレスを再度チェックするかまたは管理者に連絡ください。"
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "申し訳ございませんが、求められるページが見つかりませんでした。"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -545,17 +483,14 @@
 
 msgid "The bill has been modified"
 msgstr "明細が変更されました"
 
 msgid "The email %(email)s is not valid"
 msgstr "メールアドレス%(email)sは無効"
 
-msgid "The project identifier is %(project)s"
-msgstr "プロジェクト名は%(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "アクセスしたいプロジェクトは存在していなくて、…したいですか"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "この管理者パスワードは正しくないでウ。%(num)d試行しか残っていません。"
 
 msgid "This private code is not the right one"
@@ -566,17 +501,14 @@
 
 msgid "Time"
 msgstr "時間"
 
 msgid "To whom?"
 msgstr "誰まで？"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "何度もログインに失敗したので、時間をおいてから再度ログインして下さい。"
-
 msgid "Try out the demo"
 msgstr "デモを試す"
 
 msgid "Unknown project"
 msgstr "未知のプロジェクト"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ja/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/ja/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2020-11-11 16:28+0000\n"
 "Last-Translator: Jwen921 <yangjingwen0921@gmail.com>\n"
 "Language: ja\n"
 "Language-Team: Japanese <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/ja/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "費用を共有するため、%(project)sが作られました"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "無効な入力です。数字と「+ - * / 」の演算子しか入力できません。"
 
 msgid "Project name"
 msgstr "プロジェクトの名前"
@@ -46,19 +50,16 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
-msgstr "以前のJSONファイルをインポートする"
-
-msgid "Import"
-msgstr "インポート"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "プロジェクトの名前"
 
 msgid "Private code"
 msgstr "暗証コード"
 
@@ -112,25 +113,25 @@
 
 msgid "Password confirmation"
 msgstr "パスワードの確認"
 
 msgid "Reset password"
 msgstr "パスワードの再設定"
 
-msgid "Date"
-msgstr "日付"
+msgid "When?"
+msgstr "いつ？"
 
 msgid "What?"
 msgstr "何ですか？"
 
-msgid "Payer"
-msgstr "支払人"
+msgid "Who paid?"
+msgstr "誰が支払った？"
 
-msgid "Amount paid"
-msgstr "支払額"
+msgid "How much?"
+msgstr "いくら？"
 
 msgid "Currency"
 msgstr "通貨"
 
 msgid "External link"
 msgstr "外部リンク"
 
@@ -146,17 +147,14 @@
 msgid "Submit and add a new one"
 msgstr "確認して、新しいのを作成します"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "初期プロジェクト: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "数値を空値にしてはいけません"
-
 msgid "Name"
 msgstr "名前"
 
 msgid "Weights should be positive"
 msgstr "重みは正でなければなりません"
 
 msgid "Weight"
@@ -172,21 +170,33 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "プロジェクトはすでにこのメンバーを含めています"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "招待状を出す"
+msgid "Send the invitations"
+msgstr "招待状を送る"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "メールアドレス%(email)sは無効"
 
+msgid "Logout"
+msgstr "ログアウト"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr "申し訳ございませんが、招待メールを送ったとき、エラーが発生しました。メールアドレスを再度チェックするかまたは管理者に連絡ください。"
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -206,89 +216,87 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "何度もログインに失敗したので、時間をおいてから再度ログインして下さい。"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "この管理者パスワードは正しくないでウ。%(num)d試行しか残っていません。"
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "私用コードは正しくない"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "費用を共有するため、%(project)sが作られました"
-
 msgid "A reminder email has just been sent to you"
 msgstr "催促メールがただいまあなたに送りました"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr "催促メールを送った時、エラーが発生しました。このプロジェクトはまだ使えます。"
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "プロジェクト名は%(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr "申し訳ございませんが、パスワード再設定の説明メールを送った時、エラーが発生しました。メールアドレスを一度確認してまたは管理者に連絡してください。"
 
 msgid "No token provided"
 msgstr "印が入力されていない"
 
 msgid "Invalid token"
 msgstr "無効な印"
 
 msgid "Unknown project"
 msgstr "未知のプロジェクト"
 
 msgid "Password successfully reset."
 msgstr "パスワードを再設定できました。"
 
-msgid "Project successfully uploaded"
-msgstr "プロジェクトをアップロードできました"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "無効なJSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "プロジェクトをアップロードできました"
+
 msgid "Project successfully deleted"
 msgstr "プロジェクトを削除できました"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "%(project)sの費用を共有すると、あなたが誘われた"
 
 msgid "Your invitations have been sent"
 msgstr "あなたの招待状が送られました"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr "申し訳ございませんが、招待メールを送ったとき、エラーが発生しました。メールアドレスを再度チェックするかまたは管理者に連絡ください。"
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)sが追加されました"
 
 msgid "Error activating participant"
@@ -323,14 +331,18 @@
 
 msgid "The bill has been deleted"
 msgstr "明細が削除されました"
 
 msgid "The bill has been modified"
 msgstr "明細が変更されました"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "プロジェクトの歴史を有効にする"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "プロジェクトの歴史を有効にする"
@@ -388,16 +400,17 @@
 
 msgid "Actions"
 msgstr "操作"
 
 msgid "edit"
 msgstr "編集"
 
-msgid "delete"
-msgstr "削除"
+#, fuzzy
+msgid "Delete project"
+msgstr "プロジェクトを編集する"
 
 msgid "show"
 msgstr "表示"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "現在ダッシュボードは操作できません。"
 
@@ -405,31 +418,21 @@
 msgid "Download Mobile Application"
 msgstr "携帯アプリ"
 
 #, fuzzy
 msgid "Get it on"
 msgstr "入る"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "確認？"
-
 msgid "Edit project"
 msgstr "プロジェクトを編集する"
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "プロジェクトを編集する"
 
-msgid "Import JSON"
-msgstr "JSONを導入する"
-
-msgid "Choose file"
-msgstr "ファイルを選択する"
-
 msgid "Download project's data"
 msgstr "プロジェクトのデータをダウンロードする"
 
 msgid "Bill items"
 msgstr "明細項目"
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -446,26 +449,36 @@
 
 msgid "Cancel"
 msgstr "キャンセル"
 
 msgid "Privacy Settings"
 msgstr "プライバシーの設定"
 
-msgid "Edit the project"
-msgstr "プロジェクトを編集する"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "以前のJSONファイルをインポートする"
+
+msgid "Choose file"
+msgstr "ファイルを選択する"
+
 msgid "Edit this bill"
 msgstr "明細を編集する"
 
 msgid "Add a bill"
 msgstr "新しい明細書を追加する"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "皆"
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -477,17 +490,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "参加者を追加する"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "招待状を送る"
-
 msgid "Download"
 msgstr "ダウンロードする"
 
 msgid "Disabled Project History"
 msgstr "操作できないプロジェクト歴史"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -547,62 +557,50 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "設定ページでIPアドレス記録を編集可能にすることができる"
+
 msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>このプロジェクトの歴史は操作できません。新しい操作は下に出ません。</i>で歴史を操作可能にすることができます。\n"
-"<a href=\"%(url)s\">設定ページ</a>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>下の表では操作不可になる前に、プロジェクトの歴史に対して記録された操作が反映されています。…できます。\n"
-"<a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-target"
-"=\"#confirm-erase\">プロジェクトの歴史を取り除く</a> で取り除きます.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "プロジェクトの歴史が誰かに取り除かれたかもしれません。"
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr "このプロジェクトのIP記録が操作できない一方、下の入り口の一部がIPアドレスを含めています。 "
 
 msgid "Delete stored IP addresses"
 msgstr "保存されたIPアドレスを削除する"
 
-msgid "No history to erase"
-msgstr "削除できる歴史はない"
-
-msgid "Clear Project History"
-msgstr "プロジェクトの歴史を取り除く"
-
 msgid "No IP Addresses to erase"
 msgstr "削除できるIPアドレスはない"
 
 msgid "Delete Stored IP Addresses"
 msgstr "保存されたIPアドレスを削除する"
 
+msgid "No history to erase"
+msgstr "削除できる歴史はない"
+
+msgid "Clear Project History"
+msgstr "プロジェクトの歴史を取り除く"
+
 msgid "Time"
 msgstr "時間"
 
 msgid "Event"
 msgstr "イベント"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -656,17 +654,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "支払人"
+
 msgid "Amount"
 msgstr "金額"
 
+msgid "Date"
+msgstr "日付"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "%(currency)sでの金額"
 
 #, fuzzy, python-format
 msgid "Bill %(name)s modified"
 msgstr "明細が変更されました"
@@ -768,16 +772,17 @@
 
 msgid "switch to"
 msgstr "…に切り替える"
 
 msgid "Dashboard"
 msgstr "ダッシュボード"
 
-msgid "Logout"
-msgstr "ログアウト"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "コード"
 
 msgid "Mobile Application"
 msgstr "携帯アプリ"
 
@@ -803,46 +808,40 @@
 
 msgid "you sure?"
 msgstr "確認？"
 
 msgid "Invite people"
 msgstr "人を誘う"
 
-msgid "You should start by adding participants"
-msgstr "参加者を追加して始めましょう"
-
-msgid "Add a new bill"
-msgstr "新しい明細を追加する"
-
 msgid "Newer bills"
 msgstr "もっと新しい明細"
 
 msgid "Older bills"
 msgstr "もっと古い明細"
 
-msgid "When?"
-msgstr "いつ？"
+msgid "You should start by adding participants"
+msgstr "参加者を追加して始めましょう"
 
-msgid "Who paid?"
-msgstr "誰が支払った？"
+msgid "Add a new bill"
+msgstr "新しい明細を追加する"
 
 msgid "For what?"
 msgstr "何のため？"
 
-msgid "How much?"
-msgstr "いくら？"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "%(date)sに追加された"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "%(excluded)s以外にみんな"
 
+msgid "delete"
+msgstr "削除"
+
 msgid "No bills"
 msgstr "明細なし"
 
 msgid "Nothing to list yet."
 msgstr "表示できるものはありません。"
 
 msgid "You probably want to"
@@ -887,14 +886,20 @@
 
 msgid "Share the Link"
 msgstr "リンクを共有する"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "好きの手段で以下のリンクを直接に共有できる"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "メールで送る"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -994,7 +999,71 @@
 #~ msgstr "無効な入力かプロジェクト名なし。"
 
 #~ msgid "User name incorrect"
 #~ msgstr "ユーザー名が正しくない"
 
 #~ msgid "People to notify"
 #~ msgstr "知らせたい人"
+
+#~ msgid "Import"
+#~ msgstr "インポート"
+
+#~ msgid "Amount paid"
+#~ msgstr "支払額"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "数値を空値にしてはいけません"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "プロジェクト名は%(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "無効なJSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "確認？"
+
+#~ msgid "Import JSON"
+#~ msgstr "JSONを導入する"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            "
+#~ "<i>このプロジェクトの歴史は操作できません。新しい操作は下に出ません。</i>で歴史を操作可能にすることができます。\n"
+#~ "<a href=\"%(url)s\">設定ページ</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>下の表では操作不可になる前に、プロジェクトの歴史に対して記録された操作が反映されています。…できます。\n"
+#~ "<a href=\"#\" data-toggle=\"modal\" data-"
+#~ "keyboard=\"false\" data-target=\"#confirm-"
+#~ "erase\">プロジェクトの歴史を取り除く</a> で取り除きます.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "招待状を出す"
+
+#~ msgid " show"
+#~ msgstr "表示"
+
+#~ msgid "Edit the project"
+#~ msgstr "プロジェクトを編集する"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-10-26 23:38+0200\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2021-10-17 04:56+0000\n"
 "Last-Translator: a-g-rao <athrigrao@gmail.com>\n"
 "Language: kn\n"
 "Language-Team: Kannada <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/kn/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s ನ್ನು ಸೇರಿಸಲಾಗಿದೆ"
 
 msgid "?"
 msgstr "?"
 
@@ -28,17 +28,14 @@
 
 msgid "Add"
 msgstr "ಕೂಡು"
 
 msgid "Admin password"
 msgstr "ಆಡಳಿತ ನಿರ್ವಾಹಕ ಪ್ರವೇಶ ಪದ"
 
-msgid "Amount paid"
-msgstr "ಪಾವತಿಸಿದ ಮೊತ್ತ"
-
 msgid "Back to the list"
 msgstr "ಪಟ್ಟಿಗೆ ವಾಪಸಾಗಿದ್ದೇವೆ"
 
 msgid "Create a new project"
 msgstr "ಹೊಸ ಯೋಜನೆಯನ್ನು ಸೃಷ್ಟಿಸಿ"
 
 msgid "Create the project"
@@ -73,17 +70,14 @@
 
 msgid "For whom?"
 msgstr "ಯಾರಿಂದ?"
 
 msgid "Get in"
 msgstr "ಒಳಹೊಗು"
 
-msgid "Import"
-msgstr "ಆಮದು"
-
 msgid "Invalid private code."
 msgstr "ನಮೂದಿಸಿರುವ ಸಂಕೇತಪದ ಅಮಾನ್ಯವಾಗಿದೆ."
 
 msgid "Name"
 msgstr "ಹೆಸರು"
 
 msgid "New private code"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/kn/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/kn/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2021-10-17 04:56+0000\n"
 "Last-Translator: a-g-rao <athrigrao@gmail.com>\n"
 "Language: kn\n"
 "Language-Team: Kannada <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/kn/>\n"
 "Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+"ನೀವು ನಿಮ್ಮ ಖರ್ಚು/ವೆಚ್ಚವನ್ನು ಹಂಚಿಕೊಳ್ಳಲು %(project)s ಯೋಜನೆಯನ್ನು "
+"ಸೃಷ್ಟಿಸಿದ್ದೀರಿ"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "ಮೊತ್ತ ಅಥವಾ ಪದಕಂತೆ ಸರಿಯಿಲ್ಲ. ಸಂಖ್ಯೆ ಮತ್ತು +-*/ ಎಣಿಕೆಬಳಕಗಳನ್ನು ಮಾತ್ರ "
 "ಸ್ವೀಕರಿಸಲಾಗುವುದು."
 
@@ -47,20 +53,17 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
+msgid "Compatible with Cospend"
 msgstr ""
 
-msgid "Import"
-msgstr "ಆಮದು"
-
 msgid "Project identifier"
 msgstr ""
 
 msgid "Private code"
 msgstr "ಸಂಕೇತಪದ"
 
 msgid "Create the project"
@@ -110,25 +113,25 @@
 
 msgid "Password confirmation"
 msgstr "ಪ್ರವೇಶಪದ ದೃಢೀಕರಿಸಿ"
 
 msgid "Reset password"
 msgstr "ಪ್ರವೇಶಪದ ಮರುಹೊಂದಿಸಿ"
 
-msgid "Date"
-msgstr "ದಿನಾಂಕ"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "ಏನು?"
 
-msgid "Payer"
-msgstr "ಪಾವತಿಸಿದವರು"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "ಪಾವತಿಸಿದ ಮೊತ್ತ"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "ನಾಣ್ಯಪದ್ಧತಿ"
 
 msgid "External link"
 msgstr ""
 
@@ -144,17 +147,14 @@
 msgid "Submit and add a new one"
 msgstr "ಕೋರಿಕೆ ಸಲ್ಲಿಸಿ ಹೊಸದನ್ನುಸೇರಿಸು"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr ""
 
-msgid "Bills can't be null"
-msgstr ""
-
 msgid "Name"
 msgstr "ಹೆಸರು"
 
 msgid "Weights should be positive"
 msgstr ""
 
 msgid "Weight"
@@ -169,21 +169,33 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "ಈ ಸದಸ್ಯರು ಈಗಾಗಲೆ ಈ ಯೋಜನೆಯ ಸದಸ್ಯರಾಗಿದ್ದಾರೆ"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "ಆಮಂತ್ರಣ ಕಳುಹಿಸು"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "ಮಿನ್ನಂಚೆ %(email)s ಸಮಂಜಸವಾಗಿಲ್ಲ"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} ಮತ್ತು {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, ಮತ್ತು{end_object}"
@@ -203,95 +215,88 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+msgid "Too many failed login attempts."
 msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-"ನೀವು ನಿಮ್ಮ ಖರ್ಚು/ವೆಚ್ಚವನ್ನು ಹಂಚಿಕೊಳ್ಳಲು %(project)s ಯೋಜನೆಯನ್ನು "
-"ಸೃಷ್ಟಿಸಿದ್ದೀರಿ"
-
 msgid "A reminder email has just been sent to you"
 msgstr "ನಿಮಗೆ ನೆನೆವಿ ಮಿನ್ನಂಚೆಯನ್ನು ಈಗ ಕಳುಹಿಸಲಾಗಿದೆ"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "ನಿಮಗೆ ನೆನವಿ ಮಿನ್ನಂಚೆ ಕಳುಹಿಸಲು ಪ್ರಯತ್ನಿಸಿದ್ದೆವೆ, ಆದರೆ ದೋಷವಿತ್ತು. ನೀವು "
 "ಯೋಜನೆಯನ್ನು ಸಾಮಾನ್ಯ ಪದತಿಯಂತೆ ಉಪಯೋಗಿಸ ಬಹುದು."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr "ಗೊತ್ತಿಲ್ಲದ ಯೋಜನೆ"
 
 msgid "Password successfully reset."
 msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 "%(project)s ಗಾಗಿ ನಿಮ್ಮ ಖರ್ಚು/ವೆಚ್ಚವನ್ನುಹಂಚಿಕೊಳಲ್ಲು ನಿಮ್ಮನ್ನು "
 "ಆಮಂತ್ರಿಸಲಾಗಿದೆ"
 
 msgid "Your invitations have been sent"
 msgstr "ನಿಮ್ಮ ಆಮಂತ್ರಣವನ್ನು ಕಳುಹಿಸಲಾಗಿದೆ"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s ನ್ನು ಸೇರಿಸಲಾಗಿದೆ"
 
 msgid "Error activating participant"
@@ -326,14 +331,18 @@
 
 msgid "The bill has been deleted"
 msgstr "ಬೆಲೆಪಟ್ಟಿಯನ್ನುತೆಗೆಯಲಾಗಿದೆ"
 
 msgid "The bill has been modified"
 msgstr "ಬೆಲೆಪಟ್ಟಿಯನ್ನು ಮಾರ್ಪಡಿಸಲಾಗಿದೆ"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "ಯೋಜನೆಯ ಇತಿಹಾಸವನ್ನು ತೆಗೆಯಲು ದೋಷವಾಗಿದೆ"
 
 msgid "Deleted project history."
 msgstr "ಯೋಜನೆ ಇತಿಹಾಸವನ್ನು ತೆಗೆಯಲಾಗಿದೆ."
 
 msgid "Error deleting recorded IP addresses"
@@ -386,43 +395,35 @@
 
 msgid "Actions"
 msgstr "ಕಾರ್ಯಗಳು"
 
 msgid "edit"
 msgstr "ಪರಿಷ್ಕರಿಸಿ"
 
-msgid "delete"
-msgstr "ತೆಗೆಯಿರಿ"
+msgid "Delete project"
+msgstr ""
 
 msgid "show"
 msgstr "ತೋರಿಸಿ"
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "ಯೋಜನೆಯನ್ನು ರಚಿಸಿ/ಸೃಷ್ಟಿಸಿ"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -440,26 +441,35 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+msgid "Import previously exported project"
+msgstr ""
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -470,17 +480,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -537,51 +544,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -637,17 +639,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "ಪಾವತಿಸಿದವರು"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "ದಿನಾಂಕ"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -749,15 +757,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -783,46 +792,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr "ತೆಗೆಯಿರಿ"
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -867,14 +870,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -940,7 +949,81 @@
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
 
+#~ msgid "Import previously exported JSON file"
+#~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "ಆಮದು"
+
+#~ msgid "Amount paid"
+#~ msgstr "ಪಾವತಿಸಿದ ಮೊತ್ತ"
+
+#~ msgid "Bills can't be null"
+#~ msgstr ""
+
+#~ msgid "Too many failed login attempts, please retry later."
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "ಆಮಂತ್ರಣ ಕಳುಹಿಸು"
+
+#~ msgid " show"
+#~ msgstr "ತೋರಿಸಿ"
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ms/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,73 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-07-18 12:32+0000\n"
-"Last-Translator: Kemystra <izzmin97@gmail.com>\n"
-"Language: ms\n"
-"Language-Team: Malay <https://hosted.weblate.org/projects/i-hate-money/i"
-"-hate-money/ms/>\n"
-"Plural-Forms: nplurals=1; plural=0\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: 2022-07-03 10:18+0000\n"
+"Last-Translator: Shafiq Azeez <fubukishirouk@gmail.com>\n"
+"Language: ur\n"
+"Language-Team: Urdu <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/ur/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
-msgstr "Nilai atau ungkapan yang sah. Hanya nombor dan operasi + - * / diterima."
+msgstr ""
 
 msgid "Project name"
-msgstr "Nama projek"
+msgstr "منصوبےکانام"
 
 msgid "New private code"
-msgstr "Kod peribadi baharu"
+msgstr ""
 
 msgid "Enter a new code if you want to change it"
-msgstr "Masukkan kod baharu jika kamu mahu mengubahnya"
+msgstr ""
 
 msgid "Email"
-msgstr "E-mel"
+msgstr "برقی خط (ای ميل)"
 
-#, fuzzy
 msgid "Enable project history"
-msgstr "Aktifkan sejarah projek"
+msgstr ""
 
-#, fuzzy
 msgid "Use IP tracking for project history"
-msgstr "Gunakan penjejakan IP untuk sejarah projek"
+msgstr ""
 
-#, fuzzy
 msgid "Default Currency"
-msgstr "Mata wang asal"
+msgstr ""
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
-#, fuzzy
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Projek ini tidak boleh disetkan kepada 'tiada mata wang' kerana projek "
-"ini mempunyai wang dalam beberapa bentuk mata wang"
-
-#, fuzzy
-msgid "Import previously exported JSON file"
-msgstr "Import fail JSON yang telah dieksport sebelum ini"
 
-msgid "Import"
-msgstr "Import"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr ""
 
 msgid "Private code"
-msgstr "Kod peribadi"
+msgstr ""
 
 msgid "Create the project"
-msgstr "Cipta projek ini"
+msgstr ""
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 
@@ -83,120 +77,120 @@
 msgid "euro"
 msgstr ""
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
-msgstr "Masukkan kod peribadi untuk mengesahkan penghapusan"
+msgstr ""
 
-#, fuzzy
 msgid "Unknown error"
-msgstr "Ralat yang tidak dikenalpasti"
+msgstr "نامعلوم خرابی"
 
 msgid "Invalid private code."
-msgstr "Kod peribadi tidak sah."
+msgstr ""
 
 msgid "Get in"
-msgstr "Masuk"
+msgstr ""
 
 msgid "Admin password"
-msgstr "Kata laluan pentadbir"
+msgstr ""
 
 msgid "Send me the code by email"
-msgstr "Hantar kod saya melalui e-mel"
+msgstr ""
 
 msgid "This project does not exists"
-msgstr "Projek ini tidak wujud"
+msgstr ""
 
-#, fuzzy
 msgid "Password mismatch"
-msgstr "Kata laluan tidak sama"
+msgstr ""
 
 msgid "Password"
-msgstr "Kata laluan"
+msgstr ""
 
 msgid "Password confirmation"
-msgstr "Pengesahan kata laluan"
+msgstr ""
 
-#, fuzzy
 msgid "Reset password"
-msgstr "Tetapkan semula kata laluan"
+msgstr ""
 
-msgid "Date"
-msgstr "Tarikh"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
-msgstr "Apa?"
+msgstr "کیا؟"
 
-msgid "Payer"
-msgstr "Pembayar"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "Jumlah dibayar"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
-msgstr "Mata wang"
+msgstr "سکہ رائج الوقت (کرنسی)"
 
-#, fuzzy
 msgid "External link"
-msgstr "pautan luar"
+msgstr "بیرونی لنک"
 
 msgid "A link to an external document, related to this bill"
-msgstr ""
+msgstr "اس رسید کے لیے بیرونی رستاویز کا لنک"
 
 msgid "For whom?"
-msgstr "Untuk siapa?"
+msgstr "کس کے لیے؟"
 
 msgid "Submit"
-msgstr "Hantar"
+msgstr "جمع کروائیں"
 
-#, fuzzy
 msgid "Submit and add a new one"
-msgstr "Hantar dan tambah yang baharu"
+msgstr "جمع کرکے ایک اور نیا اندراج کروائیں"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr ""
 
-#, fuzzy
-msgid "Bills can't be null"
-msgstr "Bil tidak boleh kosong"
-
 msgid "Name"
-msgstr "Nama"
+msgstr ""
 
-#, fuzzy
 msgid "Weights should be positive"
-msgstr "Berat perlulah positif"
+msgstr ""
 
-#, fuzzy
 msgid "Weight"
-msgstr "Berat"
+msgstr ""
 
 msgid "Add"
-msgstr "Tambah"
+msgstr ""
 
 msgid "The participant name is invalid"
 msgstr ""
 
-#, fuzzy
 msgid "This project already have this participant"
-msgstr "Projek ini sudah mempunyai ahli"
+msgstr ""
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr ""
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -216,89 +210,84 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+msgid "Too many failed login attempts."
 msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
 msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -333,14 +322,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr ""
 
 msgid "Deleted project history."
 msgstr ""
 
 msgid "Error deleting recorded IP addresses"
@@ -393,42 +386,33 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
+msgid "Import project"
 msgstr ""
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
@@ -447,26 +431,35 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+msgid "Import previously exported project"
+msgstr ""
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -477,17 +470,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -544,51 +534,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -644,17 +629,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "قیمت ادا کرنے والا"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr ""
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -756,15 +747,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -790,46 +782,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -874,14 +860,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -914,43 +906,81 @@
 
 msgid "Expenses by Month"
 msgstr ""
 
 msgid "Period"
 msgstr ""
 
-#~ msgid "You either provided a bad token or no project identifier."
+#~ msgid "Import previously exported JSON file"
 #~ msgstr ""
 
-#~ msgid "User name incorrect"
-#~ msgstr "Nama pengguna tidak tepat"
+#~ msgid "Import"
+#~ msgstr ""
 
-#~ msgid "People to notify"
+#~ msgid "Amount paid"
+#~ msgstr "ادا شدہ قیمت"
+
+#~ msgid "Bills can't be null"
 #~ msgstr ""
 
-#~ msgid "Error activating member"
+#~ msgid "Too many failed login attempts, please retry later."
 #~ msgstr ""
 
-#~ msgid "Error removing member"
+#~ msgid "The project identifier is %(project)s"
 #~ msgstr ""
 
 #~ msgid ""
-#~ "User '%(name)s' has been deactivated. It"
-#~ " will still appear in the users "
-#~ "list until its balance becomes zero."
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
 #~ msgstr ""
 
-#~ msgid "User '%(name)s' has been removed"
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
 #~ msgstr ""
 
-#~ msgid "User '%(name)s' has been edited"
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
 #~ msgstr ""
 
-#~ msgid "Number of members"
+#~ msgid "Send invites"
 #~ msgstr ""
 
-#~ msgid "Edit this member"
+#~ msgid " show"
 #~ msgstr ""
 
-#~ msgid "Participants to notify"
+#~ msgid "Edit the project"
 #~ msgstr ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Norwegian Bokmål (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-02-13 16:54+0000\n"
+"Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
+"Language: nb_NO\n"
 "Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/i-hate-"
 "money/i-hate-money/nb_NO/>\n"
-"Language: nb_NO\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.11-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s hver"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s har blitt lagt til"
 
@@ -67,17 +68,14 @@
 
 msgid "Amount"
 msgstr "Beløp"
 
 msgid "Amount in %(currency)s"
 msgstr "Beløp i %(currency)s"
 
-msgid "Amount paid"
-msgstr "Beløp betalt"
-
 msgid "Back to the list"
 msgstr "Tilbake til listen"
 
 msgid "Bill %(name)s added"
 msgstr "Regningen %(name)s har blitt lagt til"
 
 msgid "Bill %(name)s changed in an unknown way"
@@ -104,17 +102,14 @@
 
 msgid "Bill items"
 msgstr "Regningsoppføringer"
 
 msgid "Bills"
 msgstr "Regninger"
 
-msgid "Bills can't be null"
-msgstr "Regninger kan ikke være null"
-
 msgid "Can't remember the password?"
 msgstr "Husker du ikke passordet?"
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid ""
@@ -244,26 +239,14 @@
 
 msgid "How much?"
 msgstr "Hvor meget?"
 
 msgid "Identifier:"
 msgstr "Identifikator:"
 
-msgid "Import"
-msgstr "Importer"
-
-msgid "Import JSON"
-msgstr "Importer JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Importer tidligere eksportert JSON-fil"
-
-msgid "Invalid JSON"
-msgstr "Ugyldig JSON"
-
 msgid "Invalid private code."
 msgstr "Ugyldig privat kode"
 
 msgid "Invalid token"
 msgstr "Ugyldig symbol"
 
 msgid "Invite people"
@@ -475,17 +458,14 @@
 
 msgid "The bill has been deleted"
 msgstr "Regningen har blitt slettet"
 
 msgid "The bill has been modified"
 msgstr "Regningen har blitt endret"
 
-msgid "The project identifier is %(project)s"
-msgstr "Prosjektidentifikatoren er %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Prosjektet du prøver å få tilgang til finnes ikke. Ønsker du å"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Dette administratorpassordet er ikke rett. Kun %(num)d forsøk igjen."
 
 msgid "This private code is not the right one"
@@ -499,17 +479,14 @@
 
 msgid "Time"
 msgstr "Tid"
 
 msgid "To whom?"
 msgstr "Til hvem?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "For mange mislykkede innloggingsforsøk, prøv igjen senere."
-
 msgid "Try out the demo"
 msgstr "Prøv demonstrasjonen"
 
 msgid "Unknown error"
 msgstr "Ukjent feil"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/nb_NO/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-02-13 16:54+0000\n"
 "Last-Translator: Allan Nordhøy <epost@anotheragency.no>\n"
-"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/"
-"i-hate-money/i-hate-money/nb_NO/>\n"
 "Language: nb_NO\n"
+"Language-Team: Norwegian Bokmål <https://hosted.weblate.org/projects/i"
+"-hate-money/i-hate-money/nb_NO/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.11-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Du har akkurat opprettet \"%(project)s\" for å dele dine utgifter"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Ikke et gyldig beløp eller uttrykk. Kun nummer og operatorene + - * / "
 "godtas."
 
@@ -50,19 +54,16 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Dette prosjektet kan ikke settes til «Ingen valuta» fordi det inneholder "
 "regninger i flere valutaer."
 
-msgid "Import previously exported JSON file"
-msgstr "Importer tidligere eksportert JSON-fil"
-
-msgid "Import"
-msgstr "Importer"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Prosjektidentifikator"
 
 msgid "Private code"
 msgstr "Privat kode"
 
@@ -117,25 +118,25 @@
 
 msgid "Password confirmation"
 msgstr "Passordbekreftelse"
 
 msgid "Reset password"
 msgstr "Tilbakestill passord"
 
-msgid "Date"
-msgstr "Dato"
+msgid "When?"
+msgstr "Når?"
 
 msgid "What?"
 msgstr "Hva?"
 
-msgid "Payer"
-msgstr "Betaler"
+msgid "Who paid?"
+msgstr "Hvem betalte?"
 
-msgid "Amount paid"
-msgstr "Beløp betalt"
+msgid "How much?"
+msgstr "Hvor meget?"
 
 msgid "Currency"
 msgstr "Valuta"
 
 msgid "External link"
 msgstr "Ekstern lenke"
 
@@ -151,17 +152,14 @@
 msgid "Submit and add a new one"
 msgstr "Send inn og legg til ny"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Prosjektforvalg: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Regninger kan ikke være null"
-
 msgid "Name"
 msgstr "Navn"
 
 msgid "Weights should be positive"
 msgstr "Vekter må være positive"
 
 msgid "Weight"
@@ -177,21 +175,36 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "Allerede medlem av prosjektet"
 
 msgid "People to notify"
 msgstr "Folk å varsle"
 
-msgid "Send invites"
-msgstr "Send invitasjoner"
+msgid "Send the invitations"
+msgstr "Send ut invitasjonene"
 
 #, fuzzy, python-format
 msgid "The email %(email)s is not valid"
 msgstr "E-posten \"%(email)s\" er ikke gyldig"
 
+#, fuzzy
+msgid "Logout"
+msgstr "Logg ut"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Kunne ikke sende invitasjoner per e-post. Sjekk at e-postoppsettet på "
+"tjeneren stemmer, eller kontakt administratoren."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} og {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, og {end_object}"
@@ -211,51 +224,43 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "For mange mislykkede innloggingsforsøk, prøv igjen senere."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Dette administratorpassordet er ikke rett. Kun %(num)d forsøk igjen."
 
 msgid "Provided token is invalid"
 msgstr "Angitt symbol er ugyldig"
 
 msgid "This private code is not the right one"
 msgstr "Denne private koden er ikke rett"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Du har akkurat opprettet \"%(project)s\" for å dele dine utgifter"
-
 msgid "A reminder email has just been sent to you"
 msgstr "En påminnelse har blitt sendt til deg per e-post"
 
 #, fuzzy
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "En påminnelse ble sendt til deg per e-post, men en feil inntraff. Du kan "
 "fremdeles bruke prosjektet normalt."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Prosjektidentifikatoren er %(project)s"
-
 #, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "En feil inntraff under forsendelse av passordtilbakestilling til deg per "
 "e-post. Sjekk at e-postoppsettet til tjeneren er rett, eller kontakt "
 "administratoren."
 
 msgid "No token provided"
 msgstr "Inget symbol angitt"
@@ -266,50 +271,54 @@
 msgid "Unknown project"
 msgstr "Ukjent prosjekt"
 
 #, fuzzy
 msgid "Password successfully reset."
 msgstr "Passord tilbakestilt."
 
-#, fuzzy
-msgid "Project successfully uploaded"
-msgstr "Prosjekt opplastet"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Ugyldig JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"Kan ikke legge til regninger i flere valutaer i et prosjekt uten forvalgt "
-"valuta"
+"Kan ikke legge til regninger i flere valutaer i et prosjekt uten forvalgt"
+" valuta"
+
+#, fuzzy
+msgid "Project successfully uploaded"
+msgstr "Prosjekt opplastet"
 
 #, fuzzy
 msgid "Project successfully deleted"
 msgstr "Prosjekt slettet"
 
 #, fuzzy
 msgid "Error deleting project"
 msgstr "Kunne ikke slette prosjekt"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 "Du har blitt invitert til å dele dine utgifter i forbindelse med "
 "%(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Invitasjonene dine har blitt sendt"
 
 #, fuzzy
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Kunne ikke sende invitasjoner per e-post. Sjekk at e-postoppsettet på "
 "tjeneren stemmer, eller kontakt administratoren."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s har blitt lagt til"
@@ -350,14 +359,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Regningen har blitt slettet"
 
 msgid "The bill has been modified"
 msgstr "Regningen har blitt endret"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Skru på prosjekthistorikk"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Slettet prosjekthistorikk."
@@ -417,45 +430,36 @@
 
 msgid "Actions"
 msgstr "Handlinger"
 
 msgid "edit"
 msgstr "rediger"
 
-msgid "delete"
-msgstr "slett"
+msgid "Delete project"
+msgstr "Slett prosjekt"
 
 msgid "show"
 msgstr "vis"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Oversikten er for tiden avskrudd."
 
 msgid "Download Mobile Application"
 msgstr "Last ned mobilprogram"
 
 #, fuzzy
 msgid "Get it on"
 msgstr "Til prosjektet"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "er du sikker?"
-
 msgid "Edit project"
 msgstr "Rediger prosjekt"
 
-msgid "Delete project"
-msgstr "Slett prosjekt"
-
-msgid "Import JSON"
-msgstr "Importer JSON"
-
-msgid "Choose file"
-msgstr "Velg fil"
+#, fuzzy
+msgid "Import project"
+msgstr "Rediger prosjekt"
 
 msgid "Download project's data"
 msgstr "Last ned prosjektets data"
 
 msgid "Bill items"
 msgstr "Regningsoppføringer"
 
@@ -476,26 +480,36 @@
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid "Privacy Settings"
 msgstr "Personvernsinnstillinger"
 
-msgid "Edit the project"
-msgstr "Rediger prosjektet"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "Dette vil fjerne alle regninger og deltagere i prosjektet!"
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importer tidligere eksportert JSON-fil"
+
+msgid "Choose file"
+msgstr "Velg fil"
+
 msgid "Edit this bill"
 msgstr "Rediger denne regningen"
 
 msgid "Add a bill"
 msgstr "Legg til en regning"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Alle"
 
 msgid "No one"
 msgstr "Ingen"
 
 msgid "More options"
@@ -508,17 +522,14 @@
 msgid "Edit this participant"
 msgstr "Legg til deltager"
 
 #, fuzzy
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "ola@eksempel.no, kari@eksempel.no"
 
-msgid "Send the invitations"
-msgstr "Send ut invitasjonene"
-
 msgid "Download"
 msgstr "Last nd"
 
 #, fuzzy
 msgid "Disabled Project History"
 msgstr "Avskrudd prosjekthistorikk"
 
@@ -587,71 +598,55 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Regning %(name)s: La til %(owers_list_str)s på eierlisten"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Regning %(name)s: fjernet %(owers_list_str)s fra eierlisten"
 
-#, fuzzy, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Prosjektets historikk er avskrudd. Nye handlinger vil ikke"
-" vises nedenfor. Du kan skru på hisorikk på</i>\n"
-"            <a href=\"%(url)s\">innstillingssiden</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
 
 #, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "IP-adresseregistrering kan skrus på fra innstillingssiden"
+
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Tabellen nedenfor viser handlinger registrert før "
-"prosjekthistorikken ble avskrudd. Du kan\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">tømme prosjekthistorikken</a> for å fjerne"
-" dem.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Noen tømte antagelig prosjekthistorikken."
 
 #, fuzzy
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Noen oppføringer nedenfor inneholder IP-adresser, selv om dette "
 "prosjektet har IP-registrering avskrudd. "
 
 msgid "Delete stored IP addresses"
 msgstr "Slett lagrede IP-adresser"
 
-msgid "No history to erase"
-msgstr "Ingen historikk å slette"
-
-msgid "Clear Project History"
-msgstr "Tøm prosjekthistorikk"
-
 #, fuzzy
 msgid "No IP Addresses to erase"
 msgstr "Ingen IP-adresser å slette"
 
 #, fuzzy
 msgid "Delete Stored IP Addresses"
 msgstr "Slett lagrede IP-adresser"
 
+msgid "No history to erase"
+msgstr "Ingen historikk å slette"
+
+msgid "Clear Project History"
+msgstr "Tøm prosjekthistorikk"
+
 msgid "Time"
 msgstr "Tid"
 
 msgid "Event"
 msgstr "Hendelse"
 
 #, fuzzy
@@ -707,17 +702,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Regningen %(name)s fikk sitt navn endret til %(new_description)s"
 
 #, fuzzy, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr "Deltager %(name)s: vekting endret fra %(old_weight)s til %(new_weight)s"
 
+msgid "Payer"
+msgstr "Betaler"
+
 msgid "Amount"
 msgstr "Beløp"
 
+msgid "Date"
+msgstr "Dato"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Beløp i %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Regningen %(name)s har blitt endret"
@@ -824,17 +825,17 @@
 
 msgid "switch to"
 msgstr "bytt til"
 
 msgid "Dashboard"
 msgstr "Oversikt"
 
-#, fuzzy
-msgid "Logout"
-msgstr "Logg ut"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Kode"
 
 msgid "Mobile Application"
 msgstr "Mobilprogram"
 
@@ -861,46 +862,40 @@
 
 msgid "you sure?"
 msgstr "er du sikker?"
 
 msgid "Invite people"
 msgstr "Inviter folk"
 
-msgid "You should start by adding participants"
-msgstr "Du kan starte ved å legge til deltagere"
-
-msgid "Add a new bill"
-msgstr "Legg til en ny regning"
-
 msgid "Newer bills"
 msgstr "Nyere regninger"
 
 msgid "Older bills"
 msgstr "Eldre regninger"
 
-msgid "When?"
-msgstr "Når?"
+msgid "You should start by adding participants"
+msgstr "Du kan starte ved å legge til deltagere"
 
-msgid "Who paid?"
-msgstr "Hvem betalte?"
+msgid "Add a new bill"
+msgstr "Legg til en ny regning"
 
 msgid "For what?"
 msgstr "For hva?"
 
-msgid "How much?"
-msgstr "Hvor meget?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Lagt til %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Alle, unntagen %(excluded)s"
 
+msgid "delete"
+msgstr "slett"
+
 msgid "No bills"
 msgstr "Ingen regninger"
 
 #, fuzzy
 msgid "Nothing to list yet."
 msgstr "Ingenting å liste opp enda."
 
@@ -952,14 +947,20 @@
 #, fuzzy
 msgid "Share the Link"
 msgstr "Del lenken"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Du kan dele denne lenken slik du ønsker"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 #, fuzzy
 msgid "Send via Emails"
 msgstr "Send via e-poster"
 
 #, fuzzy
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
@@ -1223,7 +1224,76 @@
 #~ msgstr "Antall medlemmer"
 
 #~ msgid "Edit this member"
 #~ msgstr "Rediger dette medlemmet"
 
 #~ msgid "Participants to notify"
 #~ msgstr "legge til deltagere"
+
+#~ msgid "Import"
+#~ msgstr "Importer"
+
+#~ msgid "Amount paid"
+#~ msgstr "Beløp betalt"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Regninger kan ikke være null"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Prosjektidentifikatoren er %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Ugyldig JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "er du sikker?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importer JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Prosjektets historikk er "
+#~ "avskrudd. Nye handlinger vil ikke vises"
+#~ " nedenfor. Du kan skru på hisorikk"
+#~ " på</i>\n"
+#~ "            <a href=\"%(url)s\">innstillingssiden</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Tabellen nedenfor viser "
+#~ "handlinger registrert før prosjekthistorikken "
+#~ "ble avskrudd. Du kan\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">tømme prosjekthistorikken</a>"
+#~ " for å fjerne dem.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Send invitasjoner"
+
+#~ msgid " show"
+#~ msgstr "vis"
+
+#~ msgid "Edit the project"
+#~ msgstr "Rediger prosjektet"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,36 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  \n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2021-02-17 02:50+0000\n"
 "Last-Translator: Sander Kooijmans <weblate@gogognome.nl>\n"
 "Language: nl\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/nl/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Dit project heeft de geschiedenis uitgeschakeld. Nieuwe "
-"acties zullen niet hieronder verschijnen. Je kunt de geschiedenis aanzetten "
-"op de </i>\n"
-"            <a href=\"%(url)s\">instellingen-pagina</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" is vrije software"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s zijn toegevoegd"
 
@@ -89,17 +75,14 @@
 
 msgid "Amount"
 msgstr "Hoeveelheid"
 
 msgid "Amount in %(currency)s"
 msgstr "Hoeveelheid in %(currency)s"
 
-msgid "Amount paid"
-msgstr "Betaald bedrag"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Weet je zeker dat je alle vastgelegde IP-adressen wilt verwijderen van dit "
@@ -122,17 +105,14 @@
 
 msgid "Bill items"
 msgstr "Rekeningitems"
 
 msgid "Bills"
 msgstr "Rekeningen"
 
-msgid "Bills can't be null"
-msgstr "Rekeningen mogen niet null zijn"
-
 msgid "Can't remember the password?"
 msgstr "Wachtwoord vergeten?"
 
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgid "Choose file"
@@ -252,26 +232,14 @@
 
 msgid "How much?"
 msgstr "Hoeveel?"
 
 msgid "Identifier:"
 msgstr "Identificatie:"
 
-msgid "Import"
-msgstr "Importeren"
-
-msgid "Import JSON"
-msgstr "JSON importeren"
-
-msgid "Import previously exported JSON file"
-msgstr "Eerder geëxporteerd JSON-bestand importeren"
-
-msgid "Invalid JSON"
-msgstr "Ongeldige JSON"
-
 msgid "Invalid token"
 msgstr "Ongeldige toegangssleutel"
 
 msgid "Invite people"
 msgstr "Anderen uitnodigen"
 
 msgid "Invite people to join this project"
@@ -430,31 +398,14 @@
 
 msgid "Simply sharing money with others?"
 msgstr "Wil je gewoon geld verdelen met anderen?"
 
 msgid "Someone probably cleared the project history."
 msgstr "Iemand heeft waarschijnlijk de projectgeschiedenis verwijderd."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Sorry, er is iets fout gegaan bij het verzenden van een e-mail met "
-"instructies om je wachtwoord te herstellen. Controleer de e-mailinstellingen "
-"van de server of neem contact op met de beheerder."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Sorry, er is iets fout gegaan bij het verzenden van de uitnodigingsmails. "
-"Controleer de e-mailinstellingen van de server of neem contact op met de "
-"beheerder."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Sorry, de pagina die je zoekt kan niet worden gevonden."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -494,17 +445,14 @@
 
 msgid "The bill has been modified"
 msgstr "De rekening is aangepast"
 
 msgid "The email %(email)s is not valid"
 msgstr "Het e-mailadres '%(email)s' is onjuist"
 
-msgid "The project identifier is %(project)s"
-msgstr "Het project-id is %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Het project dat je probeert te benaderen bestaat niet. Wil je"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Het admin-wachtwoord is onjuist. Je kunt het nog %(num)d keer proberen."
 
@@ -516,17 +464,14 @@
 
 msgid "Time"
 msgstr "Tijd"
 
 msgid "To whom?"
 msgstr "Aan wie?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Te vaak onjuist ingelogd. Probeer het later opnieuw."
-
 msgid "Try out the demo"
 msgstr "Probeer het uit"
 
 msgid "Unknown project"
 msgstr "Onbekend project"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/nl/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/nl/LC_MESSAGES/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version:  \n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2021-02-17 02:50+0000\n"
 "Last-Translator: Sander Kooijmans <weblate@gogognome.nl>\n"
 "Language: nl\n"
 "Language-Team: Dutch <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/nl/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+"Je hebt zojuist het project '%(project)s' aangemaakt om je uitgaven te "
+"verdelen"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Geen geldig bedrag of expressie. Gebruik alleen getallen en + - * / "
 "operatoren."
 
@@ -48,19 +54,16 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
-msgstr "Eerder geëxporteerd JSON-bestand importeren"
-
-msgid "Import"
-msgstr "Importeren"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Project-id"
 
 msgid "Private code"
 msgstr "Privécode"
 
@@ -114,25 +117,25 @@
 
 msgid "Password confirmation"
 msgstr "Wachtwoord bevestigen"
 
 msgid "Reset password"
 msgstr "Wachtwoord herstellen"
 
-msgid "Date"
-msgstr "Datum"
+msgid "When?"
+msgstr "Wanneer?"
 
 msgid "What?"
 msgstr "Wat?"
 
-msgid "Payer"
-msgstr "Betaler"
+msgid "Who paid?"
+msgstr "Wie heeft er betaald?"
 
-msgid "Amount paid"
-msgstr "Betaald bedrag"
+msgid "How much?"
+msgstr "Hoeveel?"
 
 msgid "Currency"
 msgstr "Munteenheid"
 
 msgid "External link"
 msgstr "Externe link"
 
@@ -148,17 +151,14 @@
 msgid "Submit and add a new one"
 msgstr "Versturen en nieuwe toevoegen"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Projectstandaard: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Rekeningen mogen niet null zijn"
-
 msgid "Name"
 msgstr "Naam"
 
 msgid "Weights should be positive"
 msgstr "Gewichten moeten positief zijn"
 
 msgid "Weight"
@@ -174,21 +174,36 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "Deze deelnemer is al lid van het project"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "Uitnodigingen versturen"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Het e-mailadres '%(email)s' is onjuist"
 
+msgid "Logout"
+msgstr "Uitloggen"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Sorry, er is iets fout gegaan bij het verzenden van de uitnodigingsmails."
+" Controleer de e-mailinstellingen van de server of neem contact op met de"
+" beheerder."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -208,51 +223,42 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Te vaak onjuist ingelogd. Probeer het later opnieuw."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Het admin-wachtwoord is onjuist. Je kunt het nog %(num)d keer proberen."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "Deze privécode is onjuist"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-"Je hebt zojuist het project '%(project)s' aangemaakt om je uitgaven te "
-"verdelen"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Een herinneringsmail is zojuist naar u verzonden"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "We hebben geprobeerd een herinneringsmail te versturen, maar er is iets "
 "fout gegaan. Je kunt het project nog steeds normaal gebruiken."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Het project-id is %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Sorry, er is iets fout gegaan bij het verzenden van een e-mail met "
 "instructies om je wachtwoord te herstellen. Controleer de "
 "e-mailinstellingen van de server of neem contact op met de beheerder."
 
 msgid "No token provided"
 msgstr "Geen toegangssleutel opgegeven"
@@ -262,42 +268,47 @@
 
 msgid "Unknown project"
 msgstr "Onbekend project"
 
 msgid "Password successfully reset."
 msgstr "Wachtwoord is hersteld."
 
-msgid "Project successfully uploaded"
-msgstr "Project succesvol geüpload"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Ongeldige JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Project succesvol geüpload"
+
 msgid "Project successfully deleted"
 msgstr "Project is verwijderd"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Je bent uitgenodigd om je uitgaven te delen met %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Je uitnodigingen zijn verstuurd"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Sorry, er is iets fout gegaan bij het verzenden van de uitnodigingsmails."
 " Controleer de e-mailinstellingen van de server of neem contact op met de"
 " beheerder."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -337,14 +348,18 @@
 
 msgid "The bill has been deleted"
 msgstr "De rekening is verwijderd"
 
 msgid "The bill has been modified"
 msgstr "De rekening is aangepast"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Projectgeschiedenis inschakelen"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Projectgeschiedenis inschakelen"
@@ -402,16 +417,17 @@
 
 msgid "Actions"
 msgstr "Acties"
 
 msgid "edit"
 msgstr "bewerken"
 
-msgid "delete"
-msgstr "verwijderen"
+#, fuzzy
+msgid "Delete project"
+msgstr "Project aanpassen"
 
 msgid "show"
 msgstr "tonen"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "De overzichtspagina is momenteel uitgeschakeld."
 
@@ -419,31 +435,21 @@
 msgid "Download Mobile Application"
 msgstr "Mobiele app"
 
 #, fuzzy
 msgid "Get it on"
 msgstr "Inloggen"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "weet je het zeker?"
-
 msgid "Edit project"
 msgstr "Project aanpassen"
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "Project aanpassen"
 
-msgid "Import JSON"
-msgstr "JSON importeren"
-
-msgid "Choose file"
-msgstr "Bestand kiezen"
-
 msgid "Download project's data"
 msgstr "Projectgegevens downloaden"
 
 msgid "Bill items"
 msgstr "Rekeningitems"
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -462,26 +468,36 @@
 
 msgid "Cancel"
 msgstr "Annuleren"
 
 msgid "Privacy Settings"
 msgstr "Privacy-instellingen"
 
-msgid "Edit the project"
-msgstr "Project bewerken"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Eerder geëxporteerd JSON-bestand importeren"
+
+msgid "Choose file"
+msgstr "Bestand kiezen"
+
 msgid "Edit this bill"
 msgstr "Deze rekening bewerken"
 
 msgid "Add a bill"
 msgstr "Rekening toevoegen"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Iedereen"
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -493,17 +509,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "Deelnemer toevoegen"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "jan.jansen@voorbeeld.nl, maria.magdalena@website.nl"
 
-msgid "Send the invitations"
-msgstr "Uitnodigingen versturen"
-
 msgid "Download"
 msgstr "Downloaden"
 
 msgid "Disabled Project History"
 msgstr "Uitgeschakelde Projectgeschiedenis"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -567,59 +580,49 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Dit project heeft de geschiedenis uitgeschakeld. Nieuwe "
-"acties zullen niet hieronder verschijnen. Je kunt de geschiedenis "
-"aanzetten op de </i>\n"
-"            <a href=\"%(url)s\">instellingen-pagina</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
+msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
 msgstr ""
 
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Iemand heeft waarschijnlijk de projectgeschiedenis verwijderd."
+
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
-msgstr "Geen geschiedenis om te wissen"
-
-msgid "Clear Project History"
-msgstr "Verwijder Projectgeschiedenis"
-
 msgid "No IP Addresses to erase"
 msgstr "Geen IP-adressen te verwijderen"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Verwijder opgeslagen IP-adressen"
 
+msgid "No history to erase"
+msgstr "Geen geschiedenis om te wissen"
+
+msgid "Clear Project History"
+msgstr "Verwijder Projectgeschiedenis"
+
 msgid "Time"
 msgstr "Tijd"
 
 msgid "Event"
 msgstr ""
 
 msgid "IP address recording can be enabled on the settings page"
@@ -673,17 +676,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Betaler"
+
 msgid "Amount"
 msgstr "Hoeveelheid"
 
+msgid "Date"
+msgstr "Datum"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Hoeveelheid in %(currency)s"
 
 #, fuzzy, python-format
 msgid "Bill %(name)s modified"
 msgstr "De rekening is aangepast"
@@ -787,16 +796,17 @@
 
 msgid "switch to"
 msgstr "overschakelen naar"
 
 msgid "Dashboard"
 msgstr "Overzicht"
 
-msgid "Logout"
-msgstr "Uitloggen"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Code"
 
 msgid "Mobile Application"
 msgstr "Mobiele app"
 
@@ -822,46 +832,40 @@
 
 msgid "you sure?"
 msgstr "weet je het zeker?"
 
 msgid "Invite people"
 msgstr "Anderen uitnodigen"
 
-msgid "You should start by adding participants"
-msgstr "Begin met het toevoegen van deelnemers"
-
-msgid "Add a new bill"
-msgstr "Nieuwe rekening toevoegen"
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
-msgstr "Wanneer?"
+msgid "You should start by adding participants"
+msgstr "Begin met het toevoegen van deelnemers"
 
-msgid "Who paid?"
-msgstr "Wie heeft er betaald?"
+msgid "Add a new bill"
+msgstr "Nieuwe rekening toevoegen"
 
 msgid "For what?"
 msgstr "Voor wat?"
 
-msgid "How much?"
-msgstr "Hoeveel?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Toegevoegd op %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Iedereen, behalve %(excluded)s"
 
+msgid "delete"
+msgstr "verwijderen"
+
 msgid "No bills"
 msgstr "Geen rekeningen"
 
 msgid "Nothing to list yet."
 msgstr "Nog niks."
 
 msgid "You probably want to"
@@ -910,14 +914,20 @@
 
 msgid "Share the Link"
 msgstr "Link delen"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Je kunt de volgende link direct delen"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Versturen via e-mail"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1045,7 +1055,68 @@
 #~ msgstr "Je hebt een onjuiste toegangssleutel of geen project-id opgegeven."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Verkeerde gebruikersnaam"
 
 #~ msgid "People to notify"
 #~ msgstr "Te melden personen"
+
+#~ msgid "Import"
+#~ msgstr "Importeren"
+
+#~ msgid "Amount paid"
+#~ msgstr "Betaald bedrag"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Rekeningen mogen niet null zijn"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Het project-id is %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Ongeldige JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "weet je het zeker?"
+
+#~ msgid "Import JSON"
+#~ msgstr "JSON importeren"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Dit project heeft de "
+#~ "geschiedenis uitgeschakeld. Nieuwe acties "
+#~ "zullen niet hieronder verschijnen. Je "
+#~ "kunt de geschiedenis aanzetten op de "
+#~ "</i>\n"
+#~ "            <a href=\"%(url)s\">instellingen-pagina</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Uitnodigingen versturen"
+
+#~ msgid " show"
+#~ msgstr "tonen"
+
+#~ msgid "Edit the project"
+#~ msgstr "Project bewerken"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,23 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Polish (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-09-27 14:19+0000\n"
+"Last-Translator: Andrzej Ochodek <andrzej.ochodek@gmail.com>\n"
+"Language: pl\n"
 "Language-Team: Polish <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/pl/>\n"
-"Language: pl\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Poniższa tabela przedstawia działania zarejestrowane przed "
-"wyłączeniem historii projektu. Możesz\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">wyczyścić historię projektu</a>, aby je usunąć.</"
-"i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Historia tego projektu została wyłączona. Nowe działania nie "
-"pojawią się poniżej. Możesz włączyć historię w</i>\n"
-"            <a href=\"%(url)s\">ustawieniach</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "„I Hate Money” to darmowe oprogramowanie"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s każdy"
 
@@ -108,17 +80,14 @@
 
 msgid "Amount"
 msgstr "Ilość"
 
 msgid "Amount in %(currency)s"
 msgstr "Ilość w %(currency)s"
 
-msgid "Amount paid"
-msgstr "Zapłacona kwota"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Czy na pewno chcesz usunąć wszystkie zarejestrowane adresy IP z tego "
@@ -129,17 +98,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Czy na pewno chcesz usunąć całą historię tego projektu? Nie można cofnąć tej "
 "akcji."
 
-msgid "Are you sure?"
-msgstr "Czy jesteś pewien?"
-
 msgid "Authentication"
 msgstr "Uwierzytelnianie"
 
 msgid "Back to the list"
 msgstr "Powrót do listy"
 
 msgid "Balance"
@@ -175,17 +141,14 @@
 
 msgid "Bill items"
 msgstr "Zawartość rachunku"
 
 msgid "Bills"
 msgstr "Rachunki"
 
-msgid "Bills can't be null"
-msgstr "Rachunki nie mogą być zerowe"
-
 msgid "Can't remember the password?"
 msgstr "Nie pamiętasz hasła?"
 
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgid ""
@@ -383,26 +346,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "Rejestrowanie adresu IP można włączyć na stronie ustawień"
 
 msgid "Identifier:"
 msgstr "Identyfikator:"
 
-msgid "Import"
-msgstr "Importuj"
-
-msgid "Import JSON"
-msgstr "Importuj JSON"
-
-msgid "Import previously exported JSON file"
-msgstr "Zaimportuj wcześniej wyeksportowany plik JSON"
-
-msgid "Invalid JSON"
-msgstr "Niepoprawny JSON"
-
 msgid "Invalid private code."
 msgstr "Nieprawidłowy kod prywatny."
 
 msgid "Invalid token"
 msgstr "Nieprawidłowy token"
 
 msgid "Invite people"
@@ -659,31 +610,14 @@
 msgstr ""
 "Niektóre wpisy poniżej zawierają adresy IP, nawet jeśli w tym projekcie "
 "rejestrowanie IP jest wyłączone. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Ktoś prawdopodobnie wyczyścił historię projektu."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Przepraszamy, wystąpił błąd podczas wysyłania wiadomości e-mail z "
-"instrukcjami resetowania hasła. Sprawdź konfigurację e-mail serwera lub "
-"skontaktuj się z administratorem."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Przepraszamy, wystąpił błąd podczas próby wysłania wiadomości e-mail z "
-"zaproszeniem. Sprawdź konfigurację e-mail serwera lub skontaktuj się z "
-"administratorem."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Niestety nie udało nam się znaleźć strony, o którą prosiłeś."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -727,17 +661,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "Ten email %(email)s jest nieprawidłowy"
 
 msgid "The participant name is invalid"
 msgstr "Nazwa członka jest nieprawidłowa"
 
-msgid "The project identifier is %(project)s"
-msgstr "Identyfikator projektu to %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Projekt, do którego próbujesz uzyskać dostęp, nie istnieje, czy chcesz"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "To hasło administratora jest nieprawidłowe. Pozostało tylko %(num)d prób."
 
@@ -763,17 +694,14 @@
 
 msgid "Time"
 msgstr "Czas"
 
 msgid "To whom?"
 msgstr "Komu?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Zbyt wiele nieudanych prób logowania, spróbuj ponownie później."
-
 msgid "Try out the demo"
 msgstr "Wypróbuj wersję demo"
 
 msgid "Unknown error"
 msgstr "Nieznany błąd"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/pl/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/pl/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-09-27 14:19+0000\n"
 "Last-Translator: Andrzej Ochodek <andrzej.ochodek@gmail.com>\n"
-"Language-Team: Polish <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/pl/>\n"
 "Language: pl\n"
+"Language-Team: Polish <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/pl/>\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && "
+"(n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Właśnie utworzyłeś „%(project)s”, aby podzielić się wydatkami"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Niepoprawna kwota lub wyrażenie. Akceptowane są tylko liczby i operatory "
 "+ - * /."
 
@@ -42,28 +46,26 @@
 msgstr "Użyj śledzenia IP do historii projektu"
 
 msgid "Default Currency"
 msgstr "Domyślna waluta"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"Wybranie domyślnej waluty pozwala na konwersję walutową pomiędzy rachunkami"
+"Wybranie domyślnej waluty pozwala na konwersję walutową pomiędzy "
+"rachunkami"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Ten projekt nie może zostać oznaczony jako 'bez waluty', ponieważ zawiera on "
-"rachunki w różnych walutach."
+"Ten projekt nie może zostać oznaczony jako 'bez waluty', ponieważ zawiera"
+" on rachunki w różnych walutach."
 
-msgid "Import previously exported JSON file"
-msgstr "Zaimportuj wcześniej wyeksportowany plik JSON"
-
-msgid "Import"
-msgstr "Importuj"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identyfikator projektu"
 
 msgid "Private code"
 msgstr "Kod prywatny"
 
@@ -71,16 +73,16 @@
 msgstr "Stwórz projekt"
 
 #, python-format
 msgid ""
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
-"Projekt o tym identyfikatorze (\"%(project)s\") już istnieje. Wybierz nowy "
-"identyfikator"
+"Projekt o tym identyfikatorze (\"%(project)s\") już istnieje. Wybierz "
+"nowy identyfikator"
 
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr "Która waluta jest prawdziwa: euro czy petrodolar?"
 
 msgid "euro"
 msgstr "euro"
 
@@ -116,25 +118,25 @@
 
 msgid "Password confirmation"
 msgstr "Potwierdzenie hasła"
 
 msgid "Reset password"
 msgstr "Zmień hasło"
 
-msgid "Date"
-msgstr "Data"
+msgid "When?"
+msgstr "Kiedy?"
 
 msgid "What?"
 msgstr "Co?"
 
-msgid "Payer"
-msgstr "Płatnik"
+msgid "Who paid?"
+msgstr "Kto zapłacił?"
 
-msgid "Amount paid"
-msgstr "Zapłacona kwota"
+msgid "How much?"
+msgstr "Jak dużo?"
 
 msgid "Currency"
 msgstr "Waluta"
 
 msgid "External link"
 msgstr "Link zewnętrzny"
 
@@ -150,17 +152,14 @@
 msgid "Submit and add a new one"
 msgstr "Zatwierdź i dodaj nowy"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Wartość domyślna projektu: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Rachunki nie mogą być zerowe"
-
 msgid "Name"
 msgstr "Nazwa"
 
 msgid "Weights should be positive"
 msgstr "Wagi powinny być dodatnie"
 
 msgid "Weight"
@@ -174,21 +173,36 @@
 
 msgid "This project already have this participant"
 msgstr "Ten projekt ma już tego członka"
 
 msgid "People to notify"
 msgstr "Osoby do powiadomienia"
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "Wyślij zaproszenia"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Ten email %(email)s jest nieprawidłowy"
 
+msgid "Logout"
+msgstr "Wyloguj"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Przepraszamy, wystąpił błąd podczas próby wysłania wiadomości e-mail z "
+"zaproszeniem. Sprawdź konfigurację e-mail serwera lub skontaktuj się z "
+"administratorem."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} i {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object} i {end_object}"
@@ -208,49 +222,42 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Zbyt wiele nieudanych prób logowania, spróbuj ponownie później."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "To hasło administratora jest nieprawidłowe. Pozostało tylko %(num)d prób."
 
 msgid "Provided token is invalid"
 msgstr "Podany token jest niepoprawny"
 
 msgid "This private code is not the right one"
 msgstr "Ten prywatny kod jest niewłaściwy"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Właśnie utworzyłeś „%(project)s”, aby podzielić się wydatkami"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Wiadomość e-mail z przypomnieniem została właśnie wysłana"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Próbowaliśmy wysłać Ci wiadomość e-mail z przypomnieniem, ale wystąpił "
 "błąd. Nadal możesz normalnie korzystać z projektu."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Identyfikator projektu to %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Przepraszamy, wystąpił błąd podczas wysyłania wiadomości e-mail z "
 "instrukcjami resetowania hasła. Sprawdź konfigurację e-mail serwera lub "
 "skontaktuj się z administratorem."
 
 msgid "No token provided"
 msgstr "Nie podano tokena"
@@ -260,43 +267,49 @@
 
 msgid "Unknown project"
 msgstr "Nieznany projekt"
 
 msgid "Password successfully reset."
 msgstr "Hasło zostało pomyślnie zresetowane."
 
-msgid "Project successfully uploaded"
-msgstr "Projekt został pomyślnie przesłany"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Niepoprawny JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"Nie można dodawać rachunków w wielu walutach do projektu bez waluty domyślnej"
+"Nie można dodawać rachunków w wielu walutach do projektu bez waluty "
+"domyślnej"
+
+msgid "Project successfully uploaded"
+msgstr "Projekt został pomyślnie przesłany"
 
 msgid "Project successfully deleted"
 msgstr "Projekt został pomyślnie usunięty"
 
 msgid "Error deleting project"
 msgstr "Błąd podczas usuwania projektu"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Zostałeś zaproszony do podzielenia się swoimi wydatkami w %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Twoje zaproszenia zostały wysłane"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Przepraszamy, wystąpił błąd podczas próby wysłania wiadomości e-mail z "
 "zaproszeniem. Sprawdź konfigurację e-mail serwera lub skontaktuj się z "
 "administratorem."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -313,16 +326,16 @@
 msgstr "Błąd podczas usuwania uczestnika"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Uczestnik „%(name)s” został wyłączony. Będzie nadal pojawiać się na liście "
-"użytkowników, dopóki jego saldo nie wyniesie zero."
+"Uczestnik „%(name)s” został wyłączony. Będzie nadal pojawiać się na "
+"liście użytkowników, dopóki jego saldo nie wyniesie zero."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "Uczestnik „%(name)s” został usunięty"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -336,14 +349,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Rachunek został usunięty"
 
 msgid "The bill has been modified"
 msgstr "Rachunek został zmieniony"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Błąd podczas usuwania historii projektu"
 
 msgid "Deleted project history."
 msgstr "Usunięto historię projektu."
 
 msgid "Error deleting recorded IP addresses"
@@ -398,43 +415,35 @@
 
 msgid "Actions"
 msgstr "Akcje"
 
 msgid "edit"
 msgstr "edytuj"
 
-msgid "delete"
-msgstr "usuń"
+msgid "Delete project"
+msgstr "Usuń projekt"
 
 msgid "show"
 msgstr "pokaż"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Pulpit nawigacyjny jest obecnie dezaktywowany."
 
 msgid "Download Mobile Application"
 msgstr "Pobierz aplikację mobilną"
 
 msgid "Get it on"
 msgstr "Pobierz na"
 
-msgid "Are you sure?"
-msgstr "Czy jesteś pewien?"
-
 msgid "Edit project"
 msgstr "Edytuj projekt"
 
-msgid "Delete project"
-msgstr "Usuń projekt"
-
-msgid "Import JSON"
-msgstr "Importuj JSON"
-
-msgid "Choose file"
-msgstr "Wybierz plik"
+#, fuzzy
+msgid "Import project"
+msgstr "Edytuj projekt"
 
 msgid "Download project's data"
 msgstr "Pobierz dane projektu"
 
 msgid "Bill items"
 msgstr "Zawartość rachunku"
 
@@ -452,27 +461,36 @@
 
 msgid "Cancel"
 msgstr "Anuluj"
 
 msgid "Privacy Settings"
 msgstr "Ustawienia prywatności"
 
-msgid "Edit the project"
-msgstr "Edytuj projekt"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
-msgstr ""
-"Spowoduje to usunięcie wszystkich rachunków i uczestników tego projektu!"
+msgstr "Spowoduje to usunięcie wszystkich rachunków i uczestników tego projektu!"
+
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Zaimportuj wcześniej wyeksportowany plik JSON"
+
+msgid "Choose file"
+msgstr "Wybierz plik"
 
 msgid "Edit this bill"
 msgstr "Edytuj ten rachunek"
 
 msgid "Add a bill"
 msgstr "Dodaj rachunek"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Wszyscy"
 
 msgid "No one"
 msgstr "Nikt"
 
 msgid "More options"
@@ -483,17 +501,14 @@
 
 msgid "Edit this participant"
 msgstr "Edytuj tego uczestnika"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "jan.kowalski@przykład.com, anna.nowak@strona.com"
 
-msgid "Send the invitations"
-msgstr "Wyślij zaproszenia"
-
 msgid "Download"
 msgstr "Pobierz"
 
 msgid "Disabled Project History"
 msgstr "Wyłączona historia projektu"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -512,16 +527,15 @@
 msgstr "Włączona rejestracja adresu IP"
 
 msgid "History Settings Changed"
 msgstr "Ustawienia historii zmienione"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr ""
-"Rachunek %(name)s: %(property_name)s zmieniono z %(before)s na %(after)s"
+msgstr "Rachunek %(name)s: %(property_name)s zmieniono z %(before)s na %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
 msgstr "Rachunek %(name)s: %(property_name)s zmieniony na %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Potwierdź usunięcie adresów IP"
@@ -557,67 +571,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Bill %(name)s: dodano %(owers_list_str)s do listy właścicieli"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Bill %(name)s: usunięto %(owers_list_str)s z listy właścicieli"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Historia tego projektu została wyłączona. Nowe działania "
-"nie pojawią się poniżej. Możesz włączyć historię w</i>\n"
-"            <a href=\"%(url)s\">ustawieniach</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "Rejestrowanie adresu IP można włączyć na stronie ustawień"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Poniższa tabela przedstawia działania zarejestrowane przed"
-" wyłączeniem historii projektu. Możesz\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">wyczyścić historię projektu</a>, aby je "
-"usunąć.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Ktoś prawdopodobnie wyczyścił historię projektu."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Niektóre wpisy poniżej zawierają adresy IP, nawet jeśli w tym projekcie "
 "rejestrowanie IP jest wyłączone. "
 
 msgid "Delete stored IP addresses"
 msgstr "Usuń przechowywane adresy IP"
 
-msgid "No history to erase"
-msgstr "Brak historii do usunięcia"
-
-msgid "Clear Project History"
-msgstr "Wyczyść historię projektu"
-
 msgid "No IP Addresses to erase"
 msgstr "Brak adresów IP do usunięcia"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Usuń przechowywane adresy IP"
 
+msgid "No history to erase"
+msgstr "Brak historii do usunięcia"
+
+msgid "Clear Project History"
+msgstr "Wyczyść historię projektu"
+
 msgid "Time"
 msgstr "Czas"
 
 msgid "Event"
 msgstr "Wydarzenie"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -646,16 +645,15 @@
 
 #, python-format
 msgid "Project renamed to %(new_project_name)s"
 msgstr "Nazwa projektu zmieniona na %(new_project_name)s"
 
 #, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr ""
-"Adres e-mail osoby kontaktowej projektu został zmieniony na %(new_email)s"
+msgstr "Adres e-mail osoby kontaktowej projektu został zmieniony na %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Zmieniono ustawienia projektu"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
 msgstr "Uczestnik %(name)s dezaktywowany"
@@ -672,17 +670,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Rachunek %(name)s zmienił nazwę na %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr "Uczestnik %(name)s: zmiana wagi z %(old_weight)s na %(new_weight)s"
 
+msgid "Payer"
+msgstr "Płatnik"
+
 msgid "Amount"
 msgstr "Ilość"
 
+msgid "Date"
+msgstr "Data"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Ilość w %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Rachunek %(name)s zmodyfikowany"
@@ -786,16 +790,17 @@
 
 msgid "switch to"
 msgstr "przełącz na"
 
 msgid "Dashboard"
 msgstr "Kokpit"
 
-msgid "Logout"
-msgstr "Wyloguj"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Kod"
 
 msgid "Mobile Application"
 msgstr "Aplikacja mobilna"
 
@@ -820,46 +825,40 @@
 
 msgid "you sure?"
 msgstr "jesteś pewny?"
 
 msgid "Invite people"
 msgstr "Zaproś ludzi"
 
-msgid "You should start by adding participants"
-msgstr "Powinieneś zacząć od dodania uczestników"
-
-msgid "Add a new bill"
-msgstr "Dodaj nowy rachunek"
-
 msgid "Newer bills"
 msgstr "Nowsze rachunki"
 
 msgid "Older bills"
 msgstr "Starsze rachunki"
 
-msgid "When?"
-msgstr "Kiedy?"
+msgid "You should start by adding participants"
+msgstr "Powinieneś zacząć od dodania uczestników"
 
-msgid "Who paid?"
-msgstr "Kto zapłacił?"
+msgid "Add a new bill"
+msgstr "Dodaj nowy rachunek"
 
 msgid "For what?"
 msgstr "Za co?"
 
-msgid "How much?"
-msgstr "Jak dużo?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Dodano %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Wszyscy poza %(excluded)s"
 
+msgid "delete"
+msgstr "usuń"
+
 msgid "No bills"
 msgstr "Brak rachunków"
 
 msgid "Nothing to list yet."
 msgstr "Nie ma jeszcze żadnej listy."
 
 msgid "You probably want to"
@@ -910,14 +909,20 @@
 msgstr "Udostępnij link"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 "Możesz bezpośrednio udostępnić poniższy link za pośrednictwem "
 "preferowanego medium"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Wyślij przez maile"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1039,7 +1044,76 @@
 #~ msgstr "Podałeś zły token lub brak identyfikatora projektu."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Nazwa użytkownika jest niepoprawna"
 
 #~ msgid "People to notify"
 #~ msgstr "Osoby do powiadomienia"
+
+#~ msgid "Import"
+#~ msgstr "Importuj"
+
+#~ msgid "Amount paid"
+#~ msgstr "Zapłacona kwota"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Rachunki nie mogą być zerowe"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Identyfikator projektu to %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Niepoprawny JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Czy jesteś pewien?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importuj JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Historia tego projektu została"
+#~ " wyłączona. Nowe działania nie pojawią "
+#~ "się poniżej. Możesz włączyć historię "
+#~ "w</i>\n"
+#~ "            <a href=\"%(url)s\">ustawieniach</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Poniższa tabela przedstawia "
+#~ "działania zarejestrowane przed wyłączeniem "
+#~ "historii projektu. Możesz\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">wyczyścić historię "
+#~ "projektu</a>, aby je usunąć.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Wyślij zaproszenia"
+
+#~ msgid " show"
+#~ msgstr "pokaż"
+
+#~ msgid "Edit the project"
+#~ msgstr "Edytuj projekt"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Portuguese (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2023-05-05 00:47+0000\n"
+"Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
+"Language: pt\n"
 "Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-money/"
 "i-hate-money/pt/>\n"
-"Language: pt\n"
+"Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>A tabela abaixo reflete as ações registadas antes da "
-"desativação do histórico do projeto. Pode\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">limpar o histórico do projeto</a> para removê-las."
-"</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Este projeto tem o histórico desativado. Novas ações não "
-"serão exibidas abaixo. Pode ativar o histórico na</i>\n"
-"            <a href=\"%(url)s\">página de configurações</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" é um software livre"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s cada"
 
@@ -168,17 +140,14 @@
 
 msgid "Bill items"
 msgstr "Itens da fatura"
 
 msgid "Bills"
 msgstr "Contas"
 
-msgid "Bills can't be null"
-msgstr "Contas não podem ser null"
-
 msgid "Can't remember the password?"
 msgstr "Esqueceu a palavra-passe?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/pt/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,67 +1,68 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2023-05-05 00:47+0000\n"
 "Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
-"Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/pt/>\n"
-"Language: pt\n"
+"Language: pt_BR\n"
+"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/i"
+"-hate-money/i-hate-money/pt_BR/>\n"
+"Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Você acabou de criar '%(project)s' para compartilhar suas despesas"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
-"aceites."
+"aceitos."
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
 msgid "New private code"
 msgstr "Código privado novo"
 
 msgid "Enter a new code if you want to change it"
-msgstr "Digite um novo código se quiser alterá-lo"
+msgstr "Insira um novo código se quiser alterá-lo"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Ativar histórico do projeto"
 
 msgid "Use IP tracking for project history"
 msgstr "Usar rastreamento de IP para o histórico do projeto"
 
 msgid "Default Currency"
-msgstr "Moeda predefinida"
+msgstr "Moeda Padrão"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr "Definir uma moeda padrão permite a conversão de moeda entre faturas"
+msgstr "Definir uma moeda padrão permite a conversão de moeda entre contas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Este projeto não pode ser definido como 'sem moeda' porque contém faturas em "
+"O projeto não pode ser definido como 'sem moeda' porque contém contas em "
 "várias moedas."
 
-msgid "Import previously exported JSON file"
-msgstr "Importar ficheiro JSON exportado anteriormente"
-
-msgid "Import"
-msgstr "Importar"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identificador do projeto"
 
 msgid "Private code"
 msgstr "Código privado"
 
@@ -94,106 +95,118 @@
 msgid "Invalid private code."
 msgstr "Código privado inválido."
 
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
-msgstr "Palavra-passe do administrador"
+msgstr "Senha do administrador"
 
 msgid "Send me the code by email"
 msgstr "Me envie o código por e-mail"
 
 msgid "This project does not exists"
 msgstr "Este projeto não existe"
 
 msgid "Password mismatch"
-msgstr "Palavra-passe incompatível"
+msgstr "Senha incompatível"
 
 msgid "Password"
-msgstr "Palavra-passe"
+msgstr "Senha"
 
 msgid "Password confirmation"
-msgstr "Confirmação da palavra-passe"
+msgstr "Confirmação da senha"
 
 msgid "Reset password"
-msgstr "Redefinir palavra-passe"
+msgstr "Redefinir senha"
 
-msgid "Date"
-msgstr "Data"
+msgid "When?"
+msgstr "Quando?"
 
 msgid "What?"
 msgstr "O quê?"
 
-msgid "Payer"
-msgstr "Pagador"
+msgid "Who paid?"
+msgstr "Quem pagou?"
 
-msgid "Amount paid"
-msgstr "Quantia paga"
+msgid "How much?"
+msgstr "Quanto?"
 
 msgid "Currency"
 msgstr "Moeda"
 
 msgid "External link"
-msgstr "Ligação externa"
+msgstr "Link externo"
 
 msgid "A link to an external document, related to this bill"
-msgstr "Ligação para um documento externo, relacionado a essa fatura"
+msgstr "Link para um documento externo, relacionado à essa conta"
 
 msgid "For whom?"
 msgstr "Para quem?"
 
 msgid "Submit"
 msgstr "Enviar"
 
 msgid "Submit and add a new one"
 msgstr "Enviar e adicionar um novo"
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr "Projeto predefinido: %(currency)s"
-
-msgid "Bills can't be null"
-msgstr "Contas não podem ser null"
+msgstr "Projeto padrão: %(currency)s"
 
 msgid "Name"
 msgstr "Nome"
 
 msgid "Weights should be positive"
 msgstr "Pesos devem ser positivos"
 
 msgid "Weight"
 msgstr "Peso"
 
 msgid "Add"
 msgstr "Adicionar"
 
 msgid "The participant name is invalid"
-msgstr "O nome do participante é inválido"
+msgstr "'%(name)s' não é um usuário válido"
 
 msgid "This project already have this participant"
-msgstr "Este projeto já tem este participante"
+msgstr "'%(name)s' já está no projeto"
 
 msgid "People to notify"
-msgstr "Pessoas a notificar"
+msgstr "Pessoas para notificar"
 
-msgid "Send invites"
-msgstr "Enviar convites"
+msgid "Send the invitations"
+msgstr "Enviar os convites"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "O email %(email)s não é válido"
 
+msgid "Logout"
+msgstr "Sair"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Desculpe, houve um erro ao enviar os convites via e-mail. Por favor, "
+"confira a configuração de email do servidor ou entre em contato com um "
+"administrador."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr "{dual_object_0} e {dual_object_1"
+msgstr "{dual_object_0} e {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr "{previous_object} e {end_object}"
+msgstr "{previous_object}, e {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
 msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
@@ -206,297 +219,296 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Muitas tentativas de login falhas, por favor, tente novamente mais tarde."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"Esta palavra-passe de administrador não é a correta. Apenas %(num)d "
-"tentativas restantes."
+"Esta senha de administrador não é a correta. Apenas %(num)d tentativas "
+"restantes."
 
-#, fuzzy
 msgid "Provided token is invalid"
-msgstr "O token fornecido é inválido"
+msgstr "Token invalido"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado não é o correto"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Acabou de criar '%(project)s' para compartilhar as suas despesas"
-
 msgid "A reminder email has just been sent to you"
-msgstr "Um email de lembrete acabou de ser enviado a si"
+msgstr "Um email de lembrete acabou de ser enviado para você"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"Tentamos lhe enviar um email de lembrete, mas aconteceu um erro. Pode "
-"continuar usando o projeto normalmente."
-
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "O identificador do projeto é %(project)s"
+"Nós tentamos te enviar um email de lembrete, mas aconteceu um erro. Você "
+"pode continuar usando o projeto normalmente."
 
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Desculpe, houve um erro ao te enviar um email com as instruções de "
-"redefinição de palavra-passe. Por favor, confira a configuração de e-mail"
-" do servidor ou entre em contato com um administrador."
+"redefinição de senha. Por favor, confira a configuração de e-mail do "
+"servidor ou entre em contato com um administrador."
 
 msgid "No token provided"
 msgstr "Nenhum token fornecido"
 
 msgid "Invalid token"
 msgstr "Token inválido"
 
 msgid "Unknown project"
 msgstr "Projeto desconhecido"
 
 msgid "Password successfully reset."
-msgstr "Palavra-passe redefinida corretamente."
+msgstr "Senha redefinida corretamente."
 
-msgid "Project successfully uploaded"
-msgstr "Projeto enviado corretamente"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON inválido"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
+#, fuzzy
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"Não é possível adicionar faturas em várias moedas a um projeto sem moeda "
+"Não é possível adicionar contas em várias moedas a um projeto sem moeda "
 "padrão"
 
+msgid "Project successfully uploaded"
+msgstr "Projeto enviado corretamente"
+
 msgid "Project successfully deleted"
 msgstr "Projeto deletado com sucesso"
 
 msgid "Error deleting project"
-msgstr "Erro ao apagar o projeto"
+msgstr "Erro ao excluir o projeto"
+
+msgid "Unable to logout"
+msgstr ""
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr "Foi convidado a compartilhar suas despesas com %(project)s"
+msgstr "Você foi convidado a compartilhar suas despesas com %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Seus convites foram enviados"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Desculpe, houve um erro ao enviar os convites via e-mail. Por favor, "
 "confira a configuração de email do servidor ou entre em contato com um "
 "administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s foram adicionados"
 
 msgid "Error activating participant"
-msgstr "Erro ao ativar o participante"
+msgstr "Erro ao ativar usuário"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s faz parte deste projeto novamente"
 
 msgid "Error removing participant"
-msgstr "Erro ao remover o participante"
+msgstr "Erro ao remover usuário"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"O participante '%(name)s' foi desativado. Ele ainda aparecerá na lista até "
-"que o saldo dele seja zero."
+"Usuário '%(name)s' foi desativado. Ele continuará aparecendo na lista de "
+"usuários até que seu saldo seja zero."
 
-#, python-format
+#, fuzzy, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "O participante '%(name)s' foi removido"
+msgstr "Usuário '%(name)s' foi removido"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "O participante '%(name)s' foi modificado"
+msgstr "Usuário '%(name)s' foi removido"
 
 msgid "The bill has been added"
-msgstr "A fatura foi adicionada"
+msgstr "A conta foi adicionada"
 
 msgid "Error deleting bill"
-msgstr "Erro ao apagar a fatura"
+msgstr "Erro ao excluir conta"
 
 msgid "The bill has been deleted"
-msgstr "A fatura foi apagada"
+msgstr "A conta foi deletada"
 
 msgid "The bill has been modified"
-msgstr "A fatura foi modificada"
+msgstr "A conta foi modificada"
+
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
 
 msgid "Error deleting project history"
-msgstr "Erro ao apagar o histórico do projeto"
+msgstr "Erro ao deletar o histórico do projeto"
 
 msgid "Deleted project history."
 msgstr "Histórico do projeto apagado."
 
 msgid "Error deleting recorded IP addresses"
-msgstr "Erro ao apagar endereços IP gravados"
+msgstr "Erro ao excluir endereços IP salvos"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr "Endereços IP gravados apagados no histórico do projeto."
+msgstr "Endereços IP salvos no histórico de projeto deletados."
 
 msgid "Sorry, we were unable to find the page you've asked for."
-msgstr "Desculpe, não foi possível encontrar a página que solicitou."
+msgstr "Desculpe, não foi possível encontrar a página que você solicitou."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "É provável que a melhor coisa a fazer seja voltar para a página inicial."
 
 msgid "Back to the list"
 msgstr "Voltar para a lista"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Tarefas de administração estão atualmente desativadas."
 
 msgid "Authentication"
 msgstr "Autenticação"
 
 msgid "The project you are trying to access do not exist, do you want to"
-msgstr "O projeto que está tentando acessar não existe, quer"
+msgstr "O projeto que você está tentando acessar não existe, você quer"
 
 msgid "create it"
 msgstr "Criar"
 
 msgid "?"
 msgstr "?"
 
 msgid "Create a new project"
-msgstr "Criar um projeto"
+msgstr "Criar um novo projeto"
 
 msgid "Project"
 msgstr "Projeto"
 
 msgid "Number of participants"
-msgstr "Quantidade de participantes"
+msgstr "Número de usuários"
 
 msgid "Number of bills"
-msgstr "Quantidade de faturas"
+msgstr "Número de contas"
 
 msgid "Newest bill"
 msgstr "Conta mais recente"
 
 msgid "Oldest bill"
 msgstr "Conta mais antiga"
 
 msgid "Actions"
 msgstr "Ações"
 
 msgid "edit"
 msgstr "editar"
 
-msgid "delete"
-msgstr "deletar"
+msgid "Delete project"
+msgstr "Excluir projeto"
 
 msgid "show"
 msgstr "exibir"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "O Painel de Controle atualmente está desativado."
 
 msgid "Download Mobile Application"
-msgstr "Descarregar Aplicação Mobile"
+msgstr "Baixar o APP"
 
 msgid "Get it on"
-msgstr "Vamos"
-
-msgid "Are you sure?"
-msgstr "Tem certeza?"
+msgstr "Pegue agora"
 
 msgid "Edit project"
 msgstr "Editar projeto"
 
-msgid "Delete project"
-msgstr "Apagarr projeto"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Choose file"
-msgstr "Escolher ficheiro"
+#, fuzzy
+msgid "Import project"
+msgstr "Editar projeto"
 
 msgid "Download project's data"
-msgstr "Descarregar dados do projeto"
+msgstr "Baixar dados do projeto"
 
 msgid "Bill items"
-msgstr "Itens da fatura"
+msgstr "Itens da conta"
 
 msgid "Download the list of bills with owner, amount, reason,... "
-msgstr "Descarregar a lista de faturas com dono, quantia, motivo,... "
+msgstr "Baixar a lista de contas com dono, quantia, motivo,... "
 
 msgid "Settle plans"
 msgstr "Estabelecer planos"
 
 msgid "Download the list of transactions needed to settle the current bills."
-msgstr ""
-"Descarregar a lista de transações necessárias para liquidar as faturas "
-"atuais."
+msgstr "Baixar a lista de transações necessárias para liquidar as contas atuais."
 
 msgid "Can't remember the password?"
-msgstr "Esqueceu a palavra-passe?"
+msgstr "Esqueceu a senha?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Privacy Settings"
 msgstr "Configurações de Privacidade"
 
-msgid "Edit the project"
-msgstr "Editar o projeto"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
-msgstr "Isso removerá todas as faturas e os participantes deste projeto!"
+msgstr "Isso vai remover todas as contas e participantes desse projeto!"
+
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importar arquivo JSON exportado anteriormente"
+
+msgid "Choose file"
+msgstr "Escolher arquivo"
 
 msgid "Edit this bill"
-msgstr "Editar esta fatura"
+msgstr "Editar esta conta"
 
 msgid "Add a bill"
-msgstr "Adicionar uma fatura"
+msgstr "Adicionar uma conta"
+
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
 
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "No one"
-msgstr "Ninguem"
+msgstr "Ninguém"
 
 msgid "More options"
 msgstr "Mais opções"
 
 msgid "Add participant"
 msgstr "Adicionar participante"
 
 msgid "Edit this participant"
-msgstr "Editar este participante"
+msgstr "Editar usuário"
 
 msgid "john.doe@example.com, mary.moe@site.com"
-msgstr "flano.tal@exemplo.com, flana.maria@site.com"
-
-msgid "Send the invitations"
-msgstr "Enviar os convites"
+msgstr "john.doe@example.com, mary.moe@site.com"
 
 msgid "Download"
-msgstr "Descarregar"
+msgstr "Baixar"
 
 msgid "Disabled Project History"
 msgstr "Histórico do Projeto Desativado"
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr "Histórico do Projeto Desativado & Gravação de Endereço IP"
 
@@ -513,30 +525,30 @@
 msgstr "Gravação do Endereço IP Ativada"
 
 msgid "History Settings Changed"
 msgstr "Configurações do Histórico Alteradas"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr "Fatura %(name)s: %(property_name)s alterado de %(before)s a %(after)s"
+msgstr "Conta %(name)s: %(property_name)s mudou de %(before)s para %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr "Fatura %(name)s: %(property_name)s alterado a %(after)s"
+msgstr "Conta %(name)s: %(property_name)s mudou para %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar a remoção dos Endereços IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
-"Tem certeza que deseja apagar todos os endereços IP gravados deste "
+"Você tem certeza que deseja deletar todos os endereços IP gravados deste "
 "projeto?\n"
 "                O resto do histórico do projeto não será afetado. Esta "
 "ação não pode ser desfeita."
 
 msgid "Confirm deletion"
 msgstr "Confirmar exclusão"
 
@@ -551,73 +563,58 @@
 "cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todo o histórico deste projeto? Esta ação "
 "não pode ser desfeita."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr "Fatura %(name)s: adicionado %(owers_list_str)s à lista de proprietários"
+msgstr "Conta %(name)s: adicionou %(owers_list_str)s a lista de devedores"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
-msgstr "Fatura %(name)s: removido %(owers_list_str)s da lista de proprietários"
+msgstr "Conta %(name)s: removeu %(owers_list_str)s da lista de devedores"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Este projeto tem o histórico desativado. Novas ações não "
-"serão exibidas abaixo. Pode ativar o histórico na</i>\n"
-"            <a href=\"%(url)s\">página de configurações</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "A gravação do endereço IP pode ser ativada na página de configurações"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>A tabela abaixo reflete as ações registadas antes da "
-"desativação do histórico do projeto. Pode\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">limpar o histórico do projeto</a> para "
-"removê-las.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Alguém provavelmente limpou o histórico do projeto."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Algumas das entradas abaixo contém endereços IP, mesmo este projeto tendo"
 " a gravação de IP desativada. "
 
 msgid "Delete stored IP addresses"
-msgstr "Deletar endereços IP gravados"
+msgstr "Deletar endereços IP salvos"
+
+msgid "No IP Addresses to erase"
+msgstr "Não há endereços IP para apagar"
+
+msgid "Delete Stored IP Addresses"
+msgstr "Deletar endereços IP salvos"
 
 msgid "No history to erase"
 msgstr "Não há histórico para apagar"
 
 msgid "Clear Project History"
 msgstr "Limpar Histórico do Projeto"
 
-msgid "No IP Addresses to erase"
-msgstr "Não há endereços IP para apagar"
-
-msgid "Delete Stored IP Addresses"
-msgstr "Deletar endereços IP gravados"
-
 msgid "Time"
 msgstr "Tempo"
 
 msgid "Event"
 msgstr "Evento"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -635,72 +632,78 @@
 
 #, python-format
 msgid "Bill %(name)s added"
 msgstr "Conta %(name)s adicionada"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr "Participante %(name)s adicionado"
+msgstr "Usuário %(name)s adicionado"
 
 msgid "Project private code changed"
 msgstr "Código privado do projeto alterado"
 
 #, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "Projeto renomeado a %(new_project_name)s"
+msgstr "Projeto renomeado para %(new_project_name)s"
 
 #, python-format
 msgid "Project contact email changed to %(new_email)s"
 msgstr "O email de contato do projeto foi alterado para %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Configurações do projeto alteradas"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr "Participante %(name)s desativado"
+msgstr "Usuário %(name)s desativado"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr "Participante %(name)s reativado"
+msgstr "Usuário %(name)s reativado"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr "Participante %(name)s renomeado a %(new_name)s"
+msgstr "Usuário %(name)s renomeado para %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr "Fatura %(name)s renomeada a %(new_description)s"
+msgstr "Conta %(name)s renomeada para %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr "Participante %(name)s: peso alterado de %(old_weight)s a %(new_weight)s"
+msgstr "Usuário %(name)s: a carga mudou de %(old_weight)s para %(new_weight)s"
+
+msgid "Payer"
+msgstr "Pagador"
 
 msgid "Amount"
 msgstr "Quantia"
 
+msgid "Date"
+msgstr "Data"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Quantia em %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Conta %(name)s modificada"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr "Participante %(name)s modificado"
+msgstr "Usuário %(name)s modificado"
 
 #, python-format
 msgid "Bill %(name)s removed"
-msgstr "Fatura %(name)s removida"
+msgstr "Conta '%(name)s' foi removida"
 
-#, python-format
+#, fuzzy, python-format
 msgid "Participant %(name)s removed"
-msgstr "Participante %(name)s removido"
+msgstr "Usuário '%(name)s' foi removido"
 
 #, python-format
 msgid "Project %(name)s changed in an unknown way"
 msgstr "Projeto %(name)s modificado de maneira desconhecida"
 
 #, python-format
 msgid "Bill %(name)s changed in an unknown way"
@@ -719,46 +722,46 @@
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Modifique suas despesas <br />compartilhadas, facilmente"
 
 msgid "Try out the demo"
 msgstr "Experimente a demonstração"
 
 msgid "You're sharing a house?"
-msgstr "Está dividindo uma casa?"
+msgstr "Você está dividindo uma casa?"
 
 msgid "Going on holidays with friends?"
 msgstr "Indo para o feriado com os amigos?"
 
 msgid "Simply sharing money with others?"
 msgstr "Simplesmente compartilhando dinheiro com outras pessoas?"
 
 msgid "We can help!"
 msgstr "Nós podemos ajudar!"
 
 msgid "Log in to an existing project"
-msgstr "Conecte-se num projeto existente"
+msgstr "Conecte-se em um projeto existente"
 
 msgid "Log in"
 msgstr "Conecte-se"
 
 msgid "can't remember your password?"
-msgstr "não se consegue lembrar da sua palavra-passe?"
+msgstr "não consegue se lembrar da sua senha?"
 
 msgid "Create"
 msgstr "Criar"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
-"Não reutilize uma palavra-passe pessoal. Escolha um código privado e "
-"envie-o para seus amigos"
+"Não reutilize uma senha pessoal. Escolha um código privado e envie-o para"
+" seus amigos"
 
 msgid "Account manager"
-msgstr "Gestor de contas"
+msgstr "Gerenciador de contas"
 
 msgid "Bills"
 msgstr "Contas"
 
 msgid "Settle"
 msgstr "Estabelecer"
 
@@ -785,16 +788,17 @@
 
 msgid "switch to"
 msgstr "mudar para"
 
 msgid "Dashboard"
 msgstr "Painel de controle"
 
-msgid "Logout"
-msgstr "Sair"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Mobile Application"
 msgstr "Aplicação Mobile"
 
@@ -807,156 +811,156 @@
 msgid "Legal information"
 msgstr "Informações legais"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" é um software livre"
 
 msgid "you can contribute and improve it!"
-msgstr "Pode contribuir para melhorá-lo!"
+msgstr "você pode contribuir para melhorá-lo!"
 
 #, python-format
 msgid "%(amount)s each"
 msgstr "%(amount)s cada"
 
 msgid "you sure?"
 msgstr "tem certeza?"
 
 msgid "Invite people"
 msgstr "Convidar pessoas"
 
-msgid "You should start by adding participants"
-msgstr "Deveria começar adicionando pessoas"
-
-msgid "Add a new bill"
-msgstr "Adicionar uma nova fatura"
-
 msgid "Newer bills"
 msgstr "Contas mais recentes"
 
 msgid "Older bills"
 msgstr "Contas mais antigas"
 
-msgid "When?"
-msgstr "Quando?"
+msgid "You should start by adding participants"
+msgstr "Você deveria começar adicionando pessoas"
 
-msgid "Who paid?"
-msgstr "Quem pagou?"
+msgid "Add a new bill"
+msgstr "Adicionar uma nova conta"
 
 msgid "For what?"
 msgstr "Para quê?"
 
-msgid "How much?"
-msgstr "Quanto?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Adicionado em %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Todos menos %(excluded)s"
 
+msgid "delete"
+msgstr "deletar"
+
 msgid "No bills"
-msgstr "Sem faturas"
+msgstr "Sem contas"
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
 msgid "You probably want to"
-msgstr "Provavelmente gostaria de"
+msgstr "Você provavelmente gostaria de"
 
 msgid "add a bill"
-msgstr "adicionar uma fatura"
+msgstr "adicionar uma conta"
 
 msgid "add participants"
 msgstr "adicionar participantes"
 
 msgid "Password reminder"
-msgstr "Lembrete de palavra-passe"
+msgstr "Lembrete de senha"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
-"Uma ligação para redefinir a sua palavra-passe foi enviado a si, por "
-"favor verifique os seus e-mails."
+"Um link para redefinir sua senha foi enviado a você, por favor verifique "
+"seus e-mails."
 
 msgid "Return to home page"
 msgstr "Retornar à pagina inicial"
 
 msgid "Your projects"
 msgstr "Seus projetos"
 
 msgid "Reset your password"
-msgstr "Redefinir sua palavra-passe"
+msgstr "Redefinir sua senha"
 
 msgid "Invite people to join this project"
 msgstr "Convide pessoas para participar deste projeto"
 
 msgid "Share Identifier & code"
 msgstr "Compartilhar Identificador & código"
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
-"Pode compartilhar o identificador do projeto e o código privado por "
+"Você pode compartilhar o identificador do projeto e o código privado por "
 "qualquer meio de comunicação."
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
 msgid "Share the Link"
-msgstr "Compartilhar a ligação"
+msgstr "Compartilhar o Link"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
-"Pode compartilhar diretamente o seguinte ligação através do seu meio "
+"Você pode compartilhar diretamente o seguinte link através do seu meio "
 "preferido"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Enviar via E-mails"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
-"Especifique uma lista (separada por vírgulas) de endereços de e-mail que "
-"deseja notificar sobre a\n"
-"                criação deste projeto de gestão orçamental e enviaremos "
-"um e-mail para si."
+"Especifica uma lista de endereços de email (separados por vírgula) que "
+"você quer notificar acerca da\n"
+"                criação deste projeto de gestão de saldo e nós iremos "
+"enviar um email por si."
 
 msgid "Who pays?"
 msgstr "Quem paga?"
 
 msgid "To whom?"
-msgstr "A quem?"
+msgstr "Para quem?"
 
 msgid "Who?"
 msgstr "Quem?"
 
 msgid "Balance"
 msgstr "Saldo"
 
 msgid "deactivate"
-msgstr "desativar"
+msgstr "desativado"
 
 msgid "reactivate"
 msgstr "reativar"
 
 msgid "Paid"
 msgstr "Pago"
 
 msgid "Spent"
 msgstr "Gasto"
 
 msgid "Expenses by Month"
-msgstr "Despesas por mês"
+msgstr "Gastos por Mês"
 
 msgid "Period"
 msgstr "Período"
 
 #~ msgid "Participant"
 #~ msgstr "Participante"
 
@@ -966,15 +970,15 @@
 #~ msgid "Select all"
 #~ msgstr "Selecionar tudo"
 
 #~ msgid "Select none"
 #~ msgstr "Selecionar nenhum"
 
 #~ msgid "changed"
-#~ msgstr "alterado"
+#~ msgstr "modificado"
 
 #~ msgid "from"
 #~ msgstr "de"
 
 #~ msgid "to"
 #~ msgstr "para"
 
@@ -1002,23 +1006,93 @@
 #~ msgid "reactivated"
 #~ msgstr "reativado"
 
 #~ msgid "renamed to"
 #~ msgstr "renomeado para"
 
 #~ msgid "External link changed to"
-#~ msgstr "Ligação externa alterado para"
+#~ msgstr "Link externo alterado para"
 
 #~ msgid "modified"
 #~ msgstr "modificado"
 
 #~ msgid "removed"
 #~ msgstr "removido"
 
 #~ msgid "You either provided a bad token or no project identifier."
-#~ msgstr "Forneceu um token ruim ou não forneceu o identificador do projeto."
+#~ msgstr "Você forneceu um token ruim ou não forneceu o identificador do projeto."
 
 #~ msgid "User name incorrect"
-#~ msgstr "Nome de utilizador incorreto"
+#~ msgstr "Nome de usuário incorreto"
 
 #~ msgid "People to notify"
 #~ msgstr "Pessoas para notificar"
+
+#~ msgid "Import"
+#~ msgstr "Importar"
+
+#~ msgid "Amount paid"
+#~ msgstr "Quantia paga"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Contas não podem ser null"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "O identificador do projeto é %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON inválido"
+
+#~ msgid "Are you sure?"
+#~ msgstr "tem certeza?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importar JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Este projeto tem o "
+#~ "histórico desativado. Novas ações não "
+#~ "serão exibidas abaixo. Você pode ativar"
+#~ " o histórico na</i>\n"
+#~ "            <a href=\"%(url)s\">página de configurações</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>A tabela abaixo reflete "
+#~ "as ações registradas antes da "
+#~ "desativação do histórico do projeto. "
+#~ "Você pode\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">limpar o histórico "
+#~ "do projeto</a> para removê-las.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Enviar convites"
+
+#~ msgid " show"
+#~ msgstr "exibir"
+
+#~ msgid "Edit the project"
+#~ msgstr "Editar o projeto"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Portuguese (Brazil) (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2023-05-05 00:47+0000\n"
+"Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
+"Language: pt_BR\n"
 "Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/i-"
 "hate-money/i-hate-money/pt_BR/>\n"
-"Language: pt_BR\n"
+"Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>A tabela abaixo reflete as ações registradas antes da "
-"desativação do histórico do projeto. Você pode\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">limpar o histórico do projeto</a> para removê-las."
-"</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Este projeto tem o histórico desativado. Novas ações não "
-"serão exibidas abaixo. Você pode ativar o histórico na</i>\n"
-"            <a href=\"%(url)s\">página de configurações</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" é um software livre"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s cada"
 
@@ -168,17 +140,14 @@
 
 msgid "Bill items"
 msgstr "Itens da conta"
 
 msgid "Bills"
 msgstr "Contas"
 
-msgid "Bills can't be null"
-msgstr "Contas não podem ser null"
-
 msgid "Can't remember the password?"
 msgstr "Esqueceu a senha?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Choose file"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/pt_BR/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/pt/LC_MESSAGES/messages.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,68 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2023-05-05 00:47+0000\n"
 "Last-Translator: MurkBRA <anjo1077@gmail.com>\n"
-"Language-Team: Portuguese (Brazil) <https://hosted.weblate.org/projects/"
-"i-hate-money/i-hate-money/pt_BR/>\n"
-"Language: pt_BR\n"
+"Language: pt\n"
+"Language-Team: Portuguese <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/pt/>\n"
+"Plural-Forms: nplurals=2; plural=n > 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Acabou de criar '%(project)s' para compartilhar as suas despesas"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Expressão ou montante inválido. Apenas números e os operadores +=*/ são "
-"aceitos."
+"aceites."
 
 msgid "Project name"
 msgstr "Nome do projeto"
 
 msgid "New private code"
 msgstr "Código privado novo"
 
 msgid "Enter a new code if you want to change it"
-msgstr "Insira um novo código se quiser alterá-lo"
+msgstr "Digite um novo código se quiser alterá-lo"
 
 msgid "Email"
 msgstr "E-mail"
 
 msgid "Enable project history"
 msgstr "Ativar histórico do projeto"
 
 msgid "Use IP tracking for project history"
 msgstr "Usar rastreamento de IP para o histórico do projeto"
 
 msgid "Default Currency"
-msgstr "Moeda Padrão"
+msgstr "Moeda predefinida"
 
 msgid "Setting a default currency enables currency conversion between bills"
-msgstr "Definir uma moeda padrão permite a conversão de moeda entre contas"
+msgstr "Definir uma moeda padrão permite a conversão de moeda entre faturas"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"O projeto não pode ser definido como 'sem moeda' porque contém contas em "
-"várias moedas."
-
-msgid "Import previously exported JSON file"
-msgstr "Importar arquivo JSON exportado anteriormente"
+"Este projeto não pode ser definido como 'sem moeda' porque contém faturas"
+" em várias moedas."
 
-msgid "Import"
-msgstr "Importar"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Identificador do projeto"
 
 msgid "Private code"
 msgstr "Código privado"
 
@@ -94,106 +95,118 @@
 msgid "Invalid private code."
 msgstr "Código privado inválido."
 
 msgid "Get in"
 msgstr "Entrar"
 
 msgid "Admin password"
-msgstr "Senha do administrador"
+msgstr "Palavra-passe do administrador"
 
 msgid "Send me the code by email"
 msgstr "Me envie o código por e-mail"
 
 msgid "This project does not exists"
 msgstr "Este projeto não existe"
 
 msgid "Password mismatch"
-msgstr "Senha incompatível"
+msgstr "Palavra-passe incompatível"
 
 msgid "Password"
-msgstr "Senha"
+msgstr "Palavra-passe"
 
 msgid "Password confirmation"
-msgstr "Confirmação da senha"
+msgstr "Confirmação da palavra-passe"
 
 msgid "Reset password"
-msgstr "Redefinir senha"
+msgstr "Redefinir palavra-passe"
 
-msgid "Date"
-msgstr "Data"
+msgid "When?"
+msgstr "Quando?"
 
 msgid "What?"
 msgstr "O quê?"
 
-msgid "Payer"
-msgstr "Pagador"
+msgid "Who paid?"
+msgstr "Quem pagou?"
 
-msgid "Amount paid"
-msgstr "Quantia paga"
+msgid "How much?"
+msgstr "Quanto?"
 
 msgid "Currency"
 msgstr "Moeda"
 
 msgid "External link"
-msgstr "Link externo"
+msgstr "Ligação externa"
 
 msgid "A link to an external document, related to this bill"
-msgstr "Link para um documento externo, relacionado à essa conta"
+msgstr "Ligação para um documento externo, relacionado a essa fatura"
 
 msgid "For whom?"
 msgstr "Para quem?"
 
 msgid "Submit"
 msgstr "Enviar"
 
 msgid "Submit and add a new one"
 msgstr "Enviar e adicionar um novo"
 
 #, python-format
 msgid "Project default: %(currency)s"
-msgstr "Projeto padrão: %(currency)s"
-
-msgid "Bills can't be null"
-msgstr "Contas não podem ser null"
+msgstr "Projeto predefinido: %(currency)s"
 
 msgid "Name"
 msgstr "Nome"
 
 msgid "Weights should be positive"
 msgstr "Pesos devem ser positivos"
 
 msgid "Weight"
 msgstr "Peso"
 
 msgid "Add"
 msgstr "Adicionar"
 
 msgid "The participant name is invalid"
-msgstr "'%(name)s' não é um usuário válido"
+msgstr "O nome do participante é inválido"
 
 msgid "This project already have this participant"
-msgstr "'%(name)s' já está no projeto"
+msgstr "Este projeto já tem este participante"
 
 msgid "People to notify"
-msgstr "Pessoas para notificar"
+msgstr "Pessoas a notificar"
 
-msgid "Send invites"
-msgstr "Enviar convites"
+msgid "Send the invitations"
+msgstr "Enviar os convites"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "O email %(email)s não é válido"
 
+msgid "Logout"
+msgstr "Sair"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Desculpe, houve um erro ao enviar os convites via e-mail. Por favor, "
+"confira a configuração de email do servidor ou entre em contato com um "
+"administrador."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
-msgstr "{dual_object_0} e {dual_object_1}"
+msgstr "{dual_object_0} e {dual_object_1"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
-msgstr "{previous_object}, e {end_object}"
+msgstr "{previous_object} e {end_object}"
 
 #. Two items in a middle of a list with more than 5 objects
 msgid "{previous_object}, {next_object}"
 msgstr "{previous_object}, {next_object}"
 
 #. First two items of a list with more than 3 items
 msgid "{start_object}, {next_object}"
@@ -206,296 +219,298 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Muitas tentativas de login falhas, por favor, tente novamente mais tarde."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"Esta senha de administrador não é a correta. Apenas %(num)d tentativas "
-"restantes."
+"Esta palavra-passe de administrador não é a correta. Apenas %(num)d "
+"tentativas restantes."
 
+#, fuzzy
 msgid "Provided token is invalid"
-msgstr "Token invalido"
+msgstr "O token fornecido é inválido"
 
 msgid "This private code is not the right one"
 msgstr "Este código privado não é o correto"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Você acabou de criar '%(project)s' para compartilhar suas despesas"
-
 msgid "A reminder email has just been sent to you"
-msgstr "Um email de lembrete acabou de ser enviado para você"
+msgstr "Um email de lembrete acabou de ser enviado a si"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"Nós tentamos te enviar um email de lembrete, mas aconteceu um erro. Você "
-"pode continuar usando o projeto normalmente."
-
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "O identificador do projeto é %(project)s"
+"Tentamos lhe enviar um email de lembrete, mas aconteceu um erro. Pode "
+"continuar usando o projeto normalmente."
 
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Desculpe, houve um erro ao te enviar um email com as instruções de "
-"redefinição de senha. Por favor, confira a configuração de e-mail do "
-"servidor ou entre em contato com um administrador."
+"redefinição de palavra-passe. Por favor, confira a configuração de e-mail"
+" do servidor ou entre em contato com um administrador."
 
 msgid "No token provided"
 msgstr "Nenhum token fornecido"
 
 msgid "Invalid token"
 msgstr "Token inválido"
 
 msgid "Unknown project"
 msgstr "Projeto desconhecido"
 
 msgid "Password successfully reset."
-msgstr "Senha redefinida corretamente."
+msgstr "Palavra-passe redefinida corretamente."
 
-msgid "Project successfully uploaded"
-msgstr "Projeto enviado corretamente"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON inválido"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
-#, fuzzy
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"Não é possível adicionar contas em várias moedas a um projeto sem moeda "
+"Não é possível adicionar faturas em várias moedas a um projeto sem moeda "
 "padrão"
 
+msgid "Project successfully uploaded"
+msgstr "Projeto enviado corretamente"
+
 msgid "Project successfully deleted"
 msgstr "Projeto deletado com sucesso"
 
 msgid "Error deleting project"
-msgstr "Erro ao excluir o projeto"
+msgstr "Erro ao apagar o projeto"
+
+msgid "Unable to logout"
+msgstr ""
 
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
-msgstr "Você foi convidado a compartilhar suas despesas com %(project)s"
+msgstr "Foi convidado a compartilhar suas despesas com %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Seus convites foram enviados"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Desculpe, houve um erro ao enviar os convites via e-mail. Por favor, "
 "confira a configuração de email do servidor ou entre em contato com um "
 "administrador."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s foram adicionados"
 
 msgid "Error activating participant"
-msgstr "Erro ao ativar usuário"
+msgstr "Erro ao ativar o participante"
 
 #, python-format
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s faz parte deste projeto novamente"
 
 msgid "Error removing participant"
-msgstr "Erro ao remover usuário"
+msgstr "Erro ao remover o participante"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Usuário '%(name)s' foi desativado. Ele continuará aparecendo na lista de "
-"usuários até que seu saldo seja zero."
+"O participante '%(name)s' foi desativado. Ele ainda aparecerá na lista "
+"até que o saldo dele seja zero."
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Usuário '%(name)s' foi removido"
+msgstr "O participante '%(name)s' foi removido"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Usuário '%(name)s' foi removido"
+msgstr "O participante '%(name)s' foi modificado"
 
 msgid "The bill has been added"
-msgstr "A conta foi adicionada"
+msgstr "A fatura foi adicionada"
 
 msgid "Error deleting bill"
-msgstr "Erro ao excluir conta"
+msgstr "Erro ao apagar a fatura"
 
 msgid "The bill has been deleted"
-msgstr "A conta foi deletada"
+msgstr "A fatura foi apagada"
 
 msgid "The bill has been modified"
-msgstr "A conta foi modificada"
+msgstr "A fatura foi modificada"
+
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
 
 msgid "Error deleting project history"
-msgstr "Erro ao deletar o histórico do projeto"
+msgstr "Erro ao apagar o histórico do projeto"
 
 msgid "Deleted project history."
 msgstr "Histórico do projeto apagado."
 
 msgid "Error deleting recorded IP addresses"
-msgstr "Erro ao excluir endereços IP salvos"
+msgstr "Erro ao apagar endereços IP gravados"
 
 msgid "Deleted recorded IP addresses in project history."
-msgstr "Endereços IP salvos no histórico de projeto deletados."
+msgstr "Endereços IP gravados apagados no histórico do projeto."
 
 msgid "Sorry, we were unable to find the page you've asked for."
-msgstr "Desculpe, não foi possível encontrar a página que você solicitou."
+msgstr "Desculpe, não foi possível encontrar a página que solicitou."
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr "É provável que a melhor coisa a fazer seja voltar para a página inicial."
 
 msgid "Back to the list"
 msgstr "Voltar para a lista"
 
 msgid "Administration tasks are currently disabled."
 msgstr "Tarefas de administração estão atualmente desativadas."
 
 msgid "Authentication"
 msgstr "Autenticação"
 
 msgid "The project you are trying to access do not exist, do you want to"
-msgstr "O projeto que você está tentando acessar não existe, você quer"
+msgstr "O projeto que está tentando acessar não existe, quer"
 
 msgid "create it"
 msgstr "Criar"
 
 msgid "?"
 msgstr "?"
 
 msgid "Create a new project"
-msgstr "Criar um novo projeto"
+msgstr "Criar um projeto"
 
 msgid "Project"
 msgstr "Projeto"
 
 msgid "Number of participants"
-msgstr "Número de usuários"
+msgstr "Quantidade de participantes"
 
 msgid "Number of bills"
-msgstr "Número de contas"
+msgstr "Quantidade de faturas"
 
 msgid "Newest bill"
 msgstr "Conta mais recente"
 
 msgid "Oldest bill"
 msgstr "Conta mais antiga"
 
 msgid "Actions"
 msgstr "Ações"
 
 msgid "edit"
 msgstr "editar"
 
-msgid "delete"
-msgstr "deletar"
+msgid "Delete project"
+msgstr "Apagarr projeto"
 
 msgid "show"
 msgstr "exibir"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "O Painel de Controle atualmente está desativado."
 
 msgid "Download Mobile Application"
-msgstr "Baixar o APP"
+msgstr "Descarregar Aplicação Mobile"
 
 msgid "Get it on"
-msgstr "Pegue agora"
-
-#, fuzzy
-msgid "Are you sure?"
-msgstr "tem certeza?"
+msgstr "Vamos"
 
 msgid "Edit project"
 msgstr "Editar projeto"
 
-msgid "Delete project"
-msgstr "Excluir projeto"
-
-msgid "Import JSON"
-msgstr "Importar JSON"
-
-msgid "Choose file"
-msgstr "Escolher arquivo"
+#, fuzzy
+msgid "Import project"
+msgstr "Editar projeto"
 
 msgid "Download project's data"
-msgstr "Baixar dados do projeto"
+msgstr "Descarregar dados do projeto"
 
 msgid "Bill items"
-msgstr "Itens da conta"
+msgstr "Itens da fatura"
 
 msgid "Download the list of bills with owner, amount, reason,... "
-msgstr "Baixar a lista de contas com dono, quantia, motivo,... "
+msgstr "Descarregar a lista de faturas com dono, quantia, motivo,... "
 
 msgid "Settle plans"
 msgstr "Estabelecer planos"
 
 msgid "Download the list of transactions needed to settle the current bills."
-msgstr "Baixar a lista de transações necessárias para liquidar as contas atuais."
+msgstr ""
+"Descarregar a lista de transações necessárias para liquidar as faturas "
+"atuais."
 
 msgid "Can't remember the password?"
-msgstr "Esqueceu a senha?"
+msgstr "Esqueceu a palavra-passe?"
 
 msgid "Cancel"
 msgstr "Cancelar"
 
 msgid "Privacy Settings"
 msgstr "Configurações de Privacidade"
 
-msgid "Edit the project"
-msgstr "Editar o projeto"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
-msgstr "Isso vai remover todas as contas e participantes desse projeto!"
+msgstr "Isso removerá todas as faturas e os participantes deste projeto!"
+
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importar ficheiro JSON exportado anteriormente"
+
+msgid "Choose file"
+msgstr "Escolher ficheiro"
 
 msgid "Edit this bill"
-msgstr "Editar esta conta"
+msgstr "Editar esta fatura"
 
 msgid "Add a bill"
-msgstr "Adicionar uma conta"
+msgstr "Adicionar uma fatura"
+
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
 
 msgid "Everyone"
 msgstr "Todos"
 
 msgid "No one"
-msgstr "Ninguém"
+msgstr "Ninguem"
 
 msgid "More options"
 msgstr "Mais opções"
 
 msgid "Add participant"
 msgstr "Adicionar participante"
 
 msgid "Edit this participant"
-msgstr "Editar usuário"
+msgstr "Editar este participante"
 
 msgid "john.doe@example.com, mary.moe@site.com"
-msgstr "john.doe@example.com, mary.moe@site.com"
-
-msgid "Send the invitations"
-msgstr "Enviar os convites"
+msgstr "flano.tal@exemplo.com, flana.maria@site.com"
 
 msgid "Download"
-msgstr "Baixar"
+msgstr "Descarregar"
 
 msgid "Disabled Project History"
 msgstr "Histórico do Projeto Desativado"
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr "Histórico do Projeto Desativado & Gravação de Endereço IP"
 
@@ -512,30 +527,30 @@
 msgstr "Gravação do Endereço IP Ativada"
 
 msgid "History Settings Changed"
 msgstr "Configurações do Histórico Alteradas"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
-msgstr "Conta %(name)s: %(property_name)s mudou de %(before)s para %(after)s"
+msgstr "Fatura %(name)s: %(property_name)s alterado de %(before)s a %(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
-msgstr "Conta %(name)s: %(property_name)s mudou para %(after)s"
+msgstr "Fatura %(name)s: %(property_name)s alterado a %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Confirmar a remoção dos Endereços IP"
 
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
-"Você tem certeza que deseja deletar todos os endereços IP gravados deste "
+"Tem certeza que deseja apagar todos os endereços IP gravados deste "
 "projeto?\n"
 "                O resto do histórico do projeto não será afetado. Esta "
 "ação não pode ser desfeita."
 
 msgid "Confirm deletion"
 msgstr "Confirmar exclusão"
 
@@ -550,73 +565,58 @@
 "cannot be undone."
 msgstr ""
 "Tem certeza que deseja apagar todo o histórico deste projeto? Esta ação "
 "não pode ser desfeita."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
-msgstr "Conta %(name)s: adicionou %(owers_list_str)s a lista de devedores"
+msgstr "Fatura %(name)s: adicionado %(owers_list_str)s à lista de proprietários"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
-msgstr "Conta %(name)s: removeu %(owers_list_str)s da lista de devedores"
+msgstr "Fatura %(name)s: removido %(owers_list_str)s da lista de proprietários"
+
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "A gravação do endereço IP pode ser ativada na página de configurações"
 
-#, python-format
 msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Este projeto tem o histórico desativado. Novas ações não "
-"serão exibidas abaixo. Você pode ativar o histórico na</i>\n"
-"            <a href=\"%(url)s\">página de configurações</a>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>A tabela abaixo reflete as ações registradas antes da "
-"desativação do histórico do projeto. Você pode\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">limpar o histórico do projeto</a> para "
-"removê-las.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Alguém provavelmente limpou o histórico do projeto."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Algumas das entradas abaixo contém endereços IP, mesmo este projeto tendo"
 " a gravação de IP desativada. "
 
 msgid "Delete stored IP addresses"
-msgstr "Deletar endereços IP salvos"
+msgstr "Deletar endereços IP gravados"
+
+msgid "No IP Addresses to erase"
+msgstr "Não há endereços IP para apagar"
+
+msgid "Delete Stored IP Addresses"
+msgstr "Deletar endereços IP gravados"
 
 msgid "No history to erase"
 msgstr "Não há histórico para apagar"
 
 msgid "Clear Project History"
 msgstr "Limpar Histórico do Projeto"
 
-msgid "No IP Addresses to erase"
-msgstr "Não há endereços IP para apagar"
-
-msgid "Delete Stored IP Addresses"
-msgstr "Deletar endereços IP salvos"
-
 msgid "Time"
 msgstr "Tempo"
 
 msgid "Event"
 msgstr "Evento"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -634,72 +634,78 @@
 
 #, python-format
 msgid "Bill %(name)s added"
 msgstr "Conta %(name)s adicionada"
 
 #, python-format
 msgid "Participant %(name)s added"
-msgstr "Usuário %(name)s adicionado"
+msgstr "Participante %(name)s adicionado"
 
 msgid "Project private code changed"
 msgstr "Código privado do projeto alterado"
 
 #, python-format
 msgid "Project renamed to %(new_project_name)s"
-msgstr "Projeto renomeado para %(new_project_name)s"
+msgstr "Projeto renomeado a %(new_project_name)s"
 
 #, python-format
 msgid "Project contact email changed to %(new_email)s"
 msgstr "O email de contato do projeto foi alterado para %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Configurações do projeto alteradas"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
-msgstr "Usuário %(name)s desativado"
+msgstr "Participante %(name)s desativado"
 
 #, python-format
 msgid "Participant %(name)s reactivated"
-msgstr "Usuário %(name)s reativado"
+msgstr "Participante %(name)s reativado"
 
 #, python-format
 msgid "Participant %(name)s renamed to %(new_name)s"
-msgstr "Usuário %(name)s renomeado para %(new_name)s"
+msgstr "Participante %(name)s renomeado a %(new_name)s"
 
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
-msgstr "Conta %(name)s renomeada para %(new_description)s"
+msgstr "Fatura %(name)s renomeada a %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
-msgstr "Usuário %(name)s: a carga mudou de %(old_weight)s para %(new_weight)s"
+msgstr "Participante %(name)s: peso alterado de %(old_weight)s a %(new_weight)s"
+
+msgid "Payer"
+msgstr "Pagador"
 
 msgid "Amount"
 msgstr "Quantia"
 
+msgid "Date"
+msgstr "Data"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Quantia em %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Conta %(name)s modificada"
 
 #, python-format
 msgid "Participant %(name)s modified"
-msgstr "Usuário %(name)s modificado"
+msgstr "Participante %(name)s modificado"
 
 #, python-format
 msgid "Bill %(name)s removed"
-msgstr "Conta '%(name)s' foi removida"
+msgstr "Fatura %(name)s removida"
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Usuário '%(name)s' foi removido"
+msgstr "Participante %(name)s removido"
 
 #, python-format
 msgid "Project %(name)s changed in an unknown way"
 msgstr "Projeto %(name)s modificado de maneira desconhecida"
 
 #, python-format
 msgid "Bill %(name)s changed in an unknown way"
@@ -718,46 +724,46 @@
 msgid "Manage your shared <br />expenses, easily"
 msgstr "Modifique suas despesas <br />compartilhadas, facilmente"
 
 msgid "Try out the demo"
 msgstr "Experimente a demonstração"
 
 msgid "You're sharing a house?"
-msgstr "Você está dividindo uma casa?"
+msgstr "Está dividindo uma casa?"
 
 msgid "Going on holidays with friends?"
 msgstr "Indo para o feriado com os amigos?"
 
 msgid "Simply sharing money with others?"
 msgstr "Simplesmente compartilhando dinheiro com outras pessoas?"
 
 msgid "We can help!"
 msgstr "Nós podemos ajudar!"
 
 msgid "Log in to an existing project"
-msgstr "Conecte-se em um projeto existente"
+msgstr "Conecte-se num projeto existente"
 
 msgid "Log in"
 msgstr "Conecte-se"
 
 msgid "can't remember your password?"
-msgstr "não consegue se lembrar da sua senha?"
+msgstr "não se consegue lembrar da sua palavra-passe?"
 
 msgid "Create"
 msgstr "Criar"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
-"Não reutilize uma senha pessoal. Escolha um código privado e envie-o para"
-" seus amigos"
+"Não reutilize uma palavra-passe pessoal. Escolha um código privado e "
+"envie-o para seus amigos"
 
 msgid "Account manager"
-msgstr "Gerenciador de contas"
+msgstr "Gestor de contas"
 
 msgid "Bills"
 msgstr "Contas"
 
 msgid "Settle"
 msgstr "Estabelecer"
 
@@ -784,16 +790,17 @@
 
 msgid "switch to"
 msgstr "mudar para"
 
 msgid "Dashboard"
 msgstr "Painel de controle"
 
-msgid "Logout"
-msgstr "Sair"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Código"
 
 msgid "Mobile Application"
 msgstr "Aplicação Mobile"
 
@@ -806,156 +813,156 @@
 msgid "Legal information"
 msgstr "Informações legais"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" é um software livre"
 
 msgid "you can contribute and improve it!"
-msgstr "você pode contribuir para melhorá-lo!"
+msgstr "Pode contribuir para melhorá-lo!"
 
 #, python-format
 msgid "%(amount)s each"
 msgstr "%(amount)s cada"
 
 msgid "you sure?"
 msgstr "tem certeza?"
 
 msgid "Invite people"
 msgstr "Convidar pessoas"
 
-msgid "You should start by adding participants"
-msgstr "Você deveria começar adicionando pessoas"
-
-msgid "Add a new bill"
-msgstr "Adicionar uma nova conta"
-
 msgid "Newer bills"
 msgstr "Contas mais recentes"
 
 msgid "Older bills"
 msgstr "Contas mais antigas"
 
-msgid "When?"
-msgstr "Quando?"
+msgid "You should start by adding participants"
+msgstr "Deveria começar adicionando pessoas"
 
-msgid "Who paid?"
-msgstr "Quem pagou?"
+msgid "Add a new bill"
+msgstr "Adicionar uma nova fatura"
 
 msgid "For what?"
 msgstr "Para quê?"
 
-msgid "How much?"
-msgstr "Quanto?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Adicionado em %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Todos menos %(excluded)s"
 
+msgid "delete"
+msgstr "deletar"
+
 msgid "No bills"
-msgstr "Sem contas"
+msgstr "Sem faturas"
 
 msgid "Nothing to list yet."
 msgstr "Nada para listar ainda."
 
 msgid "You probably want to"
-msgstr "Você provavelmente gostaria de"
+msgstr "Provavelmente gostaria de"
 
 msgid "add a bill"
-msgstr "adicionar uma conta"
+msgstr "adicionar uma fatura"
 
 msgid "add participants"
 msgstr "adicionar participantes"
 
 msgid "Password reminder"
-msgstr "Lembrete de senha"
+msgstr "Lembrete de palavra-passe"
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
-"Um link para redefinir sua senha foi enviado a você, por favor verifique "
-"seus e-mails."
+"Uma ligação para redefinir a sua palavra-passe foi enviado a si, por "
+"favor verifique os seus e-mails."
 
 msgid "Return to home page"
 msgstr "Retornar à pagina inicial"
 
 msgid "Your projects"
 msgstr "Seus projetos"
 
 msgid "Reset your password"
-msgstr "Redefinir sua senha"
+msgstr "Redefinir sua palavra-passe"
 
 msgid "Invite people to join this project"
 msgstr "Convide pessoas para participar deste projeto"
 
 msgid "Share Identifier & code"
 msgstr "Compartilhar Identificador & código"
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
-"Você pode compartilhar o identificador do projeto e o código privado por "
+"Pode compartilhar o identificador do projeto e o código privado por "
 "qualquer meio de comunicação."
 
 msgid "Identifier:"
 msgstr "Identificador:"
 
 msgid "Share the Link"
-msgstr "Compartilhar o Link"
+msgstr "Compartilhar a ligação"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
-"Você pode compartilhar diretamente o seguinte link através do seu meio "
+"Pode compartilhar diretamente o seguinte ligação através do seu meio "
 "preferido"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Enviar via E-mails"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
-"Especifica uma lista de endereços de email (separados por vírgula) que "
-"você quer notificar acerca da\n"
-"                criação deste projeto de gestão de saldo e nós iremos "
-"enviar um email por si."
+"Especifique uma lista (separada por vírgulas) de endereços de e-mail que "
+"deseja notificar sobre a\n"
+"                criação deste projeto de gestão orçamental e enviaremos "
+"um e-mail para si."
 
 msgid "Who pays?"
 msgstr "Quem paga?"
 
 msgid "To whom?"
-msgstr "Para quem?"
+msgstr "A quem?"
 
 msgid "Who?"
 msgstr "Quem?"
 
 msgid "Balance"
 msgstr "Saldo"
 
 msgid "deactivate"
-msgstr "desativado"
+msgstr "desativar"
 
 msgid "reactivate"
 msgstr "reativar"
 
 msgid "Paid"
 msgstr "Pago"
 
 msgid "Spent"
 msgstr "Gasto"
 
 msgid "Expenses by Month"
-msgstr "Gastos por Mês"
+msgstr "Despesas por mês"
 
 msgid "Period"
 msgstr "Período"
 
 #~ msgid "Participant"
 #~ msgstr "Participante"
 
@@ -965,15 +972,15 @@
 #~ msgid "Select all"
 #~ msgstr "Selecionar tudo"
 
 #~ msgid "Select none"
 #~ msgstr "Selecionar nenhum"
 
 #~ msgid "changed"
-#~ msgstr "modificado"
+#~ msgstr "alterado"
 
 #~ msgid "from"
 #~ msgstr "de"
 
 #~ msgid "to"
 #~ msgstr "para"
 
@@ -1001,23 +1008,92 @@
 #~ msgid "reactivated"
 #~ msgstr "reativado"
 
 #~ msgid "renamed to"
 #~ msgstr "renomeado para"
 
 #~ msgid "External link changed to"
-#~ msgstr "Link externo alterado para"
+#~ msgstr "Ligação externa alterado para"
 
 #~ msgid "modified"
 #~ msgstr "modificado"
 
 #~ msgid "removed"
 #~ msgstr "removido"
 
 #~ msgid "You either provided a bad token or no project identifier."
-#~ msgstr "Você forneceu um token ruim ou não forneceu o identificador do projeto."
+#~ msgstr "Forneceu um token ruim ou não forneceu o identificador do projeto."
 
 #~ msgid "User name incorrect"
-#~ msgstr "Nome de usuário incorreto"
+#~ msgstr "Nome de utilizador incorreto"
 
 #~ msgid "People to notify"
 #~ msgstr "Pessoas para notificar"
+
+#~ msgid "Import"
+#~ msgstr "Importar"
+
+#~ msgid "Amount paid"
+#~ msgstr "Quantia paga"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Contas não podem ser null"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "O identificador do projeto é %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON inválido"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Tem certeza?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importar JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Este projeto tem o "
+#~ "histórico desativado. Novas ações não "
+#~ "serão exibidas abaixo. Pode ativar o "
+#~ "histórico na</i>\n"
+#~ "            <a href=\"%(url)s\">página de configurações</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>A tabela abaixo reflete "
+#~ "as ações registadas antes da desativação"
+#~ " do histórico do projeto. Pode\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">limpar o histórico "
+#~ "do projeto</a> para removê-las.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Enviar convites"
+
+#~ msgid " show"
+#~ msgstr "exibir"
+
+#~ msgid "Edit the project"
+#~ msgstr "Editar o projeto"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,51 +1,23 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Russian (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2023-05-07 23:52+0000\n"
+"Last-Translator: Egor Dubenetskiy <egor@banka.space>\n"
+"Language: ru\n"
 "Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/ru/>\n"
-"Language: ru\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.18-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>В таблице ниже отражены действия, записанные до отключения "
-"истории проекта. Вы можете\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">очистить историю проекта</a> to remove them.</i></"
-"p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>У этого проекта история отключена. Новые действия не появятся "
-"ниже. Вы можете включить историю в</i>\n"
-"            <a href=\"%(url)s\">настройках</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "«I hate money» — это бесплатная и свободная программа"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s с каждого"
 
@@ -169,17 +141,14 @@
 
 msgid "Bill items"
 msgstr "Пункты счета"
 
 msgid "Bills"
 msgstr "Счета"
 
-msgid "Bills can't be null"
-msgstr "Счета не могут быть нулевыми"
-
 msgid "Can't remember the password?"
 msgstr "Не помните пароль?"
 
 msgid "Cancel"
 msgstr "Отменить"
 
 msgid ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ru/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/ru/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2023-05-07 23:52+0000\n"
 "Last-Translator: Egor Dubenetskiy <egor@banka.space>\n"
-"Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/ru/>\n"
 "Language: ru\n"
+"Language-Team: Russian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/ru/>\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.18-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Вы только что создали '%(project)s' , чтобы разделить расходы"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Недопустимая сумма выражения. Принимаются только цифры и операторы + - * "
 "/ ."
 
@@ -42,28 +46,26 @@
 msgstr "Использовать отслеживание по IP для истории проекта"
 
 msgid "Default Currency"
 msgstr "Валюта по умолчанию"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"Установка валюты по умолчанию позволяет конвертировать валюту между счетами"
+"Установка валюты по умолчанию позволяет конвертировать валюту между "
+"счетами"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Для этого проекта нельзя установить режим «без валюты», так как он содержит "
-"счета в нескольких валютах."
-
-msgid "Import previously exported JSON file"
-msgstr "Импортировать ранее экспортированный JSON файл"
+"Для этого проекта нельзя установить режим «без валюты», так как он "
+"содержит счета в нескольких валютах."
 
-msgid "Import"
-msgstr "Импортировать"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Идентификатор проекта"
 
 msgid "Private code"
 msgstr "Приватный код"
 
@@ -116,25 +118,25 @@
 
 msgid "Password confirmation"
 msgstr "Подтвердите пароль"
 
 msgid "Reset password"
 msgstr "Восстановить пароль"
 
-msgid "Date"
-msgstr "Дата"
+msgid "When?"
+msgstr "Когда?"
 
 msgid "What?"
 msgstr "Что?"
 
-msgid "Payer"
-msgstr "Плательщик"
+msgid "Who paid?"
+msgstr "Кто заплатил?"
 
-msgid "Amount paid"
-msgstr "Уплаченная сумма"
+msgid "How much?"
+msgstr "Сколько?"
 
 msgid "Currency"
 msgstr "Валюта"
 
 msgid "External link"
 msgstr "Внешняя ссылка"
 
@@ -150,17 +152,14 @@
 msgid "Submit and add a new one"
 msgstr "Отправить и добавить новый"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "По умолчанию для проекта: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Счета не могут быть нулевыми"
-
 msgid "Name"
 msgstr "Имя"
 
 msgid "Weights should be positive"
 msgstr "Вес должен быть положительным"
 
 msgid "Weight"
@@ -174,21 +173,36 @@
 
 msgid "This project already have this participant"
 msgstr "В этом проекте уже есть такой участник"
 
 msgid "People to notify"
 msgstr "Кого уведомить"
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "Отправить приглашения"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Email %(email)s не правильный"
 
+msgid "Logout"
+msgstr "Выйти"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"К сожалению, при отправке электронных писем с приглашениями произошла "
+"ошибка. Пожалуйста, проверьте конфигурацию электронной почты сервера или "
+"свяжитесь с администратором."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} и {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, и {end_object}"
@@ -208,50 +222,43 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Слишком много неудачных попыток входа, попробуйте позже."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Этот пароль администратора неправильный. Осталось только %(num)d попыток."
 
 msgid "Provided token is invalid"
 msgstr "Предоставленный токен недействителен"
 
 msgid "This private code is not the right one"
 msgstr "Этот приватный код не подходит"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Вы только что создали '%(project)s' , чтобы разделить расходы"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Вам было отправлено электронное письмо с напоминанием"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Мы попытались отправить вам напоминание по электронной почте, но "
 "произошла ошибка. Вы по-прежнему можете использовать проект в обычном "
 "режиме."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Идентификатор проекта: %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "К сожалению, при отправке вам электронного письма с инструкциями по "
 "сбросу пароля произошла ошибка. Пожалуйста, проверьте конфигурацию "
 "электронной почты сервера или свяжитесь с администратором."
 
 msgid "No token provided"
 msgstr "Не предоставлен токен"
@@ -261,44 +268,49 @@
 
 msgid "Unknown project"
 msgstr "Неизвестный проект"
 
 msgid "Password successfully reset."
 msgstr "Пароль успешно восстановлен."
 
-msgid "Project successfully uploaded"
-msgstr "Проект успешно загружен"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Неправильный JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 "Невозможно добавить счета в нескольких валютах в проект без валюты по "
 "умолчанию"
 
+msgid "Project successfully uploaded"
+msgstr "Проект успешно загружен"
+
 msgid "Project successfully deleted"
 msgstr "Проект удалён"
 
 msgid "Error deleting project"
 msgstr "Ошибка при удалении проекта"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Вас пригласили разделить расходы в проект %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Ваш код приглашения был отправлен"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "К сожалению, при отправке электронных писем с приглашениями произошла "
 "ошибка. Пожалуйста, проверьте конфигурацию электронной почты сервера или "
 "свяжитесь с администратором."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -315,16 +327,16 @@
 msgstr "Ошибка при удалении участника"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Участник «%(name)s» был деактивирован. Он будет отображаться в списке до тех "
-"пор, пока его баланс не станет равным нулю."
+"Участник «%(name)s» был деактивирован. Он будет отображаться в списке до "
+"тех пор, пока его баланс не станет равным нулю."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "Участник «%(name)s» был удалён"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -338,14 +350,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Счёт был удалён"
 
 msgid "The bill has been modified"
 msgstr "Счёт был изменён"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Ошибка при удалении истории проекта"
 
 msgid "Deleted project history."
 msgstr "История проекта удалена."
 
 msgid "Error deleting recorded IP addresses"
@@ -398,44 +414,35 @@
 
 msgid "Actions"
 msgstr "Действия"
 
 msgid "edit"
 msgstr "изменить"
 
-msgid "delete"
-msgstr "удалить"
+msgid "Delete project"
+msgstr "Удалить проект"
 
 msgid "show"
 msgstr "показать"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Панель инструментов в данный момент отключена."
 
 msgid "Download Mobile Application"
 msgstr "Скачать мобильное приложение"
 
 msgid "Get it on"
 msgstr "Доступно в"
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "вы уверены?"
-
 msgid "Edit project"
 msgstr "Изменить проект"
 
-msgid "Delete project"
-msgstr "Удалить проект"
-
-msgid "Import JSON"
-msgstr "Импортировать JSON"
-
-msgid "Choose file"
-msgstr "Выбрать файл"
+#, fuzzy
+msgid "Import project"
+msgstr "Изменить проект"
 
 msgid "Download project's data"
 msgstr "Скачать данные проекта"
 
 msgid "Bill items"
 msgstr "Пункты счета"
 
@@ -455,26 +462,36 @@
 
 msgid "Cancel"
 msgstr "Отменить"
 
 msgid "Privacy Settings"
 msgstr "Настройки приватности"
 
-msgid "Edit the project"
-msgstr "Изменить проект"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "Все счета и участники этого проекта будут удалены!"
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Импортировать ранее экспортированный JSON файл"
+
+msgid "Choose file"
+msgstr "Выбрать файл"
+
 msgid "Edit this bill"
 msgstr "Изменить счёт"
 
 msgid "Add a bill"
 msgstr "Добавить счёт"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "За всех"
 
 msgid "No one"
 msgstr "Ни за кого"
 
 msgid "More options"
@@ -485,17 +502,14 @@
 
 msgid "Edit this participant"
 msgstr "Редактировать участника"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "Отправить приглашения"
-
 msgid "Download"
 msgstr "Скачать"
 
 msgid "Disabled Project History"
 msgstr "История отключенных проектов"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -515,15 +529,16 @@
 
 msgid "History Settings Changed"
 msgstr "Настройки истории изменены"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
 msgstr ""
-"Счёт %(name)s: Атрибут «%(property_name)s» изменён с %(before)s на %(after)s"
+"Счёт %(name)s: Атрибут «%(property_name)s» изменён с %(before)s на "
+"%(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
 msgstr "Счёт %(name)s: Атрибут «%(property_name)s» изменён на %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Подтвердите удаление IP-адресов"
@@ -554,74 +569,61 @@
 msgstr ""
 "Вы уверены, что хотите стереть историю проекта? Это действие нельзя "
 "отменить."
 
 #, python-format
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
-"Счёт %(name)s: Участник(и) %(owers_list_str)s добавлен(ы) в список должников"
+"Счёт %(name)s: Участник(и) %(owers_list_str)s добавлен(ы) в список "
+"должников"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
-"Счёт %(name)s: Участник(и) %(owers_list_str)s удален(ы) из списка должников"
+"Счёт %(name)s: Участник(и) %(owers_list_str)s удален(ы) из списка "
+"должников"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
 msgstr ""
-"\n"
-"            <i>У этого проекта история отключена. Новые действия не "
-"появятся ниже. Вы можете включить историю в</i>\n"
-"            <a href=\"%(url)s\">настройках</a>\n"
-"            "
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "Запись IP-адреса может быть включена на странице настроек"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
 msgstr ""
-"\n"
-"            <i>В таблице ниже отражены действия, записанные до отключения"
-" истории проекта. Вы можете\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">очистить историю проекта</a> to remove "
-"them.</i></p>\n"
-"            "
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Кто-то скорее всего стёр историю проекта."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Некоторые записи ниже содержат IP-адреса, хотя в этом проекте запись IP "
 "отключена. "
 
 msgid "Delete stored IP addresses"
 msgstr "Удалить сохраненные IP-адреса"
 
-msgid "No history to erase"
-msgstr "Нечего стирать"
-
-msgid "Clear Project History"
-msgstr "Стереть историю проекта"
-
 msgid "No IP Addresses to erase"
 msgstr "Нечего стирать"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Удалить сохраненные IP-адреса"
 
+msgid "No history to erase"
+msgstr "Нечего стирать"
+
+msgid "Clear Project History"
+msgstr "Стереть историю проекта"
+
 msgid "Time"
 msgstr "Время"
 
 msgid "Event"
 msgstr "Событие"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -675,17 +677,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Счёт %(name)s переименован в %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr "Участник %(name)s: масса изменена с %(old_weight)s на %(new_weight)s"
 
+msgid "Payer"
+msgstr "Плательщик"
+
 msgid "Amount"
 msgstr "Количество"
 
+msgid "Date"
+msgstr "Дата"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Количество в %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Счёт %(name)s изменён"
@@ -789,16 +797,17 @@
 
 msgid "switch to"
 msgstr "сменён на"
 
 msgid "Dashboard"
 msgstr "Панель инструментов"
 
-msgid "Logout"
-msgstr "Выйти"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Код"
 
 msgid "Mobile Application"
 msgstr "Мобильное приложение"
 
@@ -823,46 +832,40 @@
 
 msgid "you sure?"
 msgstr "вы уверены?"
 
 msgid "Invite people"
 msgstr "Пригласите людей"
 
-msgid "You should start by adding participants"
-msgstr "Вы должны начать с добавлением пользователей"
-
-msgid "Add a new bill"
-msgstr "Добавите новый счёт"
-
 msgid "Newer bills"
 msgstr "Новые счета"
 
 msgid "Older bills"
 msgstr "Старые счета"
 
-msgid "When?"
-msgstr "Когда?"
+msgid "You should start by adding participants"
+msgstr "Вы должны начать с добавлением пользователей"
 
-msgid "Who paid?"
-msgstr "Кто заплатил?"
+msgid "Add a new bill"
+msgstr "Добавите новый счёт"
 
 msgid "For what?"
 msgstr "За что?"
 
-msgid "How much?"
-msgstr "Сколько?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Добавлено %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "За всех, кроме %(excluded)s"
 
+msgid "delete"
+msgstr "удалить"
+
 msgid "No bills"
 msgstr "Нет счетов"
 
 msgid "Nothing to list yet."
 msgstr "Нечего перечислять еще."
 
 msgid "You probably want to"
@@ -909,14 +912,20 @@
 
 msgid "Share the Link"
 msgstr "Поделиться ссылкой"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Вы можете напрямую поделиться следующей ссылкой через любой способ связи"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Отправить по почте"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1040,7 +1049,76 @@
 #~ "либо не указали идентификатор проекта."
 
 #~ msgid "User name incorrect"
 #~ msgstr "Неправильное имя пользователя"
 
 #~ msgid "People to notify"
 #~ msgstr "Люди для уведомления"
+
+#~ msgid "Import"
+#~ msgstr "Импортировать"
+
+#~ msgid "Amount paid"
+#~ msgstr "Уплаченная сумма"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Счета не могут быть нулевыми"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Идентификатор проекта: %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Неправильный JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "вы уверены?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Импортировать JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>У этого проекта история "
+#~ "отключена. Новые действия не появятся "
+#~ "ниже. Вы можете включить историю в</i>"
+#~ "\n"
+#~ "            <a href=\"%(url)s\">настройках</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>В таблице ниже отражены "
+#~ "действия, записанные до отключения истории "
+#~ "проекта. Вы можете\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">очистить историю "
+#~ "проекта</a> to remove them.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Отправить приглашения"
+
+#~ msgid " show"
+#~ msgstr "показать"
+
+#~ msgid "Edit the project"
+#~ msgstr "Изменить проект"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/sr/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/vi/LC_MESSAGES/messages.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
-"PO-Revision-Date: 2021-04-09 13:26+0000\n"
-"Last-Translator: Rastko Sarcevic <ralesarcevic@gmail.com>\n"
-"Language: sr\n"
-"Language-Team: Serbian <https://hosted.weblate.org/projects/i-hate-"
-"money/i-hate-money/sr/>\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: Automatically generated\n"
+"Language: vi\n"
+"Language-Team: none\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr ""
@@ -27,39 +29,36 @@
 msgid "New private code"
 msgstr ""
 
 msgid "Enter a new code if you want to change it"
 msgstr ""
 
 msgid "Email"
-msgstr "Email"
+msgstr ""
 
 msgid "Enable project history"
 msgstr ""
 
 msgid "Use IP tracking for project history"
 msgstr ""
 
 msgid "Default Currency"
-msgstr "Podrazumevana Valuta"
+msgstr ""
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
+msgid "Compatible with Cospend"
 msgstr ""
 
-msgid "Import"
-msgstr "Uvezi"
-
 msgid "Project identifier"
 msgstr ""
 
 msgid "Private code"
 msgstr ""
 
 msgid "Create the project"
@@ -70,17 +69,16 @@
 "A project with this identifier (\"%(project)s\") already exists. Please "
 "choose a new identifier"
 msgstr ""
 
 msgid "Which is a real currency: Euro or Petro dollar?"
 msgstr ""
 
-#, fuzzy
 msgid "euro"
-msgstr "Period"
+msgstr ""
 
 msgid "Please, validate the captcha to proceed."
 msgstr ""
 
 msgid "Enter private code to confirm deletion"
 msgstr ""
 
@@ -90,99 +88,107 @@
 msgid "Invalid private code."
 msgstr ""
 
 msgid "Get in"
 msgstr ""
 
 msgid "Admin password"
-msgstr "Administratorska lozinka"
+msgstr ""
 
 msgid "Send me the code by email"
-msgstr "Pošalji mi kod putem email-a"
+msgstr ""
 
 msgid "This project does not exists"
 msgstr ""
 
 msgid "Password mismatch"
-msgstr "Lozinke se ne slažu"
+msgstr ""
 
 msgid "Password"
-msgstr "Lozinka"
+msgstr ""
 
 msgid "Password confirmation"
-msgstr "Potvrda lozinke"
+msgstr ""
 
 msgid "Reset password"
-msgstr "Resetuj lozinku"
+msgstr ""
 
-msgid "Date"
-msgstr "Datum"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr ""
 
-msgid "Payer"
+msgid "Who paid?"
 msgstr ""
 
-msgid "Amount paid"
-msgstr "Plaćeni iznos"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
-msgstr "Valuta"
+msgstr ""
 
 msgid "External link"
 msgstr ""
 
 msgid "A link to an external document, related to this bill"
 msgstr ""
 
 msgid "For whom?"
-msgstr "Za koga?"
+msgstr ""
 
 msgid "Submit"
-msgstr "Unesi"
+msgstr ""
 
 msgid "Submit and add a new one"
 msgstr ""
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr ""
 
-msgid "Bills can't be null"
-msgstr ""
-
 msgid "Name"
-msgstr "Ime"
+msgstr ""
 
 msgid "Weights should be positive"
-msgstr "Težine moraju biti pozitivne"
+msgstr ""
 
 msgid "Weight"
-msgstr "Težina"
+msgstr ""
 
 msgid "Add"
-msgstr "Dodaj"
+msgstr ""
 
-#, fuzzy
 msgid "The participant name is invalid"
-msgstr "Korisnik %(name)s je uklonjen"
+msgstr ""
 
 msgid "This project already have this participant"
 msgstr ""
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
-msgstr "Email %(email)s nije validan"
+msgstr ""
+
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
 
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
@@ -203,89 +209,84 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+msgid "Too many failed login attempts."
 msgstr ""
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
-msgstr "Lozinka uspešno resetovana."
+msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
 msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -300,33 +301,37 @@
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been removed"
-msgstr "Korisnik %(name)s je uklonjen"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant '%(name)s' has been modified"
-msgstr "Korisnik %(name)s je uklonjen"
+msgstr ""
 
 msgid "The bill has been added"
-msgstr "Račun je dodat"
+msgstr ""
 
 msgid "Error deleting bill"
 msgstr ""
 
 msgid "The bill has been deleted"
-msgstr "Račun je uklonjen"
+msgstr ""
 
 msgid "The bill has been modified"
-msgstr "Račun je izmenjen"
+msgstr ""
+
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
 
 msgid "Error deleting project history"
 msgstr ""
 
 msgid "Deleted project history."
 msgstr ""
 
@@ -339,126 +344,123 @@
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr ""
 
 msgid "The best thing to do is probably to get back to the main page."
 msgstr ""
 
 msgid "Back to the list"
-msgstr "Nazad na listu"
+msgstr ""
 
 msgid "Administration tasks are currently disabled."
 msgstr ""
 
-#, fuzzy
 msgid "Authentication"
-msgstr "Dokumentacija"
+msgstr ""
 
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr ""
 
 msgid "create it"
 msgstr ""
 
 msgid "?"
-msgstr "?"
+msgstr ""
 
 msgid "Create a new project"
 msgstr ""
 
 msgid "Project"
-msgstr "Projekat"
+msgstr ""
 
 msgid "Number of participants"
 msgstr ""
 
 msgid "Number of bills"
-msgstr "Broj računa"
+msgstr ""
 
 msgid "Newest bill"
-msgstr "Najnoviji račun"
+msgstr ""
 
 msgid "Oldest bill"
-msgstr "Najstariji račun"
+msgstr ""
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
-msgstr "izmeni"
+msgstr ""
 
-msgid "delete"
-msgstr "ukloni"
+msgid "Delete project"
+msgstr ""
 
 msgid "show"
-msgstr "prikaži"
+msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
-#, fuzzy
 msgid "Download Mobile Application"
-msgstr "Mobilna Aplikacija"
-
-msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
+msgid "Get it on"
 msgstr ""
 
 msgid "Edit project"
 msgstr ""
 
-#, fuzzy
-msgid "Delete project"
-msgstr "ukloni"
-
-msgid "Import JSON"
+msgid "Import project"
 msgstr ""
 
-msgid "Choose file"
-msgstr "Izaberi fajl"
-
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
-msgstr "Stavke računa"
+msgstr ""
 
 msgid "Download the list of bills with owner, amount, reason,... "
 msgstr ""
 
 msgid "Settle plans"
 msgstr ""
 
 msgid "Download the list of transactions needed to settle the current bills."
 msgstr ""
 
 msgid "Can't remember the password?"
 msgstr ""
 
 msgid "Cancel"
-msgstr "Otkaži"
+msgstr ""
 
 msgid "Privacy Settings"
-msgstr "Podešavanja Privatnosti"
+msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+msgid "Import previously exported project"
+msgstr ""
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
-msgstr "Izmeni ovaj račun"
+msgstr ""
 
 msgid "Add a bill"
-msgstr "Dodaj račun"
+msgstr ""
+
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
 
 msgid "Everyone"
-msgstr "Svi"
+msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
 msgstr ""
 
@@ -467,19 +469,16 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
-msgstr "Preuzmi"
+msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
 msgstr ""
 
@@ -534,75 +533,70 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
-msgstr "Vreme"
+msgstr ""
 
 msgid "Event"
-msgstr "Događaj"
+msgstr ""
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr ""
 
 msgid "IP address recording can be disabled on the settings page"
 msgstr ""
 
 msgid "From IP"
 msgstr ""
 
 #, python-format
 msgid "Project %(name)s added"
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s added"
-msgstr "Račun je dodat"
+msgstr ""
 
 #, python-format
 msgid "Participant %(name)s added"
 msgstr ""
 
 msgid "Project private code changed"
 msgstr ""
@@ -634,36 +628,42 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr ""
+
 msgid "Amount"
-msgstr "Iznos"
+msgstr ""
+
+msgid "Date"
+msgstr ""
 
 #, python-format
 msgid "Amount in %(currency)s"
-msgstr "Iznos u %(currency)s"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s modified"
-msgstr "Račun je izmenjen"
+msgstr ""
 
 #, python-format
 msgid "Participant %(name)s modified"
 msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Bill %(name)s removed"
-msgstr "Korisnik %(name)s je uklonjen"
+msgstr ""
 
-#, fuzzy, python-format
+#, python-format
 msgid "Participant %(name)s removed"
-msgstr "Korisnik %(name)s je uklonjen"
+msgstr ""
 
 #, python-format
 msgid "Project %(name)s changed in an unknown way"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s changed in an unknown way"
@@ -679,15 +679,15 @@
 msgid "Someone probably cleared the project history."
 msgstr ""
 
 msgid "Manage your shared <br />expenses, easily"
 msgstr ""
 
 msgid "Try out the demo"
-msgstr "Isprobaj demo verziju"
+msgstr ""
 
 msgid "You're sharing a house?"
 msgstr ""
 
 msgid "Going on holidays with friends?"
 msgstr ""
 
@@ -714,57 +714,58 @@
 "your friends"
 msgstr ""
 
 msgid "Account manager"
 msgstr ""
 
 msgid "Bills"
-msgstr "Računi"
+msgstr ""
 
 msgid "Settle"
 msgstr ""
 
 msgid "Statistics"
-msgstr "Statistika"
+msgstr ""
 
 msgid "Languages"
-msgstr "Jezici"
+msgstr ""
 
 msgid "Projects"
 msgstr ""
 
 msgid "Start a new project"
 msgstr ""
 
 msgid "History"
-msgstr "Istorija"
+msgstr ""
 
 msgid "Settings"
-msgstr "Podešavanja"
+msgstr ""
 
 msgid "Other projects :"
 msgstr ""
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
-msgstr "Kod"
+msgstr ""
 
 msgid "Mobile Application"
-msgstr "Mobilna Aplikacija"
+msgstr ""
 
 msgid "Documentation"
-msgstr "Dokumentacija"
+msgstr ""
 
 msgid "Administation Dashboard"
 msgstr ""
 
 msgid "Legal information"
 msgstr ""
 
@@ -772,53 +773,47 @@
 msgstr ""
 
 msgid "you can contribute and improve it!"
 msgstr ""
 
 #, python-format
 msgid "%(amount)s each"
-msgstr "%(amount)s svako"
+msgstr ""
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr "Dodaj novi račun"
-
 msgid "Newer bills"
-msgstr "Noviji računi"
+msgstr ""
 
 msgid "Older bills"
-msgstr "Stariji računi"
+msgstr ""
 
-msgid "When?"
-msgstr "Kada?"
+msgid "You should start by adding participants"
+msgstr ""
 
-msgid "Who paid?"
-msgstr "Ko je platio?"
+msgid "Add a new bill"
+msgstr ""
 
 msgid "For what?"
-msgstr "Za šta?"
-
-msgid "How much?"
-msgstr "Koliko?"
+msgstr ""
 
 #, python-format
 msgid "Added on %(date)s"
-msgstr "Dodato %(date)s"
+msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
-msgstr "Svi osim %(excluded)s"
+msgstr ""
+
+msgid "delete"
+msgstr ""
 
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
@@ -836,21 +831,21 @@
 
 msgid ""
 "A link to reset your password has been sent to you, please check your "
 "emails."
 msgstr ""
 
 msgid "Return to home page"
-msgstr "Vrati se na početnu stranu"
+msgstr ""
 
 msgid "Your projects"
 msgstr ""
 
 msgid "Reset your password"
-msgstr "Resetuj lozinku"
+msgstr ""
 
 msgid "Invite people to join this project"
 msgstr ""
 
 msgid "Share Identifier & code"
 msgstr ""
 
@@ -859,154 +854,132 @@
 "communication means."
 msgstr ""
 
 msgid "Identifier:"
 msgstr ""
 
 msgid "Share the Link"
-msgstr "Podelite link"
+msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
 
 msgid "Who pays?"
-msgstr "Ko plaća?"
+msgstr ""
 
 msgid "To whom?"
-msgstr "Kome?"
+msgstr ""
 
 msgid "Who?"
-msgstr "Ko?"
+msgstr ""
 
 msgid "Balance"
-msgstr "Stanje"
+msgstr ""
 
 msgid "deactivate"
 msgstr ""
 
 msgid "reactivate"
 msgstr ""
 
 msgid "Paid"
-msgstr "Plaćeno"
+msgstr ""
 
 msgid "Spent"
-msgstr "Potrošeno"
+msgstr ""
 
 msgid "Expenses by Month"
-msgstr "Mesečni troškovi"
+msgstr ""
 
 msgid "Period"
-msgstr "Period"
-
-#~ msgid "Participant"
-#~ msgstr "Učesnik"
-
-#~ msgid "Bill"
-#~ msgstr "Račun"
-
-#~ msgid "Select all"
-#~ msgstr "Izaberi sve"
-
-#~ msgid "Select none"
-#~ msgstr ""
-
-#~ msgid "changed"
-#~ msgstr ""
-
-#~ msgid "from"
-#~ msgstr ""
-
-#~ msgid "to"
-#~ msgstr ""
-
-#~ msgid "Confirm Delete"
-#~ msgstr ""
-
-#~ msgid "Added"
-#~ msgstr "Dodato"
-
-#~ msgid "Removed"
-#~ msgstr "Uklonjeno"
-
-#~ msgid "and"
-#~ msgstr "i"
-
-#~ msgid "owers list"
-#~ msgstr ""
-
-#~ msgid "added"
-#~ msgstr ""
+msgstr ""
 
-#~ msgid "Project renamed to"
+#~ msgid "Import previously exported JSON file"
 #~ msgstr ""
 
-#~ msgid "Project contact email changed to"
+#~ msgid "Import"
 #~ msgstr ""
 
-#~ msgid "deactivated"
+#~ msgid "Amount paid"
 #~ msgstr ""
 
-#~ msgid "reactivated"
+#~ msgid "Bills can't be null"
 #~ msgstr ""
 
-#~ msgid "renamed to"
+#~ msgid "Too many failed login attempts, please retry later."
 #~ msgstr ""
 
-#~ msgid "External link changed to"
+#~ msgid "The project identifier is %(project)s"
 #~ msgstr ""
 
-#~ msgid "modified"
-#~ msgstr "izmenjeno"
-
-#~ msgid "removed"
-#~ msgstr "uklonjeno"
-
-#~ msgid "changed in a unknown way"
-#~ msgstr ""
-
-#~ msgid "You either provided a bad token or no project identifier."
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
 #~ msgstr ""
 
-#~ msgid "User name incorrect"
+#~ msgid "Invalid JSON"
 #~ msgstr ""
 
-#~ msgid "This project already have this member"
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
 #~ msgstr ""
 
-#~ msgid "People to notify"
+#~ msgid "Are you sure?"
 #~ msgstr ""
 
-#~ msgid "Error activating member"
+#~ msgid "Import JSON"
 #~ msgstr ""
 
-#~ msgid "Error removing member"
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
 #~ msgstr ""
 
 #~ msgid ""
-#~ "User '%(name)s' has been deactivated. It"
-#~ " will still appear in the users "
-#~ "list until its balance becomes zero."
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
 #~ msgstr ""
 
-#~ msgid "User '%(name)s' has been edited"
+#~ msgid "Send invites"
 #~ msgstr ""
 
-#~ msgid "Number of members"
-#~ msgstr "Broj korisnika"
-
-#~ msgid "Edit this member"
+#~ msgid " show"
 #~ msgstr ""
 
-#~ msgid "Participants to notify"
+#~ msgid "Edit the project"
 #~ msgstr ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Swedish (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2023-02-07 21:51+0000\n"
+"Last-Translator: Kristoffer Grundström <swedishsailfishosuser@tutanota.com>\n"
+"Language: sv\n"
 "Language-Team: Swedish <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/sv/>\n"
-"Language: sv\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"Jag hatar pengar\" är en fri mjukvara"
 
 msgid "%(amount)s each"
 msgstr "%(amount)s var"
 
@@ -126,17 +127,14 @@
 
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Faktura %(name)s: tog bort %(owers_list_str)s från ägarlistan"
 
 msgid "Bills"
 msgstr "Räkningar"
 
-msgid "Bills can't be null"
-msgstr "Räkningar kan inte vara null"
-
 msgid "Can't remember the password?"
 msgstr "Kan du inte komma ihåg lösenordet?"
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/sv/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/sv/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2023-02-07 21:51+0000\n"
-"Last-Translator: Kristoffer Grundström <swedishsailfishosuser@tutanota.com>\n"
-"Language-Team: Swedish <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/sv/>\n"
+"Last-Translator: Kristoffer Grundström "
+"<swedishsailfishosuser@tutanota.com>\n"
 "Language: sv\n"
+"Language-Team: Swedish <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/sv/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Du har just skapat '%(project)s' för att dela ut dina kostnader"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Inte en giltig summa eller uttryck. Endast nummer och +-* /-operatörer "
 "accepteras."
 
@@ -46,22 +51,19 @@
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Det här projektet kan inte ställas in till 'ingen valuta' eftersom att det "
-"innehåller sedlar i flera olika valutor."
+"Det här projektet kan inte ställas in till 'ingen valuta' eftersom att "
+"det innehåller sedlar i flera olika valutor."
 
-msgid "Import previously exported JSON file"
-msgstr "Importera tidigare exporterad JSON-fil"
-
-msgid "Import"
-msgstr "Importera"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Projektidentifierare"
 
 msgid "Private code"
 msgstr "Privat kod"
 
@@ -114,25 +116,25 @@
 
 msgid "Password confirmation"
 msgstr "Lösenordsbekräftelse"
 
 msgid "Reset password"
 msgstr "Återställ lösenord"
 
-msgid "Date"
-msgstr "Datum"
+msgid "When?"
+msgstr "När?"
 
 msgid "What?"
 msgstr "Vad?"
 
-msgid "Payer"
-msgstr "Betalare"
+msgid "Who paid?"
+msgstr "Vem betalade?"
 
-msgid "Amount paid"
-msgstr "Betald summa"
+msgid "How much?"
+msgstr "Hur mycket?"
 
 msgid "Currency"
 msgstr "Valuta"
 
 msgid "External link"
 msgstr "Extern länk"
 
@@ -148,17 +150,14 @@
 msgid "Submit and add a new one"
 msgstr "Skicka in och lägg till en ny"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Standard för projektet: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Räkningar kan inte vara null"
-
 msgid "Name"
 msgstr "Namn"
 
 msgid "Weights should be positive"
 msgstr "Vikter borde vara positiva"
 
 msgid "Weight"
@@ -172,21 +171,36 @@
 
 msgid "This project already have this participant"
 msgstr "Det här projektet har redan den här deltagaren"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "Skicka inbjudningar"
+msgid "Send the invitations"
+msgstr "Skicka inbjudningarna"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "E-postadressen %(email)s är inte korrekt"
 
+msgid "Logout"
+msgstr "Logga ut"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Ursäkta! Det uppstod ett fel när e-post med instruktioner för att "
+"återställa ditt lösenord skulle skickas. Vänligen kontrollera serverns "
+"e-post konfiguration eller ta kontakt med administratör."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} och {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, och {end_object}"
@@ -206,98 +220,95 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "För många misslyckade inloggningsförsök, försök igen senare."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "Det här lösenordet för admin är inte det rätta. Endast %(num)d försök "
 "kvar."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "Den här privata koden är inte den rätta"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Du har just skapat '%(project)s' för att dela ut dina kostnader"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Ett e-postmeddelande med påminnelse har just skickats till dig"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Vi försökte skicka en påminnelse till din e-postadress, men det uppstod "
 "ett fel. Du kan fortfarande använda det här projektet normalt."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Projektets id är %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
-"Ursäkta! Det uppstod ett fel när e-post med instruktioner för att återställa "
-"ditt lösenord skulle skickas. Vänligen kontrollera serverns e-post "
-"konfiguration eller ta kontakt med administratör."
+"Ursäkta! Det uppstod ett fel när e-post med instruktioner för att "
+"återställa ditt lösenord skulle skickas. Vänligen kontrollera serverns "
+"e-post konfiguration eller ta kontakt med administratör."
 
 msgid "No token provided"
 msgstr "Ingen symbol tillhandahölls"
 
 msgid "Invalid token"
 msgstr "Ogiltig symbol"
 
 msgid "Unknown project"
 msgstr "Okänt projekt"
 
 msgid "Password successfully reset."
 msgstr "Återställningen av lösenordet lyckades."
 
-msgid "Project successfully uploaded"
-msgstr "Uppladdningen av projektet lyckades"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Ogiltig JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 "Kan inte lägga till sedlar i flera olika valutor till ett projekt utan "
 "standard-valuta"
 
+msgid "Project successfully uploaded"
+msgstr "Uppladdningen av projektet lyckades"
+
 msgid "Project successfully deleted"
 msgstr "Borttagningen av projektet lyckades"
 
 msgid "Error deleting project"
 msgstr "Fel uppstod när projektet skulle tas bort"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Du har bjudits in att dela ut dina kostnader för %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Dina inbjudningar har skickats"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s har lagts till"
 
 msgid "Error activating participant"
@@ -311,16 +322,16 @@
 msgstr "Fel uppstod när deltagaren skulle tas bort"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"Deltagaren '%(name)s' har inaktiverats. Den kommer fortfarande att synas i "
-"listan till dess att kontot blir tomt."
+"Deltagaren '%(name)s' har inaktiverats. Den kommer fortfarande att synas "
+"i listan till dess att kontot blir tomt."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "Deltagaren '%(name)s' togs bort"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -334,14 +345,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Räkningen har tagits bort"
 
 msgid "The bill has been modified"
 msgstr "Räkningen har blivit modifierad"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Fel uppstod när projektets historik skulle tas bort"
 
 msgid "Deleted project history."
 msgstr "Projektets historik togs bort."
 
 msgid "Error deleting recorded IP addresses"
@@ -394,44 +409,35 @@
 
 msgid "Actions"
 msgstr "Åtgärder"
 
 msgid "edit"
 msgstr "redigera"
 
-msgid "delete"
-msgstr "ta bort"
+msgid "Delete project"
+msgstr "Ta bort projektet"
 
 msgid "show"
 msgstr "visa"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Instrumentpanelen är för närvarande inaktiverad."
 
 msgid "Download Mobile Application"
 msgstr "Hämta mobilapplikation"
 
 msgid "Get it on"
 msgstr ""
 
-#, fuzzy
-msgid "Are you sure?"
-msgstr "säker?"
-
 msgid "Edit project"
 msgstr "Redigera projekt"
 
-msgid "Delete project"
-msgstr "Ta bort projektet"
-
-msgid "Import JSON"
-msgstr "Importera JSON"
-
-msgid "Choose file"
-msgstr "Välj fil"
+#, fuzzy
+msgid "Import project"
+msgstr "Redigera projekt"
 
 msgid "Download project's data"
 msgstr "Ladda ner projektets data"
 
 msgid "Bill items"
 msgstr ""
 
@@ -449,27 +455,38 @@
 
 msgid "Cancel"
 msgstr "Avbryt"
 
 msgid "Privacy Settings"
 msgstr "Inställningar för privatliv"
 
-msgid "Edit the project"
-msgstr "Redigera projektet"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
-"Det här kommer att ta bort alla fakturor och deltagare i det här projektet!"
+"Det här kommer att ta bort alla fakturor och deltagare i det här "
+"projektet!"
+
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Importera tidigare exporterad JSON-fil"
+
+msgid "Choose file"
+msgstr "Välj fil"
 
 msgid "Edit this bill"
 msgstr "Redigera den här räkningen"
 
 msgid "Add a bill"
 msgstr "Lägg till en räkning"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Alla"
 
 msgid "No one"
 msgstr "Ingen"
 
 msgid "More options"
@@ -480,17 +497,14 @@
 
 msgid "Edit this participant"
 msgstr "Redigera den här deltagaren"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@exempel.com, mary.moe@sida.com"
 
-msgid "Send the invitations"
-msgstr "Skicka inbjudningarna"
-
 msgid "Download"
 msgstr "Ladda ner"
 
 msgid "Disabled Project History"
 msgstr "Inaktiverade projekthistorik"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -510,15 +524,16 @@
 
 msgid "History Settings Changed"
 msgstr "Inställningarna för historiken har ändrats"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed from %(before)s to %(after)s"
 msgstr ""
-"Faktura %(name)s: %(property_name)s ändrades från %(before)s till %(after)s"
+"Faktura %(name)s: %(property_name)s ändrades från %(before)s till "
+"%(after)s"
 
 #, python-format
 msgid "Bill %(name)s: %(property_name)s changed to %(after)s"
 msgstr "Faktura %(name)s: %(property_name)s ändrades till %(after)s"
 
 msgid "Confirm Remove IP Adresses"
 msgstr "Bekräfta borttagning av IP-adresser"
@@ -550,55 +565,51 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Faktura %(name)s: lade till %(owers_list_str)s i ägarlistan"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Faktura %(name)s: tog bort %(owers_list_str)s från ägarlistan"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
 msgstr ""
 
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "Insamling av IP-adresser kan inaktiveras på Inställningar-sidan"
+
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Några poster här nedan innehåller IP-adresser, fastän det här projektet "
 "har IP-inspelning inaktiverat. "
 
 msgid "Delete stored IP addresses"
 msgstr "Ta bort lagrade IP-adresser"
 
-msgid "No history to erase"
-msgstr "Ingen historik att ta bort"
-
-msgid "Clear Project History"
-msgstr "Rensa projektets historik"
-
 msgid "No IP Addresses to erase"
 msgstr "Inga IP-adresser att ta bort"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Ta bort de lagrade IP-adresserna"
 
+msgid "No history to erase"
+msgstr "Ingen historik att ta bort"
+
+msgid "Clear Project History"
+msgstr "Rensa projektets historik"
+
 msgid "Time"
 msgstr "Tid"
 
 msgid "Event"
 msgstr "Händelse"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -627,16 +638,15 @@
 
 #, python-format
 msgid "Project renamed to %(new_project_name)s"
 msgstr "Projektet döptes om till %(new_project_name)s"
 
 #, python-format
 msgid "Project contact email changed to %(new_email)s"
-msgstr ""
-"Kontaktens e-postadress för det här projektet ändrades till %(new_email)s"
+msgstr "Kontaktens e-postadress för det här projektet ändrades till %(new_email)s"
 
 msgid "Project settings modified"
 msgstr "Projektets inställningar ändrades"
 
 #, python-format
 msgid "Participant %(name)s deactivated"
 msgstr "Projektet %(name)s inaktiverades"
@@ -652,19 +662,26 @@
 #, python-format
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "Faktura %(name)s döptes om till %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
-"Deltagaren %(name)s: vikten ändrades från %(old_weight)s till %(new_weight)s"
+"Deltagaren %(name)s: vikten ändrades från %(old_weight)s till "
+"%(new_weight)s"
+
+msgid "Payer"
+msgstr "Betalare"
 
 msgid "Amount"
 msgstr "Summa"
 
+msgid "Date"
+msgstr "Datum"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "Summa i %(currency)s"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "Fakturan %(name)s ändrades"
@@ -729,16 +746,16 @@
 msgid "Create"
 msgstr "Skapa"
 
 msgid ""
 "Don\\'t reuse a personal password. Choose a private code and send it to "
 "your friends"
 msgstr ""
-"Återanvänd INTE ett personligt lösenord. Välj en privat kod och skicka den "
-"till dina vänner"
+"Återanvänd INTE ett personligt lösenord. Välj en privat kod och skicka "
+"den till dina vänner"
 
 msgid "Account manager"
 msgstr "Kontoansvarig"
 
 msgid "Bills"
 msgstr "Räkningar"
 
@@ -768,16 +785,17 @@
 
 msgid "switch to"
 msgstr "byt till"
 
 msgid "Dashboard"
 msgstr "Instrumentpanel"
 
-msgid "Logout"
-msgstr "Logga ut"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Kod"
 
 msgid "Mobile Application"
 msgstr "Mobilapplikation"
 
@@ -802,46 +820,40 @@
 
 msgid "you sure?"
 msgstr "säker?"
 
 msgid "Invite people"
 msgstr "Bjud in personer"
 
-msgid "You should start by adding participants"
-msgstr "Du borde börja med att lägga till deltagare"
-
-msgid "Add a new bill"
-msgstr "Lägg till en ny räkning"
-
 msgid "Newer bills"
 msgstr "Nyare räkningar"
 
 msgid "Older bills"
 msgstr "Äldre räkningar"
 
-msgid "When?"
-msgstr "När?"
+msgid "You should start by adding participants"
+msgstr "Du borde börja med att lägga till deltagare"
 
-msgid "Who paid?"
-msgstr "Vem betalade?"
+msgid "Add a new bill"
+msgstr "Lägg till en ny räkning"
 
 msgid "For what?"
 msgstr "För vad?"
 
-msgid "How much?"
-msgstr "Hur mycket?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "Lades till %(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "Alla förutom %(excluded)s"
 
+msgid "delete"
+msgstr "ta bort"
+
 msgid "No bills"
 msgstr "Inga räkningar"
 
 msgid "Nothing to list yet."
 msgstr "Ingenting att lista än."
 
 msgid "You probably want to"
@@ -878,39 +890,45 @@
 msgid "Share Identifier & code"
 msgstr "Dela ut identifierare & kod"
 
 msgid ""
 "You can share the project identifier and the private code by any "
 "communication means."
 msgstr ""
-"Du kan dela projektets identifierare och den privata koden så som det passar "
-"dig."
+"Du kan dela projektets identifierare och den privata koden så som det "
+"passar dig."
 
 msgid "Identifier:"
 msgstr "Identifierare:"
 
 msgid "Share the Link"
 msgstr "Dela ut länken"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "Du kan direkt dela ut följande länk via föredraget media"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "Skicka via e-post"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
 "send them an email for you."
 msgstr ""
-"Ange en (delat med ett kommatecken)  lista över e-postadresser som du vill "
-"underrätta om\n"
-"                skapandet av det här budgethanteringsprojektet gör att de "
-"kommer att få ett e-postmeddelande om det."
+"Ange en (delat med ett kommatecken)  lista över e-postadresser som du "
+"vill underrätta om\n"
+"                skapandet av det här budgethanteringsprojektet gör att de"
+" kommer att få ett e-postmeddelande om det."
 
 msgid "Who pays?"
 msgstr "Vem betalar?"
 
 msgid "To whom?"
 msgstr "Till vem?"
 
@@ -999,7 +1017,68 @@
 #~ msgstr ""
 
 #~ msgid "User name incorrect"
 #~ msgstr "Användarnamnet felaktigt"
 
 #~ msgid "People to notify"
 #~ msgstr "Personer att meddela"
+
+#~ msgid "Import"
+#~ msgstr "Importera"
+
+#~ msgid "Amount paid"
+#~ msgstr "Betald summa"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Räkningar kan inte vara null"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Projektets id är %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Ogiltig JSON"
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr "säker?"
+
+#~ msgid "Import JSON"
+#~ msgstr "Importera JSON"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Skicka inbjudningar"
+
+#~ msgid " show"
+#~ msgstr "visa"
+
+#~ msgid "Edit the project"
+#~ msgstr "Redigera projektet"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,22 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2020-07-01 18:41+0000\n"
 "Last-Translator: rohitn01 <rohitmen01@gmail.com>\n"
 "Language: ta\n"
 "Language-Team: Tamil <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/ta/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s இணைக்கப்பட்டு விட்டது"
 
 msgid "A link to an external document, related to this bill"
 msgstr "இந்த மசோதா தொடர்பான வெளிப்புற ஆவணத்திற்கான இணைப்பு"
 
@@ -32,20 +32,14 @@
 
 msgid "Add"
 msgstr "கூட்டு"
 
 msgid "Admin password"
 msgstr "நிர்வாகி கடவுச்சொல்"
 
-msgid "Amount paid"
-msgstr "பணம் செலுத்தப்பட்டது"
-
-msgid "Bills can't be null"
-msgstr "பில்கள் பூஜ்யமாக இருக்க முடியாது"
-
 msgid "Create the project"
 msgstr "திட்டத்தை உருவாக்கவும்"
 
 msgid "Currency"
 msgstr "நாணய"
 
 msgid "Date"
@@ -65,23 +59,14 @@
 
 msgid "For whom?"
 msgstr "யாருக்காக?"
 
 msgid "Get in"
 msgstr "உள்ளே வா"
 
-msgid "Import"
-msgstr "இறக்குமதி"
-
-msgid "Import previously exported JSON file"
-msgstr "முன்னர் ஏற்றுமதி செய்யப்பட்ட JSON கோப்பை இறக்குமதி செய்க"
-
-msgid "Invalid JSON"
-msgstr "தவறான JSON"
-
 msgid "Invalid token"
 msgstr "செல்லுபடியாகாத டோக்கன்"
 
 msgid "Name"
 msgstr "பெயர்"
 
 msgid "No Currency"
@@ -138,54 +123,32 @@
 
 msgid "Send invites"
 msgstr "அழைப்புகளை அனுப்பு"
 
 msgid "Send me the code by email"
 msgstr "மின்னஞ்சல் மூலம் குறியீட்டை எனக்கு அனுப்புங்கள்"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"மன்னிக்கவும், கடவுச்சொல் மீட்டமைப்பு வழிமுறைகளுடன் உங்களுக்கு மின்னஞ்சல் அனுப்பும்போது பிழை "
-"ஏற்பட்டது. சேவையகத்தின் மின்னஞ்சல் உள்ளமைவை சரிபார்க்கவும் அல்லது நிர்வாகியைத் தொடர்பு "
-"கொள்ளவும்."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"மன்னிக்கவும், அழைப்பிதழ் மின்னஞ்சல்களை அனுப்ப முயற்சிக்கும்போது பிழை ஏற்பட்டது. சேவையகத்தின் "
-"மின்னஞ்சல் உள்ளமைவை சரிபார்க்கவும் அல்லது நிர்வாகியைத் தொடர்பு கொள்ளவும்."
-
 msgid "Submit"
 msgstr "சமர்ப்பிக்கவும்"
 
 msgid "Submit and add a new one"
 msgstr "சமர்ப்பித்து புதிய ஒன்றைச் சேர்க்கவும்"
 
 msgid "The email %(email)s is not valid"
 msgstr "மின்னஞ்சல் %(email)s செல்லுபடியாகாது"
 
-msgid "The project identifier is %(project)s"
-msgstr "திட்ட அடையாளங்காட்டி %(project)s"
-
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "இந்த நிர்வாகி கடவுச்சொல் சரியானது அல்ல. மட்டும் %(num)d முயற்சிகள் எஞ்சியுள்ளன."
 
 msgid "This private code is not the right one"
 msgstr "இந்த தனிப்பட்ட குறியீடு சரியானது அல்ல"
 
 msgid "This project does not exists"
 msgstr "இந்த திட்டம் இல்லை"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "உள்நுழைவு முயற்சிகள் பல தோல்வியுற்றன, பின்னர் மீண்டும் முயற்சிக்கவும்."
-
 msgid "Unknown project"
 msgstr "தெரியாத திட்டம்"
 
 msgid "Use IP tracking for project history"
 msgstr "திட்ட வரலாற்றுக்கு ஐபி கண்காணிப்பைப் பயன்படுத்தவும்"
 
 msgid ""
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ta/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/ta/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2020-07-01 18:41+0000\n"
 "Last-Translator: rohitn01 <rohitmen01@gmail.com>\n"
 "Language: ta\n"
 "Language-Team: Tamil <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/ta/>\n"
 "Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+"நீங்கள் இப்போது உருவாக்கியுள்ளீர்கள் '%(project)s' உங்கள் செலவுகளை "
+"பகிர்ந்து கொள்ள"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "சரியான அளவு அல்லது வெளிப்பாடு அல்ல. எண்கள் மற்றும் + - * / ஆபரேட்டர்கள் "
 "ஏற்றுக்கொள்ளப்படுகிறார்கள்."
 
@@ -48,19 +54,16 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
-msgstr "முன்னர் ஏற்றுமதி செய்யப்பட்ட JSON கோப்பை இறக்குமதி செய்க"
-
-msgid "Import"
-msgstr "இறக்குமதி"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "திட்ட அடையாளங்காட்டி"
 
 msgid "Private code"
 msgstr "தனியார் குறியீடு"
 
@@ -115,25 +118,25 @@
 
 msgid "Password confirmation"
 msgstr "கடவுச்சொல் உறுதிப்படுத்தல்"
 
 msgid "Reset password"
 msgstr "கடவுச்சொல்லை மீட்டமைக்க"
 
-msgid "Date"
-msgstr "தேதி"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "என்ன?"
 
-msgid "Payer"
-msgstr "செலுத்துவோர்"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "பணம் செலுத்தப்பட்டது"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "நாணய"
 
 msgid "External link"
 msgstr "வெளிப்புற இணைப்பு"
 
@@ -149,17 +152,14 @@
 msgid "Submit and add a new one"
 msgstr "சமர்ப்பித்து புதிய ஒன்றைச் சேர்க்கவும்"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "திட்ட இயல்புநிலை: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "பில்கள் பூஜ்யமாக இருக்க முடியாது"
-
 msgid "Name"
 msgstr "பெயர்"
 
 msgid "Weights should be positive"
 msgstr "எடைகள் நேர்மறையாக இருக்க வேண்டும்"
 
 msgid "Weight"
@@ -174,21 +174,36 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "இந்த திட்டத்தில் ஏற்கனவே இந்த உறுப்பினர் இருக்கிறார்"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "அழைப்புகளை அனுப்பு"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "மின்னஞ்சல் %(email)s செல்லுபடியாகாது"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"மன்னிக்கவும், அழைப்பிதழ் மின்னஞ்சல்களை அனுப்ப முயற்சிக்கும்போது பிழை "
+"ஏற்பட்டது. சேவையகத்தின் மின்னஞ்சல் உள்ளமைவை சரிபார்க்கவும் அல்லது "
+"நிர்வாகியைத் தொடர்பு கொள்ளவும்."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -208,53 +223,44 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "உள்நுழைவு முயற்சிகள் பல தோல்வியுற்றன, பின்னர் மீண்டும் முயற்சிக்கவும்."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
 "இந்த நிர்வாகி கடவுச்சொல் சரியானது அல்ல. மட்டும் %(num)d முயற்சிகள் "
 "எஞ்சியுள்ளன."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "இந்த தனிப்பட்ட குறியீடு சரியானது அல்ல"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-"நீங்கள் இப்போது உருவாக்கியுள்ளீர்கள் '%(project)s' உங்கள் செலவுகளை "
-"பகிர்ந்து கொள்ள"
-
 msgid "A reminder email has just been sent to you"
 msgstr "ஒரு நினைவூட்டல் மின்னஞ்சல் உங்களுக்கு அனுப்பப்பட்டுள்ளது"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "உங்களுக்கு நினைவூட்டல் மின்னஞ்சலை அனுப்ப முயற்சித்தோம், ஆனால் பிழை "
 "ஏற்பட்டது. நீங்கள் இன்னும் திட்டத்தை சாதாரணமாக பயன்படுத்தலாம்."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "திட்ட அடையாளங்காட்டி %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "மன்னிக்கவும், கடவுச்சொல் மீட்டமைப்பு வழிமுறைகளுடன் உங்களுக்கு மின்னஞ்சல் "
 "அனுப்பும்போது பிழை ஏற்பட்டது. சேவையகத்தின் மின்னஞ்சல் உள்ளமைவை "
 "சரிபார்க்கவும் அல்லது நிர்வாகியைத் தொடர்பு கொள்ளவும்."
 
 msgid "No token provided"
 msgstr "டோக்கன் வழங்கப்படவில்லை"
@@ -264,42 +270,47 @@
 
 msgid "Unknown project"
 msgstr "தெரியாத திட்டம்"
 
 msgid "Password successfully reset."
 msgstr "கடவுச்சொல் வெற்றிகரமாக மீட்டமைக்கப்படுகிறது."
 
-msgid "Project successfully uploaded"
-msgstr "திட்டம் வெற்றிகரமாக பதிவேற்றப்பட்டது"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "தவறான JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "திட்டம் வெற்றிகரமாக பதிவேற்றப்பட்டது"
+
 msgid "Project successfully deleted"
 msgstr "திட்டம் வெற்றிகரமாக நீக்கப்பட்டது"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "உங்கள் செலவுகளை பகிர்ந்து கொள்ள அழைக்கப்பட்டுள்ளீர்கள் %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "உங்கள் அழைப்புகள் அனுப்பப்பட்டுள்ளன"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "மன்னிக்கவும், அழைப்பிதழ் மின்னஞ்சல்களை அனுப்ப முயற்சிக்கும்போது பிழை "
 "ஏற்பட்டது. சேவையகத்தின் மின்னஞ்சல் உள்ளமைவை சரிபார்க்கவும் அல்லது "
 "நிர்வாகியைத் தொடர்பு கொள்ளவும்."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -337,14 +348,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "திட்ட வரலாற்றை இயக்கு"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "திட்ட வரலாற்றை இயக்கு"
@@ -399,46 +414,38 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
-msgstr ""
+#, fuzzy
+msgid "Delete project"
+msgstr "திட்டத்தை உருவாக்கவும்"
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 #, fuzzy
 msgid "Get it on"
 msgstr "உள்ளே வா"
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "திட்டத்தை உருவாக்கவும்"
 
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
-
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -455,26 +462,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "முன்னர் ஏற்றுமதி செய்யப்பட்ட JSON கோப்பை இறக்குமதி செய்க"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -485,17 +502,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -552,51 +566,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -652,17 +661,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "செலுத்துவோர்"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "தேதி"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -764,15 +779,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -798,46 +814,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -882,14 +892,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1025,7 +1041,60 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "இறக்குமதி"
+
+#~ msgid "Amount paid"
+#~ msgstr "பணம் செலுத்தப்பட்டது"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "பில்கள் பூஜ்யமாக இருக்க முடியாது"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "திட்ட அடையாளங்காட்டி %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "தவறான JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "அழைப்புகளை அனுப்பு"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Telugu (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-10-04 14:19+0000\n"
+"Last-Translator: Sharan J <sharanjs1999@gmail.com>\n"
+"Language: te\n"
 "Language-Team: Telugu <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/te/>\n"
-"Language: te\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s కలపబడ్డారు"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s మళ్ళీ ఈ ప్రాజెక్ట్ లో కలపబడ్డారు"
 
@@ -24,20 +25,14 @@
 
 msgid "A reminder email has just been sent to you"
 msgstr "మీకు ఇప్పుడే రిమైండర్ ఇమెయిల్ పంపబడింది"
 
 msgid "Add"
 msgstr "కూడు"
 
-msgid "Amount paid"
-msgstr "చెల్లించిన మొత్తం"
-
-msgid "Bills can't be null"
-msgstr "బిల్లులు శూన్యం కాకూడదు"
-
 msgid ""
 "Cannot add bills in multiple currencies to a project without default currency"
 msgstr "డిఫాల్ట్ కరెన్సీ లేకుండా ప్రాజెక్ట్‌కు బహుళ కరెన్సీలలో బిల్లులను జోడించలేరు"
 
 msgid "Create the project"
 msgstr "ప్రాజెక్ట్ ని సృష్టించు"
 
@@ -73,23 +68,14 @@
 
 msgid "For whom?"
 msgstr "ఎవరి కోసం?"
 
 msgid "Get in"
 msgstr "లోపలి వేళ్ళు"
 
-msgid "Import"
-msgstr "దిగుమతి చెయ్యి"
-
-msgid "Import previously exported JSON file"
-msgstr "గతంలో ఎగుమతి చేసిన JSON ఫైల్‌ని దిగుమతి చేయి"
-
-msgid "Invalid JSON"
-msgstr "చెల్లని JSON"
-
 msgid "Invalid private code."
 msgstr "ప్రైవేట్ కోడ్ తప్పు."
 
 msgid "Invalid token"
 msgstr "చెల్లని టోకెన్"
 
 msgid "Name"
@@ -148,41 +134,23 @@
 
 msgid "Send me the code by email"
 msgstr "నాకు ఇమెయిల్ ద్వారా కోడ్ ని పంపు"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "డిఫాల్ట్ కరెన్సీని సెట్ చేయడం వలన బిల్లుల మధ్య కరెన్సీ మార్పిడిని కుదురుతుంది"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"క్షమించండి, పాస్‌వర్డ్ రీసెట్ సూచనలతో కూడిన ఇమెయిల్‌ను మీకు పంపుతున్నప్పుడు ఎర్రర్ వొచింది. దయచేసి సర్వర్ "
-"యొక్క ఇమెయిల్ కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా నిర్వాహకుడిని సంప్రదించండి."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"క్షమించండి, ఆహ్వాన ఇమెయిల్‌లను పంపడానికి ప్రయత్నిస్తున్నప్పుడు ఎర్రర్ వొచింది . దయచేసి సర్వర్ యొక్క ఇమెయిల్ "
-"కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా నిర్వాహకుడిని సంప్రదించండి."
-
 msgid "Submit"
 msgstr "సమర్పించు"
 
 msgid "The email %(email)s is not valid"
 msgstr "ఇమెయిల్ %(email)s చెల్లుబాటు కాదు"
 
 msgid "The participant name is invalid"
 msgstr "పాల్గొనేవారి పేరు చెల్లదు"
 
-msgid "The project identifier is %(project)s"
-msgstr "ప్రాజెక్ట్ ఐడెంటిఫైయర్ %(project)s"
-
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "ఈ అడ్మిన్ పాస్‌వర్డ్ సరైనది కాదు. %(num)d ప్రయత్నాలు మాత్రమే మిగిలి ఉన్నాయి."
 
 msgid "This private code is not the right one"
 msgstr "ఈ రహస్య కోడ్ సరైనది కాదు"
 
 msgid "This project already have this participant"
@@ -192,17 +160,14 @@
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr "ఈ ప్రాజెక్ట్ బహుళ కరెన్సీలలో బిల్లులను కలిగి ఉన్నందున 'నో కరెన్సీ'కి సెట్ చెయ్యడం కుదరదు."
 
 msgid "This project does not exists"
 msgstr "ఈ ప్రాజెక్ట్ కనుగొనబడలేదు"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "చాలా ఎక్కువ లాగిన్ ప్రయత్నాలు విఫలమయ్యాయి, దయచేసి తర్వాత మళ్లీ ప్రయత్నించండి."
-
 msgid "Unknown error"
 msgstr "గుర్తించలేని ఎర్రర్"
 
 msgid "Unknown project"
 msgstr "తెలియని ప్రాజెక్ట్"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/te/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/te/LC_MESSAGES/messages.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,27 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-04 15:24+0200\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-10-04 14:19+0000\n"
 "Last-Translator: Sharan J <sharanjs1999@gmail.com>\n"
-"Language-Team: Telugu <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/te/>\n"
 "Language: te\n"
+"Language-Team: Telugu <https://hosted.weblate.org/projects/i-hate-money/i"
+"-hate-money/te/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"Generated-By: Babel 2.9.0\n"
+
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "మీ ఖర్చులను పంచుకోవడానికి మీరు '%(project)s'ని సృష్టించారు"
 
 #, fuzzy
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "మీరు ఇచ్చిన లెక్కింపు సరైనది కాదు . సంఖ్యలు మరియు + - * / మాత్రమే "
@@ -42,28 +47,26 @@
 
 #, fuzzy
 msgid "Default Currency"
 msgstr "డిఫాల్ట్ కరెన్సీ"
 
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr ""
-"డిఫాల్ట్ కరెన్సీని సెట్ చేయడం వలన బిల్లుల మధ్య కరెన్సీ మార్పిడిని కుదురుతుంది"
+"డిఫాల్ట్ కరెన్సీని సెట్ చేయడం వలన బిల్లుల మధ్య కరెన్సీ మార్పిడిని "
+"కుదురుతుంది"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"ఈ ప్రాజెక్ట్ బహుళ కరెన్సీలలో బిల్లులను కలిగి ఉన్నందున 'నో కరెన్సీ'కి సెట్ "
-"చెయ్యడం కుదరదు."
+"ఈ ప్రాజెక్ట్ బహుళ కరెన్సీలలో బిల్లులను కలిగి ఉన్నందున 'నో కరెన్సీ'కి సెట్"
+" చెయ్యడం కుదరదు."
 
-msgid "Import previously exported JSON file"
-msgstr "గతంలో ఎగుమతి చేసిన JSON ఫైల్‌ని దిగుమతి చేయి"
-
-msgid "Import"
-msgstr "దిగుమతి చెయ్యి"
+msgid "Compatible with Cospend"
+msgstr ""
 
 #, fuzzy
 msgid "Project identifier"
 msgstr "ప్రాజెక్ట్ ఐడెంటిఫైయర్"
 
 #, fuzzy
 msgid "Private code"
@@ -121,25 +124,25 @@
 #, fuzzy
 msgid "Password confirmation"
 msgstr "పాస్ వర్డ్ ధృవీకరణ"
 
 msgid "Reset password"
 msgstr "పాస్ వర్డ్ రీసెట్ చేయి"
 
-msgid "Date"
-msgstr "తేదీ"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "ఏమిటి?"
 
-msgid "Payer"
-msgstr "చెల్లింపుదారు"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "చెల్లించిన మొత్తం"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "కరెన్సీ"
 
 msgid "External link"
 msgstr "బాహ్య లింకు"
 
@@ -156,17 +159,14 @@
 msgid "Submit and add a new one"
 msgstr "సమర్పించి, కొత్తదాన్ని జోడించండి"
 
 #, fuzzy, python-format
 msgid "Project default: %(currency)s"
 msgstr "ప్రాజెక్ట్ డిఫాల్ట్: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "బిల్లులు శూన్యం కాకూడదు"
-
 msgid "Name"
 msgstr "పేరు"
 
 msgid "Weights should be positive"
 msgstr "బరువులు సానుకూలంగా ఉండాలి"
 
 msgid "Weight"
@@ -180,21 +180,36 @@
 
 msgid "This project already have this participant"
 msgstr "ఈ ప్రాజెక్ట్‌లో ఇప్పటికే ఈ పాల్గునేవారు ఉన్నారు"
 
 msgid "People to notify"
 msgstr "తెలియజేయాల్సిన వ్యక్తులు"
 
-msgid "Send invites"
-msgstr "ఆహ్వానాలు పంపు"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "ఇమెయిల్ %(email)s చెల్లుబాటు కాదు"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"క్షమించండి, ఆహ్వాన ఇమెయిల్‌లను పంపడానికి ప్రయత్నిస్తున్నప్పుడు ఎర్రర్ "
+"వొచింది . దయచేసి సర్వర్ యొక్క ఇమెయిల్ కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా "
+"నిర్వాహకుడిని సంప్రదించండి."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} మరియు {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, మరియు {end_object}"
@@ -214,100 +229,101 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr ""
-"చాలా ఎక్కువ లాగిన్ ప్రయత్నాలు విఫలమయ్యాయి, దయచేసి తర్వాత మళ్లీ ప్రయత్నించండి."
+"చాలా ఎక్కువ లాగిన్ ప్రయత్నాలు విఫలమయ్యాయి, దయచేసి తర్వాత మళ్లీ "
+"ప్రయత్నించండి."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr ""
-"ఈ అడ్మిన్ పాస్‌వర్డ్ సరైనది కాదు. %(num)d ప్రయత్నాలు మాత్రమే మిగిలి ఉన్నాయి."
+"ఈ అడ్మిన్ పాస్‌వర్డ్ సరైనది కాదు. %(num)d ప్రయత్నాలు మాత్రమే మిగిలి "
+"ఉన్నాయి."
 
 msgid "Provided token is invalid"
 msgstr "ఇవ్వబడ్డ టోకెన్ చెల్లుబాటు కాదు"
 
 msgid "This private code is not the right one"
 msgstr "ఈ రహస్య కోడ్ సరైనది కాదు"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "మీ ఖర్చులను పంచుకోవడానికి మీరు '%(project)s'ని సృష్టించారు"
-
 msgid "A reminder email has just been sent to you"
 msgstr "మీకు ఇప్పుడే రిమైండర్ ఇమెయిల్ పంపబడింది"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
-"మేము మీకు రిమైండర్ ఇమెయిల్ పంపడానికి ప్రయత్నించాము, కానీ ఒక ఎర్రర్ వొచింది . "
-"మీరు ప్రాజెక్ట్‌ను సాధారణంగా ఉపయోగించవచ్చు."
-
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "ప్రాజెక్ట్ ఐడెంటిఫైయర్ %(project)s"
+"మేము మీకు రిమైండర్ ఇమెయిల్ పంపడానికి ప్రయత్నించాము, కానీ ఒక ఎర్రర్ "
+"వొచింది . మీరు ప్రాజెక్ట్‌ను సాధారణంగా ఉపయోగించవచ్చు."
 
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
-"క్షమించండి, పాస్‌వర్డ్ రీసెట్ సూచనలతో కూడిన ఇమెయిల్‌ను మీకు పంపుతున్నప్పుడు "
-"ఎర్రర్ వొచింది. దయచేసి సర్వర్ యొక్క ఇమెయిల్ కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా"
-" నిర్వాహకుడిని సంప్రదించండి."
+"క్షమించండి, పాస్‌వర్డ్ రీసెట్ సూచనలతో కూడిన ఇమెయిల్‌ను మీకు "
+"పంపుతున్నప్పుడు ఎర్రర్ వొచింది. దయచేసి సర్వర్ యొక్క ఇమెయిల్ "
+"కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా నిర్వాహకుడిని సంప్రదించండి."
 
 msgid "No token provided"
 msgstr "ఎలాంటి టోకెన్ ఇవ్వబడలేదు"
 
 msgid "Invalid token"
 msgstr "చెల్లని టోకెన్"
 
 msgid "Unknown project"
 msgstr "తెలియని ప్రాజెక్ట్"
 
 msgid "Password successfully reset."
 msgstr "పాస్ వర్డ్ విజయవంతంగా రీసెట్ చేయబడింది."
 
-msgid "Project successfully uploaded"
-msgstr "ప్రాజెక్ట్ విజయవంతంగా అప్ లోడ్ చేయబడింది"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "చెల్లని JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
-"డిఫాల్ట్ కరెన్సీ లేకుండా ప్రాజెక్ట్‌కు బహుళ కరెన్సీలలో బిల్లులను జోడించలేరు"
+"డిఫాల్ట్ కరెన్సీ లేకుండా ప్రాజెక్ట్‌కు బహుళ కరెన్సీలలో బిల్లులను "
+"జోడించలేరు"
+
+msgid "Project successfully uploaded"
+msgstr "ప్రాజెక్ట్ విజయవంతంగా అప్ లోడ్ చేయబడింది"
 
 msgid "Project successfully deleted"
 msgstr "ప్రాజెక్ట్ విజయవంతంగా తొలగించబడింది"
 
 msgid "Error deleting project"
 msgstr "ప్రాజెక్ట్‌ను తొలగించడంలో ఎర్రర్ వొచింది"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "%(project)s కోసం మీ ఖర్చులను పంచుకోవడానికి మీరు ఆహ్వానించబడ్డారు"
 
 msgid "Your invitations have been sent"
 msgstr "మీ ఆహ్వానాలు పంపబడ్డాయి"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
-"క్షమించండి, ఆహ్వాన ఇమెయిల్‌లను పంపడానికి ప్రయత్నిస్తున్నప్పుడు ఎర్రర్ వొచింది"
-" . దయచేసి సర్వర్ యొక్క ఇమెయిల్ కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా "
+"క్షమించండి, ఆహ్వాన ఇమెయిల్‌లను పంపడానికి ప్రయత్నిస్తున్నప్పుడు ఎర్రర్ "
+"వొచింది . దయచేసి సర్వర్ యొక్క ఇమెయిల్ కాన్ఫిగరేషన్‌ను తనిఖీ చేయండి లేదా "
 "నిర్వాహకుడిని సంప్రదించండి."
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s కలపబడ్డారు"
 
 msgid "Error activating participant"
@@ -321,16 +337,16 @@
 msgstr "పాల్గొనేవారిని తొలగించడంలో ఎర్రర్ వొచింది"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"పార్టిసిపెంట్ '%(name)s' డియాక్టివేట్ చేయబడ్డారు. వీరి బ్యాలెన్స్ సున్నాకి "
-"చేరే వరకు జాబితాలో కనిపిస్తుంది."
+"పార్టిసిపెంట్ '%(name)s' డియాక్టివేట్ చేయబడ్డారు. వీరి బ్యాలెన్స్ "
+"సున్నాకి చేరే వరకు జాబితాలో కనిపిస్తుంది."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "పార్టిసిపెంట్ '%(name)s' తీసివేయబడ్డారు"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -344,14 +360,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr ""
 
 msgid "Deleted project history."
 msgstr ""
 
 msgid "Error deleting recorded IP addresses"
@@ -404,43 +424,35 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "ప్రాజెక్ట్ ని సృష్టించు"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -458,26 +470,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "గతంలో ఎగుమతి చేసిన JSON ఫైల్‌ని దిగుమతి చేయి"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -488,17 +510,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -555,51 +574,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -655,17 +669,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "చెల్లింపుదారు"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "తేదీ"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -767,15 +787,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -801,46 +822,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -885,14 +900,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -924,7 +945,60 @@
 msgstr ""
 
 msgid "Expenses by Month"
 msgstr ""
 
 msgid "Period"
 msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "దిగుమతి చెయ్యి"
+
+#~ msgid "Amount paid"
+#~ msgstr "చెల్లించిన మొత్తం"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "బిల్లులు శూన్యం కాకూడదు"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "ప్రాజెక్ట్ ఐడెంటిఫైయర్ %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "చెల్లని JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "ఆహ్వానాలు పంపు"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,35 +1,32 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
 "PO-Revision-Date: 2021-09-16 14:36+0000\n"
 "Last-Translator: PPNplus <ppnplus@protonmail.com>\n"
 "Language: th\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/i-hate-money/i-hate-"
 "money/th/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "A reminder email has just been sent to you"
 msgstr "ส่งอีเมลเตือนความจำให้คุณแล้ว"
 
 msgid "Add"
 msgstr "เพิ่ม"
 
 msgid "Admin password"
 msgstr "รหัสผ่านผู้ดูแล"
 
-msgid "Amount paid"
-msgstr "จำนวนเงินที่จ่าย"
-
 msgid "Can't remember the password?"
 msgstr "หากจำรหัสผ่านไม่ได้"
 
 msgid "Cancel"
 msgstr "ยกเลิก"
 
 msgid "Create the project"
@@ -61,17 +58,14 @@
 
 msgid "For whom?"
 msgstr "ให้ใคร?"
 
 msgid "Get in"
 msgstr "เข้าด้านใน"
 
-msgid "Import"
-msgstr "นำเข้า"
-
 msgid "Name"
 msgstr "ชื่อ"
 
 msgid "No Currency"
 msgstr "ไม่มีสกุลเงิน"
 
 msgid "No one"
@@ -118,17 +112,14 @@
 
 msgid "This project does not exists"
 msgstr "โครงการนี้ไม่มีอยู่"
 
 msgid "To whom?"
 msgstr "ให้ใคร?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "เข้าสู่ระบบล้มเหลวหลายครั้ง โปรดลองอีกครั้งในภายหลัง"
-
 msgid "Unknown error"
 msgstr "ข้อผิดพลาดที่ไม่รู้จัก"
 
 msgid "Use IP tracking for project history"
 msgstr "ใช้การติดตามที่อยู่ IP สำหรับประวัติโครงการ"
 
 msgid "What?"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/th/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/th/LC_MESSAGES/messages.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2021-09-16 14:36+0000\n"
 "Last-Translator: PPNplus <ppnplus@protonmail.com>\n"
 "Language: th\n"
 "Language-Team: Thai <https://hosted.weblate.org/projects/i-hate-money/i"
 "-hate-money/th/>\n"
 "Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr ""
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 
 msgid "Project name"
 msgstr "ชื่อโครงการ"
@@ -45,20 +49,17 @@
 msgstr ""
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 
-msgid "Import previously exported JSON file"
+msgid "Compatible with Cospend"
 msgstr ""
 
-msgid "Import"
-msgstr "นำเข้า"
-
 msgid "Project identifier"
 msgstr ""
 
 msgid "Private code"
 msgstr ""
 
 msgid "Create the project"
@@ -108,25 +109,25 @@
 
 msgid "Password confirmation"
 msgstr "ยืนยันรหัสผ่าน"
 
 msgid "Reset password"
 msgstr "รีเซ็ตรหัสผ่าน"
 
-msgid "Date"
-msgstr "วันที่"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "อะไร?"
 
-msgid "Payer"
-msgstr "ผู้จ่าย"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "จำนวนเงินที่จ่าย"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "สกุลเงิน"
 
 msgid "External link"
 msgstr "ลิงก์ภายนอก"
 
@@ -142,17 +143,14 @@
 msgid "Submit and add a new one"
 msgstr "ส่งและเพิ่มอันใหม่"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "ค่าเริ่มต้นของโครงการ: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr ""
-
 msgid "Name"
 msgstr "ชื่อ"
 
 msgid "Weights should be positive"
 msgstr ""
 
 msgid "Weight"
@@ -166,21 +164,33 @@
 
 msgid "This project already have this participant"
 msgstr ""
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "ส่งคำเชิญ"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "อีเมล %(email)s ไม่ถูกต้อง"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} และ {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object}, และ {end_object}"
@@ -200,89 +210,85 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "เข้าสู่ระบบล้มเหลวหลายครั้ง โปรดลองอีกครั้งในภายหลัง"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "รหัสผ่านผู้ดูแลนี้ไม่ถูกต้อง สามารถพยายามเข้าสู่ระบบได้อีก %(num)d ครั้ง"
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr ""
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr ""
-
 msgid "A reminder email has just been sent to you"
 msgstr "ส่งอีเมลเตือนความจำให้คุณแล้ว"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr ""
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr ""
 
 msgid "Invalid token"
 msgstr ""
 
 msgid "Unknown project"
 msgstr ""
 
 msgid "Password successfully reset."
 msgstr ""
 
-msgid "Project successfully uploaded"
+msgid "Unable to parse CSV"
 msgstr ""
 
-msgid "Invalid JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
 msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr ""
+
 msgid "Project successfully deleted"
 msgstr ""
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr ""
 
 msgid "Your invitations have been sent"
 msgstr ""
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr ""
 
 msgid "Error activating participant"
@@ -317,14 +323,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr ""
 
 msgid "Deleted project history."
 msgstr ""
 
 msgid "Error deleting recorded IP addresses"
@@ -377,43 +387,35 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
+msgid "Delete project"
 msgstr ""
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 msgid "Get it on"
 msgstr ""
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
-msgid "Delete project"
-msgstr ""
-
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
+#, fuzzy
+msgid "Import project"
+msgstr "สร้างโครงการ"
 
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
@@ -431,26 +433,35 @@
 
 msgid "Cancel"
 msgstr "ยกเลิก"
 
 msgid "Privacy Settings"
 msgstr "การตั้งค่าความเป็นส่วนตัว"
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+msgid "Import previously exported project"
+msgstr ""
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "ทุกคน"
 
 msgid "No one"
 msgstr "ไม่มีใคร"
 
 msgid "More options"
@@ -461,17 +472,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr "ดาวน์โหลด"
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -528,51 +536,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -628,17 +631,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "ผู้จ่าย"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "วันที่"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -740,15 +749,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -774,46 +784,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -858,14 +862,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -936,7 +946,79 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
+
+#~ msgid "Import previously exported JSON file"
+#~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "นำเข้า"
+
+#~ msgid "Amount paid"
+#~ msgstr "จำนวนเงินที่จ่าย"
+
+#~ msgid "Bills can't be null"
+#~ msgstr ""
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "ส่งคำเชิญ"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.mo`

 * *Files 11% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,50 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Turkish (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-11-07 10:07+0000\n"
+"Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
+"Language: tr\n"
 "Language-Team: Turkish <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/tr/>\n"
-"Language: tr\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.2\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Aşağıdaki tablo, proje geçmişini devre dışı bırakmadan önce "
-"kaydedilen eylemleri göstermektedir. Bunları kaldırmak için\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">proje geçmişini temizleyebilirsiniz</a>.</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Bu projenin geçmişi devre dışı bırakıldı. Yeni eylemler "
-"aşağıda görünmeyecek. Geçmişi\n"
-"            <a href=\"%(url)s\"> ayarlar sayfasında</a>  "
-"etkinleştirebilirsiniz</i>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "\"I hate money\" özgür bir yazılımdır"
 
 msgid "%(amount)s each"
 msgstr "her biri %(amount)s"
 
@@ -108,17 +80,14 @@
 
 msgid "Amount"
 msgstr "Miktar"
 
 msgid "Amount in %(currency)s"
 msgstr "%(currency)s olarak miktar"
 
-msgid "Amount paid"
-msgstr "Ödenen tutar"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "Kaydedilen tüm IP adreslerini bu projeden silmek istediğinize emin misiniz?\n"
@@ -128,17 +97,14 @@
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr ""
 "Bu proje için tüm geçmişi silmek istediğinize emin misiniz? Bu işlem geri "
 "alınamaz."
 
-msgid "Are you sure?"
-msgstr "Emin misiniz?"
-
 msgid "Authentication"
 msgstr "Kimlik doğrulama"
 
 msgid "Back to the list"
 msgstr "Listeye geri dön"
 
 msgid "Balance"
@@ -175,17 +141,14 @@
 
 msgid "Bill items"
 msgstr "Fatura ögeleri"
 
 msgid "Bills"
 msgstr "Faturalar"
 
-msgid "Bills can't be null"
-msgstr "Faturalar boş olamaz"
-
 msgid "Can't remember the password?"
 msgstr "Parolayı hatırlayamıyor musunuz?"
 
 msgid "Cancel"
 msgstr "İptal"
 
 msgid ""
@@ -383,26 +346,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "IP adresi kaydetme ayarlar sayfasında etkinleştirilebilir"
 
 msgid "Identifier:"
 msgstr "Tanımlayıcı:"
 
-msgid "Import"
-msgstr "İçe aktar"
-
-msgid "Import JSON"
-msgstr "JSON'u içe aktar"
-
-msgid "Import previously exported JSON file"
-msgstr "Önceden dışa aktarılan JSON dosyasını içe aktar"
-
-msgid "Invalid JSON"
-msgstr "Geçersiz JSON"
-
 msgid "Invalid private code."
 msgstr "Geçersiz özel kod."
 
 msgid "Invalid token"
 msgstr "Geçersiz belirteç"
 
 msgid "Invite people"
@@ -661,30 +612,14 @@
 msgstr ""
 "Bu projede IP kaydetme devre dışı bırakılmış olsa da aşağıdaki bazı girdiler "
 "IP adresleri içermektedir. "
 
 msgid "Someone probably cleared the project history."
 msgstr "Birisi muhtemelen proje geçmişini temizledi."
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"Maalesef, parola sıfırlama talimatlarını içeren e-posta gönderilirken bir "
-"hata oluştu. Lütfen sunucunun e-posta yapılandırmasına göz atın veya "
-"yöneticiye başvurun."
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"Maalesef davet e-postalarını göndermeye çalışırken bir hata oluştu. Lütfen "
-"sunucunun e-posta yapılandırmasına göz atın veya yöneticiye başvurun."
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "Maalesef, istediğiniz sayfayı bulamadık."
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -727,17 +662,14 @@
 
 msgid "The email %(email)s is not valid"
 msgstr "%(email)s e-posta adresi geçerli değil"
 
 msgid "The participant name is invalid"
 msgstr "Katılımcı adı geçersiz"
 
-msgid "The project identifier is %(project)s"
-msgstr "Proje tanımlayıcısı %(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "Erişmeye çalıştığınız proje mevcut değil, ister misiniz"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Bu yönetici parolası doğru değil. Yalnızca %(num)d tane deneme kaldı."
 
 msgid "This private code is not the right one"
@@ -761,18 +693,14 @@
 
 msgid "Time"
 msgstr "Zaman"
 
 msgid "To whom?"
 msgstr "Kime?"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr ""
-"Çok fazla başarısız oturum açma denemesi, lütfen daha sonra tekrar deneyin."
-
 msgid "Try out the demo"
 msgstr "Tanıtım sürümünü deneyin"
 
 msgid "Unknown error"
 msgstr "Bilinmeyen hata"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/tr/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/tr/LC_MESSAGES/messages.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-11-07 10:07+0000\n"
 "Last-Translator: Oğuz Ersen <oguz@ersen.moe>\n"
-"Language-Team: Turkish <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/tr/>\n"
 "Language: tr\n"
+"Language-Team: Turkish <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/tr/>\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.2\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Giderlerinizi paylaşmak için '%(project)s' oluşturdunuz"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr ""
 "Geçerli bir miktar veya ifade değil. Yalnızca rakamlar ve + - * / "
 "operatörleri kabul edilir."
 
@@ -51,19 +55,16 @@
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
 "Bu proje, birden fazla para biriminde faturalar içerdiğinden 'para birimi"
 " yok' olarak ayarlanamaz."
 
-msgid "Import previously exported JSON file"
-msgstr "Önceden dışa aktarılan JSON dosyasını içe aktar"
-
-msgid "Import"
-msgstr "İçe aktar"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Proje tanımlayıcısı"
 
 msgid "Private code"
 msgstr "Özel kod"
 
@@ -116,25 +117,25 @@
 
 msgid "Password confirmation"
 msgstr "Parola onayı"
 
 msgid "Reset password"
 msgstr "Parolayı sıfırla"
 
-msgid "Date"
-msgstr "Tarih"
+msgid "When?"
+msgstr "Ne zaman?"
 
 msgid "What?"
 msgstr "Ne?"
 
-msgid "Payer"
-msgstr "Mükellefi"
+msgid "Who paid?"
+msgstr "Kim ödedi?"
 
-msgid "Amount paid"
-msgstr "Ödenen tutar"
+msgid "How much?"
+msgstr "Ne kadar?"
 
 msgid "Currency"
 msgstr "Para birimi"
 
 msgid "External link"
 msgstr "Harici bağlantı"
 
@@ -150,17 +151,14 @@
 msgid "Submit and add a new one"
 msgstr "Gönder ve yeni bir tane ekle"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Proje öntanımlı değeri: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Faturalar boş olamaz"
-
 msgid "Name"
 msgstr "Ad"
 
 msgid "Weights should be positive"
 msgstr "Ağırlıklar pozitif olmalıdır"
 
 msgid "Weight"
@@ -174,21 +172,36 @@
 
 msgid "This project already have this participant"
 msgstr "Bu projede bu katılımcı zaten var"
 
 msgid "People to notify"
 msgstr "Bildirilecek kişiler"
 
-msgid "Send invites"
-msgstr "Davet gönder"
+msgid "Send the invitations"
+msgstr "Davetleri gönder"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "%(email)s e-posta adresi geçerli değil"
 
+msgid "Logout"
+msgstr "Oturumu kapat"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+"Maalesef davet e-postalarını göndermeye çalışırken bir hata oluştu. "
+"Lütfen sunucunun e-posta yapılandırmasına göz atın veya yöneticiye "
+"başvurun."
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} ve {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object} ve {end_object}"
@@ -208,51 +221,44 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr ""
 "Çok fazla başarısız oturum açma denemesi, lütfen daha sonra tekrar "
 "deneyin."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Bu yönetici parolası doğru değil. Yalnızca %(num)d tane deneme kaldı."
 
 msgid "Provided token is invalid"
 msgstr "Sağlanan belirteç geçersiz"
 
 msgid "This private code is not the right one"
 msgstr "Bu özel kod doğru değil"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Giderlerinizi paylaşmak için '%(project)s' oluşturdunuz"
-
 msgid "A reminder email has just been sent to you"
 msgstr "Size bir hatırlatma e-postası gönderildi"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 "Size bir hatırlatma e-postası göndermeye çalıştık, ancak bir hata oluştu."
 " Projeyi yine de normal şekilde kullanabilirsiniz."
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Proje tanımlayıcısı %(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 "Maalesef, parola sıfırlama talimatlarını içeren e-posta gönderilirken bir"
 " hata oluştu. Lütfen sunucunun e-posta yapılandırmasına göz atın veya "
 "yöneticiye başvurun."
 
 msgid "No token provided"
 msgstr "Belirteç sağlanmadı"
@@ -262,44 +268,49 @@
 
 msgid "Unknown project"
 msgstr "Bilinmeyen proje"
 
 msgid "Password successfully reset."
 msgstr "Parola başarıyla sıfırlandı."
 
-msgid "Project successfully uploaded"
-msgstr "Proje başarıyla karşıya yüklendi"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Geçersiz JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 "Öntanımlı para birimi olmayan bir projeye birden fazla para biriminde "
 "fatura eklenemez"
 
+msgid "Project successfully uploaded"
+msgstr "Proje başarıyla karşıya yüklendi"
+
 msgid "Project successfully deleted"
 msgstr "Proje başarıyla silindi"
 
 msgid "Error deleting project"
 msgstr "Proje silinirken hata oluştu"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "%(project)s için giderlerinizi paylaşmaya davet edildiniz"
 
 msgid "Your invitations have been sent"
 msgstr "Davetleriniz gönderildi"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 "Maalesef davet e-postalarını göndermeye çalışırken bir hata oluştu. "
 "Lütfen sunucunun e-posta yapılandırmasına göz atın veya yöneticiye "
 "başvurun."
 
 #, python-format
 msgid "%(member)s has been added"
@@ -316,16 +327,16 @@
 msgstr "Katılımcı kaldırılırken hata oluştu"
 
 #, python-format
 msgid ""
 "Participant '%(name)s' has been deactivated. It will still appear in the "
 "list until its balance reach zero."
 msgstr ""
-"'%(name)s' katılımcısı devre dışı bırakıldı. Bakiyesi sıfır oluncaya kadar "
-"listede görünmeye devam edecektir."
+"'%(name)s' katılımcısı devre dışı bırakıldı. Bakiyesi sıfır oluncaya "
+"kadar listede görünmeye devam edecektir."
 
 #, python-format
 msgid "Participant '%(name)s' has been removed"
 msgstr "'%(name)s' katılımcısı kaldırıldı"
 
 #, python-format
 msgid "Participant '%(name)s' has been modified"
@@ -339,14 +350,18 @@
 
 msgid "The bill has been deleted"
 msgstr "Fatura silindi"
 
 msgid "The bill has been modified"
 msgstr "Fatura değiştirildi"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "Proje geçmişi silinirken hata oluştu"
 
 msgid "Deleted project history."
 msgstr "Proje geçmişi silindi."
 
 msgid "Error deleting recorded IP addresses"
@@ -399,43 +414,35 @@
 
 msgid "Actions"
 msgstr "Eylemler"
 
 msgid "edit"
 msgstr "düzenle"
 
-msgid "delete"
-msgstr "sil"
+msgid "Delete project"
+msgstr "Projeyi sil"
 
 msgid "show"
 msgstr "göster"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "Gösterge paneli şu anda devre dışı."
 
 msgid "Download Mobile Application"
 msgstr "Telefon Uygulamasını İndir"
 
 msgid "Get it on"
 msgstr "Alın"
 
-msgid "Are you sure?"
-msgstr "Emin misiniz?"
-
 msgid "Edit project"
 msgstr "Projeyi düzenle"
 
-msgid "Delete project"
-msgstr "Projeyi sil"
-
-msgid "Import JSON"
-msgstr "JSON'u içe aktar"
-
-msgid "Choose file"
-msgstr "Dosya seç"
+#, fuzzy
+msgid "Import project"
+msgstr "Projeyi düzenle"
 
 msgid "Download project's data"
 msgstr "Proje verilerini indir"
 
 msgid "Bill items"
 msgstr "Fatura ögeleri"
 
@@ -453,26 +460,36 @@
 
 msgid "Cancel"
 msgstr "İptal"
 
 msgid "Privacy Settings"
 msgstr "Gizlilik Ayarları"
 
-msgid "Edit the project"
-msgstr "Projeyi düzenle"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "Bu, bu projedeki tüm faturaları ve katılımcıları kaldıracaktır!"
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Önceden dışa aktarılan JSON dosyasını içe aktar"
+
+msgid "Choose file"
+msgstr "Dosya seç"
+
 msgid "Edit this bill"
 msgstr "Bu faturayı düzenle"
 
 msgid "Add a bill"
 msgstr "Bir fatura ekle"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "Herkes"
 
 msgid "No one"
 msgstr "Hiç kimse"
 
 msgid "More options"
@@ -483,17 +500,14 @@
 
 msgid "Edit this participant"
 msgstr "Bu katılımcıyı düzenle"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "Davetleri gönder"
-
 msgid "Download"
 msgstr "İndir"
 
 msgid "Disabled Project History"
 msgstr "Proje Geçmişi Devre Dışı"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -558,68 +572,52 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "Fatura %(name)s: %(owers_list_str)s borçlular listesine eklendi"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "Fatura %(name)s: %(owers_list_str)s borçlular listesinden kaldırıldı"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Bu projenin geçmişi devre dışı bırakıldı. Yeni eylemler "
-"aşağıda görünmeyecek. Geçmişi\n"
-"            <a href=\"%(url)s\"> ayarlar sayfasında</a>  "
-"etkinleştirebilirsiniz</i>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "IP adresi kaydetme ayarlar sayfasında etkinleştirilebilir"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>Aşağıdaki tablo, proje geçmişini devre dışı bırakmadan "
-"önce kaydedilen eylemleri göstermektedir. Bunları kaldırmak için\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">proje geçmişini "
-"temizleyebilirsiniz</a>.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "Birisi muhtemelen proje geçmişini temizledi."
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 "Bu projede IP kaydetme devre dışı bırakılmış olsa da aşağıdaki bazı "
 "girdiler IP adresleri içermektedir. "
 
 msgid "Delete stored IP addresses"
 msgstr "Kaydedilen IP adreslerini sil"
 
-msgid "No history to erase"
-msgstr "Silinecek geçmiş yok"
-
-msgid "Clear Project History"
-msgstr "Proje Geçmişini Temizle"
-
 msgid "No IP Addresses to erase"
 msgstr "Silinecek IP adresi yok"
 
 msgid "Delete Stored IP Addresses"
 msgstr "Kaydedilen IP Adreslerini Sil"
 
+msgid "No history to erase"
+msgstr "Silinecek geçmiş yok"
+
+msgid "Clear Project History"
+msgstr "Proje Geçmişini Temizle"
+
 msgid "Time"
 msgstr "Zaman"
 
 msgid "Event"
 msgstr "Etkinlik"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -675,17 +673,23 @@
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 "Katılımcı %(name)s: %(old_weight)s olan ağırlık %(new_weight)s olarak "
 "değiştirildi"
 
+msgid "Payer"
+msgstr "Mükellefi"
+
 msgid "Amount"
 msgstr "Miktar"
 
+msgid "Date"
+msgstr "Tarih"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "%(currency)s olarak miktar"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "%(name)s faturası değiştirildi"
@@ -789,16 +793,17 @@
 
 msgid "switch to"
 msgstr "geçiş yap"
 
 msgid "Dashboard"
 msgstr "Gösterge Paneli"
 
-msgid "Logout"
-msgstr "Oturumu kapat"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "Kod"
 
 msgid "Mobile Application"
 msgstr "Telefon Uygulaması"
 
@@ -823,46 +828,40 @@
 
 msgid "you sure?"
 msgstr "emin misiniz?"
 
 msgid "Invite people"
 msgstr "İnsanları davet et"
 
-msgid "You should start by adding participants"
-msgstr "Katılımcıları ekleyerek başlamalısınız"
-
-msgid "Add a new bill"
-msgstr "Yeni bir fatura ekle"
-
 msgid "Newer bills"
 msgstr "Daha yeni faturalar"
 
 msgid "Older bills"
 msgstr "Daha eski faturalar"
 
-msgid "When?"
-msgstr "Ne zaman?"
+msgid "You should start by adding participants"
+msgstr "Katılımcıları ekleyerek başlamalısınız"
 
-msgid "Who paid?"
-msgstr "Kim ödedi?"
+msgid "Add a new bill"
+msgstr "Yeni bir fatura ekle"
 
 msgid "For what?"
 msgstr "Ne için?"
 
-msgid "How much?"
-msgstr "Ne kadar?"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "%(date)s tarihinde eklendi"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "%(excluded)s hariç herkes"
 
+msgid "delete"
+msgstr "sil"
+
 msgid "No bills"
 msgstr "Fatura yok"
 
 msgid "Nothing to list yet."
 msgstr "Henüz listelenecek bir şey yok."
 
 msgid "You probably want to"
@@ -913,14 +912,20 @@
 msgstr "Bağlantıyı Paylaş"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 "Aşağıdaki bağlantıyı tercih ettiğiniz ortam aracılığıyla doğrudan "
 "paylaşabilirsiniz"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "E-posta ile Gönder"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1054,7 +1059,77 @@
 #~ msgstr "Üye sayısı"
 
 #~ msgid "Edit this member"
 #~ msgstr "Bu üyeyi düzenle"
 
 #~ msgid "Participants to notify"
 #~ msgstr "katılımcılar ekle"
+
+#~ msgid "Import"
+#~ msgstr "İçe aktar"
+
+#~ msgid "Amount paid"
+#~ msgstr "Ödenen tutar"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Faturalar boş olamaz"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Proje tanımlayıcısı %(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Geçersiz JSON"
+
+#~ msgid "Are you sure?"
+#~ msgstr "Emin misiniz?"
+
+#~ msgid "Import JSON"
+#~ msgstr "JSON'u içe aktar"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Bu projenin geçmişi devre "
+#~ "dışı bırakıldı. Yeni eylemler aşağıda "
+#~ "görünmeyecek. Geçmişi\n"
+#~ "            <a href=\"%(url)s\"> ayarlar "
+#~ "sayfasında</a>  etkinleştirebilirsiniz</i>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>Aşağıdaki tablo, proje "
+#~ "geçmişini devre dışı bırakmadan önce "
+#~ "kaydedilen eylemleri göstermektedir. Bunları "
+#~ "kaldırmak için\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">proje geçmişini "
+#~ "temizleyebilirsiniz</a>.</i></p>\n"
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "Davet gönder"
+
+#~ msgid " show"
+#~ msgstr "göster"
+
+#~ msgid "Edit the project"
+#~ msgstr "Projeyi düzenle"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,23 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Ukrainian (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-09-17 10:24+0000\n"
+"Last-Translator: Dmytro Onopa <dmytro.onopa@gmail.com>\n"
+"Language: uk\n"
 "Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-money/i-"
 "hate-money/uk/>\n"
-"Language: uk\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "%(member)s has been added"
 msgstr "%(member)s додано"
 
 msgid "%(name)s is part of this project again"
 msgstr "%(name)s знову частина цього проекту"
 
@@ -32,20 +33,14 @@
 
 msgid "Add"
 msgstr "Додати"
 
 msgid "Admin password"
 msgstr "Пароль адміністратора"
 
-msgid "Amount paid"
-msgstr "Виплачувана сума"
-
-msgid "Bills can't be null"
-msgstr "Рахунки не можуть бути порожніми"
-
 msgid "Create the project"
 msgstr "Створити проєкт"
 
 msgid "Currency"
 msgstr "Валюта"
 
 msgid "Date"
@@ -71,23 +66,14 @@
 
 msgid "For whom?"
 msgstr "Для кого?"
 
 msgid "Get in"
 msgstr "Отримати в"
 
-msgid "Import"
-msgstr "Імпортувати"
-
-msgid "Import previously exported JSON file"
-msgstr "Імпортувати попередньо експортований JSON файл"
-
-msgid "Invalid JSON"
-msgstr "Недійсний JSON"
-
 msgid "Invalid private code."
 msgstr "Помилковий приватний ключ"
 
 msgid "Invalid token"
 msgstr "Недійсний токен"
 
 msgid "Name"
@@ -164,17 +150,14 @@
 
 msgid "Submit and add a new one"
 msgstr "Підтвердити та додати ще один"
 
 msgid "The email %(email)s is not valid"
 msgstr "Поштові скриньки %(email)s не дійсні"
 
-msgid "The project identifier is %(project)s"
-msgstr "Ідентифікатор проєкту %(project)s"
-
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Цей пароль адміністратора не вірний. Залишилося тільки %(num)d спроб."
 
 msgid "This private code is not the right one"
 msgstr "Цей приватний код не підходить"
 
 msgid ""
@@ -183,17 +166,14 @@
 msgstr ""
 "Цей проект не може бути встановлено у значення \"Без валюти\", оскільки він "
 "містить декілько валют в рахунках."
 
 msgid "This project does not exists"
 msgstr "Цей проєкт не існує"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "Забагато невдалих спроб увійти, будь ласка спробуйте пізніше."
-
 msgid "Unknown error"
 msgstr "Невідома помилка"
 
 msgid "Unknown project"
 msgstr "Невідомий проєкт"
 
 msgid "Use IP tracking for project history"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/uk/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/uk/LC_MESSAGES/messages.po`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-09-17 10:24+0000\n"
 "Last-Translator: Dmytro Onopa <dmytro.onopa@gmail.com>\n"
-"Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-money/"
-"i-hate-money/uk/>\n"
 "Language: uk\n"
+"Language-Team: Ukrainian <https://hosted.weblate.org/projects/i-hate-"
+"money/i-hate-money/uk/>\n"
+"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "Ви щойно створили '%(project)s', щоб поділитися витратами"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "Не вірна сума чи вираз. Приймаються тільки числа та оператори + - * /."
 
 msgid "Project name"
 msgstr "Назва проєкту"
@@ -45,22 +49,19 @@
 msgid "Setting a default currency enables currency conversion between bills"
 msgstr "Встановлення типової валюти уможливлює конвертацію валюти між векселями"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr ""
-"Цей проект не може бути встановлено у значення \"Без валюти\", оскільки він "
-"містить декілько валют в рахунках."
+"Цей проект не може бути встановлено у значення \"Без валюти\", оскільки "
+"він містить декілько валют в рахунках."
 
-msgid "Import previously exported JSON file"
-msgstr "Імпортувати попередньо експортований JSON файл"
-
-msgid "Import"
-msgstr "Імпортувати"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "Ідентифікатор проєкту"
 
 msgid "Private code"
 msgstr "Приватний код"
 
@@ -113,25 +114,25 @@
 
 msgid "Password confirmation"
 msgstr "Підтвердження паролю"
 
 msgid "Reset password"
 msgstr "Скинути пароль"
 
-msgid "Date"
-msgstr "Дата"
+msgid "When?"
+msgstr ""
 
 msgid "What?"
 msgstr "Що?"
 
-msgid "Payer"
-msgstr "Платник"
+msgid "Who paid?"
+msgstr ""
 
-msgid "Amount paid"
-msgstr "Виплачувана сума"
+msgid "How much?"
+msgstr ""
 
 msgid "Currency"
 msgstr "Валюта"
 
 msgid "External link"
 msgstr "Зовнішнє посилання"
 
@@ -147,17 +148,14 @@
 msgid "Submit and add a new one"
 msgstr "Підтвердити та додати ще один"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "Типове для проєкту: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "Рахунки не можуть бути порожніми"
-
 msgid "Name"
 msgstr "Назва"
 
 msgid "Weights should be positive"
 msgstr "Вага має бути додатною"
 
 msgid "Weight"
@@ -173,21 +171,33 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "У цьому проєкті вже є такий учасник"
 
 msgid "People to notify"
 msgstr ""
 
-msgid "Send invites"
-msgstr "Відправити запрошення"
+msgid "Send the invitations"
+msgstr ""
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "Поштові скриньки %(email)s не дійсні"
 
+msgid "Logout"
+msgstr ""
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr ""
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr ""
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr ""
@@ -207,89 +217,85 @@
 msgid "{prefix}: {error}"
 msgstr ""
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr ""
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "Забагато невдалих спроб увійти, будь ласка спробуйте пізніше."
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "Цей пароль адміністратора не вірний. Залишилося тільки %(num)d спроб."
 
 msgid "Provided token is invalid"
 msgstr ""
 
 msgid "This private code is not the right one"
 msgstr "Цей приватний код не підходить"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "Ви щойно створили '%(project)s', щоб поділитися витратами"
-
 msgid "A reminder email has just been sent to you"
 msgstr ""
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr ""
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "Ідентифікатор проєкту %(project)s"
-
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr ""
 
 msgid "No token provided"
 msgstr "Не надано токен"
 
 msgid "Invalid token"
 msgstr "Недійсний токен"
 
 msgid "Unknown project"
 msgstr "Невідомий проєкт"
 
 msgid "Password successfully reset."
 msgstr "Пароль з успіхом відновлено."
 
-msgid "Project successfully uploaded"
-msgstr "Проєкт з успіхом завантажено"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "Недійсний JSON"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr ""
 
+msgid "Project successfully uploaded"
+msgstr "Проєкт з успіхом завантажено"
+
 msgid "Project successfully deleted"
 msgstr "Проєкт з успіхом видалено"
 
 msgid "Error deleting project"
 msgstr ""
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "Вас запросили поділитися своїми витратами у %(project)s"
 
 msgid "Your invitations have been sent"
 msgstr "Ваші запрошення відправленні"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr ""
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "%(member)s додано"
 
 msgid "Error activating participant"
@@ -324,14 +330,18 @@
 
 msgid "The bill has been deleted"
 msgstr ""
 
 msgid "The bill has been modified"
 msgstr ""
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 #, fuzzy
 msgid "Error deleting project history"
 msgstr "Ввімкнути історію проєкту"
 
 #, fuzzy
 msgid "Deleted project history."
 msgstr "Ввімкнути історію проєкту"
@@ -386,46 +396,38 @@
 
 msgid "Actions"
 msgstr ""
 
 msgid "edit"
 msgstr ""
 
-msgid "delete"
-msgstr ""
+#, fuzzy
+msgid "Delete project"
+msgstr "Створити проєкт"
 
 msgid "show"
 msgstr ""
 
 msgid "The Dashboard is currently deactivated."
 msgstr ""
 
 msgid "Download Mobile Application"
 msgstr ""
 
 #, fuzzy
 msgid "Get it on"
 msgstr "Отримати в"
 
-msgid "Are you sure?"
-msgstr ""
-
 msgid "Edit project"
 msgstr ""
 
 #, fuzzy
-msgid "Delete project"
+msgid "Import project"
 msgstr "Створити проєкт"
 
-msgid "Import JSON"
-msgstr ""
-
-msgid "Choose file"
-msgstr ""
-
 msgid "Download project's data"
 msgstr ""
 
 msgid "Bill items"
 msgstr ""
 
 msgid "Download the list of bills with owner, amount, reason,... "
@@ -442,26 +444,36 @@
 
 msgid "Cancel"
 msgstr ""
 
 msgid "Privacy Settings"
 msgstr ""
 
-msgid "Edit the project"
+msgid "Save changes"
 msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr ""
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "Імпортувати попередньо експортований JSON файл"
+
+msgid "Choose file"
+msgstr ""
+
 msgid "Edit this bill"
 msgstr ""
 
 msgid "Add a bill"
 msgstr ""
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr ""
 
 msgid "No one"
 msgstr ""
 
 msgid "More options"
@@ -472,17 +484,14 @@
 
 msgid "Edit this participant"
 msgstr ""
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr ""
 
-msgid "Send the invitations"
-msgstr ""
-
 msgid "Download"
 msgstr ""
 
 msgid "Disabled Project History"
 msgstr ""
 
 msgid "Disabled Project History & IP Address Recording"
@@ -539,51 +548,46 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr ""
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
+msgstr ""
+
+msgid "You can enable history on the settings page."
 msgstr ""
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
+msgstr ""
+
+msgid "You can clear the project history to remove them."
 msgstr ""
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr ""
 
 msgid "Delete stored IP addresses"
 msgstr ""
 
-msgid "No history to erase"
+msgid "No IP Addresses to erase"
 msgstr ""
 
-msgid "Clear Project History"
+msgid "Delete Stored IP Addresses"
 msgstr ""
 
-msgid "No IP Addresses to erase"
+msgid "No history to erase"
 msgstr ""
 
-msgid "Delete Stored IP Addresses"
+msgid "Clear Project History"
 msgstr ""
 
 msgid "Time"
 msgstr ""
 
 msgid "Event"
 msgstr ""
@@ -639,17 +643,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr ""
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr ""
 
+msgid "Payer"
+msgstr "Платник"
+
 msgid "Amount"
 msgstr ""
 
+msgid "Date"
+msgstr "Дата"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr ""
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr ""
@@ -751,15 +761,16 @@
 
 msgid "switch to"
 msgstr ""
 
 msgid "Dashboard"
 msgstr ""
 
-msgid "Logout"
+#, python-format
+msgid "Please retry after %(date)s."
 msgstr ""
 
 msgid "Code"
 msgstr ""
 
 msgid "Mobile Application"
 msgstr ""
@@ -785,46 +796,40 @@
 
 msgid "you sure?"
 msgstr ""
 
 msgid "Invite people"
 msgstr ""
 
-msgid "You should start by adding participants"
-msgstr ""
-
-msgid "Add a new bill"
-msgstr ""
-
 msgid "Newer bills"
 msgstr ""
 
 msgid "Older bills"
 msgstr ""
 
-msgid "When?"
+msgid "You should start by adding participants"
 msgstr ""
 
-msgid "Who paid?"
+msgid "Add a new bill"
 msgstr ""
 
 msgid "For what?"
 msgstr ""
 
-msgid "How much?"
-msgstr ""
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr ""
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr ""
 
+msgid "delete"
+msgstr ""
+
 msgid "No bills"
 msgstr ""
 
 msgid "Nothing to list yet."
 msgstr ""
 
 msgid "You probably want to"
@@ -869,14 +874,20 @@
 
 msgid "Share the Link"
 msgstr ""
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr ""
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr ""
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1023,7 +1034,76 @@
 #~ msgstr ""
 
 #~ msgid "Edit this member"
 #~ msgstr ""
 
 #~ msgid "Participants to notify"
 #~ msgstr ""
+
+#~ msgid "Import"
+#~ msgstr "Імпортувати"
+
+#~ msgid "Amount paid"
+#~ msgstr "Виплачувана сума"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "Рахунки не можуть бути порожніми"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "Ідентифікатор проєкту %(project)s"
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "sending you an email with password "
+#~ "reset instructions. Please check the "
+#~ "email configuration of the server or "
+#~ "contact the administrator."
+#~ msgstr ""
+
+#~ msgid "Invalid JSON"
+#~ msgstr "Недійсний JSON"
+
+#~ msgid ""
+#~ "Sorry, there was an error while "
+#~ "trying to send the invitation emails."
+#~ " Please check the email configuration "
+#~ "of the server or contact the "
+#~ "administrator."
+#~ msgstr ""
+
+#~ msgid "Are you sure?"
+#~ msgstr ""
+
+#~ msgid "Import JSON"
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+
+#~ msgid "Send invites"
+#~ msgstr "Відправити запрошення"
+
+#~ msgid " show"
+#~ msgstr ""
+
+#~ msgid "Edit the project"
+#~ msgstr ""
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/ur/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/ur/LC_MESSAGES/messages.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,28 +1,26 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Urdu (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-07-03 10:18+0000\n"
+"Last-Translator: Shafiq Azeez <fubukishirouk@gmail.com>\n"
+"Language: ur\n"
 "Language-Team: Urdu <https://hosted.weblate.org/projects/i-hate-money/i-hate-"
 "money/ur/>\n"
-"Language: ur\n"
+"Plural-Forms: nplurals=2; plural=n != 1\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.13.1-dev\n"
+"Generated-By: Babel 2.9.0\n"
 
 msgid "A link to an external document, related to this bill"
 msgstr "اس رسید کے لیے بیرونی رستاویز کا لنک"
 
-msgid "Amount paid"
-msgstr "ادا شدہ قیمت"
-
 msgid "Currency"
 msgstr "سکہ رائج الوقت (کرنسی)"
 
 msgid "Email"
 msgstr "برقی خط (ای ميل)"
 
 msgid "External link"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo` & `ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,48 +1,22 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Chinese (Simplified) (I Hate Money)\n"
+"Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"POT-Creation-Date: 2023-07-13 18:12+0200\n"
+"PO-Revision-Date: 2022-07-21 05:15+0000\n"
+"Last-Translator: z.liu <zwliu07@live.com>\n"
+"Language: zh_Hans\n"
 "Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/i-"
 "hate-money/i-hate-money/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.14-dev\n"
-
-msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to disabling "
-"project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">clear project history</a> to remove them.</i></p>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>The table below下表显示的是之前的禁用项目历史纪录 reflects "
-"actions recorded prior to disabling project history. 你可以通过\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" data-"
-"target=\"#confirm-erase\">清除项目记录</a> t来移除他们.</i></p>\n"
-"            "
-
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't appear "
-"below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
-msgstr ""
-"\n"
-"            <i>此项目历史已禁用，新操作无法显示，你可以启用历史</i>\n"
-"            <a href=\"%(url)s\">设置页面</a>\n"
-"            "
+"Generated-By: Babel 2.9.0\n"
 
 msgid "\"I hate money\" is free software"
 msgstr "“I hate money\"是一个免费软件"
 
 msgid "%(amount)s each"
 msgstr "美人%(amount)s"
 
@@ -102,34 +76,28 @@
 
 msgid "Amount"
 msgstr "数量"
 
 msgid "Amount in %(currency)s"
 msgstr "%(currency)s的数量是"
 
-msgid "Amount paid"
-msgstr "支付金额"
-
 msgid ""
 "Are you sure you want to delete all recorded IP addresses from this "
 "project?\n"
 "                The rest of the project history will be unaffected. This "
 "action cannot be undone."
 msgstr ""
 "你确定要删除此项目里所有的IP地址吗？\n"
 "项目其他内容不受影响，此操作不可撤回。"
 
 msgid ""
 "Are you sure you want to erase all history for this project? This action "
 "cannot be undone."
 msgstr "确定删除此项目所有记录？此操作不可撤回。"
 
-msgid "Are you sure?"
-msgstr "是否确定？"
-
 msgid "Back to the list"
 msgstr "返回列表"
 
 msgid "Balance"
 msgstr "余额"
 
 msgid "Bill %(name)s added"
@@ -161,17 +129,14 @@
 
 msgid "Bill items"
 msgstr "单据项目"
 
 msgid "Bills"
 msgstr "帐单"
 
-msgid "Bills can't be null"
-msgstr "数字不能为零"
-
 msgid "Can't remember the password?"
 msgstr "忘记密码？"
 
 msgid "Cancel"
 msgstr "取消"
 
 msgid ""
@@ -356,26 +321,14 @@
 
 msgid "IP address recording can be enabled on the settings page"
 msgstr "IP地址记录可在设置里启用"
 
 msgid "Identifier:"
 msgstr "标识符："
 
-msgid "Import"
-msgstr "导入"
-
-msgid "Import JSON"
-msgstr "导入json文件"
-
-msgid "Import previously exported JSON file"
-msgstr "导入之前的JSON 文件"
-
-msgid "Invalid JSON"
-msgstr "JSON无效"
-
 msgid "Invalid private code."
 msgstr "无效的私人代码。"
 
 msgid "Invalid token"
 msgstr "无效符号"
 
 msgid "Invite people"
@@ -607,28 +560,14 @@
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr "以下条目包含IP地址，但此项目禁用IP记录 "
 
 msgid "Someone probably cleared the project history."
 msgstr "某人清理了项目历史记录。"
 
-msgid ""
-"Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or contact "
-"the administrator."
-msgstr ""
-"对不起，在发送重设密码的邮件时除了错误。请检查邮件服务器的配置或者联系管理"
-"员。"
-
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. Please "
-"check the email configuration of the server or contact the administrator."
-msgstr ""
-"对不起，在发送邀请邮件时发生了错误。请检查邮箱的服务器配置或者联系管理员。"
-
 msgid "Sorry, we were unable to find the page you've asked for."
 msgstr "抱歉，我们无法找到您要求的页面。"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify about "
 "the\n"
 "                creation of this budget management project and we will send "
@@ -666,17 +605,14 @@
 
 msgid "The bill has been modified"
 msgstr "帐单已修改"
 
 msgid "The email %(email)s is not valid"
 msgstr "此邮箱%(email)s不存在"
 
-msgid "The project identifier is %(project)s"
-msgstr "项目的标识符是%(project)s"
-
 msgid "The project you are trying to access do not exist, do you want to"
 msgstr "该项目不存在，你是否要"
 
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "管理密码有误，只剩 %(num)d次尝试机会。"
 
 msgid "This private code is not the right one"
@@ -695,17 +631,14 @@
 
 msgid "Time"
 msgstr "时间"
 
 msgid "To whom?"
 msgstr "给谁？"
 
-msgid "Too many failed login attempts, please retry later."
-msgstr "登录失败次数过多，请稍后重试。"
-
 msgid "Try out the demo"
 msgstr "试试小样"
 
 msgid "Unknown error"
 msgstr "未知错误"
 
 msgid "Unknown project"
```

### Comparing `ihatemoney-6.0.0/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po` & `ihatemoney-6.0.1/ihatemoney/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
+
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-11-01 18:01+0100\n"
+"POT-Creation-Date: 2023-07-14 10:01+0200\n"
 "PO-Revision-Date: 2022-07-21 05:15+0000\n"
 "Last-Translator: z.liu <zwliu07@live.com>\n"
-"Language-Team: Chinese (Simplified) <https://hosted.weblate.org/projects/"
-"i-hate-money/i-hate-money/zh_Hans/>\n"
 "Language: zh_Hans\n"
+"Language-Team: Chinese (Simplified) "
+"<https://hosted.weblate.org/projects/i-hate-money/i-hate-money/zh_Hans/>"
+"\n"
+"Plural-Forms: nplurals=1; plural=0\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.14-dev\n"
 "Generated-By: Babel 2.9.0\n"
 
+#, python-format
+msgid "You have just created '%(project)s' to share your expenses"
+msgstr "你新建了一个‘%(project)s'来分担你的花费"
+
 msgid ""
 "Not a valid amount or expression. Only numbers and + - * / operators are "
 "accepted."
 msgstr "金额或符号无效。仅限数字与+-*/符号。"
 
 msgid "Project name"
 msgstr "账目名称"
@@ -45,19 +50,16 @@
 msgstr "设置默认货币可实现账单之间的货币转换"
 
 msgid ""
 "This project cannot be set to 'no currency' because it contains bills in "
 "multiple currencies."
 msgstr "此项目不能设置为“无货币”，因为它包含多种货币的账单。"
 
-msgid "Import previously exported JSON file"
-msgstr "导入之前的JSON 文件"
-
-msgid "Import"
-msgstr "导入"
+msgid "Compatible with Cospend"
+msgstr ""
 
 msgid "Project identifier"
 msgstr "账目名称"
 
 msgid "Private code"
 msgstr "共享密钥"
 
@@ -108,25 +110,25 @@
 
 msgid "Password confirmation"
 msgstr "密码确认"
 
 msgid "Reset password"
 msgstr "密码重置"
 
-msgid "Date"
-msgstr "日期"
+msgid "When?"
+msgstr "什么时候？"
 
 msgid "What?"
 msgstr "什么？"
 
-msgid "Payer"
-msgstr "支付人"
+msgid "Who paid?"
+msgstr "谁付的钱？"
 
-msgid "Amount paid"
-msgstr "支付金额"
+msgid "How much?"
+msgstr "多少？"
 
 msgid "Currency"
 msgstr "货币"
 
 msgid "External link"
 msgstr "外部链接"
 
@@ -142,17 +144,14 @@
 msgid "Submit and add a new one"
 msgstr "确定并添加另一个"
 
 #, python-format
 msgid "Project default: %(currency)s"
 msgstr "默认项目: %(currency)s"
 
-msgid "Bills can't be null"
-msgstr "数字不能为零"
-
 msgid "Name"
 msgstr "姓名"
 
 msgid "Weights should be positive"
 msgstr "权重必须大于零"
 
 msgid "Weight"
@@ -168,21 +167,33 @@
 #, fuzzy
 msgid "This project already have this participant"
 msgstr "此项目已经包含此成员了"
 
 msgid "People to notify"
 msgstr "需要通知的人"
 
-msgid "Send invites"
+msgid "Send the invitations"
 msgstr "发送邀请"
 
 #, python-format
 msgid "The email %(email)s is not valid"
 msgstr "此邮箱%(email)s不存在"
 
+msgid "Logout"
+msgstr "退出"
+
+msgid "Please check the email configuration of the server."
+msgstr ""
+
+#, fuzzy, python-format
+msgid ""
+"Please check the email configuration of the server or contact the "
+"administrator: %(admin_email)s"
+msgstr "对不起，在发送邀请邮件时发生了错误。请检查邮箱的服务器配置或者联系管理员。"
+
 #. List with two items only
 msgid "{dual_object_0} and {dual_object_1}"
 msgstr "{dual_object_0} 和 {dual_object_1}"
 
 #. Last two items of a list with more than 3 items
 msgid "{previous_object}, and {end_object}"
 msgstr "{previous_object} 和 {end_object}"
@@ -202,89 +213,87 @@
 msgid "{prefix}: {error}"
 msgstr "{prefix}: {error}"
 
 #. Form error with a list of errors
 msgid "{prefix}:<br />{errors}"
 msgstr "{prefix}:<br />{errors}"
 
-msgid "Too many failed login attempts, please retry later."
+#, fuzzy
+msgid "Too many failed login attempts."
 msgstr "登录失败次数过多，请稍后重试。"
 
 #, python-format
 msgid "This admin password is not the right one. Only %(num)d attempts left."
 msgstr "管理密码有误，只剩 %(num)d次尝试机会。"
 
 msgid "Provided token is invalid"
 msgstr "所提供的口令无效"
 
 msgid "This private code is not the right one"
 msgstr "专用码不正确"
 
-#, python-format
-msgid "You have just created '%(project)s' to share your expenses"
-msgstr "你新建了一个‘%(project)s'来分担你的花费"
-
 msgid "A reminder email has just been sent to you"
 msgstr "发送了提醒邮件给你"
 
 msgid ""
 "We tried to send you an reminder email, but there was an error. You can "
 "still use the project normally."
 msgstr "我们试着发送提醒邮件给你，但是出了问题。你仍可以正常使用。"
 
-#, python-format
-msgid "The project identifier is %(project)s"
-msgstr "项目的标识符是%(project)s"
-
+#, fuzzy
 msgid ""
 "Sorry, there was an error while sending you an email with password reset "
-"instructions. Please check the email configuration of the server or "
-"contact the administrator."
+"instructions."
 msgstr "对不起，在发送重设密码的邮件时除了错误。请检查邮件服务器的配置或者联系管理员。"
 
 msgid "No token provided"
 msgstr "没有符号"
 
 msgid "Invalid token"
 msgstr "无效符号"
 
 msgid "Unknown project"
 msgstr "未知项目"
 
 msgid "Password successfully reset."
 msgstr "密码重置成功。"
 
-msgid "Project successfully uploaded"
-msgstr "项目成功上传"
+msgid "Unable to parse CSV"
+msgstr ""
 
-msgid "Invalid JSON"
-msgstr "JSON无效"
+#, python-format
+msgid "Missing attribute: %(attribute)s"
+msgstr ""
 
 msgid ""
 "Cannot add bills in multiple currencies to a project without default "
 "currency"
 msgstr "无法在没有设置默认货币的项目中添加多种货币的账单"
 
+msgid "Project successfully uploaded"
+msgstr "项目成功上传"
+
 msgid "Project successfully deleted"
 msgstr "项目成功删除"
 
 msgid "Error deleting project"
 msgstr "删除项目时出错"
 
+msgid "Unable to logout"
+msgstr ""
+
 #, python-format
 msgid "You have been invited to share your expenses for %(project)s"
 msgstr "你被邀请进入 %(project)s来分担你的花费"
 
 msgid "Your invitations have been sent"
 msgstr "你的申请已发出"
 
-msgid ""
-"Sorry, there was an error while trying to send the invitation emails. "
-"Please check the email configuration of the server or contact the "
-"administrator."
+#, fuzzy
+msgid "Sorry, there was an error while trying to send the invitation emails."
 msgstr "对不起，在发送邀请邮件时发生了错误。请检查邮箱的服务器配置或者联系管理员。"
 
 #, python-format
 msgid "%(member)s has been added"
 msgstr "已添加%(member)s"
 
 #, fuzzy
@@ -321,14 +330,18 @@
 
 msgid "The bill has been deleted"
 msgstr "账单已删除"
 
 msgid "The bill has been modified"
 msgstr "帐单已修改"
 
+#, python-format
+msgid "%(lang)s is not a supported language"
+msgstr ""
+
 msgid "Error deleting project history"
 msgstr "删除项目历史记录时出错"
 
 msgid "Deleted project history."
 msgstr "已删除的项目历史记录。"
 
 msgid "Error deleting recorded IP addresses"
@@ -383,43 +396,35 @@
 
 msgid "Actions"
 msgstr "操作"
 
 msgid "edit"
 msgstr "编辑"
 
-msgid "delete"
-msgstr "删除"
+msgid "Delete project"
+msgstr "删除项目"
 
 msgid "show"
 msgstr "显示"
 
 msgid "The Dashboard is currently deactivated."
 msgstr "操作面板失效。"
 
 msgid "Download Mobile Application"
 msgstr "下载移动应用程序"
 
 msgid "Get it on"
 msgstr "获取"
 
-msgid "Are you sure?"
-msgstr "是否确定？"
-
 msgid "Edit project"
 msgstr "编辑项目"
 
-msgid "Delete project"
-msgstr "删除项目"
-
-msgid "Import JSON"
-msgstr "导入json文件"
-
-msgid "Choose file"
-msgstr "选择文件"
+#, fuzzy
+msgid "Import project"
+msgstr "编辑项目"
 
 msgid "Download project's data"
 msgstr "下载项目数据"
 
 msgid "Bill items"
 msgstr "单据项目"
 
@@ -437,26 +442,36 @@
 
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Privacy Settings"
 msgstr "隐私设置"
 
-msgid "Edit the project"
-msgstr "编辑项目"
+msgid "Save changes"
+msgstr ""
 
 msgid "This will remove all bills and participants in this project!"
 msgstr "这将删除此项目的所有账单和参与者！"
 
+#, fuzzy
+msgid "Import previously exported project"
+msgstr "导入之前的JSON 文件"
+
+msgid "Choose file"
+msgstr "选择文件"
+
 msgid "Edit this bill"
 msgstr "编辑帐单"
 
 msgid "Add a bill"
 msgstr "添加账单"
 
+msgid "Simple operations are allowed, e.g. (18+36.2)/3"
+msgstr ""
+
 msgid "Everyone"
 msgstr "每个人"
 
 msgid "No one"
 msgstr "无人"
 
 msgid "More options"
@@ -468,17 +483,14 @@
 #, fuzzy
 msgid "Edit this participant"
 msgstr "添加参与人"
 
 msgid "john.doe@example.com, mary.moe@site.com"
 msgstr "john.doe@example.com, mary.moe@site.com"
 
-msgid "Send the invitations"
-msgstr "发送邀请"
-
 msgid "Download"
 msgstr "下载"
 
 msgid "Disabled Project History"
 msgstr "禁用项目历史"
 
 msgid "Disabled Project History & IP Address Recording"
@@ -537,63 +549,50 @@
 msgid "Bill %(name)s: added %(owers_list_str)s to owers list"
 msgstr "帐单 %(name)s：将 %(owers_list_str)s 添加到所有者列表"
 
 #, python-format
 msgid "Bill %(name)s: removed %(owers_list_str)s from owers list"
 msgstr "账单 %(name)s：从所有者列表中删除了 %(owers_list_str)s"
 
-#, python-format
-msgid ""
-"\n"
-"            <i>This project has history disabled. New actions won't "
-"appear below. You can enable history on the</i>\n"
-"            <a href=\"%(url)s\">settings page</a>\n"
-"            "
+msgid "This project has history disabled. New actions won't appear below."
 msgstr ""
-"\n"
-"            <i>此项目历史已禁用，新操作无法显示，你可以启用历史</i>\n"
-"            <a href=\"%(url)s\">设置页面</a>\n"
-"            "
+
+#, fuzzy
+msgid "You can enable history on the settings page."
+msgstr "IP地址记录可在设置里启用"
 
 msgid ""
-"\n"
-"            <i>The table below reflects actions recorded prior to "
-"disabling project history. You can\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">clear project history</a> to remove "
-"them.</i></p>\n"
-"            "
+"The table below reflects actions recorded prior to disabling project "
+"history."
 msgstr ""
-"\n"
-"            <i>The table below下表显示的是之前的禁用项目历史纪录 reflects actions recorded"
-" prior to disabling project history. 你可以通过\n"
-"            <a href=\"#\" data-toggle=\"modal\" data-keyboard=\"false\" "
-"data-target=\"#confirm-erase\">清除项目记录</a> t来移除他们.</i></p>\n"
-"            "
+
+#, fuzzy
+msgid "You can clear the project history to remove them."
+msgstr "某人清理了项目历史记录。"
 
 msgid ""
 "Some entries below contain IP addresses, even though this project has IP "
 "recording disabled. "
 msgstr "以下条目包含IP地址，但此项目禁用IP记录 "
 
 msgid "Delete stored IP addresses"
 msgstr "删除已储存的IP地址"
 
-msgid "No history to erase"
-msgstr "无历史纪录"
-
-msgid "Clear Project History"
-msgstr "清除项目历史"
-
 msgid "No IP Addresses to erase"
 msgstr "无IP地址"
 
 msgid "Delete Stored IP Addresses"
 msgstr "删除已储存AP地址"
 
+msgid "No history to erase"
+msgstr "无历史纪录"
+
+msgid "Clear Project History"
+msgstr "清除项目历史"
+
 msgid "Time"
 msgstr "时间"
 
 msgid "Event"
 msgstr "事件"
 
 msgid "IP address recording can be enabled on the settings page"
@@ -647,17 +646,23 @@
 msgid "Bill %(name)s renamed to %(new_description)s"
 msgstr "账单 %(name)s 更名为 %(new_description)s"
 
 #, python-format
 msgid "Participant %(name)s: weight changed from %(old_weight)s to %(new_weight)s"
 msgstr "成员 %(name)s：权重从%(old_weight)s变为%(new_weight)s"
 
+msgid "Payer"
+msgstr "支付人"
+
 msgid "Amount"
 msgstr "数量"
 
+msgid "Date"
+msgstr "日期"
+
 #, python-format
 msgid "Amount in %(currency)s"
 msgstr "%(currency)s的数量是"
 
 #, python-format
 msgid "Bill %(name)s modified"
 msgstr "帐单 %(name)s 已修改"
@@ -759,16 +764,17 @@
 
 msgid "switch to"
 msgstr "切换到"
 
 msgid "Dashboard"
 msgstr "操作面板"
 
-msgid "Logout"
-msgstr "退出"
+#, python-format
+msgid "Please retry after %(date)s."
+msgstr ""
 
 msgid "Code"
 msgstr "代码"
 
 msgid "Mobile Application"
 msgstr "手机软件"
 
@@ -794,46 +800,40 @@
 
 msgid "you sure?"
 msgstr "确定？"
 
 msgid "Invite people"
 msgstr "邀请别人"
 
-msgid "You should start by adding participants"
-msgstr "从添加参与人开始"
-
-msgid "Add a new bill"
-msgstr "添加新帐单"
-
 msgid "Newer bills"
 msgstr "最新账单"
 
 msgid "Older bills"
 msgstr "最旧帐单"
 
-msgid "When?"
-msgstr "什么时候？"
+msgid "You should start by adding participants"
+msgstr "从添加参与人开始"
 
-msgid "Who paid?"
-msgstr "谁付的钱？"
+msgid "Add a new bill"
+msgstr "添加新帐单"
 
 msgid "For what?"
 msgstr "什么东西？"
 
-msgid "How much?"
-msgstr "多少？"
-
 #, python-format
 msgid "Added on %(date)s"
 msgstr "添加到%(date)s"
 
 #, python-format
 msgid "Everyone but %(excluded)s"
 msgstr "除了%(excluded)s的每个人"
 
+msgid "delete"
+msgstr "删除"
+
 msgid "No bills"
 msgstr "没有账单"
 
 msgid "Nothing to list yet."
 msgstr "没有列表。"
 
 msgid "You probably want to"
@@ -878,14 +878,20 @@
 
 msgid "Share the Link"
 msgstr "分享链接"
 
 msgid "You can directly share the following link via your prefered medium"
 msgstr "你可以直接通过你喜欢的媒体分享链接"
 
+msgid "Scan QR code"
+msgstr ""
+
+msgid "Use a mobile device with a compatible app."
+msgstr ""
+
 msgid "Send via Emails"
 msgstr "邮件发送"
 
 msgid ""
 "Specify a (comma separated) list of email adresses you want to notify "
 "about the\n"
 "                creation of this budget management project and we will "
@@ -1013,7 +1019,73 @@
 #~ msgstr "会员人数"
 
 #~ msgid "Edit this member"
 #~ msgstr "编辑成员"
 
 #~ msgid "Participants to notify"
 #~ msgstr "添加参与人"
+
+#~ msgid "Import"
+#~ msgstr "导入"
+
+#~ msgid "Amount paid"
+#~ msgstr "支付金额"
+
+#~ msgid "Bills can't be null"
+#~ msgstr "数字不能为零"
+
+#~ msgid "The project identifier is %(project)s"
+#~ msgstr "项目的标识符是%(project)s"
+
+#~ msgid "Invalid JSON"
+#~ msgstr "JSON无效"
+
+#~ msgid "Are you sure?"
+#~ msgstr "是否确定？"
+
+#~ msgid "Import JSON"
+#~ msgstr "导入json文件"
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>This project has history "
+#~ "disabled. New actions won't appear "
+#~ "below. You can enable history on "
+#~ "the</i>\n"
+#~ "            <a href=\"%(url)s\">settings page</a>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>此项目历史已禁用，新操作无法显示，你可以启用历史</i>\n"
+#~ "            <a href=\"%(url)s\">设置页面</a>\n"
+#~ "            "
+
+#~ msgid ""
+#~ "\n"
+#~ "            <i>The table below reflects "
+#~ "actions recorded prior to disabling "
+#~ "project history. You can\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">clear project history</a>"
+#~ " to remove them.</i></p>\n"
+#~ "            "
+#~ msgstr ""
+#~ "\n"
+#~ "            <i>The table below下表显示的是之前的禁用项目历史纪录 "
+#~ "reflects actions recorded prior to "
+#~ "disabling project history. 你可以通过\n"
+#~ "            <a href=\"#\" data-"
+#~ "toggle=\"modal\" data-keyboard=\"false\" data-"
+#~ "target=\"#confirm-erase\">清除项目记录</a> t来移除他们.</i></p>\n"
+#~ ""
+#~ "            "
+
+#~ msgid "Send invites"
+#~ msgstr "发送邀请"
+
+#~ msgid " show"
+#~ msgstr "显示"
+
+#~ msgid "Edit the project"
+#~ msgstr "编辑项目"
+
```

### Comparing `ihatemoney-6.0.0/ihatemoney/utils.py` & `ihatemoney-6.0.1/ihatemoney/utils.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/versioning.py` & `ihatemoney-6.0.1/ihatemoney/versioning.py`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney/web.py` & `ihatemoney-6.0.1/ihatemoney/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,21 @@
     if "project_id" in values or not hasattr(g, "project"):
         return
     if current_app.url_map.is_endpoint_expecting(endpoint, "project_id"):
         values["project_id"] = g.project.id
 
 
 @main.url_value_preprocessor
+def migrate_session(endpoint, values):
+    if "projects" in session and isinstance(session["projects"], list):
+        # Migrate https://github.com/spiral-project/ihatemoney/pull/1082
+        session["projects"] = {id: name for (id, name) in session["projects"]}
+
+
+@main.url_value_preprocessor
 def set_show_admin_dashboard_link(endpoint, values):
     """Sets the "show_admin_dashboard_link" variable application wide
     in order to use it in the layout template.
     """
 
     g.show_admin_dashboard_link = (
         current_app.config["ACTIVATE_ADMIN_DASHBOARD"]
@@ -318,16 +325,15 @@
         if form.validate():
             # save the object in the db
             project = form.save()
             db.session.add(project)
             db.session.commit()
 
             # create the session object (authenticate)
-            session[project.id] = True
-            session.update()
+            set_authorized_project(project)
 
             # send reminder email
             g.project = project
             success = send_creation_email(project)
             if success:
                 flash(
                     _("A reminder email has just been sent to you"), category="success"
```

### Comparing `ihatemoney-6.0.0/ihatemoney.egg-info/PKG-INFO` & `ihatemoney-6.0.1/ihatemoney.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihatemoney
-Version: 6.0.0
+Version: 6.0.1
 Summary: A simple shared budget manager web application.
 Home-page: https://github.com/spiral-project/ihatemoney
 Author: Alexis Métaireau & contributors
 Author-email: alexis@notmyidea.org
 License: Custom BSD Beerware
 Description: UNKNOWN
 Keywords: web,budget
```

### Comparing `ihatemoney-6.0.0/ihatemoney.egg-info/SOURCES.txt` & `ihatemoney-6.0.1/ihatemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/ihatemoney.egg-info/requires.txt` & `ihatemoney-6.0.1/ihatemoney.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ihatemoney-6.0.0/setup.cfg` & `ihatemoney-6.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ihatemoney
-version = 6.0.0
+version = 6.0.1
 url = https://github.com/spiral-project/ihatemoney
 description = A simple shared budget manager web application.
 long_description = file: README.rst, CHANGELOG.rst
 author = Alexis Métaireau & contributors
 author_email = alexis@notmyidea.org
 keywords = web, budget
 license = Custom BSD Beerware
```

