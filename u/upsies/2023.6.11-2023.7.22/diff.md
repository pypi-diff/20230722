# Comparing `tmp/upsies-2023.6.11.tar.gz` & `tmp/upsies-2023.7.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upsies-2023.6.11.tar", last modified: Sun Jun 11 11:33:55 2023, max compression
+gzip compressed data, was "upsies-2023.7.22.tar", last modified: Sat Jul 22 15:06:37 2023, max compression
```

## Comparing `upsies-2023.6.11.tar` & `upsies-2023.7.22.tar`

### file list

```diff
@@ -1,259 +1,259 @@
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.966841 upsies-2023.6.11/
--rw-------   0 ich       (1000) ich       (1000)    35149 2021-06-11 16:56:53.000000 upsies-2023.6.11/LICENSE
--rw-------   0 ich       (1000) ich       (1000)     2637 2023-06-11 11:33:55.966841 upsies-2023.6.11/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     1815 2023-04-25 13:55:04.000000 upsies-2023.6.11/README.rst
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.754842 upsies-2023.6.11/docs/
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.754842 upsies-2023.6.11/docs/_ext/
--rw-------   0 ich       (1000) ich       (1000)     2805 2021-10-10 10:59:55.000000 upsies-2023.6.11/docs/_ext/cli_reference.py
--rw-------   0 ich       (1000) ich       (1000)      571 2023-04-25 13:55:04.000000 upsies-2023.6.11/docs/conf.py
--rw-------   0 ich       (1000) ich       (1000)     1772 2023-06-11 11:33:26.000000 upsies-2023.6.11/pyproject.toml
--rw-------   0 ich       (1000) ich       (1000)       38 2023-06-11 11:33:55.966841 upsies-2023.6.11/setup.cfg
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.758842 upsies-2023.6.11/tests/
--rw-------   0 ich       (1000) ich       (1000)     1598 2023-05-26 17:05:24.000000 upsies-2023.6.11/tests/conftest.py
--rw-------   0 ich       (1000) ich       (1000)     3565 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/errors_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.778842 upsies-2023.6.11/tests/jobs_test/
--rw-------   0 ich       (1000) ich       (1000)     3036 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/jobs_test/add_torrent_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    18181 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/choice_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     4769 2023-01-16 18:34:35.000000 upsies-2023.6.11/tests/jobs_test/copy_torrent_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    18147 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/jobs_test/create_torrent_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     4787 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/custom_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     4769 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/imghost_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    36618 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/job_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    30782 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/mediainfo_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    15638 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/poster_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     7757 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/queue_job_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    18248 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/scene_check_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     3547 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/scene_search_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    35363 2023-05-25 13:46:48.000000 upsies-2023.6.11/tests/jobs_test/screenshots_job_test.py
--rw-------   0 ich       (1000) ich       (1000)     5619 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/set_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    12625 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/jobs_test/submit_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    14134 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/jobs_test/text_field_job_test.py
--rw-------   0 ich       (1000) ich       (1000)    27694 2023-05-26 17:03:17.000000 upsies-2023.6.11/tests/jobs_test/webdb_search_job_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.782842 upsies-2023.6.11/tests/trackers_test/
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.782842 upsies-2023.6.11/tests/trackers_test/base/
--rw-------   0 ich       (1000) ich       (1000)     3420 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_base_howto_test.py
--rw-------   0 ich       (1000) ich       (1000)     6319 2023-04-25 14:57:27.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_base_test.py
--rw-------   0 ich       (1000) ich       (1000)     6206 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_config_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    69602 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/base/tracker_jobs_base_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.790842 upsies-2023.6.11/tests/trackers_test/bhd/
--rw-------   0 ich       (1000) ich       (1000)     5905 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)    28649 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)    11005 2023-04-25 14:57:27.000000 upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_test.py
--rw-------   0 ich       (1000) ich       (1000)     1347 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/conftest.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.798842 upsies-2023.6.11/tests/trackers_test/mtv/
--rw-------   0 ich       (1000) ich       (1000)     4438 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)    31545 2023-06-06 17:48:16.000000 upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)    31622 2023-04-25 14:57:27.000000 upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.802842 upsies-2023.6.11/tests/trackers_test/nbl/
--rw-------   0 ich       (1000) ich       (1000)     1577 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)     4726 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_jobs_test.py
--rw-------   0 ich       (1000) ich       (1000)     6113 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.806842 upsies-2023.6.11/tests/trackers_test/ptp/
--rw-------   0 ich       (1000) ich       (1000)     4113 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/ptp/ptp_tracker_config_test.py
--rw-------   0 ich       (1000) ich       (1000)    31683 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/trackers_test/ptp/ptp_tracker_test.py
--rw-------   0 ich       (1000) ich       (1000)     1916 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/trackers_test/trackers_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.750842 upsies-2023.6.11/tests/uis_test/
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.810842 upsies-2023.6.11/tests/uis_test/tui_test/
--rw-------   0 ich       (1000) ich       (1000)    21480 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/uis_test/tui_test/tui_test.py
--rw-------   0 ich       (1000) ich       (1000)     1425 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/uis_test/tui_test/tui_utils_test.py
--rw-------   0 ich       (1000) ich       (1000)     4429 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/uis_test/tui_test/tui_widgets_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.846841 upsies-2023.6.11/tests/utils_test/
--rw-------   0 ich       (1000) ich       (1000)     9433 2023-05-25 09:31:21.000000 upsies-2023.6.11/tests/utils_test/argtypes_test.py
--rw-------   0 ich       (1000) ich       (1000)     9133 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/utils_test/btclient_test.py
--rw-------   0 ich       (1000) ich       (1000)    35526 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/configfiles_test.py
--rw-------   0 ich       (1000) ich       (1000)     1266 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/country_test.py
--rw-------   0 ich       (1000) ich       (1000)     9048 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/daemon_test.py
--rw-------   0 ich       (1000) ich       (1000)    31470 2023-06-11 08:46:28.000000 upsies-2023.6.11/tests/utils_test/fs_test.py
--rw-------   0 ich       (1000) ich       (1000)     3723 2023-04-28 07:24:11.000000 upsies-2023.6.11/tests/utils_test/html_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.854842 upsies-2023.6.11/tests/utils_test/http_test/
--rw-------   0 ich       (1000) ich       (1000)     1474 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/http_test/conftest.py
--rw-------   0 ich       (1000) ich       (1000)    54514 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/http_test/http_test.py
--rw-------   0 ich       (1000) ich       (1000)     1233 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/http_test/http_tls_test.py
--rw-------   0 ich       (1000) ich       (1000)     1750 2023-05-25 13:46:48.000000 upsies-2023.6.11/tests/utils_test/image_optimize_test.py
--rw-------   0 ich       (1000) ich       (1000)     7391 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/image_resize_test.py
--rw-------   0 ich       (1000) ich       (1000)    12900 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/image_screenshot_test.py
--rw-------   0 ich       (1000) ich       (1000)      425 2021-07-26 09:11:09.000000 upsies-2023.6.11/tests/utils_test/image_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.854842 upsies-2023.6.11/tests/utils_test/imghosts_test/
--rw-------   0 ich       (1000) ich       (1000)     3390 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/freeimage_test.py
--rw-------   0 ich       (1000) ich       (1000)     3690 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imgbb_test.py
--rw-------   0 ich       (1000) ich       (1000)     1932 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imgbox_test.py
--rw-------   0 ich       (1000) ich       (1000)    14346 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_base_test.py
--rw-------   0 ich       (1000) ich       (1000)     3055 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_common_test.py
--rw-------   0 ich       (1000) ich       (1000)     2791 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_test.py
--rw-------   0 ich       (1000) ich       (1000)     6927 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/imghosts_test/ptpimg_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.866841 upsies-2023.6.11/tests/utils_test/predbs_test/
--rw-------   0 ich       (1000) ich       (1000)     1173 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/conftest.py
--rw-------   0 ich       (1000) ich       (1000)     6369 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/corruptnet_test.py
--rw-------   0 ich       (1000) ich       (1000)     5723 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbclub_test.py
--rw-------   0 ich       (1000) ich       (1000)     6719 2023-06-11 11:33:26.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbde_test.py
--rw-------   0 ich       (1000) ich       (1000)     5710 2023-05-29 17:37:37.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbovh_test.py
--rw-------   0 ich       (1000) ich       (1000)     8255 2023-06-06 17:48:16.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_base_test.py
--rw-------   0 ich       (1000) ich       (1000)     8539 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_common_test.py
--rw-------   0 ich       (1000) ich       (1000)    49224 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_integration_test.py
--rw-------   0 ich       (1000) ich       (1000)    22846 2023-06-05 13:33:01.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_multi_test.py
--rw-------   0 ich       (1000) ich       (1000)     1900 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/predbs_test/predbs_test.py
--rw-------   0 ich       (1000) ich       (1000)    22438 2023-05-31 14:49:34.000000 upsies-2023.6.11/tests/utils_test/predbs_test/srrdb_test.py
--rw-------   0 ich       (1000) ich       (1000)     9604 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/release_episodes_test.py
--rw-------   0 ich       (1000) ich       (1000)    31672 2023-06-01 13:28:44.000000 upsies-2023.6.11/tests/utils_test/release_info_test.py
--rw-------   0 ich       (1000) ich       (1000)    64364 2023-06-06 17:48:16.000000 upsies-2023.6.11/tests/utils_test/release_name_test.py
--rw-------   0 ich       (1000) ich       (1000)     5455 2021-09-30 12:51:20.000000 upsies-2023.6.11/tests/utils_test/signal_test.py
--rw-------   0 ich       (1000) ich       (1000)     9667 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/string_test.py
--rw-------   0 ich       (1000) ich       (1000)     2695 2023-03-13 14:34:58.000000 upsies-2023.6.11/tests/utils_test/subproc_test.py
--rw-------   0 ich       (1000) ich       (1000)    11884 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/subtitle_test.py
--rw-------   0 ich       (1000) ich       (1000)     3156 2021-06-11 16:56:53.000000 upsies-2023.6.11/tests/utils_test/timestamp_test.py
--rw-------   0 ich       (1000) ich       (1000)    30246 2023-05-26 16:44:13.000000 upsies-2023.6.11/tests/utils_test/torrent_test.py
--rw-------   0 ich       (1000) ich       (1000)    14894 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/types_test.py
--rw-------   0 ich       (1000) ich       (1000)     5089 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/update_test.py
--rw-------   0 ich       (1000) ich       (1000)    13913 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/utils_test.py
--rw-------   0 ich       (1000) ich       (1000)    72586 2023-06-01 13:28:44.000000 upsies-2023.6.11/tests/utils_test/video_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.874841 upsies-2023.6.11/tests/utils_test/webdbs_test/
--rw-------   0 ich       (1000) ich       (1000)     1423 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/conftest.py
--rw-------   0 ich       (1000) ich       (1000)    37489 2023-04-28 13:26:51.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/imdb_test.py
--rw-------   0 ich       (1000) ich       (1000)    20288 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/tmdb_test.py
--rw-------   0 ich       (1000) ich       (1000)    25066 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/tvmaze_test.py
--rw-------   0 ich       (1000) ich       (1000)     4812 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_base_test.py
--rw-------   0 ich       (1000) ich       (1000)    19231 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_common_test.py
--rw-------   0 ich       (1000) ich       (1000)     1903 2023-04-25 13:55:04.000000 upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_test.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.878841 upsies-2023.6.11/upsies/
--rw-------   0 ich       (1000) ich       (1000)     1117 2023-06-11 11:33:26.000000 upsies-2023.6.11/upsies/__init__.py
--rw-------   0 ich       (1000) ich       (1000)       73 2022-03-13 08:26:06.000000 upsies-2023.6.11/upsies/__main__.py
--rw-------   0 ich       (1000) ich       (1000)     1399 2023-03-19 11:08:21.000000 upsies-2023.6.11/upsies/constants.py
--rw-------   0 ich       (1000) ich       (1000)     2058 2023-05-26 09:17:09.000000 upsies-2023.6.11/upsies/defaults.py
--rw-------   0 ich       (1000) ich       (1000)     6274 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/errors.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.886841 upsies-2023.6.11/upsies/jobs/
--rw-------   0 ich       (1000) ich       (1000)      215 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    27889 2023-06-05 13:24:27.000000 upsies-2023.6.11/upsies/jobs/base.py
--rw-------   0 ich       (1000) ich       (1000)     2165 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/custom.py
--rw-------   0 ich       (1000) ich       (1000)    21011 2023-06-01 14:38:39.000000 upsies-2023.6.11/upsies/jobs/dialog.py
--rw-------   0 ich       (1000) ich       (1000)     3707 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/imghost.py
--rw-------   0 ich       (1000) ich       (1000)     4807 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     7596 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/poster.py
--rw-------   0 ich       (1000) ich       (1000)     8681 2023-06-05 13:24:22.000000 upsies-2023.6.11/upsies/jobs/scene.py
--rw-------   0 ich       (1000) ich       (1000)    17965 2023-05-25 13:46:48.000000 upsies-2023.6.11/upsies/jobs/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     2770 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/jobs/set.py
--rw-------   0 ich       (1000) ich       (1000)     7977 2023-06-05 13:23:49.000000 upsies-2023.6.11/upsies/jobs/submit.py
--rw-------   0 ich       (1000) ich       (1000)    13075 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/jobs/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    13899 2023-06-01 14:34:49.000000 upsies-2023.6.11/upsies/jobs/webdb.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.886841 upsies-2023.6.11/upsies/trackers/
--rw-------   0 ich       (1000) ich       (1000)     1385 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.894841 upsies-2023.6.11/upsies/trackers/base/
--rw-------   0 ich       (1000) ich       (1000)      149 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/base/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3222 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/trackers/base/_howto.py
--rw-------   0 ich       (1000) ich       (1000)     3102 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/trackers/base/config.py
--rw-------   0 ich       (1000) ich       (1000)    33425 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/trackers/base/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     5985 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/base/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.898841 upsies-2023.6.11/upsies/trackers/bhd/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.6.11/upsies/trackers/bhd/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     3643 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/bhd/config.py
--rw-------   0 ich       (1000) ich       (1000)    15623 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/bhd/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     6243 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/bhd/tracker.py
--rw-------   0 ich       (1000) ich       (1000)     3647 2023-05-26 15:12:26.000000 upsies-2023.6.11/upsies/trackers/dummy.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.902841 upsies-2023.6.11/upsies/trackers/mtv/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/mtv/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2306 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/mtv/config.py
--rw-------   0 ich       (1000) ich       (1000)    10049 2023-06-06 17:48:16.000000 upsies-2023.6.11/upsies/trackers/mtv/jobs.py
--rw-------   0 ich       (1000) ich       (1000)    12862 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/mtv/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.906841 upsies-2023.6.11/upsies/trackers/nbl/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.6.11/upsies/trackers/nbl/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     1059 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/nbl/config.py
--rw-------   0 ich       (1000) ich       (1000)     1855 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/nbl/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     3969 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/nbl/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.914841 upsies-2023.6.11/upsies/trackers/ptp/
--rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/ptp/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     2146 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/trackers/ptp/config.py
--rw-------   0 ich       (1000) ich       (1000)    27925 2023-05-25 09:30:06.000000 upsies-2023.6.11/upsies/trackers/ptp/jobs.py
--rw-------   0 ich       (1000) ich       (1000)     2001 2023-04-25 14:57:27.000000 upsies-2023.6.11/upsies/trackers/ptp/metadata.py
--rw-------   0 ich       (1000) ich       (1000)    15920 2023-04-28 13:48:23.000000 upsies-2023.6.11/upsies/trackers/ptp/tracker.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.914841 upsies-2023.6.11/upsies/uis/
--rw-------   0 ich       (1000) ich       (1000)       24 2021-06-11 16:55:41.000000 upsies-2023.6.11/upsies/uis/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.922841 upsies-2023.6.11/upsies/uis/tui/
--rw-------   0 ich       (1000) ich       (1000)       55 2022-03-13 08:25:17.000000 upsies-2023.6.11/upsies/uis/tui/__init__.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.926841 upsies-2023.6.11/upsies/uis/tui/commands/
--rw-------   0 ich       (1000) ich       (1000)     1319 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/__init__.py
--rw-------   0 ich       (1000) ich       (1000)    15239 2023-06-07 15:27:08.000000 upsies-2023.6.11/upsies/uis/tui/commands/base.py
--rw-------   0 ich       (1000) ich       (1000)     1942 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     3500 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/poster.py
--rw-------   0 ich       (1000) ich       (1000)     2513 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/release_name.py
--rw-------   0 ich       (1000) ich       (1000)     2710 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/scene.py
--rw-------   0 ich       (1000) ich       (1000)     4546 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/uis/tui/commands/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)     5152 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/set.py
--rw-------   0 ich       (1000) ich       (1000)     8323 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/uis/tui/commands/submit.py
--rw-------   0 ich       (1000) ich       (1000)     8424 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/uis/tui/commands/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/upload_images.py
--rw-------   0 ich       (1000) ich       (1000)     1799 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/commands/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     3061 2022-03-13 08:27:19.000000 upsies-2023.6.11/upsies/uis/tui/headless.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.930841 upsies-2023.6.11/upsies/uis/tui/jobwidgets/
--rw-------   0 ich       (1000) ich       (1000)      947 2021-06-11 16:56:53.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     6992 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/base.py
--rw-------   0 ich       (1000) ich       (1000)      252 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/config.py
--rw-------   0 ich       (1000) ich       (1000)      202 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/custom.py
--rw-------   0 ich       (1000) ich       (1000)     1902 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/dialog.py
--rw-------   0 ich       (1000) ich       (1000)      767 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/imghost.py
--rw-------   0 ich       (1000) ich       (1000)      205 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/mediainfo.py
--rw-------   0 ich       (1000) ich       (1000)     1105 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/poster.py
--rw-------   0 ich       (1000) ich       (1000)     4143 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/scene.py
--rw-------   0 ich       (1000) ich       (1000)     1649 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/screenshots.py
--rw-------   0 ich       (1000) ich       (1000)      686 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/submit.py
--rw-------   0 ich       (1000) ich       (1000)     8671 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/torrent.py
--rw-------   0 ich       (1000) ich       (1000)     9727 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/jobwidgets/webdb.py
--rw-------   0 ich       (1000) ich       (1000)     2865 2023-06-07 15:14:22.000000 upsies-2023.6.11/upsies/uis/tui/main.py
--rw-------   0 ich       (1000) ich       (1000)     1345 2022-10-25 10:31:19.000000 upsies-2023.6.11/upsies/uis/tui/style.py
--rw-------   0 ich       (1000) ich       (1000)     9795 2023-06-05 13:36:26.000000 upsies-2023.6.11/upsies/uis/tui/tui.py
--rw-------   0 ich       (1000) ich       (1000)      626 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/utils.py
--rw-------   0 ich       (1000) ich       (1000)    13814 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/uis/tui/widgets.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.950841 upsies-2023.6.11/upsies/utils/
--rw-------   0 ich       (1000) ich       (1000)    13326 2023-06-05 13:36:24.000000 upsies-2023.6.11/upsies/utils/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     5658 2023-05-25 09:31:21.000000 upsies-2023.6.11/upsies/utils/argtypes.py
--rw-------   0 ich       (1000) ich       (1000)      302 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/browser.py
--rw-------   0 ich       (1000) ich       (1000)     4303 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/utils/btclient.py
--rw-------   0 ich       (1000) ich       (1000)    15025 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/configfiles.py
--rw-------   0 ich       (1000) ich       (1000)     1825 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/country.py
--rw-------   0 ich       (1000) ich       (1000)     7285 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/daemon.py
--rw-------   0 ich       (1000) ich       (1000)    17924 2023-06-11 11:33:26.000000 upsies-2023.6.11/upsies/utils/fs.py
--rw-------   0 ich       (1000) ich       (1000)     2353 2023-05-25 13:46:48.000000 upsies-2023.6.11/upsies/utils/html.py
--rw-------   0 ich       (1000) ich       (1000)    23553 2023-05-26 16:34:04.000000 upsies-2023.6.11/upsies/utils/http.py
--rw-------   0 ich       (1000) ich       (1000)    10178 2023-05-25 13:46:48.000000 upsies-2023.6.11/upsies/utils/image.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.954841 upsies-2023.6.11/upsies/utils/imghosts/
--rw-------   0 ich       (1000) ich       (1000)     1391 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/imghosts/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     7453 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/imghosts/base.py
--rw-------   0 ich       (1000) ich       (1000)     1147 2021-06-11 16:56:53.000000 upsies-2023.6.11/upsies/utils/imghosts/common.py
--rw-------   0 ich       (1000) ich       (1000)     1011 2021-10-31 14:15:29.000000 upsies-2023.6.11/upsies/utils/imghosts/dummy.py
--rw-------   0 ich       (1000) ich       (1000)     1997 2021-11-27 15:46:37.000000 upsies-2023.6.11/upsies/utils/imghosts/freeimage.py
--rw-------   0 ich       (1000) ich       (1000)     2517 2021-11-26 16:53:37.000000 upsies-2023.6.11/upsies/utils/imghosts/imgbb.py
--rw-------   0 ich       (1000) ich       (1000)      912 2021-10-19 13:17:48.000000 upsies-2023.6.11/upsies/utils/imghosts/imgbox.py
--rw-------   0 ich       (1000) ich       (1000)     3154 2023-04-23 11:00:43.000000 upsies-2023.6.11/upsies/utils/imghosts/ptpimg.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.958841 upsies-2023.6.11/upsies/utils/predbs/
--rw-------   0 ich       (1000) ich       (1000)     1364 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/predbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     9619 2023-06-06 17:48:16.000000 upsies-2023.6.11/upsies/utils/predbs/base.py
--rw-------   0 ich       (1000) ich       (1000)     4128 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/predbs/common.py
--rw-------   0 ich       (1000) ich       (1000)     2278 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/corruptnet.py
--rw-------   0 ich       (1000) ich       (1000)    20881 2023-06-05 13:43:50.000000 upsies-2023.6.11/upsies/utils/predbs/multi.py
--rw-------   0 ich       (1000) ich       (1000)     2176 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/predbclub.py
--rw-------   0 ich       (1000) ich       (1000)     2414 2023-06-11 11:33:26.000000 upsies-2023.6.11/upsies/utils/predbs/predbde.py
--rw-------   0 ich       (1000) ich       (1000)     2169 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/predbovh.py
--rw-------   0 ich       (1000) ich       (1000)     5425 2023-05-29 17:37:37.000000 upsies-2023.6.11/upsies/utils/predbs/query.py
--rw-------   0 ich       (1000) ich       (1000)     6654 2023-05-31 14:49:34.000000 upsies-2023.6.11/upsies/utils/predbs/srrdb.py
--rw-------   0 ich       (1000) ich       (1000)    56212 2023-06-01 13:28:44.000000 upsies-2023.6.11/upsies/utils/release.py
--rw-------   0 ich       (1000) ich       (1000)     3931 2023-02-19 13:31:01.000000 upsies-2023.6.11/upsies/utils/signal.py
--rw-------   0 ich       (1000) ich       (1000)     3922 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/string.py
--rw-------   0 ich       (1000) ich       (1000)     1908 2023-03-31 14:19:32.000000 upsies-2023.6.11/upsies/utils/subproc.py
--rw-------   0 ich       (1000) ich       (1000)     7760 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/subtitle.py
--rw-------   0 ich       (1000) ich       (1000)     2034 2021-09-23 10:04:01.000000 upsies-2023.6.11/upsies/utils/timestamp.py
--rw-------   0 ich       (1000) ich       (1000)    19315 2023-05-26 16:44:13.000000 upsies-2023.6.11/upsies/utils/torrent.py
--rw-------   0 ich       (1000) ich       (1000)    11165 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/types.py
--rw-------   0 ich       (1000) ich       (1000)     2927 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/update.py
--rw-------   0 ich       (1000) ich       (1000)    35111 2023-06-01 13:28:44.000000 upsies-2023.6.11/upsies/utils/video.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.962841 upsies-2023.6.11/upsies/utils/webdbs/
--rw-------   0 ich       (1000) ich       (1000)     1140 2023-01-16 18:31:24.000000 upsies-2023.6.11/upsies/utils/webdbs/__init__.py
--rw-------   0 ich       (1000) ich       (1000)     8898 2023-04-28 13:26:45.000000 upsies-2023.6.11/upsies/utils/webdbs/base.py
--rw-------   0 ich       (1000) ich       (1000)    12546 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/webdbs/common.py
--rw-------   0 ich       (1000) ich       (1000)    17839 2023-04-28 13:48:23.000000 upsies-2023.6.11/upsies/utils/webdbs/imdb.py
--rw-------   0 ich       (1000) ich       (1000)    12105 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/webdbs/tmdb.py
--rw-------   0 ich       (1000) ich       (1000)     9757 2023-04-25 13:55:04.000000 upsies-2023.6.11/upsies/utils/webdbs/tvmaze.py
-drwx------   0 ich       (1000) ich       (1000)        0 2023-06-11 11:33:55.878841 upsies-2023.6.11/upsies.egg-info/
--rw-------   0 ich       (1000) ich       (1000)     2637 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/PKG-INFO
--rw-------   0 ich       (1000) ich       (1000)     7413 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/SOURCES.txt
--rw-------   0 ich       (1000) ich       (1000)        1 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/dependency_links.txt
--rw-------   0 ich       (1000) ich       (1000)       47 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/entry_points.txt
--rw-------   0 ich       (1000) ich       (1000)      320 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/requires.txt
--rw-------   0 ich       (1000) ich       (1000)       65 2023-06-11 11:33:55.000000 upsies-2023.6.11/upsies.egg-info/top_level.txt
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.602943 upsies-2023.7.22/
+-rw-------   0 ich       (1000) ich       (1000)    35149 2023-07-03 13:15:51.000000 upsies-2023.7.22/LICENSE
+-rw-------   0 ich       (1000) ich       (1000)     2637 2023-07-22 15:06:37.602943 upsies-2023.7.22/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     1815 2023-04-25 13:55:04.000000 upsies-2023.7.22/README.rst
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.550943 upsies-2023.7.22/docs/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.550943 upsies-2023.7.22/docs/_ext/
+-rw-------   0 ich       (1000) ich       (1000)     2805 2021-10-10 10:59:55.000000 upsies-2023.7.22/docs/_ext/cli_reference.py
+-rw-------   0 ich       (1000) ich       (1000)      571 2023-04-25 13:55:04.000000 upsies-2023.7.22/docs/conf.py
+-rw-------   0 ich       (1000) ich       (1000)     1772 2023-06-11 11:33:26.000000 upsies-2023.7.22/pyproject.toml
+-rw-------   0 ich       (1000) ich       (1000)       38 2023-07-22 15:06:37.602943 upsies-2023.7.22/setup.cfg
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.550943 upsies-2023.7.22/tests/
+-rw-------   0 ich       (1000) ich       (1000)     1598 2023-05-26 17:05:24.000000 upsies-2023.7.22/tests/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     3565 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/errors_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.554943 upsies-2023.7.22/tests/jobs_test/
+-rw-------   0 ich       (1000) ich       (1000)     3036 2023-05-26 16:44:13.000000 upsies-2023.7.22/tests/jobs_test/add_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18181 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/choice_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4769 2023-01-16 18:34:35.000000 upsies-2023.7.22/tests/jobs_test/copy_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18147 2023-05-26 16:44:13.000000 upsies-2023.7.22/tests/jobs_test/create_torrent_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4787 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/custom_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4769 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/imghost_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    36618 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/job_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    30782 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/mediainfo_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    15638 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/poster_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7757 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/queue_job_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    18248 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/scene_check_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3547 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/scene_search_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    35363 2023-05-25 13:46:48.000000 upsies-2023.7.22/tests/jobs_test/screenshots_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5619 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/set_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    12625 2023-05-25 09:31:21.000000 upsies-2023.7.22/tests/jobs_test/submit_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14134 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/jobs_test/text_field_job_test.py
+-rw-------   0 ich       (1000) ich       (1000)    27694 2023-05-26 17:03:17.000000 upsies-2023.7.22/tests/jobs_test/webdb_search_job_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.554943 upsies-2023.7.22/tests/trackers_test/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.554943 upsies-2023.7.22/tests/trackers_test/base/
+-rw-------   0 ich       (1000) ich       (1000)     3420 2023-05-25 09:31:21.000000 upsies-2023.7.22/tests/trackers_test/base/tracker_base_howto_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6319 2023-04-25 14:57:27.000000 upsies-2023.7.22/tests/trackers_test/base/tracker_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6206 2023-05-25 09:31:21.000000 upsies-2023.7.22/tests/trackers_test/base/tracker_config_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    69602 2023-05-25 09:31:21.000000 upsies-2023.7.22/tests/trackers_test/base/tracker_jobs_base_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.558943 upsies-2023.7.22/tests/trackers_test/bhd/
+-rw-------   0 ich       (1000) ich       (1000)     5905 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/bhd/bhd_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    28649 2023-05-25 09:31:21.000000 upsies-2023.7.22/tests/trackers_test/bhd/bhd_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    11005 2023-04-25 14:57:27.000000 upsies-2023.7.22/tests/trackers_test/bhd/bhd_tracker_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1347 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/conftest.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.558943 upsies-2023.7.22/tests/trackers_test/mtv/
+-rw-------   0 ich       (1000) ich       (1000)     4438 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/mtv/mtv_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    33087 2023-07-22 15:04:27.000000 upsies-2023.7.22/tests/trackers_test/mtv/mtv_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31622 2023-04-25 14:57:27.000000 upsies-2023.7.22/tests/trackers_test/mtv/mtv_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.558943 upsies-2023.7.22/tests/trackers_test/nbl/
+-rw-------   0 ich       (1000) ich       (1000)     1577 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/nbl/nbl_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4726 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/nbl/nbl_tracker_jobs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6113 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/nbl/nbl_tracker_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.558943 upsies-2023.7.22/tests/trackers_test/ptp/
+-rw-------   0 ich       (1000) ich       (1000)     4113 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/ptp/ptp_tracker_config_test.py
+-rw-------   0 ich       (1000) ich       (1000)    32070 2023-07-22 15:04:27.000000 upsies-2023.7.22/tests/trackers_test/ptp/ptp_tracker_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1916 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/trackers_test/trackers_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.550943 upsies-2023.7.22/tests/uis_test/
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.558943 upsies-2023.7.22/tests/uis_test/tui_test/
+-rw-------   0 ich       (1000) ich       (1000)    21480 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/uis_test/tui_test/tui_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1425 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/uis_test/tui_test/tui_utils_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4429 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/uis_test/tui_test/tui_widgets_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.566943 upsies-2023.7.22/tests/utils_test/
+-rw-------   0 ich       (1000) ich       (1000)     9433 2023-05-25 09:31:21.000000 upsies-2023.7.22/tests/utils_test/argtypes_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9133 2023-05-26 16:44:13.000000 upsies-2023.7.22/tests/utils_test/btclient_test.py
+-rw-------   0 ich       (1000) ich       (1000)    35526 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/configfiles_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1266 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/country_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9048 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/daemon_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31470 2023-06-11 08:46:28.000000 upsies-2023.7.22/tests/utils_test/fs_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3723 2023-04-28 07:24:11.000000 upsies-2023.7.22/tests/utils_test/html_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.566943 upsies-2023.7.22/tests/utils_test/http_test/
+-rw-------   0 ich       (1000) ich       (1000)     1474 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/http_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    54514 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/http_test/http_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1233 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/http_test/http_tls_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1750 2023-05-25 13:46:48.000000 upsies-2023.7.22/tests/utils_test/image_optimize_test.py
+-rw-------   0 ich       (1000) ich       (1000)     7391 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/image_resize_test.py
+-rw-------   0 ich       (1000) ich       (1000)    12900 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/image_screenshot_test.py
+-rw-------   0 ich       (1000) ich       (1000)      425 2021-07-26 09:11:09.000000 upsies-2023.7.22/tests/utils_test/image_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.570943 upsies-2023.7.22/tests/utils_test/imghosts_test/
+-rw-------   0 ich       (1000) ich       (1000)     3390 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/freeimage_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3690 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/imgbb_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1932 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/imgbox_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14346 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/imghost_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3055 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/imghost_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2791 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/imghost_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6927 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/imghosts_test/ptpimg_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.574943 upsies-2023.7.22/tests/utils_test/predbs_test/
+-rw-------   0 ich       (1000) ich       (1000)     1173 2023-05-29 17:37:37.000000 upsies-2023.7.22/tests/utils_test/predbs_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)     6369 2023-05-29 17:37:37.000000 upsies-2023.7.22/tests/utils_test/predbs_test/corruptnet_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5723 2023-05-29 17:37:37.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbclub_test.py
+-rw-------   0 ich       (1000) ich       (1000)     6719 2023-06-11 11:33:26.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbde_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5710 2023-05-29 17:37:37.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbovh_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8255 2023-06-06 17:48:16.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbs_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)     8539 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbs_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)    49224 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbs_integration_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22848 2023-07-22 15:04:27.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbs_multi_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1900 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/predbs_test/predbs_test.py
+-rw-------   0 ich       (1000) ich       (1000)    22438 2023-05-31 14:49:34.000000 upsies-2023.7.22/tests/utils_test/predbs_test/srrdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9604 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/release_episodes_test.py
+-rw-------   0 ich       (1000) ich       (1000)    31672 2023-06-01 13:28:44.000000 upsies-2023.7.22/tests/utils_test/release_info_test.py
+-rw-------   0 ich       (1000) ich       (1000)    64364 2023-06-06 17:48:16.000000 upsies-2023.7.22/tests/utils_test/release_name_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5455 2021-09-30 12:51:20.000000 upsies-2023.7.22/tests/utils_test/signal_test.py
+-rw-------   0 ich       (1000) ich       (1000)     9667 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/string_test.py
+-rw-------   0 ich       (1000) ich       (1000)     2695 2023-03-13 14:34:58.000000 upsies-2023.7.22/tests/utils_test/subproc_test.py
+-rw-------   0 ich       (1000) ich       (1000)    11884 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/subtitle_test.py
+-rw-------   0 ich       (1000) ich       (1000)     3156 2021-06-11 16:56:53.000000 upsies-2023.7.22/tests/utils_test/timestamp_test.py
+-rw-------   0 ich       (1000) ich       (1000)    30246 2023-05-26 16:44:13.000000 upsies-2023.7.22/tests/utils_test/torrent_test.py
+-rw-------   0 ich       (1000) ich       (1000)    14894 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/types_test.py
+-rw-------   0 ich       (1000) ich       (1000)     5089 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/update_test.py
+-rw-------   0 ich       (1000) ich       (1000)    13913 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/utils_test.py
+-rw-------   0 ich       (1000) ich       (1000)    72586 2023-06-01 13:28:44.000000 upsies-2023.7.22/tests/utils_test/video_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.574943 upsies-2023.7.22/tests/utils_test/webdbs_test/
+-rw-------   0 ich       (1000) ich       (1000)     1423 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/conftest.py
+-rw-------   0 ich       (1000) ich       (1000)    37489 2023-04-28 13:26:51.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/imdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)    20288 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/tmdb_test.py
+-rw-------   0 ich       (1000) ich       (1000)    25066 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/tvmaze_test.py
+-rw-------   0 ich       (1000) ich       (1000)     4812 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/webdbs_base_test.py
+-rw-------   0 ich       (1000) ich       (1000)    19231 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/webdbs_common_test.py
+-rw-------   0 ich       (1000) ich       (1000)     1903 2023-04-25 13:55:04.000000 upsies-2023.7.22/tests/utils_test/webdbs_test/webdbs_test.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.574943 upsies-2023.7.22/upsies/
+-rw-------   0 ich       (1000) ich       (1000)     1117 2023-07-22 15:04:27.000000 upsies-2023.7.22/upsies/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)       73 2022-03-13 08:26:06.000000 upsies-2023.7.22/upsies/__main__.py
+-rw-------   0 ich       (1000) ich       (1000)     1399 2023-03-19 11:08:21.000000 upsies-2023.7.22/upsies/constants.py
+-rw-------   0 ich       (1000) ich       (1000)     2058 2023-05-26 09:17:09.000000 upsies-2023.7.22/upsies/defaults.py
+-rw-------   0 ich       (1000) ich       (1000)     6274 2023-05-26 16:44:13.000000 upsies-2023.7.22/upsies/errors.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.578943 upsies-2023.7.22/upsies/jobs/
+-rw-------   0 ich       (1000) ich       (1000)      215 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/jobs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    27889 2023-06-05 13:24:27.000000 upsies-2023.7.22/upsies/jobs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     2165 2023-07-03 09:11:46.000000 upsies-2023.7.22/upsies/jobs/custom.py
+-rw-------   0 ich       (1000) ich       (1000)    21011 2023-06-01 14:38:39.000000 upsies-2023.7.22/upsies/jobs/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)     3707 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/jobs/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)     4807 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/jobs/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     7596 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/jobs/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     8681 2023-07-09 09:28:38.000000 upsies-2023.7.22/upsies/jobs/scene.py
+-rw-------   0 ich       (1000) ich       (1000)    17965 2023-05-25 13:46:48.000000 upsies-2023.7.22/upsies/jobs/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     2770 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/jobs/set.py
+-rw-------   0 ich       (1000) ich       (1000)     7977 2023-06-05 13:23:49.000000 upsies-2023.7.22/upsies/jobs/submit.py
+-rw-------   0 ich       (1000) ich       (1000)    13075 2023-06-30 14:50:32.000000 upsies-2023.7.22/upsies/jobs/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    13899 2023-06-01 14:34:49.000000 upsies-2023.7.22/upsies/jobs/webdb.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.578943 upsies-2023.7.22/upsies/trackers/
+-rw-------   0 ich       (1000) ich       (1000)     1385 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.578943 upsies-2023.7.22/upsies/trackers/base/
+-rw-------   0 ich       (1000) ich       (1000)      149 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/base/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3222 2023-05-25 09:31:21.000000 upsies-2023.7.22/upsies/trackers/base/_howto.py
+-rw-------   0 ich       (1000) ich       (1000)     3102 2023-05-25 09:31:21.000000 upsies-2023.7.22/upsies/trackers/base/config.py
+-rw-------   0 ich       (1000) ich       (1000)    33425 2023-05-25 09:31:21.000000 upsies-2023.7.22/upsies/trackers/base/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     5985 2023-04-25 14:57:27.000000 upsies-2023.7.22/upsies/trackers/base/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.582943 upsies-2023.7.22/upsies/trackers/bhd/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.7.22/upsies/trackers/bhd/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     3643 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/bhd/config.py
+-rw-------   0 ich       (1000) ich       (1000)    15623 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/bhd/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     6243 2023-04-25 14:57:27.000000 upsies-2023.7.22/upsies/trackers/bhd/tracker.py
+-rw-------   0 ich       (1000) ich       (1000)     3647 2023-05-26 15:12:26.000000 upsies-2023.7.22/upsies/trackers/dummy.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.582943 upsies-2023.7.22/upsies/trackers/mtv/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/mtv/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2306 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/mtv/config.py
+-rw-------   0 ich       (1000) ich       (1000)    10331 2023-07-22 15:04:27.000000 upsies-2023.7.22/upsies/trackers/mtv/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)    12971 2023-07-22 15:04:27.000000 upsies-2023.7.22/upsies/trackers/mtv/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.582943 upsies-2023.7.22/upsies/trackers/nbl/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-28 07:24:11.000000 upsies-2023.7.22/upsies/trackers/nbl/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     1059 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/nbl/config.py
+-rw-------   0 ich       (1000) ich       (1000)     1855 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/nbl/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     3969 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/nbl/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.582943 upsies-2023.7.22/upsies/trackers/ptp/
+-rw-------   0 ich       (1000) ich       (1000)      119 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/ptp/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     2146 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/trackers/ptp/config.py
+-rw-------   0 ich       (1000) ich       (1000)    27925 2023-05-25 09:30:06.000000 upsies-2023.7.22/upsies/trackers/ptp/jobs.py
+-rw-------   0 ich       (1000) ich       (1000)     2001 2023-04-25 14:57:27.000000 upsies-2023.7.22/upsies/trackers/ptp/metadata.py
+-rw-------   0 ich       (1000) ich       (1000)    15920 2023-04-28 13:48:23.000000 upsies-2023.7.22/upsies/trackers/ptp/tracker.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.582943 upsies-2023.7.22/upsies/uis/
+-rw-------   0 ich       (1000) ich       (1000)       24 2021-06-11 16:55:41.000000 upsies-2023.7.22/upsies/uis/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.582943 upsies-2023.7.22/upsies/uis/tui/
+-rw-------   0 ich       (1000) ich       (1000)       55 2022-03-13 08:25:17.000000 upsies-2023.7.22/upsies/uis/tui/__init__.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.586943 upsies-2023.7.22/upsies/uis/tui/commands/
+-rw-------   0 ich       (1000) ich       (1000)     1319 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)    15239 2023-06-07 15:27:08.000000 upsies-2023.7.22/upsies/uis/tui/commands/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1942 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     3500 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     2513 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/release_name.py
+-rw-------   0 ich       (1000) ich       (1000)     2710 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     4546 2023-05-25 09:31:21.000000 upsies-2023.7.22/upsies/uis/tui/commands/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)     5152 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/set.py
+-rw-------   0 ich       (1000) ich       (1000)     8323 2023-05-26 16:44:13.000000 upsies-2023.7.22/upsies/uis/tui/commands/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     8424 2023-05-26 16:44:13.000000 upsies-2023.7.22/upsies/uis/tui/commands/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/upload_images.py
+-rw-------   0 ich       (1000) ich       (1000)     1799 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/commands/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     3061 2022-03-13 08:27:19.000000 upsies-2023.7.22/upsies/uis/tui/headless.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.590943 upsies-2023.7.22/upsies/uis/tui/jobwidgets/
+-rw-------   0 ich       (1000) ich       (1000)      947 2021-06-11 16:56:53.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     6992 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/base.py
+-rw-------   0 ich       (1000) ich       (1000)      252 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/config.py
+-rw-------   0 ich       (1000) ich       (1000)      202 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/custom.py
+-rw-------   0 ich       (1000) ich       (1000)     1902 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/dialog.py
+-rw-------   0 ich       (1000) ich       (1000)      767 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/imghost.py
+-rw-------   0 ich       (1000) ich       (1000)      205 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/mediainfo.py
+-rw-------   0 ich       (1000) ich       (1000)     1105 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/poster.py
+-rw-------   0 ich       (1000) ich       (1000)     4595 2023-07-22 15:04:27.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/scene.py
+-rw-------   0 ich       (1000) ich       (1000)     1649 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/screenshots.py
+-rw-------   0 ich       (1000) ich       (1000)      686 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/submit.py
+-rw-------   0 ich       (1000) ich       (1000)     8671 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)     9727 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/jobwidgets/webdb.py
+-rw-------   0 ich       (1000) ich       (1000)     2865 2023-06-07 15:14:22.000000 upsies-2023.7.22/upsies/uis/tui/main.py
+-rw-------   0 ich       (1000) ich       (1000)     1345 2022-10-25 10:31:19.000000 upsies-2023.7.22/upsies/uis/tui/style.py
+-rw-------   0 ich       (1000) ich       (1000)     9795 2023-07-03 09:13:51.000000 upsies-2023.7.22/upsies/uis/tui/tui.py
+-rw-------   0 ich       (1000) ich       (1000)      626 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/utils.py
+-rw-------   0 ich       (1000) ich       (1000)    13814 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/uis/tui/widgets.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.598943 upsies-2023.7.22/upsies/utils/
+-rw-------   0 ich       (1000) ich       (1000)    13326 2023-06-05 13:36:24.000000 upsies-2023.7.22/upsies/utils/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     5658 2023-05-25 09:31:21.000000 upsies-2023.7.22/upsies/utils/argtypes.py
+-rw-------   0 ich       (1000) ich       (1000)      302 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/browser.py
+-rw-------   0 ich       (1000) ich       (1000)     4303 2023-05-26 16:44:13.000000 upsies-2023.7.22/upsies/utils/btclient.py
+-rw-------   0 ich       (1000) ich       (1000)    15025 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/configfiles.py
+-rw-------   0 ich       (1000) ich       (1000)     1825 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/country.py
+-rw-------   0 ich       (1000) ich       (1000)     7285 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/daemon.py
+-rw-------   0 ich       (1000) ich       (1000)    17924 2023-06-11 11:33:26.000000 upsies-2023.7.22/upsies/utils/fs.py
+-rw-------   0 ich       (1000) ich       (1000)     2353 2023-05-25 13:46:48.000000 upsies-2023.7.22/upsies/utils/html.py
+-rw-------   0 ich       (1000) ich       (1000)    23553 2023-05-26 16:34:04.000000 upsies-2023.7.22/upsies/utils/http.py
+-rw-------   0 ich       (1000) ich       (1000)    10178 2023-05-25 13:46:48.000000 upsies-2023.7.22/upsies/utils/image.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.598943 upsies-2023.7.22/upsies/utils/imghosts/
+-rw-------   0 ich       (1000) ich       (1000)     1391 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/imghosts/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     7453 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/imghosts/base.py
+-rw-------   0 ich       (1000) ich       (1000)     1147 2021-06-11 16:56:53.000000 upsies-2023.7.22/upsies/utils/imghosts/common.py
+-rw-------   0 ich       (1000) ich       (1000)     1011 2021-10-31 14:15:29.000000 upsies-2023.7.22/upsies/utils/imghosts/dummy.py
+-rw-------   0 ich       (1000) ich       (1000)     1997 2021-11-27 15:46:37.000000 upsies-2023.7.22/upsies/utils/imghosts/freeimage.py
+-rw-------   0 ich       (1000) ich       (1000)     2517 2021-11-26 16:53:37.000000 upsies-2023.7.22/upsies/utils/imghosts/imgbb.py
+-rw-------   0 ich       (1000) ich       (1000)      912 2021-10-19 13:17:48.000000 upsies-2023.7.22/upsies/utils/imghosts/imgbox.py
+-rw-------   0 ich       (1000) ich       (1000)     3154 2023-04-23 11:00:43.000000 upsies-2023.7.22/upsies/utils/imghosts/ptpimg.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.598943 upsies-2023.7.22/upsies/utils/predbs/
+-rw-------   0 ich       (1000) ich       (1000)     1364 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/predbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     9619 2023-07-09 09:28:41.000000 upsies-2023.7.22/upsies/utils/predbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)     4128 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/predbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)     2278 2023-05-29 17:37:37.000000 upsies-2023.7.22/upsies/utils/predbs/corruptnet.py
+-rw-------   0 ich       (1000) ich       (1000)    20883 2023-07-22 15:04:27.000000 upsies-2023.7.22/upsies/utils/predbs/multi.py
+-rw-------   0 ich       (1000) ich       (1000)     2176 2023-05-29 17:37:37.000000 upsies-2023.7.22/upsies/utils/predbs/predbclub.py
+-rw-------   0 ich       (1000) ich       (1000)     2414 2023-06-11 11:33:26.000000 upsies-2023.7.22/upsies/utils/predbs/predbde.py
+-rw-------   0 ich       (1000) ich       (1000)     2169 2023-05-29 17:37:37.000000 upsies-2023.7.22/upsies/utils/predbs/predbovh.py
+-rw-------   0 ich       (1000) ich       (1000)     5425 2023-05-29 17:37:37.000000 upsies-2023.7.22/upsies/utils/predbs/query.py
+-rw-------   0 ich       (1000) ich       (1000)     6654 2023-07-09 09:28:44.000000 upsies-2023.7.22/upsies/utils/predbs/srrdb.py
+-rw-------   0 ich       (1000) ich       (1000)    56212 2023-07-22 14:29:26.000000 upsies-2023.7.22/upsies/utils/release.py
+-rw-------   0 ich       (1000) ich       (1000)     3931 2023-02-19 13:31:01.000000 upsies-2023.7.22/upsies/utils/signal.py
+-rw-------   0 ich       (1000) ich       (1000)     3922 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/string.py
+-rw-------   0 ich       (1000) ich       (1000)     1908 2023-03-31 14:19:32.000000 upsies-2023.7.22/upsies/utils/subproc.py
+-rw-------   0 ich       (1000) ich       (1000)     7760 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/subtitle.py
+-rw-------   0 ich       (1000) ich       (1000)     2034 2021-09-23 10:04:01.000000 upsies-2023.7.22/upsies/utils/timestamp.py
+-rw-------   0 ich       (1000) ich       (1000)    19315 2023-07-02 09:14:38.000000 upsies-2023.7.22/upsies/utils/torrent.py
+-rw-------   0 ich       (1000) ich       (1000)    11165 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/types.py
+-rw-------   0 ich       (1000) ich       (1000)     2927 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/update.py
+-rw-------   0 ich       (1000) ich       (1000)    35111 2023-06-01 13:28:44.000000 upsies-2023.7.22/upsies/utils/video.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.602943 upsies-2023.7.22/upsies/utils/webdbs/
+-rw-------   0 ich       (1000) ich       (1000)     1140 2023-01-16 18:31:24.000000 upsies-2023.7.22/upsies/utils/webdbs/__init__.py
+-rw-------   0 ich       (1000) ich       (1000)     8898 2023-04-28 13:26:45.000000 upsies-2023.7.22/upsies/utils/webdbs/base.py
+-rw-------   0 ich       (1000) ich       (1000)    12546 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/webdbs/common.py
+-rw-------   0 ich       (1000) ich       (1000)    17839 2023-04-28 13:48:23.000000 upsies-2023.7.22/upsies/utils/webdbs/imdb.py
+-rw-------   0 ich       (1000) ich       (1000)    12105 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/webdbs/tmdb.py
+-rw-------   0 ich       (1000) ich       (1000)     9757 2023-04-25 13:55:04.000000 upsies-2023.7.22/upsies/utils/webdbs/tvmaze.py
+drwx------   0 ich       (1000) ich       (1000)        0 2023-07-22 15:06:37.574943 upsies-2023.7.22/upsies.egg-info/
+-rw-------   0 ich       (1000) ich       (1000)     2637 2023-07-22 15:06:37.000000 upsies-2023.7.22/upsies.egg-info/PKG-INFO
+-rw-------   0 ich       (1000) ich       (1000)     7413 2023-07-22 15:06:37.000000 upsies-2023.7.22/upsies.egg-info/SOURCES.txt
+-rw-------   0 ich       (1000) ich       (1000)        1 2023-07-22 15:06:37.000000 upsies-2023.7.22/upsies.egg-info/dependency_links.txt
+-rw-------   0 ich       (1000) ich       (1000)       47 2023-07-22 15:06:37.000000 upsies-2023.7.22/upsies.egg-info/entry_points.txt
+-rw-------   0 ich       (1000) ich       (1000)      320 2023-07-22 15:06:37.000000 upsies-2023.7.22/upsies.egg-info/requires.txt
+-rw-------   0 ich       (1000) ich       (1000)       46 2023-07-22 15:06:37.000000 upsies-2023.7.22/upsies.egg-info/top_level.txt
```

### Comparing `upsies-2023.6.11/LICENSE` & `upsies-2023.7.22/LICENSE`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/PKG-INFO` & `upsies-2023.7.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2023.6.11
+Version: 2023.7.22
 Summary: Media metadata aggregator
 Author-email: plotski <plotski@example.org>
 License: GPL-3.0-or-later
 Project-URL: Repository, https://codeberg.org/plotski/upsies
 Project-URL: Documentation, https://upsies.readthedocs.io
 Project-URL: Bug Tracker, https://codeberg.org/plotski/upsies/issues
 Project-URL: Changelog, https://codeberg.org/plotski/upsies/raw/branch/master/NEWS
```

### Comparing `upsies-2023.6.11/README.rst` & `upsies-2023.7.22/README.rst`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/docs/_ext/cli_reference.py` & `upsies-2023.7.22/docs/_ext/cli_reference.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/docs/conf.py` & `upsies-2023.7.22/docs/conf.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/pyproject.toml` & `upsies-2023.7.22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/conftest.py` & `upsies-2023.7.22/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/errors_test.py` & `upsies-2023.7.22/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/add_torrent_job_test.py` & `upsies-2023.7.22/tests/jobs_test/add_torrent_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/choice_job_test.py` & `upsies-2023.7.22/tests/jobs_test/choice_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/copy_torrent_job_test.py` & `upsies-2023.7.22/tests/jobs_test/copy_torrent_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/create_torrent_job_test.py` & `upsies-2023.7.22/tests/jobs_test/create_torrent_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/custom_job_test.py` & `upsies-2023.7.22/tests/jobs_test/custom_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/imghost_job_test.py` & `upsies-2023.7.22/tests/jobs_test/imghost_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/job_base_test.py` & `upsies-2023.7.22/tests/jobs_test/job_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/mediainfo_job_test.py` & `upsies-2023.7.22/tests/jobs_test/mediainfo_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/poster_job_test.py` & `upsies-2023.7.22/tests/jobs_test/poster_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/queue_job_base_test.py` & `upsies-2023.7.22/tests/jobs_test/queue_job_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/scene_check_job_test.py` & `upsies-2023.7.22/tests/jobs_test/scene_check_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/scene_search_job_test.py` & `upsies-2023.7.22/tests/jobs_test/scene_search_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/screenshots_job_test.py` & `upsies-2023.7.22/tests/jobs_test/screenshots_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/set_job_test.py` & `upsies-2023.7.22/tests/jobs_test/set_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/submit_job_test.py` & `upsies-2023.7.22/tests/jobs_test/submit_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/text_field_job_test.py` & `upsies-2023.7.22/tests/jobs_test/text_field_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/jobs_test/webdb_search_job_test.py` & `upsies-2023.7.22/tests/jobs_test/webdb_search_job_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/base/tracker_base_howto_test.py` & `upsies-2023.7.22/tests/trackers_test/base/tracker_base_howto_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/base/tracker_base_test.py` & `upsies-2023.7.22/tests/trackers_test/base/tracker_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/base/tracker_config_base_test.py` & `upsies-2023.7.22/tests/trackers_test/base/tracker_config_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/base/tracker_jobs_base_test.py` & `upsies-2023.7.22/tests/trackers_test/base/tracker_jobs_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_config_test.py` & `upsies-2023.7.22/tests/trackers_test/bhd/bhd_tracker_config_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_jobs_test.py` & `upsies-2023.7.22/tests/trackers_test/bhd/bhd_tracker_jobs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/bhd/bhd_tracker_test.py` & `upsies-2023.7.22/tests/trackers_test/bhd/bhd_tracker_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/conftest.py` & `upsies-2023.7.22/tests/trackers_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_config_test.py` & `upsies-2023.7.22/tests/trackers_test/mtv/mtv_tracker_config_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_jobs_test.py` & `upsies-2023.7.22/tests/trackers_test/mtv/mtv_tracker_jobs_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from unittest.mock import AsyncMock, MagicMock, Mock, PropertyMock, call
 
 import pytest
 
-from upsies import __homepage__, __project_name__, utils
+from upsies import __homepage__, __project_name__, errors, utils
 from upsies.trackers import mtv
 
 
 @pytest.fixture
 def tracker():
     tracker = Mock()
     tracker.name = 'mtv'
@@ -422,14 +422,47 @@
 
     assert mocks.mock_calls == [
         call.fetch_info(
             webdb=mtv_tracker_jobs.imdb,
             webdb_id=mtv_tracker_jobs.imdb_id,
         ),
     ]
+
+@pytest.mark.asyncio
+async def test_MtvTrackerJobs_generate_title__getting_title_from_predb_fails(mtv_tracker_jobs_for_generate_title, mocker):
+    mtv_tracker_jobs, mocks = mtv_tracker_jobs_for_generate_title
+    mtv_tracker_jobs.scene_check_job.is_scene_release = True
+    type(mtv_tracker_jobs).chosen_release_type = PropertyMock(return_value=utils.release.ReleaseType.movie)
+    mocks.scene_search.side_effect = errors.RequestError('Your request sucks')
+    mtv_tracker_jobs.release_name.__str__.return_value = 'Generated.Title-ARF'
+
+    return_value = await mtv_tracker_jobs.generate_title()
+    assert return_value == 'Generated.Title-ARF'
+
+    assert mocks.mock_calls == [
+        call.scene_search(mtv_tracker_jobs.content_path),
+    ]
+
+@pytest.mark.asyncio
+async def test_MtvTrackerJobs_generate_title__getting_title_from_webdb_fails(mtv_tracker_jobs_for_generate_title, mocker):
+    mtv_tracker_jobs, mocks = mtv_tracker_jobs_for_generate_title
+    mtv_tracker_jobs.scene_check_job.is_scene_release = False
+    type(mtv_tracker_jobs).chosen_release_type = PropertyMock(return_value='whatever')
+    mocks.fetch_info.side_effect = errors.RequestError('Your request sucks')
+    mtv_tracker_jobs.release_name.__str__.return_value = 'Generated.Title-ARF'
+
+    return_value = await mtv_tracker_jobs.generate_title()
+    assert return_value == 'Generated.Title-ARF'
+
+    assert mocks.mock_calls == [
+        call.fetch_info(
+            webdb=mtv_tracker_jobs.imdb,
+            webdb_id=mtv_tracker_jobs.imdb_id,
+        ),
+    ]
 
 
 @pytest.mark.parametrize(
     argnames='title, exp_exception',
     argvalues=(
         ('Valid.Title', None),
         ('', ValueError('Title must not be empty')),
```

### Comparing `upsies-2023.6.11/tests/trackers_test/mtv/mtv_tracker_test.py` & `upsies-2023.7.22/tests/trackers_test/mtv/mtv_tracker_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_config_test.py` & `upsies-2023.7.22/tests/trackers_test/nbl/nbl_tracker_config_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_jobs_test.py` & `upsies-2023.7.22/tests/trackers_test/nbl/nbl_tracker_jobs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/nbl/nbl_tracker_test.py` & `upsies-2023.7.22/tests/trackers_test/nbl/nbl_tracker_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/ptp/ptp_tracker_config_test.py` & `upsies-2023.7.22/tests/trackers_test/ptp/ptp_tracker_config_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/trackers_test/ptp/ptp_tracker_test.py` & `upsies-2023.7.22/tests/trackers_test/ptp/ptp_tracker_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,49 +506,60 @@
             debug_file='http_dumps.ptp/ptp_upload',
         ),
         call._handle_upload_response(mocks.post.return_value),
     ]
 
 
 @pytest.mark.parametrize(
-    argnames='response, exp_result',
+    argnames='response, exp_result, exp_calls',
     argvalues=(
         pytest.param(
             MockResponse(headers={'Location': 'torrents.php?id=123'}),
             '{base_url}/torrents.php?id=123',
+            [],
             id='Redirect to torrent page URL',
         ),
         pytest.param(
             MockResponse(headers={'Location': 'foo.php?id=123'}),
             errors.RequestError('Failed to interpret response (see ptp_upload_failed.html)'),
+            [
+                call.html_dump(str(MockResponse()), 'ptp_upload_failed.html'),
+            ],
             id='Redirect to other URL',
         ),
         pytest.param(
             MockResponse(),
             errors.RequestError('Failed to interpret response (see ptp_upload_failed.html)'),
+            [
+                call.html_dump(str(MockResponse()), 'ptp_upload_failed.html'),
+            ],
             id='No redirect',
         ),
         pytest.param(
             MockResponse(html='<html><div class="alert">  Your upload is <b>no good</b>!\n</html>'),
             errors.RequestError('Upload failed: Your upload is no good!'),
+            [],
             id='Error message is found',
         ),
     ),
 )
-def test_PtpTracker_handle_upload_response(response, exp_result, tracker, mocker):
+def test_PtpTracker_handle_upload_response(response, exp_result, exp_calls, tracker, mocker):
     mocks = Mock()
     mocks.attach_mock(mocker.patch.object(tracker, 'error'), 'error')
+    mocks.attach_mock(mocker.patch('upsies.utils.html.dump'), 'html_dump')
 
     if isinstance(exp_result, Exception):
         with pytest.raises(type(exp_result), match=rf'^{re.escape(str(exp_result))}$'):
             tracker._handle_upload_response(response)
     else:
         return_value = tracker._handle_upload_response(response)
         assert return_value == exp_result.format(base_url=tracker._base_url)
 
+    assert mocks.mock_calls == exp_calls
+
 
 @pytest.mark.parametrize(
     argnames='imdb_id_digits, exp_return_value',
     argvalues=(
         ('1234567890', '1234567890'),
         ('123456789', '123456789'),
         ('12345678', '12345678'),
```

### Comparing `upsies-2023.6.11/tests/trackers_test/trackers_test.py` & `upsies-2023.7.22/tests/trackers_test/trackers_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/uis_test/tui_test/tui_test.py` & `upsies-2023.7.22/tests/uis_test/tui_test/tui_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/uis_test/tui_test/tui_utils_test.py` & `upsies-2023.7.22/tests/uis_test/tui_test/tui_utils_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/uis_test/tui_test/tui_widgets_test.py` & `upsies-2023.7.22/tests/uis_test/tui_test/tui_widgets_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/argtypes_test.py` & `upsies-2023.7.22/tests/utils_test/argtypes_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/btclient_test.py` & `upsies-2023.7.22/tests/utils_test/btclient_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/configfiles_test.py` & `upsies-2023.7.22/tests/utils_test/configfiles_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/country_test.py` & `upsies-2023.7.22/tests/utils_test/country_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/daemon_test.py` & `upsies-2023.7.22/tests/utils_test/daemon_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/fs_test.py` & `upsies-2023.7.22/tests/utils_test/fs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/html_test.py` & `upsies-2023.7.22/tests/utils_test/html_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/http_test/conftest.py` & `upsies-2023.7.22/tests/utils_test/http_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/http_test/http_test.py` & `upsies-2023.7.22/tests/utils_test/http_test/http_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/http_test/http_tls_test.py` & `upsies-2023.7.22/tests/utils_test/http_test/http_tls_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/image_optimize_test.py` & `upsies-2023.7.22/tests/utils_test/image_optimize_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/image_resize_test.py` & `upsies-2023.7.22/tests/utils_test/image_resize_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/image_screenshot_test.py` & `upsies-2023.7.22/tests/utils_test/image_screenshot_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/freeimage_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/freeimage_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/imgbb_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/imgbb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/imgbox_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/imgbox_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_base_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/imghost_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_common_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/imghost_common_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/imghost_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/imghost_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/imghosts_test/ptpimg_test.py` & `upsies-2023.7.22/tests/utils_test/imghosts_test/ptpimg_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/conftest.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/corruptnet_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/corruptnet_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbclub_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbclub_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbde_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbde_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbovh_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbovh_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbs_base_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbs_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbs_common_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbs_common_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbs_integration_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbs_integration_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbs_multi_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbs_multi_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     predb_mock = mocker.patch('upsies.utils.predbs.predb', side_effect=exp_predbs)
     multipredb = multi.MultiPredbApi()
     assert multipredb._predbs == exp_predbs
     assert predb_mock.call_args_list == [
         call('srrdb'),
         # call('corruptnet'),
         # call('predbovh'),
-        call('predbclub'),
+        # call('predbclub'),
         call('predbde'),
     ]
 
 
 @pytest.fixture
 def multipredb():
     predbs = [Mock(), Mock(), Mock()]
```

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/predbs_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/predbs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/predbs_test/srrdb_test.py` & `upsies-2023.7.22/tests/utils_test/predbs_test/srrdb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/release_episodes_test.py` & `upsies-2023.7.22/tests/utils_test/release_episodes_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/release_info_test.py` & `upsies-2023.7.22/tests/utils_test/release_info_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/release_name_test.py` & `upsies-2023.7.22/tests/utils_test/release_name_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/signal_test.py` & `upsies-2023.7.22/tests/utils_test/signal_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/string_test.py` & `upsies-2023.7.22/tests/utils_test/string_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/subproc_test.py` & `upsies-2023.7.22/tests/utils_test/subproc_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/subtitle_test.py` & `upsies-2023.7.22/tests/utils_test/subtitle_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/timestamp_test.py` & `upsies-2023.7.22/tests/utils_test/timestamp_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/torrent_test.py` & `upsies-2023.7.22/tests/utils_test/torrent_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/types_test.py` & `upsies-2023.7.22/tests/utils_test/types_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/update_test.py` & `upsies-2023.7.22/tests/utils_test/update_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/utils_test.py` & `upsies-2023.7.22/tests/utils_test/utils_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/video_test.py` & `upsies-2023.7.22/tests/utils_test/video_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/conftest.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/conftest.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/imdb_test.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/imdb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/tmdb_test.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/tmdb_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/tvmaze_test.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/tvmaze_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_base_test.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/webdbs_base_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_common_test.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/webdbs_common_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/tests/utils_test/webdbs_test/webdbs_test.py` & `upsies-2023.7.22/tests/utils_test/webdbs_test/webdbs_test.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/__init__.py` & `upsies-2023.7.22/upsies/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __project_name__ = 'upsies'
 __description__ = 'Media metadata aggregator'
 __homepage__ = 'https://upsies.readthedocs.io'
-__version__ = '2023.06.11'
+__version__ = '2023.07.22'
 
 
 def application_setup(config):
     """
     This function should be called by the UI ASAP when `config` is available
 
     :param config: :class:`~.configfiles.ConfigFiles` instance
```

### Comparing `upsies-2023.6.11/upsies/constants.py` & `upsies-2023.7.22/upsies/constants.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/defaults.py` & `upsies-2023.7.22/upsies/defaults.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/errors.py` & `upsies-2023.7.22/upsies/errors.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/base.py` & `upsies-2023.7.22/upsies/jobs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/custom.py` & `upsies-2023.7.22/upsies/jobs/custom.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/dialog.py` & `upsies-2023.7.22/upsies/jobs/dialog.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/imghost.py` & `upsies-2023.7.22/upsies/jobs/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/mediainfo.py` & `upsies-2023.7.22/upsies/jobs/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/poster.py` & `upsies-2023.7.22/upsies/jobs/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/scene.py` & `upsies-2023.7.22/upsies/jobs/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/screenshots.py` & `upsies-2023.7.22/upsies/jobs/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/set.py` & `upsies-2023.7.22/upsies/jobs/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/submit.py` & `upsies-2023.7.22/upsies/jobs/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/torrent.py` & `upsies-2023.7.22/upsies/jobs/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/jobs/webdb.py` & `upsies-2023.7.22/upsies/jobs/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/__init__.py` & `upsies-2023.7.22/upsies/trackers/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/base/_howto.py` & `upsies-2023.7.22/upsies/trackers/base/_howto.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/base/config.py` & `upsies-2023.7.22/upsies/trackers/base/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/base/jobs.py` & `upsies-2023.7.22/upsies/trackers/base/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/base/tracker.py` & `upsies-2023.7.22/upsies/trackers/base/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/bhd/config.py` & `upsies-2023.7.22/upsies/trackers/bhd/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/bhd/jobs.py` & `upsies-2023.7.22/upsies/trackers/bhd/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/bhd/tracker.py` & `upsies-2023.7.22/upsies/trackers/bhd/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/dummy.py` & `upsies-2023.7.22/upsies/trackers/dummy.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/mtv/config.py` & `upsies-2023.7.22/upsies/trackers/mtv/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/mtv/jobs.py` & `upsies-2023.7.22/upsies/trackers/mtv/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Concrete :class:`~.base.TrackerJobsBase` subclass for MTV
 """
 
 import functools
 import re
 
-from ... import __homepage__, __project_name__, jobs, utils
+from ... import __homepage__, __project_name__, errors, jobs, utils
 from ...utils.release import ReleaseType
 from ..base import TrackerJobsBase
 
 import logging  # isort:skip
 _log = logging.getLogger(__name__)
 
 
@@ -161,24 +161,32 @@
             **self.common_job_args(),
         )
 
     async def generate_title(self):
         assert self.scene_check_job.is_finished
         assert self.imdb_job.is_finished
 
-        if self.chosen_release_type in (ReleaseType.movie, ReleaseType.episode):
-            if self.scene_check_job.is_scene_release:
-                # Use the scene release name. We rely on scene_check_job making sure
-                # that the file/directory name is the correct release name.
-                search_results = await utils.predbs.MultiPredbApi().search(self.content_path)
-                assert len(search_results) >= 1, search_results
-                return search_results[0]
+        try:
+            if self.chosen_release_type in (ReleaseType.movie, ReleaseType.episode):
+                if self.scene_check_job.is_scene_release:
+                    # Use the original scene release name instead of a
+                    # standardized release name. We rely on scene_check_job
+                    # making sure that the file/directory name is the correct
+                    # release name.
+                    search_results = await utils.predbs.MultiPredbApi().search(self.content_path)
+                    assert len(search_results) >= 1, search_results
+                    return search_results[0]
+
+            # We're dealing with a non-scene release or season pack.
+            # We may generate a title.
+            await self.release_name.fetch_info(webdb=self.imdb, webdb_id=self.imdb_id)
+
+        except errors.RequestError as e:
+            _log.debug('Fetching title failed: %r', e)
 
-        # Non-scene release or season pack. We may generate a title.
-        await self.release_name.fetch_info(webdb=self.imdb, webdb_id=self.imdb_id)
         return str(self.release_name)
 
     def validate_title(self, text):
         if not text.strip():
             raise ValueError('Title must not be empty')
 
         match = re.search(rf'(?:{utils.release.DELIM}|$)(UNKNOWN_([A-Z_]+))(?:{utils.release.DELIM}|$)', text)
```

### Comparing `upsies-2023.6.11/upsies/trackers/mtv/tracker.py` & `upsies-2023.7.22/upsies/trackers/mtv/tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         return torrent_page_url
 
     async def _make_autofill_request(self, tracker_jobs):
         # First request uploads the torrent file. We extract "tempfileid" and
         # "tempfilename" from the returned HTML form that must be returned in
         # the second request. We can also extract the autogenerated "taglist".
         post_data = await self._prepare_post_data(tracker_jobs.post_data_autofill)
+        _log.debug('Autofil POST data: %r', post_data)
         post_files = {
             'file_input': {
                 'file': tracker_jobs.torrent_filepath,
                 'mimetype': 'application/x-bittorrent',
             },
         }
 
@@ -164,14 +165,15 @@
             _log.debug('Failed to extract values from autofill response: %s', e)
             self._raise_error(doc, msg_prefix='Upload failed')
 
     async def _make_upload_request(self, tracker_jobs, autofill_post_data):
         # Second request combines our metadata with server-generated data from
         # _make_autofill_request().
         post_data = await self._prepare_post_data(tracker_jobs.post_data_upload)
+        _log.debug('Upload POST data: %r', post_data)
         post_data.update(autofill_post_data)
 
         response = await utils.http.post(
             url=self._upload_url,
             cache=False,
             user_agent=True,
             follow_redirects=False,
```

### Comparing `upsies-2023.6.11/upsies/trackers/nbl/config.py` & `upsies-2023.7.22/upsies/trackers/nbl/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/nbl/jobs.py` & `upsies-2023.7.22/upsies/trackers/nbl/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/nbl/tracker.py` & `upsies-2023.7.22/upsies/trackers/nbl/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/ptp/config.py` & `upsies-2023.7.22/upsies/trackers/ptp/config.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/ptp/jobs.py` & `upsies-2023.7.22/upsies/trackers/ptp/jobs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/ptp/metadata.py` & `upsies-2023.7.22/upsies/trackers/ptp/metadata.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/trackers/ptp/tracker.py` & `upsies-2023.7.22/upsies/trackers/ptp/tracker.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/__init__.py` & `upsies-2023.7.22/upsies/uis/tui/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/base.py` & `upsies-2023.7.22/upsies/uis/tui/commands/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/mediainfo.py` & `upsies-2023.7.22/upsies/uis/tui/commands/mediainfo.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/poster.py` & `upsies-2023.7.22/upsies/uis/tui/commands/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/release_name.py` & `upsies-2023.7.22/upsies/uis/tui/commands/release_name.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/scene.py` & `upsies-2023.7.22/upsies/uis/tui/commands/scene.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/screenshots.py` & `upsies-2023.7.22/upsies/uis/tui/commands/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/set.py` & `upsies-2023.7.22/upsies/uis/tui/commands/set.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/submit.py` & `upsies-2023.7.22/upsies/uis/tui/commands/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/torrent.py` & `upsies-2023.7.22/upsies/uis/tui/commands/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/upload_images.py` & `upsies-2023.7.22/upsies/uis/tui/commands/upload_images.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/commands/webdb.py` & `upsies-2023.7.22/upsies/uis/tui/commands/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/headless.py` & `upsies-2023.7.22/upsies/uis/tui/headless.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/__init__.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/base.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/dialog.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/dialog.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/imghost.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/imghost.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/poster.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/poster.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/scene.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/scene.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,19 @@
             self._activity_indicator.active = True
 
         self._radiolist.on_accepted = handle_release_name
         self._radiolist.choices = [(release_name, release_name) for release_name in release_names]
         self._radiolist.choices.append(('This is not a scene release', None))
 
         self._question.text = 'Pick the correct release name:'
+
+        # We must tell the TUI to invalidate the job list because we are now
+        # focusable, and the keypress focus may still be unset (keypresses are
+        # ignored).
+        self.job.signal.emit('refresh_job_list')
         self.invalidate()
 
     def _ask_is_scene_release(self, is_scene_release):
         _log.debug('Confirming guess: %r', is_scene_release)
 
         self._activity_indicator.active = False
 
@@ -92,14 +97,19 @@
             self.invalidate()
 
         self._radiolist.choices = (make_choice(True), make_choice(False))
         self._radiolist.focused_choice = make_choice(is_scene_release)
         self._radiolist.on_accepted = handle_is_scene_release
 
         self._question.text = 'Is this a scene release?'
+
+        # We must tell the TUI to invalidate the job list because we are now
+        # focusable, and the keypress focus may still be unset (keypresses are
+        # ignored).
+        self.job.signal.emit('refresh_job_list')
         self.invalidate()
 
     @functools.cached_property
     def runtime_widget(self):
         return HSplit(
             children=[
                 ConditionalContainer(
```

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/screenshots.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/screenshots.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/submit.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/submit.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/torrent.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/jobwidgets/webdb.py` & `upsies-2023.7.22/upsies/uis/tui/jobwidgets/webdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/main.py` & `upsies-2023.7.22/upsies/uis/tui/main.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/style.py` & `upsies-2023.7.22/upsies/uis/tui/style.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/tui.py` & `upsies-2023.7.22/upsies/uis/tui/tui.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/utils.py` & `upsies-2023.7.22/upsies/uis/tui/utils.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/uis/tui/widgets.py` & `upsies-2023.7.22/upsies/uis/tui/widgets.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/__init__.py` & `upsies-2023.7.22/upsies/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/argtypes.py` & `upsies-2023.7.22/upsies/utils/argtypes.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/btclient.py` & `upsies-2023.7.22/upsies/utils/btclient.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/configfiles.py` & `upsies-2023.7.22/upsies/utils/configfiles.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/country.py` & `upsies-2023.7.22/upsies/utils/country.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/daemon.py` & `upsies-2023.7.22/upsies/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/fs.py` & `upsies-2023.7.22/upsies/utils/fs.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/html.py` & `upsies-2023.7.22/upsies/utils/html.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/http.py` & `upsies-2023.7.22/upsies/utils/http.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/image.py` & `upsies-2023.7.22/upsies/utils/image.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/__init__.py` & `upsies-2023.7.22/upsies/utils/imghosts/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/base.py` & `upsies-2023.7.22/upsies/utils/imghosts/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/common.py` & `upsies-2023.7.22/upsies/utils/imghosts/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/dummy.py` & `upsies-2023.7.22/upsies/utils/imghosts/dummy.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/freeimage.py` & `upsies-2023.7.22/upsies/utils/imghosts/freeimage.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/imgbb.py` & `upsies-2023.7.22/upsies/utils/imghosts/imgbb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/imgbox.py` & `upsies-2023.7.22/upsies/utils/imghosts/imgbox.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/imghosts/ptpimg.py` & `upsies-2023.7.22/upsies/utils/imghosts/ptpimg.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/__init__.py` & `upsies-2023.7.22/upsies/utils/predbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/base.py` & `upsies-2023.7.22/upsies/utils/predbs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/common.py` & `upsies-2023.7.22/upsies/utils/predbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/corruptnet.py` & `upsies-2023.7.22/upsies/utils/predbs/corruptnet.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/multi.py` & `upsies-2023.7.22/upsies/utils/predbs/multi.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     :param predbs: Sequence of :class:`~.PredbApiBase` instances
     """
 
     DEFAULT_PREDB_NAMES = (
         'srrdb',
         # 'corruptnet',
         # 'predbovh',
-        'predbclub',
+        # 'predbclub',
         'predbde',
     )
 
     def __init__(self, predbs=None):
         if predbs:
             self._predbs = predbs
         else:
```

### Comparing `upsies-2023.6.11/upsies/utils/predbs/predbclub.py` & `upsies-2023.7.22/upsies/utils/predbs/predbclub.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/predbde.py` & `upsies-2023.7.22/upsies/utils/predbs/predbde.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/predbovh.py` & `upsies-2023.7.22/upsies/utils/predbs/predbovh.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/query.py` & `upsies-2023.7.22/upsies/utils/predbs/query.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/predbs/srrdb.py` & `upsies-2023.7.22/upsies/utils/predbs/srrdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/release.py` & `upsies-2023.7.22/upsies/utils/release.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/signal.py` & `upsies-2023.7.22/upsies/utils/signal.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/string.py` & `upsies-2023.7.22/upsies/utils/string.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/subproc.py` & `upsies-2023.7.22/upsies/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/subtitle.py` & `upsies-2023.7.22/upsies/utils/subtitle.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/timestamp.py` & `upsies-2023.7.22/upsies/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/torrent.py` & `upsies-2023.7.22/upsies/utils/torrent.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/types.py` & `upsies-2023.7.22/upsies/utils/types.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/update.py` & `upsies-2023.7.22/upsies/utils/update.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/video.py` & `upsies-2023.7.22/upsies/utils/video.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/webdbs/__init__.py` & `upsies-2023.7.22/upsies/utils/webdbs/__init__.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/webdbs/base.py` & `upsies-2023.7.22/upsies/utils/webdbs/base.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/webdbs/common.py` & `upsies-2023.7.22/upsies/utils/webdbs/common.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/webdbs/imdb.py` & `upsies-2023.7.22/upsies/utils/webdbs/imdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/webdbs/tmdb.py` & `upsies-2023.7.22/upsies/utils/webdbs/tmdb.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies/utils/webdbs/tvmaze.py` & `upsies-2023.7.22/upsies/utils/webdbs/tvmaze.py`

 * *Files identical despite different names*

### Comparing `upsies-2023.6.11/upsies.egg-info/PKG-INFO` & `upsies-2023.7.22/upsies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upsies
-Version: 2023.6.11
+Version: 2023.7.22
 Summary: Media metadata aggregator
 Author-email: plotski <plotski@example.org>
 License: GPL-3.0-or-later
 Project-URL: Repository, https://codeberg.org/plotski/upsies
 Project-URL: Documentation, https://upsies.readthedocs.io
 Project-URL: Bug Tracker, https://codeberg.org/plotski/upsies/issues
 Project-URL: Changelog, https://codeberg.org/plotski/upsies/raw/branch/master/NEWS
```

### Comparing `upsies-2023.6.11/upsies.egg-info/SOURCES.txt` & `upsies-2023.7.22/upsies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

