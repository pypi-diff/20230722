# Comparing `tmp/tator-1.0.5.tar.gz` & `tmp/tator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tator-1.0.5.tar", last modified: Mon Jun 19 16:04:04 2023, max compression
+gzip compressed data, was "tator-1.1.0.tar", last modified: Sat Jul 22 18:59:40 2023, max compression
```

## Comparing `tator-1.0.5.tar` & `tator-1.1.0.tar`

### file list

```diff
@@ -1,292 +1,293 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.314694 tator-1.0.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-06-19 15:53:28.000000 tator-1.0.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-19 16:04:04.314694 tator-1.0.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-06-19 15:53:28.000000 tator-1.0.5/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-06-19 15:53:28.000000 tator-1.0.5/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-19 16:04:04.314694 tator-1.0.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-06-19 15:53:28.000000 tator-1.0.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-06-19 15:53:28.000000 tator-1.0.5/tator/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator/extractor/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/env_launcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12295 2023-06-19 15:53:28.000000 tator-1.0.5/tator/extractor/extractor.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator/openapi/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-06-19 15:53:28.000000 tator-1.0.5/tator/openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.278693 tator-1.0.5/tator/openapi/tator_openapi/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12710 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.278693 tator-1.0.5/tator/openapi/tator_openapi/api/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/api/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1854040 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/api/tator_api.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/api_client.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/configuration.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.298693 tator-1.0.5/tator/openapi/tator_openapi/models/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12120 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/models/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8163 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/affiliation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_parameter.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4152 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/analysis.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3980 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/analysis_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/announcement.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/applet.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/applet_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/archive_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11001 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_filter_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12663 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_operation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/audio_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/autocomplete_service.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bad_request_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bookmark.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_gcp_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_s3_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/bucket_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/change_log.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5302 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/clone_media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/color_map.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/concat_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/create_list_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/create_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/credentials.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/download_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/download_info_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/email_attachment_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/email_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/encode_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-06-19 16:03:59.000000 tator-1.0.5/tator/openapi/tator_openapi/models/favorite.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/favorite_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/favorite_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/feed_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/file_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/fill.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/float_array_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/generic_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/generic_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/get_cloned_media_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/image_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/invitation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/invitation_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/invitation_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_node.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4849 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/job_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_suggestion.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/leaf_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/live_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/live_update_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10180 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/localization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18245 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_files.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_next.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_prev.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14774 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_stats.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/media_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/membership.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/membership_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/membership_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/message_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/multi_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/not_found_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/notify_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/organization.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/organization_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/organization_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/password_reset_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/project.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/project_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/project_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/resolution_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/s3_storage_config.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/section.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/section_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/section_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10960 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_delete.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_id_query.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_merge_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_trim_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_type.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_type_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_type_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/state_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/token.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/transcode.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10545 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/transcode_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/upload_completion_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/upload_info.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/upload_part.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/user.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/user_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7852 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/user_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/version.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/version_spec.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/version_update.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/video_clip.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9722 2023-06-19 16:04:00.000000 tator-1.0.5/tator/openapi/tator_openapi/models/video_definition.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-06-19 16:04:02.000000 tator-1.0.5/tator/openapi/tator_openapi/rest.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.302693 tator-1.0.5/tator/transcode/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6547 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/__main__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/black.mp4
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/create_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/delete_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9425 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/determine_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/make_fragment_info.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5938 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/make_thumbnails.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/prepare.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19001 2023-06-19 15:53:28.000000 tator-1.0.5/tator/transcode/transcode.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.306693 tator-1.0.5/tator/util/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/_download_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7168 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/_upload_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      648 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/chunked_create.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/chunked_file_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_leaf_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_localization_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11100 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_media_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_state_list.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4489 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/concat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/download_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/download_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/find_single_change.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/full_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_api.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_images.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2219 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_paginator.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/get_parser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1729 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/live_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/md5sum.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17897 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7283 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/multi_stream.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/register_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/register_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/tator-symbol.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/to_dataframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/update_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/upload_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3315 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/upload_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1813 2023-06-19 15:53:28.000000 tator-1.0.5/tator/util/upload_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-06-19 15:53:28.000000 tator-1.0.5/tator/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.274693 tator-1.0.5/tator.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11773 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-19 16:04:04.000000 tator-1.0.5/tator.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-19 16:04:04.314694 tator-1.0.5/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_a_float_array.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_algorithm.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_algorithm_launch.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_applet.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_archive_date.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attachment.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attribute_type_addition.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attribute_type_deletion.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attribute_type_mutation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_attributes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23749 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_change_log.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7204 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_membership.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_section.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_clone_version.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3601 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_collection.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_download_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_extract.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12346 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_file_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_get_clip.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_getframe.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1770 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_import_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_job_cancel.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_job_cluster.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_leaf.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_leaf_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2996 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_local_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_localization.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_localization_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_localization_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6973 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_media.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_media_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3773 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_poly.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_project_thumbnail.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9638 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_search.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_state.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_state_graphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_state_type.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_stategraphic.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_temporary_file.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_tracks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5487 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_transcode.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_util_media_manipulation.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_util_media_util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-06-19 15:53:28.000000 tator-1.0.5/test/test_version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.420867 tator-1.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      106 2023-07-22 18:49:40.000000 tator-1.1.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-07-22 18:59:40.416867 tator-1.1.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      667 2023-07-22 18:49:40.000000 tator-1.1.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2023-07-22 18:49:40.000000 tator-1.1.0/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-22 18:59:40.420867 tator-1.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3673 2023-07-22 18:49:40.000000 tator-1.1.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.380866 tator-1.1.0/tator/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      600 2023-07-22 18:49:40.000000 tator-1.1.0/tator/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.380866 tator-1.1.0/tator/extractor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:49:40.000000 tator-1.1.0/tator/extractor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3621 2023-07-22 18:49:40.000000 tator-1.1.0/tator/extractor/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2023-07-22 18:49:40.000000 tator-1.1.0/tator/extractor/env_launcher.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12298 2023-07-22 18:49:40.000000 tator-1.1.0/tator/extractor/extractor.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.380866 tator-1.1.0/tator/openapi/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       61 2023-07-22 18:49:40.000000 tator-1.1.0/tator/openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.384866 tator-1.1.0/tator/openapi/tator_openapi/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12670 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.384866 tator-1.1.0/tator/openapi/tator_openapi/api/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      150 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/api/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  2010477 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/api/tator_api.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    26204 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/api_client.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13489 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/configuration.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3713 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.404867 tator-1.1.0/tator/openapi/tator_openapi/models/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12080 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/models/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8289 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/affiliation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4305 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/affiliation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3513 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/affiliation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8842 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/algorithm.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3019 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_manifest.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3697 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3905 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_parameter.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8339 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5083 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/announcement.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6017 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/applet.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4903 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/applet_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/archive_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4121 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_combinator_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10923 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_filter_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12585 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_operation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14079 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3763 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5270 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14933 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8054 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/audio_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4042 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/autocomplete_service.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6295 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/auxiliary_file_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3705 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bad_request_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5353 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bookmark.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3479 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bookmark_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3495 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bookmark_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8573 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10945 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket_gcp_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4117 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket_oci_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6268 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket_oci_native_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6022 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket_s3_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7814 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7376 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/bucket_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5847 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/change_log.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3855 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/change_log_description_of_change.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3754 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5300 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/clone_media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6715 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/color_map.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3762 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/concat_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4324 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/create_list_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4228 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/create_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4548 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/credentials.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3485 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/download_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3223 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/download_info_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3850 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/email_attachment_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5904 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9514 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/encode_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7681 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/favorite.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6659 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/favorite_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/favorite_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/feed_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9920 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6208 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6170 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/file_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/file_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/file_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7650 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/file_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3854 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/fill.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5778 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/float_array_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4789 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/generic_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3653 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/generic_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3741 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/get_cloned_media_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/image_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9423 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/invitation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4364 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/invitation_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4424 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/invitation_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7272 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/job.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6531 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/job_cluster.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/job_cluster_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5756 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/job_node.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6287 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/job_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6072 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/job_spec_failure_email_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6316 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6786 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4398 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5040 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4165 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_suggestion.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6760 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5066 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4306 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5245 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/leaf_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3816 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/live_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4001 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/live_update_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    20648 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9814 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10180 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3743 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6826 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15764 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11602 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11084 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8114 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15159 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/localization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    18930 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10699 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10188 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_files.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5974 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_next.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3141 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_prev.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    15998 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5697 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_stats.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14738 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    14015 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11297 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    16079 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/media_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8877 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/membership.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5693 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/membership_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4593 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/membership_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3057 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/message_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5004 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/multi_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3077 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/not_found_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/notify_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6630 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/organization.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5620 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/organization_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5486 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/organization_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3234 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/password_reset_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13571 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/project.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9161 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/project_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8503 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/project_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8779 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/resolution_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/s3_storage_config.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7613 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/section.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6657 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/section_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/section_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12378 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8124 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_bulk_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    11740 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_bulk_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_delete.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6810 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_id_query.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3465 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_merge_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8846 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_trim_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13336 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_type.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12260 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_type_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6953 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_type_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9375 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/state_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7383 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/temporary_file.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5689 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/temporary_file_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2925 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/token.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3363 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/transcode.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10987 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/transcode_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4532 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/upload_completion_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4597 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/upload_info.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3883 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/upload_part.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7129 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/user.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8946 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/user_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     9465 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/user_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7988 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/version.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5820 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/version_spec.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5694 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/version_update.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4827 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/video_clip.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    10920 2023-07-22 18:59:36.000000 tator-1.1.0/tator/openapi/tator_openapi/models/video_definition.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    13486 2023-07-22 18:59:38.000000 tator-1.1.0/tator/openapi/tator_openapi/rest.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.408867 tator-1.1.0/tator/transcode/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7131 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/__main__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2105 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/black.mp4
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2175 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/create_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      993 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/delete_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9425 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/determine_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2286 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/make_fragment_info.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5938 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/make_thumbnails.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3559 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/prepare.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19475 2023-07-22 18:49:40.000000 tator-1.1.0/tator/transcode/transcode.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.412867 tator-1.1.0/tator/util/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2061 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2012 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/_download_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7168 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/_upload_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1681 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/chunked_file_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4470 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_leaf_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1544 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7441 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_localization_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2510 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11130 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_media_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1999 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2099 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1647 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6560 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_state_list.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2486 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2140 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4507 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/concat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1464 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/download_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4887 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2002 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/download_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2963 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/find_single_change.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1072 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/full_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      790 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/get_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2448 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/get_images.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3224 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/get_paginator.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      508 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/get_parser.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4282 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1732 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/live_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1989 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/md5sum.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3194 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17899 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7301 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/multi_stream.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2322 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/register_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2027 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/register_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5653 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/tator-symbol.png
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      530 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/to_dataframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2055 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/update_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1551 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/upload_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2008 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/upload_generic_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3476 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/upload_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1663 2023-07-22 18:49:40.000000 tator-1.1.0/tator/util/upload_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-07-22 18:49:40.000000 tator-1.1.0/tator/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.380866 tator-1.1.0/tator.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      321 2023-07-22 18:59:40.000000 tator-1.1.0/tator.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11802 2023-07-22 18:59:40.000000 tator-1.1.0/tator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-22 18:59:40.000000 tator-1.1.0/tator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       97 2023-07-22 18:59:40.000000 tator-1.1.0/tator.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-07-22 18:59:40.000000 tator-1.1.0/tator.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-22 18:59:40.416867 tator-1.1.0/test/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4863 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_a_float_array.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13689 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_algorithm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9519 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_algorithm_launch.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6577 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_applet.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1538 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_archive_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      945 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_attachment.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8615 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_attribute_type_addition.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2760 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_attribute_type_deletion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12411 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_attribute_type_mutation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_attributes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23755 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_change_log.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4177 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_chunked_create.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1517 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7222 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      576 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1209 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_membership.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_section.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1083 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      797 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_clone_version.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3604 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_collection.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6149 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_download_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2123 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_extract.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13655 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3140 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_file_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      585 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_get_clip.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      531 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_getframe.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_import_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2558 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_job_cancel.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1772 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_job_cluster.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3364 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_leaf.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1593 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_leaf_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3031 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_local_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9199 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_localization.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17733 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_localization_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2321 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_localization_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10371 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_media.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1423 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_media_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4905 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_poly.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      397 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_project_thumbnail.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9540 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_search.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9393 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_state.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1854 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_state_graphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1970 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_state_type.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1597 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_stategraphic.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1469 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_temporary_file.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3884 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_tracks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5502 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_transcode.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1923 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_util_media_manipulation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_util_media_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      912 2023-07-22 18:49:40.000000 tator-1.1.0/test/test_version.py
```

### Comparing `tator-1.0.5/README.md` & `tator-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/setup.py` & `tator-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/__init__.py` & `tator-1.1.0/tator/__init__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/extractor/__main__.py` & `tator-1.1.0/tator/extractor/__main__.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/extractor/env_launcher.py` & `tator-1.1.0/tator/extractor/env_launcher.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/extractor/extractor.py` & `tator-1.1.0/tator/extractor/extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             "md5": md5sum,
             "gid": upload_gid,
             "uid": str(uuid.uuid1()),
         },
     ]
     response = api.create_media_list(project, media_spec)
     assert isinstance(response, CreateResponse)
-    media_id = response.id
+    media_id = response.id[0]
 
     # Peel apart api to get host/token combo (TODO: not great)
     host = api.api_client.configuration.host
     token = api.api_client.configuration.api_key['Authorization']
     with tempfile.TemporaryDirectory(dir=work_dir) as td:
         try:
             thumb_path = os.path.join(td, f"{uuid.uuid4()}.jpg")
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/__init__.py` & `tator-1.1.0/tator/openapi/tator_openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: v1
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.0.5"
+__version__ = "1.1.0"
 
 # import apis into sdk package
 from tator.openapi.tator_openapi.api.tator_api import TatorApi
 
 # import ApiClient
 from tator.openapi.tator_openapi.api_client import ApiClient
 from tator.openapi.tator_openapi.configuration import Configuration
@@ -32,16 +32,14 @@
 from tator.openapi.tator_openapi.models.affiliation_spec import AffiliationSpec
 from tator.openapi.tator_openapi.models.affiliation_update import AffiliationUpdate
 from tator.openapi.tator_openapi.models.algorithm import Algorithm
 from tator.openapi.tator_openapi.models.algorithm_manifest import AlgorithmManifest
 from tator.openapi.tator_openapi.models.algorithm_manifest_spec import AlgorithmManifestSpec
 from tator.openapi.tator_openapi.models.algorithm_parameter import AlgorithmParameter
 from tator.openapi.tator_openapi.models.algorithm_spec import AlgorithmSpec
-from tator.openapi.tator_openapi.models.analysis import Analysis
-from tator.openapi.tator_openapi.models.analysis_spec import AnalysisSpec
 from tator.openapi.tator_openapi.models.announcement import Announcement
 from tator.openapi.tator_openapi.models.applet import Applet
 from tator.openapi.tator_openapi.models.applet_spec import AppletSpec
 from tator.openapi.tator_openapi.models.archive_config import ArchiveConfig
 from tator.openapi.tator_openapi.models.attribute_combinator_spec import AttributeCombinatorSpec
 from tator.openapi.tator_openapi.models.attribute_filter_spec import AttributeFilterSpec
 from tator.openapi.tator_openapi.models.attribute_operation_spec import AttributeOperationSpec
@@ -98,14 +96,15 @@
 from tator.openapi.tator_openapi.models.invitation_spec import InvitationSpec
 from tator.openapi.tator_openapi.models.invitation_update import InvitationUpdate
 from tator.openapi.tator_openapi.models.job import Job
 from tator.openapi.tator_openapi.models.job_cluster import JobCluster
 from tator.openapi.tator_openapi.models.job_cluster_spec import JobClusterSpec
 from tator.openapi.tator_openapi.models.job_node import JobNode
 from tator.openapi.tator_openapi.models.job_spec import JobSpec
+from tator.openapi.tator_openapi.models.job_spec_failure_email_spec import JobSpecFailureEmailSpec
 from tator.openapi.tator_openapi.models.leaf import Leaf
 from tator.openapi.tator_openapi.models.leaf_bulk_update import LeafBulkUpdate
 from tator.openapi.tator_openapi.models.leaf_id_query import LeafIdQuery
 from tator.openapi.tator_openapi.models.leaf_spec import LeafSpec
 from tator.openapi.tator_openapi.models.leaf_suggestion import LeafSuggestion
 from tator.openapi.tator_openapi.models.leaf_type import LeafType
 from tator.openapi.tator_openapi.models.leaf_type_spec import LeafTypeSpec
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/api/tator_api.py` & `tator-1.1.0/tator/openapi/tator_openapi/api/tator_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -51,27 +51,27 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -102,27 +102,27 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -145,27 +145,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -215,16 +215,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -249,14 +247,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -2691,15 +2692,15 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
-        :return: :class:`tator.models.CreateResponse`
+        :return: :class:`tator.models.CreateListResponse`
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.create_media_list_with_http_info(project, body, **kwargs)  # noqa: E501
 
     def create_media_list_with_http_info(self, project, body, **kwargs):  # noqa: E501
@@ -2720,15 +2721,15 @@
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
-        :return: tuple(:class:`tator.models.CreateResponse`, status_code(int), headers(HTTPHeaderDict))
+        :return: tuple(:class:`tator.models.CreateListResponse`, status_code(int), headers(HTTPHeaderDict))
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
@@ -2792,15 +2793,15 @@
             '/rest/Medias/{project}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='CreateResponse',  # noqa: E501
+            response_type='CreateListResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
@@ -3559,15 +3560,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
     def create_section(self, project, section_spec, **kwargs):
         """create_section
 
-        Create section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.   Note: In order for a section to be interpreted properly, the tator_user_sections attribute of the SectionSpec cannot be None. The front end assigns a uuid1 string for this attribute, but it is not required to follow this pattern.
+        Create section.  Sections represent groups of media using saved queries.   Note: In order for a section to be interpreted properly, the tator_user_sections attribute of the SectionSpec cannot be None. The front end assigns a uuid1 string for this attribute, but it is not required to follow this pattern.
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_section(project, section_spec, async_req=True)
         >>> result = thread.get()
 
@@ -3586,15 +3587,15 @@
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.create_section_with_http_info(project, section_spec, **kwargs)  # noqa: E501
 
     def create_section_with_http_info(self, project, section_spec, **kwargs):  # noqa: E501
         """
-        Create section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.   Note: In order for a section to be interpreted properly, the tator_user_sections attribute of the SectionSpec cannot be None. The front end assigns a uuid1 string for this attribute, but it is not required to follow this pattern.  # noqa: E501
+        Create section.  Sections represent groups of media using saved queries.   Note: In order for a section to be interpreted properly, the tator_user_sections attribute of the SectionSpec cannot be None. The front end assigns a uuid1 string for this attribute, but it is not required to follow this pattern.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.create_section_with_http_info(project, section_spec, async_req=True)
         >>> result = thread.get()
 
@@ -6676,15 +6677,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param LeafIdQuery leaf_id_query:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -6718,15 +6720,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param LeafIdQuery leaf_id_query:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -6753,14 +6756,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'leaf_id_query'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -6823,14 +6827,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -7116,42 +7123,44 @@
 
         >>> thread = api.delete_localization_list(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param LocalizationBulkDelete localization_bulk_delete:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -7172,42 +7181,44 @@
 
         >>> thread = api.delete_localization_list_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param LocalizationBulkDelete localization_bulk_delete:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -7220,14 +7231,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -7238,14 +7250,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'frame',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
@@ -7292,14 +7305,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -7337,14 +7353,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'frame' in local_var_params and local_var_params['frame'] is not None:  # noqa: E501
             query_params.append(('frame', local_var_params['frame']))  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
@@ -7659,36 +7678,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param MediaIdQuery media_id_query:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -7719,36 +7738,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param MediaIdQuery media_id_query:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -7771,27 +7790,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -7847,16 +7866,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -7881,14 +7898,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -8414,15 +8434,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
     def delete_section(self, id, **kwargs):
         """delete_section
 
-        Delete section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media. 
+        Delete section.  Sections represent groups of media using saved queries. 
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_section(id, async_req=True)
         >>> result = thread.get()
 
@@ -8440,15 +8460,15 @@
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.delete_section_with_http_info(id, **kwargs)  # noqa: E501
 
     def delete_section_with_http_info(self, id, **kwargs):  # noqa: E501
         """
-        Delete section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.   # noqa: E501
+        Delete section.  Sections represent groups of media using saved queries.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.delete_section_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
@@ -8668,41 +8688,43 @@
 
         >>> thread = api.delete_state_list(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param StateBulkDelete state_bulk_delete:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -8723,41 +8745,43 @@
 
         >>> thread = api.delete_state_list_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param StateBulkDelete state_bulk_delete:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -8770,14 +8794,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -8788,14 +8813,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -8839,14 +8865,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -8884,14 +8913,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -9443,36 +9475,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param MediaIdQuery media_id_query:
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -9503,36 +9535,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param MediaIdQuery media_id_query:
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
@@ -9555,27 +9587,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -9631,16 +9663,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -9665,14 +9695,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -10557,127 +10590,14 @@
             auth_settings=auth_settings,
             async_req=local_var_params.get('async_req'),
             _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
-    def get_anonymous_gateway_schema(self, **kwargs):
-        """get_anonymous_gateway_schema
-
-        Allows for logging into Tator as an anonymous user. 
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_anonymous_gateway_schema(async_req=True)
-        >>> result = thread.get()
-
-        :param bool async_req: execute request asynchronously
-        :param str redirect: URI to redirect to after logging in as anonymous user. Defaults to /projects.
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts. Default is 300.
-        :return: :class:`tator.models.list[object]`
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_anonymous_gateway_schema_with_http_info(**kwargs)  # noqa: E501
-
-    def get_anonymous_gateway_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """
-        Allows for logging into Tator as an anonymous user.   # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_anonymous_gateway_schema_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param bool async_req: execute request asynchronously
-        :param str redirect: URI to redirect to after logging in as anonymous user. Defaults to /projects.
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts. Default is 300.
-        :return: tuple(:class:`tator.models.list[object]`, status_code(int), headers(HTTPHeaderDict))
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        local_var_params = locals()
-
-        all_params = [
-            'redirect'
-        ]
-        all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout'
-            ]
-        )
-
-        for key, val in six.iteritems(local_var_params['kwargs']):
-            if key not in all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_anonymous_gateway_schema" % key
-                )
-            local_var_params[key] = val
-        del local_var_params['kwargs']
-
-        collection_formats = {}
-
-        path_params = {}
-
-        query_params = []
-        if 'redirect' in local_var_params and local_var_params['redirect'] is not None:  # noqa: E501
-            query_params.append(('redirect', local_var_params['redirect']))  # noqa: E501
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/plain'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['SessionAuth', 'TokenAuth']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/anonymous-gateway', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='list[object]',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=local_var_params.get('async_req'),
-            _return_http_data_only=local_var_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=local_var_params.get('_preload_content', True),
-            _request_timeout=local_var_params.get('_request_timeout',300),
-            collection_formats=collection_formats)
-
     def get_applet(self, id, **kwargs):
         """get_applet
 
         Get registered applet file
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
@@ -12793,15 +12713,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -12833,15 +12754,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -12865,15 +12787,16 @@
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -12932,14 +12855,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -14472,15 +14398,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -14513,15 +14440,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -14546,15 +14474,16 @@
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -14616,14 +14545,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -14674,15 +14606,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -14716,15 +14649,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -14750,15 +14684,16 @@
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -14824,14 +14759,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -14887,15 +14825,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -14928,15 +14867,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -14961,15 +14901,16 @@
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -15031,14 +14972,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -15089,15 +15033,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -15131,15 +15076,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -15165,15 +15111,16 @@
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -15239,14 +15186,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -15645,42 +15595,44 @@
 
         >>> thread = api.get_localization_count(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -15700,42 +15652,44 @@
 
         >>> thread = api.get_localization_count_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -15747,14 +15701,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -15765,14 +15720,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'frame',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
@@ -15818,14 +15774,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -15863,14 +15822,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'frame' in local_var_params and local_var_params['frame'] is not None:  # noqa: E501
             query_params.append(('frame', local_var_params['frame']))  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
@@ -15936,42 +15898,44 @@
         >>> thread = api.get_localization_count_by_id(project, localization_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param LocalizationIdQuery localization_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -15992,42 +15956,44 @@
         >>> thread = api.get_localization_count_by_id_with_http_info(project, localization_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param LocalizationIdQuery localization_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -16040,14 +16006,15 @@
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'localization_id_query',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -16058,14 +16025,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'frame',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
@@ -16115,14 +16083,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -16160,14 +16131,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'frame' in local_var_params and local_var_params['frame'] is not None:  # noqa: E501
             query_params.append(('frame', local_var_params['frame']))  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
@@ -16375,42 +16349,44 @@
 
         >>> thread = api.get_localization_list(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -16430,42 +16406,44 @@
 
         >>> thread = api.get_localization_list_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -16477,14 +16455,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -16495,14 +16474,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'frame',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
@@ -16548,14 +16528,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -16593,14 +16576,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'frame' in local_var_params and local_var_params['frame'] is not None:  # noqa: E501
             query_params.append(('frame', local_var_params['frame']))  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
@@ -16666,42 +16652,44 @@
         >>> thread = api.get_localization_list_by_id(project, localization_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param LocalizationIdQuery localization_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -16722,42 +16710,44 @@
         >>> thread = api.get_localization_list_by_id_with_http_info(project, localization_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param LocalizationIdQuery localization_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -16770,14 +16760,15 @@
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'localization_id_query',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -16788,14 +16779,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'frame',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
@@ -16845,14 +16837,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -16890,14 +16885,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'frame' in local_var_params and local_var_params['frame'] is not None:  # noqa: E501
             query_params.append(('frame', local_var_params['frame']))  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
@@ -17218,14 +17216,15 @@
 
         >>> thread = api.get_media(id, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int id: A unique integer identifying a media. (required)
         :param int presigned: If given, all `path` fields in `media_files` will be replaced with presigned URLs that can be downloaded without authentication. The value is the expiration time of the URLs in seconds.
+        :param bool no_cache: If `True`, and `presigned` is specified, a new presigned url will be generated.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -17245,14 +17244,15 @@
 
         >>> thread = api.get_media_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int id: A unique integer identifying a media. (required)
         :param int presigned: If given, all `path` fields in `media_files` will be replaced with presigned URLs that can be downloaded without authentication. The value is the expiration time of the URLs in seconds.
+        :param bool no_cache: If `True`, and `presigned` is specified, a new presigned url will be generated.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -17263,15 +17263,16 @@
                  returns the request thread.
         """
 
         local_var_params = locals()
 
         all_params = [
             'id',
-            'presigned'
+            'presigned',
+            'no_cache'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -17300,14 +17301,16 @@
         path_params = {}
         if 'id' in local_var_params:
             path_params['id'] = local_var_params['id']  # noqa: E501
 
         query_params = []
         if 'presigned' in local_var_params and local_var_params['presigned'] is not None:  # noqa: E501
             query_params.append(('presigned', local_var_params['presigned']))  # noqa: E501
+        if 'no_cache' in local_var_params and local_var_params['no_cache'] is not None:  # noqa: E501
+            query_params.append(('no_cache', local_var_params['no_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -17354,36 +17357,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -17413,36 +17416,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -17464,27 +17467,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -17539,16 +17542,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -17573,14 +17574,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -17654,36 +17658,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -17714,36 +17718,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -17766,27 +17770,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -17845,16 +17849,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -17879,14 +17881,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -17965,37 +17970,38 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param int presigned: If given, all `path` fields in `media_files` will be replaced with presigned URLs that can be downloaded without authentication. The value is the expiration time of the URLs in seconds.
+        :param bool no_cache: If `True`, and `presigned` is specified, a new presigned url will be generated.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -18025,37 +18031,38 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param int presigned: If given, all `path` fields in `media_files` will be replaced with presigned URLs that can be downloaded without authentication. The value is the expiration time of the URLs in seconds.
+        :param bool no_cache: If `True`, and `presigned` is specified, a new presigned url will be generated.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -18077,37 +18084,38 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
             'related_attribute_null',
             'encoded_related_search',
-            'presigned'
+            'presigned',
+            'no_cache'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -18157,16 +18165,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -18191,14 +18197,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -18219,14 +18228,16 @@
         if 'related_attribute_null' in local_var_params and local_var_params['related_attribute_null'] is not None:  # noqa: E501
             query_params.append(('related_attribute_null', local_var_params['related_attribute_null']))  # noqa: E501
             collection_formats['related_attribute_null'] = 'csv'  # noqa: E501
         if 'encoded_related_search' in local_var_params and local_var_params['encoded_related_search'] is not None:  # noqa: E501
             query_params.append(('encoded_related_search', local_var_params['encoded_related_search']))  # noqa: E501
         if 'presigned' in local_var_params and local_var_params['presigned'] is not None:  # noqa: E501
             query_params.append(('presigned', local_var_params['presigned']))  # noqa: E501
+        if 'no_cache' in local_var_params and local_var_params['no_cache'] is not None:  # noqa: E501
+            query_params.append(('no_cache', local_var_params['no_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -18274,37 +18285,38 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param int presigned: If given, all `path` fields in `media_files` will be replaced with presigned URLs that can be downloaded without authentication. The value is the expiration time of the URLs in seconds.
+        :param bool no_cache: If `True`, and `presigned` is specified, a new presigned url will be generated.
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -18335,37 +18347,38 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param int presigned: If given, all `path` fields in `media_files` will be replaced with presigned URLs that can be downloaded without authentication. The value is the expiration time of the URLs in seconds.
+        :param bool no_cache: If `True`, and `presigned` is specified, a new presigned url will be generated.
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -18388,37 +18401,38 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
             'related_attribute_null',
             'encoded_related_search',
-            'presigned'
+            'presigned',
+            'no_cache'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -18472,16 +18486,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -18506,14 +18518,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -18534,14 +18549,16 @@
         if 'related_attribute_null' in local_var_params and local_var_params['related_attribute_null'] is not None:  # noqa: E501
             query_params.append(('related_attribute_null', local_var_params['related_attribute_null']))  # noqa: E501
             collection_formats['related_attribute_null'] = 'csv'  # noqa: E501
         if 'encoded_related_search' in local_var_params and local_var_params['encoded_related_search'] is not None:  # noqa: E501
             query_params.append(('encoded_related_search', local_var_params['encoded_related_search']))  # noqa: E501
         if 'presigned' in local_var_params and local_var_params['presigned'] is not None:  # noqa: E501
             query_params.append(('presigned', local_var_params['presigned']))  # noqa: E501
+        if 'no_cache' in local_var_params and local_var_params['no_cache'] is not None:  # noqa: E501
+            query_params.append(('no_cache', local_var_params['no_cache']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -18594,36 +18611,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -18653,36 +18670,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -18704,27 +18721,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -18779,16 +18796,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -18813,14 +18828,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -18893,36 +18911,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -18952,36 +18970,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -19003,27 +19021,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -19078,16 +19096,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -19112,14 +19128,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -19192,36 +19211,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -19251,36 +19270,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -19302,27 +19321,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -19377,16 +19396,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -19411,14 +19428,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -20669,15 +20689,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
     def get_section(self, id, **kwargs):
         """get_section
 
-        Get section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media. 
+        Get section.  Sections represent groups of media using saved queries. 
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_section(id, async_req=True)
         >>> result = thread.get()
 
@@ -20695,15 +20715,15 @@
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.get_section_with_http_info(id, **kwargs)  # noqa: E501
 
     def get_section_with_http_info(self, id, **kwargs):  # noqa: E501
         """
-        Get section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.   # noqa: E501
+        Get section.  Sections represent groups of media using saved queries.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_section_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
@@ -20786,15 +20806,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
     def get_section_list(self, project, **kwargs):
         """get_section_list
 
-        Get section list.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.   
+        Get section list.  Sections represent groups of media using saved queries.   
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_section_list(project, async_req=True)
         >>> result = thread.get()
 
@@ -20814,15 +20834,15 @@
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.get_section_list_with_http_info(project, **kwargs)  # noqa: E501
 
     def get_section_list_with_http_info(self, project, **kwargs):  # noqa: E501
         """
-        Get section list.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.     # noqa: E501
+        Get section list.  Sections represent groups of media using saved queries.     # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_section_list_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
@@ -21041,41 +21061,43 @@
 
         >>> thread = api.get_state_count(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -21095,41 +21117,43 @@
 
         >>> thread = api.get_state_count_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -21141,14 +21165,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -21159,14 +21184,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -21209,14 +21235,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -21254,14 +21283,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -21325,41 +21357,43 @@
         >>> thread = api.get_state_count_by_id(project, state_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param StateIdQuery state_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -21380,41 +21414,43 @@
         >>> thread = api.get_state_count_by_id_with_http_info(project, state_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param StateIdQuery state_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -21427,14 +21463,15 @@
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'state_id_query',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -21445,14 +21482,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -21499,14 +21537,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -21544,14 +21585,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -21764,41 +21808,43 @@
 
         >>> thread = api.get_state_list(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -21818,41 +21864,43 @@
 
         >>> thread = api.get_state_list_with_http_info(project, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -21864,14 +21912,15 @@
         """
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -21882,14 +21931,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -21932,14 +21982,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -21977,14 +22030,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -22048,41 +22104,43 @@
         >>> thread = api.get_state_list_by_id(project, state_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param StateIdQuery state_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -22103,41 +22161,43 @@
         >>> thread = api.get_state_list_by_id_with_http_info(project, state_id_query, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param StateIdQuery state_id_query: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -22150,14 +22210,15 @@
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'state_id_query',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -22168,14 +22229,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -22222,14 +22284,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -22267,14 +22332,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -22959,36 +23027,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -23018,36 +23086,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -23069,27 +23137,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -23144,16 +23212,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -23178,14 +23244,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -23259,36 +23328,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -23319,36 +23388,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -23371,27 +23440,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -23450,16 +23519,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -23484,14 +23551,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -27921,15 +27991,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -27963,15 +28034,16 @@
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -27997,15 +28069,16 @@
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
-            'encoded_search'
+            'encoded_search',
+            'sort_by'
         ]
         all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout'
@@ -28071,14 +28144,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -28382,42 +28458,44 @@
         >>> thread = api.update_localization_list(project, localization_bulk_update, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param LocalizationBulkUpdate localization_bulk_update: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -28438,42 +28516,44 @@
         >>> thread = api.update_localization_list_with_http_info(project, localization_bulk_update, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param LocalizationBulkUpdate localization_bulk_update: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param int frame: Frame number of this localization if it is in a video.
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -28486,14 +28566,15 @@
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'localization_bulk_update',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -28504,14 +28585,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'frame',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
@@ -28561,14 +28643,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -28606,14 +28691,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'frame' in local_var_params and local_var_params['frame'] is not None:  # noqa: E501
             query_params.append(('frame', local_var_params['frame']))  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
@@ -28955,36 +29043,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -29015,36 +29103,36 @@
         :param str dtype: Data type of the files, either image or video.
         :param str md5: MD5 sum of the media file.
         :param str gid: Upload group ID of the media file.
         :param str uid: Upload unique ID of the media file.
         :param int after: If given, all results returned will be after the media with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str after_name: If given, all results returned will be after the media with this name. The `start` and `stop` parameters are relative to this modified range.
         :param str archive_lifecycle: Archive lifecycle of the files, one of live (live only), archived (to_archive, archived, or to_live), or all. Defaults to 'live'
-        :param str annotation_search: Lucene query syntax string for use with Elasticsearch. See [reference](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax). This search is applied to child annotations of media only.
         :param str elemental_id: Elemental ID to search for
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -29067,27 +29155,27 @@
             'dtype',
             'md5',
             'gid',
             'uid',
             'after',
             'after_name',
             'archive_lifecycle',
-            'annotation_search',
             'elemental_id',
             'attribute',
             'attribute_lt',
             'attribute_lte',
             'attribute_gt',
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -29146,16 +29234,14 @@
             query_params.append(('uid', local_var_params['uid']))  # noqa: E501
         if 'after' in local_var_params and local_var_params['after'] is not None:  # noqa: E501
             query_params.append(('after', local_var_params['after']))  # noqa: E501
         if 'after_name' in local_var_params and local_var_params['after_name'] is not None:  # noqa: E501
             query_params.append(('after_name', local_var_params['after_name']))  # noqa: E501
         if 'archive_lifecycle' in local_var_params and local_var_params['archive_lifecycle'] is not None:  # noqa: E501
             query_params.append(('archive_lifecycle', local_var_params['archive_lifecycle']))  # noqa: E501
-        if 'annotation_search' in local_var_params and local_var_params['annotation_search'] is not None:  # noqa: E501
-            query_params.append(('annotation_search', local_var_params['annotation_search']))  # noqa: E501
         if 'elemental_id' in local_var_params and local_var_params['elemental_id'] is not None:  # noqa: E501
             query_params.append(('elemental_id', local_var_params['elemental_id']))  # noqa: E501
         if 'attribute' in local_var_params and local_var_params['attribute'] is not None:  # noqa: E501
             query_params.append(('attribute', local_var_params['attribute']))  # noqa: E501
             collection_formats['attribute'] = 'csv'  # noqa: E501
         if 'attribute_lt' in local_var_params and local_var_params['attribute_lt'] is not None:  # noqa: E501
             query_params.append(('attribute_lt', local_var_params['attribute_lt']))  # noqa: E501
@@ -29180,14 +29266,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
@@ -29765,15 +29854,15 @@
             _preload_content=local_var_params.get('_preload_content', True),
             _request_timeout=local_var_params.get('_request_timeout',300),
             collection_formats=collection_formats)
 
     def update_section(self, id, section_update, **kwargs):
         """update_section
 
-        Update section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media. 
+        Update section.  Sections represent groups of media using saved queries. 
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_section(id, section_update, async_req=True)
         >>> result = thread.get()
 
@@ -29792,15 +29881,15 @@
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         return self.update_section_with_http_info(id, section_update, **kwargs)  # noqa: E501
 
     def update_section_with_http_info(self, id, section_update, **kwargs):  # noqa: E501
         """
-        Update section.  Sections represent groups of media using saved queries. The queries can be in the form of a [lucene search string](https://www.elastic.co/guide/en/elasticsearch/reference/7.10/query-dsl-query-string-query.html#query-string-syntax) or a list of [boolean filter queries](https://www.elastic.co/guide/en/elasticsearch/reference/current/query-dsl-bool-query.html) applied to either media or child annotations of media.   # noqa: E501
+        Update section.  Sections represent groups of media using saved queries.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_section_with_http_info(id, section_update, async_req=True)
         >>> result = thread.get()
 
@@ -30037,41 +30126,43 @@
         >>> thread = api.update_state_list(project, state_bulk_update, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param StateBulkUpdate state_bulk_update: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts. Default is 300.
@@ -30092,41 +30183,43 @@
         >>> thread = api.update_state_list_with_http_info(project, state_bulk_update, async_req=True)
         >>> result = thread.get()
 
         :param bool async_req: execute request asynchronously
         :param int project: A unique integer identifying a project. (required)
         :param StateBulkUpdate state_bulk_update: (required)
         :param list[int] media_id: Comma-separated list of media IDs.
+        :param list[int] related_id: Comma-separated list of related IDs. If querying States, one can supply a list of related localization ids to filter on.If querying Localizations, one can supply a list of related state ids to filter on.
         :param int section: Unique integer identifying a media section.
         :param int type: Unique integer identifying a annotation type.
         :param list[int] version: List of integers representing versions to fetch
         :param int after: If given, all results returned will be after the localization with this ID. The `start` and `stop` parameters are relative to this modified range.
         :param str elemental_id: Elemental ID to search for
-        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.An exception occurs if an Elasticsearch query is triggered and pagination parameters (start or stop) are included.
+        :param int merge: Reduce result set based on a server side merge. If multiple versions are selected and a variant of the object exists in both versions, the merge logic will return 1 or 0 objects. Example:  Version B derives off Version A. An object, with the same elemental id \"foo\" exists on both. If Version B over A is selected and merge is turned on: + The \"foo\" present on Version B is returned  + If the \"foo\" on version B is deleted, no \"foo\" is returned.
         :param int show_deleted: Include in the return set objects that have `variant_deleted` set to True.
         :param list[str] attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].
         :param list[str] attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].
         :param list[str] attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.
         :param int start: Pagination start index. Index of the first item in a larger list to return.
         :param int stop: Pagination stop index. Non-inclusive index of the last item in a larger list to return.
-        :param str encoded_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter
+        :param str encoded_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec
+        :param list[str] sort_by: Field names to sort results by. Built-in names should be prefixed with '$', attributes must not be.                   Because the schema supports sorting by a list of attributes (effectively grouping), we have to utilize a special character to inform direction.         Uses the common convention of '-'; thus `[\"$name\", \"-$id\"]` would sort by name ascending and break tie-breakers(grouping) by descending by id.          An example REST query will sort all localizations in project 1, by label descending and sort any ties by ascending x.          `rest/Localizations/1?sort_by=-Label&sort_by=$x`           A table of built-ins available for a given type:                          | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
         :param list[str] related_attribute: Attribute equality filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lt: Attribute less than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_lte: Attribute less than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gt: Attribute greater than filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_gte: Attribute greater than or equal filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_contains: Attribute contains filter. Format is attribute1::value1,[attribute2::value2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_distance: Range filter for geoposition attributes. Format is attribute1::distance_km2::lat2::lon2,[attribute2::distancekm2::lat2::lon2].This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
         :param list[str] related_attribute_null: Attribute null filter. Returns elements for which a given attribute is not defined.This filter is applied to related data of the primary object.On the Media endpoint, this searches on related metadata(States/Localizations).On metadata endpoints, this searches on related media.
-        :param str encoded_related_search: Binary64 encoded string representing an `Object_Search` defined in /components/AttributeOperationFilter applied against related objects
+        :param str encoded_related_search: Base64 encoded string representing an `Object_Search` defined in /components/AttributeOperationSpec applied against related objects
         :param _return_http_data_only: response data without head status code
                                        and headers
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
@@ -30139,14 +30232,15 @@
 
         local_var_params = locals()
 
         all_params = [
             'project',
             'state_bulk_update',
             'media_id',
+            'related_id',
             'section',
             'type',
             'version',
             'after',
             'elemental_id',
             'merge',
             'show_deleted',
@@ -30157,14 +30251,15 @@
             'attribute_gte',
             'attribute_contains',
             'attribute_distance',
             'attribute_null',
             'start',
             'stop',
             'encoded_search',
+            'sort_by',
             'related_attribute',
             'related_attribute_lt',
             'related_attribute_lte',
             'related_attribute_gt',
             'related_attribute_gte',
             'related_attribute_contains',
             'related_attribute_distance',
@@ -30211,14 +30306,17 @@
         if 'project' in local_var_params:
             path_params['project'] = local_var_params['project']  # noqa: E501
 
         query_params = []
         if 'media_id' in local_var_params and local_var_params['media_id'] is not None:  # noqa: E501
             query_params.append(('media_id', local_var_params['media_id']))  # noqa: E501
             collection_formats['media_id'] = 'csv'  # noqa: E501
+        if 'related_id' in local_var_params and local_var_params['related_id'] is not None:  # noqa: E501
+            query_params.append(('related_id', local_var_params['related_id']))  # noqa: E501
+            collection_formats['related_id'] = 'csv'  # noqa: E501
         if 'section' in local_var_params and local_var_params['section'] is not None:  # noqa: E501
             query_params.append(('section', local_var_params['section']))  # noqa: E501
         if 'type' in local_var_params and local_var_params['type'] is not None:  # noqa: E501
             query_params.append(('type', local_var_params['type']))  # noqa: E501
         if 'version' in local_var_params and local_var_params['version'] is not None:  # noqa: E501
             query_params.append(('version', local_var_params['version']))  # noqa: E501
             collection_formats['version'] = 'csv'  # noqa: E501
@@ -30256,14 +30354,17 @@
             collection_formats['attribute_null'] = 'csv'  # noqa: E501
         if 'start' in local_var_params and local_var_params['start'] is not None:  # noqa: E501
             query_params.append(('start', local_var_params['start']))  # noqa: E501
         if 'stop' in local_var_params and local_var_params['stop'] is not None:  # noqa: E501
             query_params.append(('stop', local_var_params['stop']))  # noqa: E501
         if 'encoded_search' in local_var_params and local_var_params['encoded_search'] is not None:  # noqa: E501
             query_params.append(('encoded_search', local_var_params['encoded_search']))  # noqa: E501
+        if 'sort_by' in local_var_params and local_var_params['sort_by'] is not None:  # noqa: E501
+            query_params.append(('sort_by', local_var_params['sort_by']))  # noqa: E501
+            collection_formats['sort_by'] = 'multi'  # noqa: E501
         if 'related_attribute' in local_var_params and local_var_params['related_attribute'] is not None:  # noqa: E501
             query_params.append(('related_attribute', local_var_params['related_attribute']))  # noqa: E501
             collection_formats['related_attribute'] = 'csv'  # noqa: E501
         if 'related_attribute_lt' in local_var_params and local_var_params['related_attribute_lt'] is not None:  # noqa: E501
             query_params.append(('related_attribute_lt', local_var_params['related_attribute_lt']))  # noqa: E501
             collection_formats['related_attribute_lt'] = 'csv'  # noqa: E501
         if 'related_attribute_lte' in local_var_params and local_var_params['related_attribute_lte'] is not None:  # noqa: E501
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/api_client.py` & `tator-1.1.0/tator/openapi/tator_openapi/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.5/python'
+        self.user_agent = 'OpenAPI-Generator/1.1.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/configuration.py` & `tator-1.1.0/tator/openapi/tator_openapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.0.5".\
+               "SDK Package Version: 1.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/exceptions.py` & `tator-1.1.0/tator/openapi/tator_openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/__init__.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 from tator.openapi.tator_openapi.models.affiliation_spec import AffiliationSpec
 from tator.openapi.tator_openapi.models.affiliation_update import AffiliationUpdate
 from tator.openapi.tator_openapi.models.algorithm import Algorithm
 from tator.openapi.tator_openapi.models.algorithm_manifest import AlgorithmManifest
 from tator.openapi.tator_openapi.models.algorithm_manifest_spec import AlgorithmManifestSpec
 from tator.openapi.tator_openapi.models.algorithm_parameter import AlgorithmParameter
 from tator.openapi.tator_openapi.models.algorithm_spec import AlgorithmSpec
-from tator.openapi.tator_openapi.models.analysis import Analysis
-from tator.openapi.tator_openapi.models.analysis_spec import AnalysisSpec
 from tator.openapi.tator_openapi.models.announcement import Announcement
 from tator.openapi.tator_openapi.models.applet import Applet
 from tator.openapi.tator_openapi.models.applet_spec import AppletSpec
 from tator.openapi.tator_openapi.models.archive_config import ArchiveConfig
 from tator.openapi.tator_openapi.models.attribute_combinator_spec import AttributeCombinatorSpec
 from tator.openapi.tator_openapi.models.attribute_filter_spec import AttributeFilterSpec
 from tator.openapi.tator_openapi.models.attribute_operation_spec import AttributeOperationSpec
@@ -84,14 +82,15 @@
 from tator.openapi.tator_openapi.models.invitation_spec import InvitationSpec
 from tator.openapi.tator_openapi.models.invitation_update import InvitationUpdate
 from tator.openapi.tator_openapi.models.job import Job
 from tator.openapi.tator_openapi.models.job_cluster import JobCluster
 from tator.openapi.tator_openapi.models.job_cluster_spec import JobClusterSpec
 from tator.openapi.tator_openapi.models.job_node import JobNode
 from tator.openapi.tator_openapi.models.job_spec import JobSpec
+from tator.openapi.tator_openapi.models.job_spec_failure_email_spec import JobSpecFailureEmailSpec
 from tator.openapi.tator_openapi.models.leaf import Leaf
 from tator.openapi.tator_openapi.models.leaf_bulk_update import LeafBulkUpdate
 from tator.openapi.tator_openapi.models.leaf_id_query import LeafIdQuery
 from tator.openapi.tator_openapi.models.leaf_spec import LeafSpec
 from tator.openapi.tator_openapi.models.leaf_suggestion import LeafSuggestion
 from tator.openapi.tator_openapi.models.leaf_type import LeafType
 from tator.openapi.tator_openapi.models.leaf_type_spec import LeafTypeSpec
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/affiliation.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/affiliation.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,61 +30,61 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'email': 'str',
         'first_name': 'str',
         'id': 'int',
         'last_name': 'str',
-        'organization': 'int',
+        'organization_id': 'int',
         'permission': 'str',
-        'user': 'int',
+        'user_id': 'int',
         'username': 'str'
     }
 
     attribute_map = {
         'email': 'email',
         'first_name': 'first_name',
         'id': 'id',
         'last_name': 'last_name',
-        'organization': 'organization',
+        'organization_id': 'organization_id',
         'permission': 'permission',
-        'user': 'user',
+        'user_id': 'user_id',
         'username': 'username'
     }
 
-    def __init__(self, email=None, first_name=None, id=None, last_name=None, organization=None, permission=None, user=None, username=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, email=None, first_name=None, id=None, last_name=None, organization_id=None, permission=None, user_id=None, username=None, local_vars_configuration=None):  # noqa: E501
         """Affiliation - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._email = None
         self._first_name = None
         self._id = None
         self._last_name = None
-        self._organization = None
+        self._organization_id = None
         self._permission = None
-        self._user = None
+        self._user_id = None
         self._username = None
         self.discriminator = None
 
         if email is not None:
             self.email = email
         if first_name is not None:
             self.first_name = first_name
         if id is not None:
             self.id = id
         if last_name is not None:
             self.last_name = last_name
-        if organization is not None:
-            self.organization = organization
+        if organization_id is not None:
+            self.organization_id = organization_id
         if permission is not None:
             self.permission = permission
-        if user is not None:
-            self.user = user
+        if user_id is not None:
+            self.user_id = user_id
         if username is not None:
             self.username = username
 
     @property
     def email(self):
         """
         Email address of user.
@@ -165,36 +165,36 @@
         :param last_name: The last_name of this Affiliation.
         :type: str
         """
 
         self._last_name = last_name
 
     @property
-    def organization(self):
+    def organization_id(self):
         """
         Unique integer identifying an organization.
 
-        :return: The organization of this Affiliation. 
+        :return: The organization_id of this Affiliation. 
         :rtype: int
         """
-        return self._organization
+        return self._organization_id
 
-    @organization.setter
-    def organization(self, organization):
+    @organization_id.setter
+    def organization_id(self, organization_id):
         """
         Unique integer identifying an organization.
 
-        :param organization: The organization of this Affiliation.
+        :param organization_id: The organization_id of this Affiliation.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                organization is not None and organization < 1):  # noqa: E501
-            raise ValueError("Invalid value for `organization`, must be a value greater than or equal to `1`")  # noqa: E501
+                organization_id is not None and organization_id < 1):  # noqa: E501
+            raise ValueError("Invalid value for `organization_id`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._organization = organization
+        self._organization_id = organization_id
 
     @property
     def permission(self):
         """
         User permission level for the organization.
 
         :return: The permission of this Affiliation. 
@@ -216,36 +216,36 @@
                 "Invalid value for `permission` ({0}), must be one of {1}"  # noqa: E501
                 .format(permission, allowed_values)
             )
 
         self._permission = permission
 
     @property
-    def user(self):
+    def user_id(self):
         """
         Unique integer identifying a user.
 
-        :return: The user of this Affiliation. 
+        :return: The user_id of this Affiliation. 
         :rtype: int
         """
-        return self._user
+        return self._user_id
 
-    @user.setter
-    def user(self, user):
+    @user_id.setter
+    def user_id(self, user_id):
         """
         Unique integer identifying a user.
 
-        :param user: The user of this Affiliation.
+        :param user_id: The user_id of this Affiliation.
         :type: int
         """
         if (self.local_vars_configuration.client_side_validation and
-                user is not None and user < 1):  # noqa: E501
-            raise ValueError("Invalid value for `user`, must be a value greater than or equal to `1`")  # noqa: E501
+                user_id is not None and user_id < 1):  # noqa: E501
+            raise ValueError("Invalid value for `user_id`, must be a value greater than or equal to `1`")  # noqa: E501
 
-        self._user = user
+        self._user_id = user_id
 
     @property
     def username(self):
         """
         Username for the membership.
 
         :return: The username of this Affiliation.
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/affiliation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/affiliation_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/affiliation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_manifest.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_manifest_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_parameter.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_parameter.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/algorithm_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/algorithm_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/analysis.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/download_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,117 +14,91 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Analysis(object):
+class DownloadInfo(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'data_query': 'str',
-        'id': 'int',
-        'name': 'str'
+        'key': 'str',
+        'url': 'str'
     }
 
     attribute_map = {
-        'data_query': 'data_query',
-        'id': 'id',
-        'name': 'name'
+        'key': 'key',
+        'url': 'url'
     }
 
-    def __init__(self, data_query='*', id=None, name=None, local_vars_configuration=None):  # noqa: E501
-        """Analysis - a model defined in OpenAPI"""
+    def __init__(self, key=None, url=None, local_vars_configuration=None):  # noqa: E501
+        """DownloadInfo - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._data_query = None
-        self._id = None
-        self._name = None
+        self._key = None
+        self._url = None
         self.discriminator = None
 
-        if data_query is not None:
-            self.data_query = data_query
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
+        if key is not None:
+            self.key = key
+        if url is not None:
+            self.url = url
 
     @property
-    def data_query(self):
+    def key(self):
         """
-        Lucene query string used to retrieve entities to analyze.
+        Object key.
 
-        :return: The data_query of this Analysis. 
+        :return: The key of this DownloadInfo. 
         :rtype: str
         """
-        return self._data_query
+        return self._key
 
-    @data_query.setter
-    def data_query(self, data_query):
+    @key.setter
+    def key(self, key):
         """
-        Lucene query string used to retrieve entities to analyze.
+        Object key.
 
-        :param data_query: The data_query of this Analysis.
+        :param key: The key of this DownloadInfo.
         :type: str
         """
 
-        self._data_query = data_query
+        self._key = key
 
     @property
-    def id(self):
+    def url(self):
         """
-        Unique integer identifying the analysis.
+        URL for downloading object specified by key.
 
-        :return: The id of this Analysis. 
-        :rtype: int
-        """
-        return self._id
-
-    @id.setter
-    def id(self, id):
-        """
-        Unique integer identifying the analysis.
-
-        :param id: The id of this Analysis.
-        :type: int
-        """
-
-        self._id = id
-
-    @property
-    def name(self):
-        """
-        Name of analysis.
-
-        :return: The name of this Analysis. 
+        :return: The url of this DownloadInfo. 
         :rtype: str
         """
-        return self._name
+        return self._url
 
-    @name.setter
-    def name(self, name):
+    @url.setter
+    def url(self, url):
         """
-        Name of analysis.
+        URL for downloading object specified by key.
 
-        :param name: The name of this Analysis.
+        :param url: The url of this DownloadInfo.
         :type: str
         """
 
-        self._name = name
+        self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -152,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Analysis):
+        if not isinstance(other, DownloadInfo):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Analysis):
+        if not isinstance(other, DownloadInfo):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/analysis_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/fill.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,93 +14,97 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class AnalysisSpec(object):
+class Fill(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'data_query': 'str',
-        'name': 'str'
+        'color': 'object',
+        'style': 'str'
     }
 
     attribute_map = {
-        'data_query': 'data_query',
-        'name': 'name'
+        'color': 'color',
+        'style': 'style'
     }
 
-    def __init__(self, data_query='*', name=None, local_vars_configuration=None):  # noqa: E501
-        """AnalysisSpec - a model defined in OpenAPI"""
+    def __init__(self, color=None, style=None, local_vars_configuration=None):  # noqa: E501
+        """Fill - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._data_query = None
-        self._name = None
+        self._color = None
+        self._style = None
         self.discriminator = None
 
-        self.data_query = data_query
-        self.name = name
+        if color is not None:
+            self.color = color
+        if style is not None:
+            self.style = style
 
     @property
-    def data_query(self):
+    def color(self):
         """
-        Lucene query string used to retrieve entities to analyze.
+        RGB array, RGBA array, or hex string.
 
-        :return: The data_query of this AnalysisSpec. 
-        :rtype: str
+        :return: The color of this Fill. 
+        :rtype: object
         """
-        return self._data_query
+        return self._color
 
-    @data_query.setter
-    def data_query(self, data_query):
+    @color.setter
+    def color(self, color):
         """
-        Lucene query string used to retrieve entities to analyze.
+        RGB array, RGBA array, or hex string.
 
-        :param data_query: The data_query of this AnalysisSpec.
-        :type: str
+        :param color: The color of this Fill.
+        :type: object
         """
-        if self.local_vars_configuration.client_side_validation and data_query is None:  # noqa: E501
-            raise ValueError("Invalid value for `data_query`, must not be `None`")  # noqa: E501
 
-        self._data_query = data_query
+        self._color = color
 
     @property
-    def name(self):
+    def style(self):
         """
-        Name of analysis.
+        Type of fill effect
 
-        :return: The name of this AnalysisSpec. 
+        :return: The style of this Fill. 
         :rtype: str
         """
-        return self._name
+        return self._style
 
-    @name.setter
-    def name(self, name):
+    @style.setter
+    def style(self, style):
         """
-        Name of analysis.
+        Type of fill effect
 
-        :param name: The name of this AnalysisSpec.
+        :param style: The style of this Fill.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and name is None:  # noqa: E501
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
+        allowed_values = ["fill", "blur", "gray"]  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and style not in allowed_values:  # noqa: E501
+            raise ValueError(
+                "Invalid value for `style` ({0}), must be one of {1}"  # noqa: E501
+                .format(style, allowed_values)
+            )
 
-        self._name = name
+        self._style = style
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -128,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, AnalysisSpec):
+        if not isinstance(other, Fill):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, AnalysisSpec):
+        if not isinstance(other, Fill):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/announcement.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/announcement.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/applet.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/applet_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/applet_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/archive_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/archive_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_combinator_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_combinator_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_filter_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_filter_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,25 +62,25 @@
         if operation is not None:
             self.operation = operation
         self.value = value
 
     @property
     def attribute(self):
         """
-        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |                |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|               | section           | Media section                          |       X       |   X    |   X    |        |       |               | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |               | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |               | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |               | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |               | name              | The name of the element                |               |        |   X    |    X   |   X   |               | fps               | The frames per second                  |               |        |   X    |        |       |               | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |               | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |               | archive_state     | The current archive state of the media |               |        |   X    |        |       |               | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |               | width or height   | Geometric sizes                        |               |        |        |        |       |                               
+        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
 
         :return: The attribute of this AttributeFilterSpec. 
         :rtype: str
         """
         return self._attribute
 
     @attribute.setter
     def attribute(self, attribute):
         """
-        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |                |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|               | section           | Media section                          |       X       |   X    |   X    |        |       |               | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |               | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |               | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |               | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |               | name              | The name of the element                |               |        |   X    |    X   |   X   |               | fps               | The frames per second                  |               |        |   X    |        |       |               | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |               | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |               | archive_state     | The current archive state of the media |               |        |   X    |        |       |               | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |               | width or height   | Geometric sizes                        |               |        |        |        |       |                               
+        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
 
         :param attribute: The attribute of this AttributeFilterSpec.
         :type: str
         """
 
         self._attribute = attribute
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_operation_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_operation_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,25 +120,25 @@
         """
 
         self._operations = operations
 
     @property
     def attribute(self):
         """
-        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |                |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|               | section           | Media section                          |       X       |   X    |   X    |        |       |               | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |               | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |               | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |               | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |               | name              | The name of the element                |               |        |   X    |    X   |   X   |               | fps               | The frames per second                  |               |        |   X    |        |       |               | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |               | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |               | archive_state     | The current archive state of the media |               |        |   X    |        |       |               | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |               | width or height   | Geometric sizes                        |               |        |        |        |       |                               
+        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
 
         :return: The attribute of this AttributeOperationSpec. 
         :rtype: str
         """
         return self._attribute
 
     @attribute.setter
     def attribute(self, attribute):
         """
-        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |                |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|               | section           | Media section                          |       X       |   X    |   X    |        |       |               | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |               | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |               | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |               | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |               | name              | The name of the element                |               |        |   X    |    X   |   X   |               | fps               | The frames per second                  |               |        |   X    |        |       |               | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |               | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |               | archive_state     | The current archive state of the media |               |        |   X    |        |       |               | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |               | width or height   | Geometric sizes                        |               |        |        |        |       |                               
+        Name of the attribute or field to search on.                               Given a user defined type (Localization, State, or Media) with defined attributes                any attribute is searchable by its name. If a Localization has an attribute named 'Species'                the name to use to search on that column is 'Species'.                 Additional built-in columns are available to search on dependent on the underlying metadata               type being searched. To search a built in field, a '$' character must be used in front of the column               name from main.models.                              The following table shows common columns and to which types they apply. Any internal column                of the model may be searched in this manner.                              '$' must precede these names in search attempts. E.g. `created_by` is supplied as `$created_by`.                    | Name              | Description                            | Localizations | States | Medias | Leaves | Files |      |-------------------|----------------------------------------|---------------|--------|--------|--------|-------|     | section           | Media section                          |       X       |   X    |   X    |        |       |     | created_datetime  | The time of creation for this datum    |       X       |   X    |   X    |    X   |   X   |     | created_by        | The user id who created this datum     |       X       |   X    |   X    |    X   |   X   |     | modified_datetime | The last modification time             |       X       |   X    |   X    |    X   |   X   |     | modified_by       | The last modification user             |       X       |   X    |   X    |    X   |   X   |     | name              | The name of the element                |               |        |   X    |    X   |   X   |     | fps               | The frames per second                  |               |        |   X    |        |       |     | deleted           | Whether the media is marked deleted    |               |        |   X    |    X   |   X   |     | variant_deleted   | Whether the metadata is marked deleted |       X       |   X    |        |        |       |     | archive_state     | The current archive state of the media |               |        |   X    |        |       |     | x, y, u, or v     | Geometric coordinates                  |               |        |        |        |       |     | width or height   | Geometric sizes                        |               |        |        |        |       |     | incident          | Available when doing a related search  |               |        |   X    |        |       |    
 
         :param attribute: The attribute of this AttributeOperationSpec.
         :type: str
         """
 
         self._attribute = attribute
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_delete.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/attribute_type_update_attribute_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/audio_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/audio_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/autocomplete_service.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/autocomplete_service.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/auxiliary_file_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/auxiliary_file_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bad_request_response.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bad_request_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bookmark.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bookmark.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bookmark_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bookmark_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bookmark_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_gcp_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket_gcp_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket_oci_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_oci_native_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket_oci_native_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_s3_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket_s3_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/bucket_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/bucket_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/change_log.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/change_log.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/change_log_description_of_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/change_log_description_of_change_new.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/clone_media_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/clone_media_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,25 +55,25 @@
         self.dest_project = dest_project
         self.dest_section = dest_section
         self.dest_type = dest_type
 
     @property
     def dest_project(self):
         """
-        Unique integer identyifying destination project.
+        Unique integer identifying destination project.
 
         :return: The dest_project of this CloneMediaSpec. 
         :rtype: int
         """
         return self._dest_project
 
     @dest_project.setter
     def dest_project(self, dest_project):
         """
-        Unique integer identyifying destination project.
+        Unique integer identifying destination project.
 
         :param dest_project: The dest_project of this CloneMediaSpec.
         :type: int
         """
         if self.local_vars_configuration.client_side_validation and dest_project is None:  # noqa: E501
             raise ValueError("Invalid value for `dest_project`, must not be `None`")  # noqa: E501
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/color_map.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/color_map.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/concat_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/concat_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/create_list_response.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/create_list_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/create_response.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/create_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/credentials.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/credentials.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/download_info.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/live_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,89 +14,89 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class DownloadInfo(object):
+class LiveDefinition(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'key': 'str',
+        'feeds': 'list[FeedDefinition]',
         'url': 'str'
     }
 
     attribute_map = {
-        'key': 'key',
+        'feeds': 'feeds',
         'url': 'url'
     }
 
-    def __init__(self, key=None, url=None, local_vars_configuration=None):  # noqa: E501
-        """DownloadInfo - a model defined in OpenAPI"""
+    def __init__(self, feeds=None, url=None, local_vars_configuration=None):  # noqa: E501
+        """LiveDefinition - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._key = None
+        self._feeds = None
         self._url = None
         self.discriminator = None
 
-        if key is not None:
-            self.key = key
-        if url is not None:
-            self.url = url
+        self.feeds = feeds
+        self.url = url
 
     @property
-    def key(self):
+    def feeds(self):
         """
-        Object key.
 
-        :return: The key of this DownloadInfo. 
-        :rtype: str
+        :return: The feeds of this LiveDefinition. 
+        :rtype: list[FeedDefinition]
         """
-        return self._key
+        return self._feeds
 
-    @key.setter
-    def key(self, key):
+    @feeds.setter
+    def feeds(self, feeds):
         """
-        Object key.
 
-        :param key: The key of this DownloadInfo.
-        :type: str
+        :param feeds: The feeds of this LiveDefinition.
+        :type: list[FeedDefinition]
         """
+        if self.local_vars_configuration.client_side_validation and feeds is None:  # noqa: E501
+            raise ValueError("Invalid value for `feeds`, must not be `None`")  # noqa: E501
 
-        self._key = key
+        self._feeds = feeds
 
     @property
     def url(self):
         """
-        URL for downloading object specified by key.
+        URL to streaming server.
 
-        :return: The url of this DownloadInfo. 
+        :return: The url of this LiveDefinition. 
         :rtype: str
         """
         return self._url
 
     @url.setter
     def url(self, url):
         """
-        URL for downloading object specified by key.
+        URL to streaming server.
 
-        :param url: The url of this DownloadInfo.
+        :param url: The url of this LiveDefinition.
         :type: str
         """
+        if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
+            raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
         self._url = url
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -126,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, DownloadInfo):
+        if not isinstance(other, LiveDefinition):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, DownloadInfo):
+        if not isinstance(other, LiveDefinition):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/download_info_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/download_info_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/email_attachment_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/email_attachment_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/email_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/email_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/encode_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/encode_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/favorite.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/favorite.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/favorite_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/favorite_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/favorite_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/favorite_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/feed_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/feed_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/file.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/file_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/file_type.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/file_type_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/file_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/file_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/file_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/file_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/file_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/fill.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/get_cloned_media_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,97 +14,91 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Fill(object):
+class GetClonedMediaResponse(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'color': 'object',
-        'style': 'str'
+        'ids': 'list[int]',
+        'message': 'str'
     }
 
     attribute_map = {
-        'color': 'color',
-        'style': 'style'
+        'ids': 'ids',
+        'message': 'message'
     }
 
-    def __init__(self, color=None, style=None, local_vars_configuration=None):  # noqa: E501
-        """Fill - a model defined in OpenAPI"""
+    def __init__(self, ids=None, message=None, local_vars_configuration=None):  # noqa: E501
+        """GetClonedMediaResponse - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._color = None
-        self._style = None
+        self._ids = None
+        self._message = None
         self.discriminator = None
 
-        if color is not None:
-            self.color = color
-        if style is not None:
-            self.style = style
+        if ids is not None:
+            self.ids = ids
+        if message is not None:
+            self.message = message
 
     @property
-    def color(self):
+    def ids(self):
         """
-        RGB array, RGBA array, or hex string.
+        List of unique integers identifying cloned objects.
 
-        :return: The color of this Fill. 
-        :rtype: object
+        :return: The ids of this GetClonedMediaResponse. 
+        :rtype: list[int]
         """
-        return self._color
+        return self._ids
 
-    @color.setter
-    def color(self, color):
+    @ids.setter
+    def ids(self, ids):
         """
-        RGB array, RGBA array, or hex string.
+        List of unique integers identifying cloned objects.
 
-        :param color: The color of this Fill.
-        :type: object
+        :param ids: The ids of this GetClonedMediaResponse.
+        :type: list[int]
         """
 
-        self._color = color
+        self._ids = ids
 
     @property
-    def style(self):
+    def message(self):
         """
-        Type of fill effect
+        Message indicating return of cloned media list.
 
-        :return: The style of this Fill. 
+        :return: The message of this GetClonedMediaResponse. 
         :rtype: str
         """
-        return self._style
+        return self._message
 
-    @style.setter
-    def style(self, style):
+    @message.setter
+    def message(self, message):
         """
-        Type of fill effect
+        Message indicating return of cloned media list.
 
-        :param style: The style of this Fill.
+        :param message: The message of this GetClonedMediaResponse.
         :type: str
         """
-        allowed_values = ["fill", "blur", "gray"]  # noqa: E501
-        if self.local_vars_configuration.client_side_validation and style not in allowed_values:  # noqa: E501
-            raise ValueError(
-                "Invalid value for `style` ({0}), must be one of {1}"  # noqa: E501
-                .format(style, allowed_values)
-            )
 
-        self._style = style
+        self._message = message
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -132,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Fill):
+        if not isinstance(other, GetClonedMediaResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Fill):
+        if not isinstance(other, GetClonedMediaResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/float_array_query.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/float_array_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/generic_file.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/generic_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/generic_file_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/generic_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/get_cloned_media_response.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/notify_spec.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,91 +14,92 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class GetClonedMediaResponse(object):
+class NotifySpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'ids': 'list[int]',
-        'message': 'str'
+        'message': 'str',
+        'send_as_file': 'int'
     }
 
     attribute_map = {
-        'ids': 'ids',
-        'message': 'message'
+        'message': 'message',
+        'send_as_file': 'send_as_file'
     }
 
-    def __init__(self, ids=None, message=None, local_vars_configuration=None):  # noqa: E501
-        """GetClonedMediaResponse - a model defined in OpenAPI"""
+    def __init__(self, message=None, send_as_file=None, local_vars_configuration=None):  # noqa: E501
+        """NotifySpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._ids = None
         self._message = None
+        self._send_as_file = None
         self.discriminator = None
 
-        if ids is not None:
-            self.ids = ids
-        if message is not None:
-            self.message = message
+        self.message = message
+        if send_as_file is not None:
+            self.send_as_file = send_as_file
 
     @property
-    def ids(self):
+    def message(self):
         """
-        List of unique integers identifying cloned objects.
+        Message to send to administrators.
 
-        :return: The ids of this GetClonedMediaResponse. 
-        :rtype: list[int]
+        :return: The message of this NotifySpec. 
+        :rtype: str
         """
-        return self._ids
+        return self._message
 
-    @ids.setter
-    def ids(self, ids):
+    @message.setter
+    def message(self, message):
         """
-        List of unique integers identifying cloned objects.
+        Message to send to administrators.
 
-        :param ids: The ids of this GetClonedMediaResponse.
-        :type: list[int]
+        :param message: The message of this NotifySpec.
+        :type: str
         """
+        if self.local_vars_configuration.client_side_validation and message is None:  # noqa: E501
+            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
-        self._ids = ids
+        self._message = message
 
     @property
-    def message(self):
+    def send_as_file(self):
         """
-        Message indicating return of cloned media list.
+        Whether to send message as a file. (0 or 1)
 
-        :return: The message of this GetClonedMediaResponse. 
-        :rtype: str
+        :return: The send_as_file of this NotifySpec. 
+        :rtype: int
         """
-        return self._message
+        return self._send_as_file
 
-    @message.setter
-    def message(self, message):
+    @send_as_file.setter
+    def send_as_file(self, send_as_file):
         """
-        Message indicating return of cloned media list.
+        Whether to send message as a file. (0 or 1)
 
-        :param message: The message of this GetClonedMediaResponse.
-        :type: str
+        :param send_as_file: The send_as_file of this NotifySpec.
+        :type: int
         """
 
-        self._message = message
+        self._send_as_file = send_as_file
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -126,18 +127,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, GetClonedMediaResponse):
+        if not isinstance(other, NotifySpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, GetClonedMediaResponse):
+        if not isinstance(other, NotifySpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/image_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/image_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/invitation.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/invitation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/invitation_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/invitation_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/invitation_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/invitation_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/job.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/job.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/job_cluster_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/job_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/job_node.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/job_node.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/job_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_type_spec.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,119 +14,142 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class JobSpec(object):
+class LeafTypeSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'algorithm_name': 'str',
-        'extra_params': 'list[AlgorithmParameter]',
-        'media_ids': 'list[int]'
+        'attribute_types': 'list[AttributeType]',
+        'description': 'str',
+        'elemental_id': 'str',
+        'name': 'str'
     }
 
     attribute_map = {
-        'algorithm_name': 'algorithm_name',
-        'extra_params': 'extra_params',
-        'media_ids': 'media_ids'
+        'attribute_types': 'attribute_types',
+        'description': 'description',
+        'elemental_id': 'elemental_id',
+        'name': 'name'
     }
 
-    def __init__(self, algorithm_name=None, extra_params=None, media_ids=None, local_vars_configuration=None):  # noqa: E501
-        """JobSpec - a model defined in OpenAPI"""
+    def __init__(self, attribute_types=None, description='', elemental_id=None, name=None, local_vars_configuration=None):  # noqa: E501
+        """LeafTypeSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._algorithm_name = None
-        self._extra_params = None
-        self._media_ids = None
+        self._attribute_types = None
+        self._description = None
+        self._elemental_id = None
+        self._name = None
         self.discriminator = None
 
-        self.algorithm_name = algorithm_name
-        if extra_params is not None:
-            self.extra_params = extra_params
-        self.media_ids = media_ids
+        if attribute_types is not None:
+            self.attribute_types = attribute_types
+        if description is not None:
+            self.description = description
+        self.elemental_id = elemental_id
+        if name is not None:
+            self.name = name
 
     @property
-    def algorithm_name(self):
+    def attribute_types(self):
         """
-        Name of the algorithm to execute.
+        Attribute type definitions.
 
-        :return: The algorithm_name of this JobSpec. 
+        :return: The attribute_types of this LeafTypeSpec. 
+        :rtype: list[AttributeType]
+        """
+        return self._attribute_types
+
+    @attribute_types.setter
+    def attribute_types(self, attribute_types):
+        """
+        Attribute type definitions.
+
+        :param attribute_types: The attribute_types of this LeafTypeSpec.
+        :type: list[AttributeType]
+        """
+
+        self._attribute_types = attribute_types
+
+    @property
+    def description(self):
+        """
+        Description of the leaf type.
+
+        :return: The description of this LeafTypeSpec. 
         :rtype: str
         """
-        return self._algorithm_name
+        return self._description
 
-    @algorithm_name.setter
-    def algorithm_name(self, algorithm_name):
+    @description.setter
+    def description(self, description):
         """
-        Name of the algorithm to execute.
+        Description of the leaf type.
 
-        :param algorithm_name: The algorithm_name of this JobSpec.
+        :param description: The description of this LeafTypeSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and algorithm_name is None:  # noqa: E501
-            raise ValueError("Invalid value for `algorithm_name`, must not be `None`")  # noqa: E501
 
-        self._algorithm_name = algorithm_name
+        self._description = description
 
     @property
-    def extra_params(self):
+    def elemental_id(self):
         """
-        Extra parameters to pass into the algorithm
+        The elemental ID of the object.
 
-        :return: The extra_params of this JobSpec. 
-        :rtype: list[AlgorithmParameter]
+        :return: The elemental_id of this LeafTypeSpec. 
+        :rtype: str
         """
-        return self._extra_params
+        return self._elemental_id
 
-    @extra_params.setter
-    def extra_params(self, extra_params):
+    @elemental_id.setter
+    def elemental_id(self, elemental_id):
         """
-        Extra parameters to pass into the algorithm
+        The elemental ID of the object.
 
-        :param extra_params: The extra_params of this JobSpec.
-        :type: list[AlgorithmParameter]
+        :param elemental_id: The elemental_id of this LeafTypeSpec.
+        :type: str
         """
 
-        self._extra_params = extra_params
+        self._elemental_id = elemental_id
 
     @property
-    def media_ids(self):
+    def name(self):
         """
-        List of media IDs.
+        Name of the leaf type.
 
-        :return: The media_ids of this JobSpec. 
-        :rtype: list[int]
+        :return: The name of this LeafTypeSpec. 
+        :rtype: str
         """
-        return self._media_ids
+        return self._name
 
-    @media_ids.setter
-    def media_ids(self, media_ids):
+    @name.setter
+    def name(self, name):
         """
-        List of media IDs.
+        Name of the leaf type.
 
-        :param media_ids: The media_ids of this JobSpec.
-        :type: list[int]
+        :param name: The name of this LeafTypeSpec.
+        :type: str
         """
-        if self.local_vars_configuration.client_side_validation and media_ids is None:  # noqa: E501
-            raise ValueError("Invalid value for `media_ids`, must not be `None`")  # noqa: E501
 
-        self._media_ids = media_ids
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -154,18 +177,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobSpec):
+        if not isinstance(other, LeafTypeSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, JobSpec):
+        if not isinstance(other, LeafTypeSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_bulk_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_id_query.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_suggestion.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_suggestion.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/upload_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,142 +14,117 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class LeafTypeSpec(object):
+class UploadInfo(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'attribute_types': 'list[AttributeType]',
-        'description': 'str',
-        'elemental_id': 'str',
-        'name': 'str'
+        'key': 'str',
+        'upload_id': 'str',
+        'urls': 'list[str]'
     }
 
     attribute_map = {
-        'attribute_types': 'attribute_types',
-        'description': 'description',
-        'elemental_id': 'elemental_id',
-        'name': 'name'
+        'key': 'key',
+        'upload_id': 'upload_id',
+        'urls': 'urls'
     }
 
-    def __init__(self, attribute_types=None, description='', elemental_id=None, name=None, local_vars_configuration=None):  # noqa: E501
-        """LeafTypeSpec - a model defined in OpenAPI"""
+    def __init__(self, key=None, upload_id=None, urls=None, local_vars_configuration=None):  # noqa: E501
+        """UploadInfo - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._attribute_types = None
-        self._description = None
-        self._elemental_id = None
-        self._name = None
+        self._key = None
+        self._upload_id = None
+        self._urls = None
         self.discriminator = None
 
-        if attribute_types is not None:
-            self.attribute_types = attribute_types
-        if description is not None:
-            self.description = description
-        self.elemental_id = elemental_id
-        if name is not None:
-            self.name = name
+        if key is not None:
+            self.key = key
+        if upload_id is not None:
+            self.upload_id = upload_id
+        if urls is not None:
+            self.urls = urls
 
     @property
-    def attribute_types(self):
+    def key(self):
         """
-        Attribute type definitions.
+        An object key that can be supplied to the `Transcode` or `Media` or `File` endpoint after the file has been uploaded.
 
-        :return: The attribute_types of this LeafTypeSpec. 
-        :rtype: list[AttributeType]
-        """
-        return self._attribute_types
-
-    @attribute_types.setter
-    def attribute_types(self, attribute_types):
-        """
-        Attribute type definitions.
-
-        :param attribute_types: The attribute_types of this LeafTypeSpec.
-        :type: list[AttributeType]
-        """
-
-        self._attribute_types = attribute_types
-
-    @property
-    def description(self):
-        """
-        Description of the leaf type.
-
-        :return: The description of this LeafTypeSpec. 
+        :return: The key of this UploadInfo. 
         :rtype: str
         """
-        return self._description
+        return self._key
 
-    @description.setter
-    def description(self, description):
+    @key.setter
+    def key(self, key):
         """
-        Description of the leaf type.
+        An object key that can be supplied to the `Transcode` or `Media` or `File` endpoint after the file has been uploaded.
 
-        :param description: The description of this LeafTypeSpec.
+        :param key: The key of this UploadInfo.
         :type: str
         """
 
-        self._description = description
+        self._key = key
 
     @property
-    def elemental_id(self):
+    def upload_id(self):
         """
-        The elemental ID of the object.
+        An upload ID that can be supplied to the `UploadCompletion` endpoint after the file has been uploaded. Only contains a value if `num_parts` > 1.
 
-        :return: The elemental_id of this LeafTypeSpec. 
+        :return: The upload_id of this UploadInfo. 
         :rtype: str
         """
-        return self._elemental_id
+        return self._upload_id
 
-    @elemental_id.setter
-    def elemental_id(self, elemental_id):
+    @upload_id.setter
+    def upload_id(self, upload_id):
         """
-        The elemental ID of the object.
+        An upload ID that can be supplied to the `UploadCompletion` endpoint after the file has been uploaded. Only contains a value if `num_parts` > 1.
 
-        :param elemental_id: The elemental_id of this LeafTypeSpec.
+        :param upload_id: The upload_id of this UploadInfo.
         :type: str
         """
 
-        self._elemental_id = elemental_id
+        self._upload_id = upload_id
 
     @property
-    def name(self):
+    def urls(self):
         """
-        Name of the leaf type.
+        One or more URLs for upload via one PUT request per URL.
 
-        :return: The name of this LeafTypeSpec. 
-        :rtype: str
+        :return: The urls of this UploadInfo. 
+        :rtype: list[str]
         """
-        return self._name
+        return self._urls
 
-    @name.setter
-    def name(self, name):
+    @urls.setter
+    def urls(self, urls):
         """
-        Name of the leaf type.
+        One or more URLs for upload via one PUT request per URL.
 
-        :param name: The name of this LeafTypeSpec.
-        :type: str
+        :param urls: The urls of this UploadInfo.
+        :type: list[str]
         """
 
-        self._name = name
+        self._urls = urls
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -177,18 +152,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LeafTypeSpec):
+        if not isinstance(other, UploadInfo):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LeafTypeSpec):
+        if not isinstance(other, UploadInfo):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/leaf_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/leaf_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/live_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/transcode.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,91 +14,87 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class LiveDefinition(object):
+class Transcode(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'feeds': 'list[FeedDefinition]',
-        'url': 'str'
+        'job': 'Job',
+        'spec': 'TranscodeSpec'
     }
 
     attribute_map = {
-        'feeds': 'feeds',
-        'url': 'url'
+        'job': 'job',
+        'spec': 'spec'
     }
 
-    def __init__(self, feeds=None, url=None, local_vars_configuration=None):  # noqa: E501
-        """LiveDefinition - a model defined in OpenAPI"""
+    def __init__(self, job=None, spec=None, local_vars_configuration=None):  # noqa: E501
+        """Transcode - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._feeds = None
-        self._url = None
+        self._job = None
+        self._spec = None
         self.discriminator = None
 
-        self.feeds = feeds
-        self.url = url
+        if job is not None:
+            self.job = job
+        if spec is not None:
+            self.spec = spec
 
     @property
-    def feeds(self):
+    def job(self):
         """
 
-        :return: The feeds of this LiveDefinition. 
-        :rtype: list[FeedDefinition]
+        :return: The job of this Transcode. 
+        :rtype: Job
         """
-        return self._feeds
+        return self._job
 
-    @feeds.setter
-    def feeds(self, feeds):
+    @job.setter
+    def job(self, job):
         """
 
-        :param feeds: The feeds of this LiveDefinition.
-        :type: list[FeedDefinition]
+        :param job: The job of this Transcode.
+        :type: Job
         """
-        if self.local_vars_configuration.client_side_validation and feeds is None:  # noqa: E501
-            raise ValueError("Invalid value for `feeds`, must not be `None`")  # noqa: E501
 
-        self._feeds = feeds
+        self._job = job
 
     @property
-    def url(self):
+    def spec(self):
         """
-        URL to streaming server.
 
-        :return: The url of this LiveDefinition. 
-        :rtype: str
+        :return: The spec of this Transcode. 
+        :rtype: TranscodeSpec
         """
-        return self._url
+        return self._spec
 
-    @url.setter
-    def url(self, url):
+    @spec.setter
+    def spec(self, spec):
         """
-        URL to streaming server.
 
-        :param url: The url of this LiveDefinition.
-        :type: str
+        :param spec: The spec of this Transcode.
+        :type: TranscodeSpec
         """
-        if self.local_vars_configuration.client_side_validation and url is None:  # noqa: E501
-            raise ValueError("Invalid value for `url`, must not be `None`")  # noqa: E501
 
-        self._url = url
+        self._spec = spec
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -126,18 +122,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, LiveDefinition):
+        if not isinstance(other, Transcode):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, LiveDefinition):
+        if not isinstance(other, Transcode):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/live_update_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/live_update_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_delete.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_bulk_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_delete.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_id_query.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_type.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/localization_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/localization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         'created_by': 'int',
         'created_datetime': 'str',
         'elemental_id': 'str',
         'fps': 'float',
         'gid': 'str',
         'height': 'int',
         'id': 'int',
+        'incident': 'int',
         'last_edit_end': 'datetime',
         'last_edit_start': 'datetime',
         'md5': 'str',
         'media_files': 'MediaFiles',
         'modified_by': 'int',
         'modified_datetime': 'str',
         'name': 'str',
@@ -64,14 +65,15 @@
         'created_by': 'created_by',
         'created_datetime': 'created_datetime',
         'elemental_id': 'elemental_id',
         'fps': 'fps',
         'gid': 'gid',
         'height': 'height',
         'id': 'id',
+        'incident': 'incident',
         'last_edit_end': 'last_edit_end',
         'last_edit_start': 'last_edit_start',
         'md5': 'md5',
         'media_files': 'media_files',
         'modified_by': 'modified_by',
         'modified_datetime': 'modified_datetime',
         'name': 'name',
@@ -79,15 +81,15 @@
         'project': 'project',
         'summary_level': 'summary_level',
         'type': 'type',
         'uid': 'uid',
         'width': 'width'
     }
 
-    def __init__(self, archive_state=None, archive_status_date=None, attributes=None, codec=None, created_by=None, created_datetime=None, elemental_id=None, fps=None, gid=None, height=None, id=None, last_edit_end=None, last_edit_start=None, md5=None, media_files=None, modified_by=None, modified_datetime=None, name=None, num_frames=None, project=None, summary_level=None, type=None, uid=None, width=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archive_state=None, archive_status_date=None, attributes=None, codec=None, created_by=None, created_datetime=None, elemental_id=None, fps=None, gid=None, height=None, id=None, incident=None, last_edit_end=None, last_edit_start=None, md5=None, media_files=None, modified_by=None, modified_datetime=None, name=None, num_frames=None, project=None, summary_level=None, type=None, uid=None, width=None, local_vars_configuration=None):  # noqa: E501
         """Media - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._archive_state = None
         self._archive_status_date = None
@@ -96,14 +98,15 @@
         self._created_by = None
         self._created_datetime = None
         self._elemental_id = None
         self._fps = None
         self._gid = None
         self._height = None
         self._id = None
+        self._incident = None
         self._last_edit_end = None
         self._last_edit_start = None
         self._md5 = None
         self._media_files = None
         self._modified_by = None
         self._modified_datetime = None
         self._name = None
@@ -132,14 +135,15 @@
             self.fps = fps
         if gid is not None:
             self.gid = gid
         if height is not None:
             self.height = height
         if id is not None:
             self.id = id
+        self.incident = incident
         if last_edit_end is not None:
             self.last_edit_end = last_edit_end
         if last_edit_start is not None:
             self.last_edit_start = last_edit_start
         if md5 is not None:
             self.md5 = md5
         if media_files is not None:
@@ -397,14 +401,35 @@
         :param id: The id of this Media.
         :type: int
         """
 
         self._id = id
 
     @property
+    def incident(self):
+        """
+        If doing a related search, will contain the number of matching metadata hits in this media.
+
+        :return: The incident of this Media. 
+        :rtype: int
+        """
+        return self._incident
+
+    @incident.setter
+    def incident(self, incident):
+        """
+        If doing a related search, will contain the number of matching metadata hits in this media.
+
+        :param incident: The incident of this Media.
+        :type: int
+        """
+
+        self._incident = incident
+
+    @property
     def last_edit_end(self):
         """
         Datetime of the end of the session when this media or its annotations were last edited.
 
         :return: The last_edit_end of this Media. 
         :rtype: datetime
         """
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_bulk_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_bulk_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_files.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_files.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_id_query.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_next.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_next.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_prev.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_prev.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         'elemental_id': 'str',
         'fps': 'float',
         'gid': 'str',
         'height': 'int',
         'md5': 'str',
         'name': 'str',
         'num_frames': 'int',
+        'reference_only': 'int',
         'section': 'str',
         'summary_level': 'int',
         'thumbnail_gif_url': 'str',
         'thumbnail_url': 'str',
         'type': 'int',
         'uid': 'str',
         'url': 'str',
@@ -56,40 +57,42 @@
         'elemental_id': 'elemental_id',
         'fps': 'fps',
         'gid': 'gid',
         'height': 'height',
         'md5': 'md5',
         'name': 'name',
         'num_frames': 'num_frames',
+        'reference_only': 'reference_only',
         'section': 'section',
         'summary_level': 'summary_level',
         'thumbnail_gif_url': 'thumbnail_gif_url',
         'thumbnail_url': 'thumbnail_url',
         'type': 'type',
         'uid': 'uid',
         'url': 'url',
         'user_elemental_id': 'user_elemental_id',
         'width': 'width'
     }
 
-    def __init__(self, attributes=None, codec=None, elemental_id=None, fps=None, gid=None, height=None, md5=None, name=None, num_frames=None, section=None, summary_level=None, thumbnail_gif_url=None, thumbnail_url=None, type=None, uid=None, url=None, user_elemental_id=None, width=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, codec=None, elemental_id=None, fps=None, gid=None, height=None, md5=None, name=None, num_frames=None, reference_only=0, section=None, summary_level=None, thumbnail_gif_url=None, thumbnail_url=None, type=None, uid=None, url=None, user_elemental_id=None, width=None, local_vars_configuration=None):  # noqa: E501
         """MediaSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
         self._codec = None
         self._elemental_id = None
         self._fps = None
         self._gid = None
         self._height = None
         self._md5 = None
         self._name = None
         self._num_frames = None
+        self._reference_only = None
         self._section = None
         self._summary_level = None
         self._thumbnail_gif_url = None
         self._thumbnail_url = None
         self._type = None
         self._uid = None
         self._url = None
@@ -104,14 +107,16 @@
         self.fps = fps
         if gid is not None:
             self.gid = gid
         self.height = height
         self.md5 = md5
         self.name = name
         self.num_frames = num_frames
+        if reference_only is not None:
+            self.reference_only = reference_only
         self.section = section
         if summary_level is not None:
             self.summary_level = summary_level
         if thumbnail_gif_url is not None:
             self.thumbnail_gif_url = thumbnail_gif_url
         if thumbnail_url is not None:
             self.thumbnail_url = thumbnail_url
@@ -314,14 +319,38 @@
         :param num_frames: The num_frames of this MediaSpec.
         :type: int
         """
 
         self._num_frames = num_frames
 
     @property
+    def reference_only(self):
+        """
+        Do not import the media resources into Tator. This causes the image to be accessed at the supplied URL upon access in the UI. Valid for images only.
+
+        :return: The reference_only of this MediaSpec. 
+        :rtype: int
+        """
+        return self._reference_only
+
+    @reference_only.setter
+    def reference_only(self, reference_only):
+        """
+        Do not import the media resources into Tator. This causes the image to be accessed at the supplied URL upon access in the UI. Valid for images only.
+
+        :param reference_only: The reference_only of this MediaSpec.
+        :type: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                reference_only is not None and reference_only > 1):  # noqa: E501
+            raise ValueError("Invalid value for `reference_only`, must be a value less than or equal to `1`")  # noqa: E501
+
+        self._reference_only = reference_only
+
+    @property
     def section(self):
         """
         Media section name.
 
         :return: The section of this MediaSpec. 
         :rtype: str
         """
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_stats.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_stats.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_type.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_type_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/media_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/media_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/membership.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/membership_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/membership_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/membership_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/membership_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/message_response.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/message_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/multi_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/multi_definition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/not_found_response.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/not_found_response.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/notify_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/upload_completion_spec.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,92 +14,117 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class NotifySpec(object):
+class UploadCompletionSpec(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'message': 'str',
-        'send_as_file': 'int'
+        'key': 'str',
+        'parts': 'list[UploadPart]',
+        'upload_id': 'str'
     }
 
     attribute_map = {
-        'message': 'message',
-        'send_as_file': 'send_as_file'
+        'key': 'key',
+        'parts': 'parts',
+        'upload_id': 'upload_id'
     }
 
-    def __init__(self, message=None, send_as_file=None, local_vars_configuration=None):  # noqa: E501
-        """NotifySpec - a model defined in OpenAPI"""
+    def __init__(self, key=None, parts=None, upload_id=None, local_vars_configuration=None):  # noqa: E501
+        """UploadCompletionSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._message = None
-        self._send_as_file = None
+        self._key = None
+        self._parts = None
+        self._upload_id = None
         self.discriminator = None
 
-        self.message = message
-        if send_as_file is not None:
-            self.send_as_file = send_as_file
+        if key is not None:
+            self.key = key
+        if parts is not None:
+            self.parts = parts
+        if upload_id is not None:
+            self.upload_id = upload_id
 
     @property
-    def message(self):
+    def key(self):
         """
-        Message to send to administrators.
+        An object key that can be supplied to the `Transcode` or `Media` endpoint after the file has been uploaded.
 
-        :return: The message of this NotifySpec. 
+        :return: The key of this UploadCompletionSpec. 
         :rtype: str
         """
-        return self._message
+        return self._key
 
-    @message.setter
-    def message(self, message):
+    @key.setter
+    def key(self, key):
         """
-        Message to send to administrators.
+        An object key that can be supplied to the `Transcode` or `Media` endpoint after the file has been uploaded.
 
-        :param message: The message of this NotifySpec.
+        :param key: The key of this UploadCompletionSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and message is None:  # noqa: E501
-            raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
-        self._message = message
+        self._key = key
 
     @property
-    def send_as_file(self):
+    def parts(self):
         """
-        Whether to send message as a file. (0 or 1)
+        List of objects containing part number for each PUT request and ETag header from each response.
 
-        :return: The send_as_file of this NotifySpec. 
-        :rtype: int
+        :return: The parts of this UploadCompletionSpec. 
+        :rtype: list[UploadPart]
         """
-        return self._send_as_file
+        return self._parts
 
-    @send_as_file.setter
-    def send_as_file(self, send_as_file):
+    @parts.setter
+    def parts(self, parts):
         """
-        Whether to send message as a file. (0 or 1)
+        List of objects containing part number for each PUT request and ETag header from each response.
 
-        :param send_as_file: The send_as_file of this NotifySpec.
-        :type: int
+        :param parts: The parts of this UploadCompletionSpec.
+        :type: list[UploadPart]
         """
 
-        self._send_as_file = send_as_file
+        self._parts = parts
+
+    @property
+    def upload_id(self):
+        """
+        An upload ID.
+
+        :return: The upload_id of this UploadCompletionSpec. 
+        :rtype: str
+        """
+        return self._upload_id
+
+    @upload_id.setter
+    def upload_id(self, upload_id):
+        """
+        An upload ID.
+
+        :param upload_id: The upload_id of this UploadCompletionSpec.
+        :type: str
+        """
+
+        self._upload_id = upload_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -127,18 +152,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotifySpec):
+        if not isinstance(other, UploadCompletionSpec):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, NotifySpec):
+        if not isinstance(other, UploadCompletionSpec):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/organization.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/organization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/organization_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/organization_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/organization_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/organization_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/password_reset_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/password_reset_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/project.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/project.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/project_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/project_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/project_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/project_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/resolution_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/resolution_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/s3_storage_config.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/s3_storage_config.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/section.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/section_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/section_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/section_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/section_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_delete.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_bulk_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_bulk_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_bulk_update.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,47 +32,50 @@
     openapi_types = {
         'attributes': 'dict(str, object)',
         'float_array': 'list[FloatArrayQuery]',
         'ids': 'list[int]',
         'localization_ids': 'list[int]',
         'media_ids': 'list[int]',
         'media_query': 'str',
+        'new_elemental_id': 'str',
         'new_version': 'int',
         'null_attributes': 'list[str]',
         'object_search': 'AttributeOperationSpec',
         'reset_attributes': 'list[str]',
         'user_elemental_id': 'str'
     }
 
     attribute_map = {
         'attributes': 'attributes',
         'float_array': 'float_array',
         'ids': 'ids',
         'localization_ids': 'localization_ids',
         'media_ids': 'media_ids',
         'media_query': 'media_query',
+        'new_elemental_id': 'new_elemental_id',
         'new_version': 'new_version',
         'null_attributes': 'null_attributes',
         'object_search': 'object_search',
         'reset_attributes': 'reset_attributes',
         'user_elemental_id': 'user_elemental_id'
     }
 
-    def __init__(self, attributes=None, float_array=None, ids=None, localization_ids=None, media_ids=None, media_query=None, new_version=None, null_attributes=None, object_search=None, reset_attributes=None, user_elemental_id=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, float_array=None, ids=None, localization_ids=None, media_ids=None, media_query=None, new_elemental_id=None, new_version=None, null_attributes=None, object_search=None, reset_attributes=None, user_elemental_id=None, local_vars_configuration=None):  # noqa: E501
         """StateBulkUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
         self._float_array = None
         self._ids = None
         self._localization_ids = None
         self._media_ids = None
         self._media_query = None
+        self._new_elemental_id = None
         self._new_version = None
         self._null_attributes = None
         self._object_search = None
         self._reset_attributes = None
         self._user_elemental_id = None
         self.discriminator = None
 
@@ -84,14 +87,16 @@
             self.ids = ids
         if localization_ids is not None:
             self.localization_ids = localization_ids
         if media_ids is not None:
             self.media_ids = media_ids
         if media_query is not None:
             self.media_query = media_query
+        if new_elemental_id is not None:
+            self.new_elemental_id = new_elemental_id
         if new_version is not None:
             self.new_version = new_version
         if null_attributes is not None:
             self.null_attributes = null_attributes
         if object_search is not None:
             self.object_search = object_search
         if reset_attributes is not None:
@@ -222,14 +227,35 @@
         :param media_query: The media_query of this StateBulkUpdate.
         :type: str
         """
 
         self._media_query = media_query
 
     @property
+    def new_elemental_id(self):
+        """
+        The new elemental ID for these objects
+
+        :return: The new_elemental_id of this StateBulkUpdate. 
+        :rtype: str
+        """
+        return self._new_elemental_id
+
+    @new_elemental_id.setter
+    def new_elemental_id(self, new_elemental_id):
+        """
+        The new elemental ID for these objects
+
+        :param new_elemental_id: The new_elemental_id of this StateBulkUpdate.
+        :type: str
+        """
+
+        self._new_elemental_id = new_elemental_id
+
+    @property
     def new_version(self):
         """
         Unique integer identifying a new version for these objects
 
         :return: The new_version of this StateBulkUpdate. 
         :rtype: int
         """
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_delete.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_delete.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_id_query.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_id_query.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_merge_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_merge_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_trim_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_trim_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_type.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_type_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_type_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_type_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_type_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/state_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/state_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/temporary_file_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/temporary_file_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/token.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/token.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/transcode.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/upload_part.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,87 +14,91 @@
 import re  # noqa: F401
 
 import six
 
 from ..configuration import Configuration
 
 
-class Transcode(object):
+class UploadPart(object):
     """
     """
 
     """
     Attributes:
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
-        'job': 'Job',
-        'spec': 'TranscodeSpec'
+        'e_tag': 'str',
+        'part_number': 'int'
     }
 
     attribute_map = {
-        'job': 'job',
-        'spec': 'spec'
+        'e_tag': 'ETag',
+        'part_number': 'PartNumber'
     }
 
-    def __init__(self, job=None, spec=None, local_vars_configuration=None):  # noqa: E501
-        """Transcode - a model defined in OpenAPI"""
+    def __init__(self, e_tag=None, part_number=None, local_vars_configuration=None):  # noqa: E501
+        """UploadPart - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
-        self._job = None
-        self._spec = None
+        self._e_tag = None
+        self._part_number = None
         self.discriminator = None
 
-        if job is not None:
-            self.job = job
-        if spec is not None:
-            self.spec = spec
+        if e_tag is not None:
+            self.e_tag = e_tag
+        if part_number is not None:
+            self.part_number = part_number
 
     @property
-    def job(self):
+    def e_tag(self):
         """
+        Content of ETag header returned from PUT request for an upload part. NOTE: key is case-sensitive!
 
-        :return: The job of this Transcode. 
-        :rtype: Job
+        :return: The e_tag of this UploadPart. 
+        :rtype: str
         """
-        return self._job
+        return self._e_tag
 
-    @job.setter
-    def job(self, job):
+    @e_tag.setter
+    def e_tag(self, e_tag):
         """
+        Content of ETag header returned from PUT request for an upload part. NOTE: key is case-sensitive!
 
-        :param job: The job of this Transcode.
-        :type: Job
+        :param e_tag: The e_tag of this UploadPart.
+        :type: str
         """
 
-        self._job = job
+        self._e_tag = e_tag
 
     @property
-    def spec(self):
+    def part_number(self):
         """
+        Part number for the given ETag response header. NOTE: key is case-sensitive!
 
-        :return: The spec of this Transcode. 
-        :rtype: TranscodeSpec
+        :return: The part_number of this UploadPart. 
+        :rtype: int
         """
-        return self._spec
+        return self._part_number
 
-    @spec.setter
-    def spec(self, spec):
+    @part_number.setter
+    def part_number(self, part_number):
         """
+        Part number for the given ETag response header. NOTE: key is case-sensitive!
 
-        :param spec: The spec of this Transcode.
-        :type: TranscodeSpec
+        :param part_number: The part_number of this UploadPart.
+        :type: int
         """
 
-        self._spec = spec
+        self._part_number = part_number
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
@@ -122,18 +126,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Transcode):
+        if not isinstance(other, UploadPart):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Transcode):
+        if not isinstance(other, UploadPart):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/transcode_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/transcode_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,59 +27,64 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'attributes': 'object',
+        'email_spec': 'JobSpecFailureEmailSpec',
         'gid': 'str',
         'md5': 'str',
         'media_id': 'int',
         'name': 'str',
         'section': 'str',
         'size': 'int',
         'type': 'int',
         'uid': 'str',
         'url': 'str'
     }
 
     attribute_map = {
         'attributes': 'attributes',
+        'email_spec': 'email_spec',
         'gid': 'gid',
         'md5': 'md5',
         'media_id': 'media_id',
         'name': 'name',
         'section': 'section',
         'size': 'size',
         'type': 'type',
         'uid': 'uid',
         'url': 'url'
     }
 
-    def __init__(self, attributes=None, gid=None, md5=None, media_id=None, name=None, section=None, size=None, type=None, uid=None, url=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, attributes=None, email_spec=None, gid=None, md5=None, media_id=None, name=None, section=None, size=None, type=None, uid=None, url=None, local_vars_configuration=None):  # noqa: E501
         """TranscodeSpec - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._attributes = None
+        self._email_spec = None
         self._gid = None
         self._md5 = None
         self._media_id = None
         self._name = None
         self._section = None
         self._size = None
         self._type = None
         self._uid = None
         self._url = None
         self.discriminator = None
 
         self.attributes = attributes
+        self.email_spec = email_spec
         self.gid = gid
-        self.md5 = md5
+        if md5 is not None:
+            self.md5 = md5
         self.media_id = media_id
         self.name = name
         self.section = section
         if size is not None:
             self.size = size
         self.type = type
         self.uid = uid
@@ -103,14 +108,33 @@
         :param attributes: The attributes of this TranscodeSpec.
         :type: object
         """
 
         self._attributes = attributes
 
     @property
+    def email_spec(self):
+        """
+
+        :return: The email_spec of this TranscodeSpec. 
+        :rtype: JobSpecFailureEmailSpec
+        """
+        return self._email_spec
+
+    @email_spec.setter
+    def email_spec(self, email_spec):
+        """
+
+        :param email_spec: The email_spec of this TranscodeSpec.
+        :type: JobSpecFailureEmailSpec
+        """
+
+        self._email_spec = email_spec
+
+    @property
     def gid(self):
         """
         UUID generated for the job group. This value may be associated with messages generated during upload via the `Progress` endpoint, or it may be newly generated. The transcode workflow will use this value to generate progress messages.
 
         :return: The gid of this TranscodeSpec. 
         :rtype: str
         """
@@ -143,16 +167,14 @@
     def md5(self, md5):
         """
         MD5 sum of the media file.
 
         :param md5: The md5 of this TranscodeSpec.
         :type: str
         """
-        if self.local_vars_configuration.client_side_validation and md5 is None:  # noqa: E501
-            raise ValueError("Invalid value for `md5`, must not be `None`")  # noqa: E501
 
         self._md5 = md5
 
     @property
     def media_id(self):
         """
         ID of an existing media. If given, this media will be used for the transcode operation rather than creating a new object.
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/user.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/user.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/user_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/user_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/user_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/user_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,66 +27,76 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'clear_avatar': 'int',
+        'clear_profile_keys': 'list[str]',
         'elemental_id': 'str',
         'email': 'str',
         'first_name': 'str',
         'last_name': 'str',
         'new_avatar': 'str',
         'password': 'str',
-        'reset_token': 'str'
+        'reset_token': 'str',
+        'set_profile_keys': 'object'
     }
 
     attribute_map = {
         'clear_avatar': 'clear_avatar',
+        'clear_profile_keys': 'clear_profile_keys',
         'elemental_id': 'elemental_id',
         'email': 'email',
         'first_name': 'first_name',
         'last_name': 'last_name',
         'new_avatar': 'new_avatar',
         'password': 'password',
-        'reset_token': 'reset_token'
+        'reset_token': 'reset_token',
+        'set_profile_keys': 'set_profile_keys'
     }
 
-    def __init__(self, clear_avatar=0, elemental_id=None, email=None, first_name=None, last_name=None, new_avatar=None, password=None, reset_token=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, clear_avatar=0, clear_profile_keys=None, elemental_id=None, email=None, first_name=None, last_name=None, new_avatar=None, password=None, reset_token=None, set_profile_keys=None, local_vars_configuration=None):  # noqa: E501
         """UserUpdate - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._clear_avatar = None
+        self._clear_profile_keys = None
         self._elemental_id = None
         self._email = None
         self._first_name = None
         self._last_name = None
         self._new_avatar = None
         self._password = None
         self._reset_token = None
+        self._set_profile_keys = None
         self.discriminator = None
 
         if clear_avatar is not None:
             self.clear_avatar = clear_avatar
+        if clear_profile_keys is not None:
+            self.clear_profile_keys = clear_profile_keys
         if elemental_id is not None:
             self.elemental_id = elemental_id
         if email is not None:
             self.email = email
         if first_name is not None:
             self.first_name = first_name
         if last_name is not None:
             self.last_name = last_name
         if new_avatar is not None:
             self.new_avatar = new_avatar
         if password is not None:
             self.password = password
         if reset_token is not None:
             self.reset_token = reset_token
+        if set_profile_keys is not None:
+            self.set_profile_keys = set_profile_keys
 
     @property
     def clear_avatar(self):
         """
         Set to >0 to clear the current avatar of the user
 
         :return: The clear_avatar of this UserUpdate. 
@@ -102,14 +112,35 @@
         :param clear_avatar: The clear_avatar of this UserUpdate.
         :type: int
         """
 
         self._clear_avatar = clear_avatar
 
     @property
+    def clear_profile_keys(self):
+        """
+        Clear the given keys from the profile dictionary
+
+        :return: The clear_profile_keys of this UserUpdate. 
+        :rtype: list[str]
+        """
+        return self._clear_profile_keys
+
+    @clear_profile_keys.setter
+    def clear_profile_keys(self, clear_profile_keys):
+        """
+        Clear the given keys from the profile dictionary
+
+        :param clear_profile_keys: The clear_profile_keys of this UserUpdate.
+        :type: list[str]
+        """
+
+        self._clear_profile_keys = clear_profile_keys
+
+    @property
     def elemental_id(self):
         """
         Unique ID for a user across clusters/deployments
 
         :return: The elemental_id of this UserUpdate. 
         :rtype: str
         """
@@ -248,14 +279,35 @@
 
         :param reset_token: The reset_token of this UserUpdate.
         :type: str
         """
 
         self._reset_token = reset_token
 
+    @property
+    def set_profile_keys(self):
+        """
+        Key/Value Pairs to set atomically
+
+        :return: The set_profile_keys of this UserUpdate. 
+        :rtype: object
+        """
+        return self._set_profile_keys
+
+    @set_profile_keys.setter
+    def set_profile_keys(self, set_profile_keys):
+        """
+        Key/Value Pairs to set atomically
+
+        :param set_profile_keys: The set_profile_keys of this UserUpdate.
+        :type: object
+        """
+
+        self._set_profile_keys = set_profile_keys
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/version.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/version_spec.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/version_spec.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/version_update.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/version_update.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/video_clip.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/video_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/models/video_definition.py` & `tator-1.1.0/tator/openapi/tator_openapi/models/video_definition.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,45 +33,48 @@
         'bit_rate': 'int',
         'codec': 'str',
         'codec_description': 'str',
         'codec_mime': 'str',
         'host': 'str',
         'http_auth': 'str',
         'path': 'str',
+        'reference_only': 'int',
         'resolution': 'list[int]',
         'segment_info': 'str',
         'size': 'int'
     }
 
     attribute_map = {
         'bit_rate': 'bit_rate',
         'codec': 'codec',
         'codec_description': 'codec_description',
         'codec_mime': 'codec_mime',
         'host': 'host',
         'http_auth': 'http_auth',
         'path': 'path',
+        'reference_only': 'reference_only',
         'resolution': 'resolution',
         'segment_info': 'segment_info',
         'size': 'size'
     }
 
-    def __init__(self, bit_rate=None, codec=None, codec_description=None, codec_mime=None, host=None, http_auth=None, path=None, resolution=None, segment_info=None, size=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, bit_rate=None, codec=None, codec_description=None, codec_mime=None, host=None, http_auth=None, path=None, reference_only=0, resolution=None, segment_info=None, size=None, local_vars_configuration=None):  # noqa: E501
         """VideoDefinition - a model defined in OpenAPI"""
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._bit_rate = None
         self._codec = None
         self._codec_description = None
         self._codec_mime = None
         self._host = None
         self._http_auth = None
         self._path = None
+        self._reference_only = None
         self._resolution = None
         self._segment_info = None
         self._size = None
         self.discriminator = None
 
         if bit_rate is not None:
             self.bit_rate = bit_rate
@@ -81,14 +84,16 @@
         if codec_mime is not None:
             self.codec_mime = codec_mime
         if host is not None:
             self.host = host
         if http_auth is not None:
             self.http_auth = http_auth
         self.path = path
+        if reference_only is not None:
+            self.reference_only = reference_only
         self.resolution = resolution
         if segment_info is not None:
             self.segment_info = segment_info
         if size is not None:
             self.size = size
 
     @property
@@ -239,14 +244,38 @@
         """
         if self.local_vars_configuration.client_side_validation and path is None:  # noqa: E501
             raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
         self._path = path
 
     @property
+    def reference_only(self):
+        """
+        Do not import the media resources into Tator. This causes the resources to be accessed at the supplied URL upon access in the UI.
+
+        :return: The reference_only of this VideoDefinition. 
+        :rtype: int
+        """
+        return self._reference_only
+
+    @reference_only.setter
+    def reference_only(self, reference_only):
+        """
+        Do not import the media resources into Tator. This causes the resources to be accessed at the supplied URL upon access in the UI.
+
+        :param reference_only: The reference_only of this VideoDefinition.
+        :type: int
+        """
+        if (self.local_vars_configuration.client_side_validation and
+                reference_only is not None and reference_only > 1):  # noqa: E501
+            raise ValueError("Invalid value for `reference_only`, must be a value less than or equal to `1`")  # noqa: E501
+
+        self._reference_only = reference_only
+
+    @property
     def resolution(self):
         """
         Resolution of the video in pixels (height, width).
 
         :return: The resolution of this VideoDefinition. 
         :rtype: list[int]
         """
```

### Comparing `tator-1.0.5/tator/openapi/tator_openapi/rest.py` & `tator-1.1.0/tator/openapi/tator_openapi/rest.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/__main__.py` & `tator-1.1.0/tator/transcode/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 import argparse
 import os
 import shutil
 import sys
 from uuid import uuid1
 import logging
 import subprocess
+import json
 
 from progressbar import progressbar
 
 from ..util import md5sum
+from ..util.get_api import get_api
 
 from .create_media import create_media
 from .determine_transcode import determine_transcode
 from .transcode import convert_streaming
 from .transcode import convert_archival
 from .transcode import convert_audio
 from .delete_media import delete_media
@@ -42,14 +44,15 @@
     parser.add_argument('--media_id', type=int, help="Existing media ID, if applicable",
                         default=-1)
     parser.add_argument('--gid', type=str, help="Upload group ID.")
     parser.add_argument('--uid', type=str, help="Upload unique ID.")
     parser.add_argument('--group_to', type=int, default=1080,
                          help='Vertical resolutions below this will be transcoded with '
                               'multi-headed ffmpeg.')
+    parser.add_argument('--email_spec', type=str, help="Optional email spec as a JSON string. The email will be sent upon completion of the transcode (see Email rest endpoint docs).")
     parser.add_argument('--cleanup', action='store_true',
                         help="Deletes working files after each file is transcoded and "
                              "uploaded.")
     return parser.parse_args()
 
 def get_file_paths(path, base):
     paths = {
@@ -140,14 +143,24 @@
         for key in ['transcoded', 'thumbnail', 'thumbnail_gif']:
             path = paths[key]
             if os.path.isdir(path):
                 shutil.rmtree(path)
             else:
                 os.remove(path)
 
+    # Send an email.
+    if args.email_spec:
+        api = get_api(args.host, args.token)
+        if isinstance(args.email_spec, str):
+            email_spec = json.loads(args.email_spec)
+        else:
+            email_spec = args.email_spec
+        response = api.send_email(args.project, email_spec=email_spec)
+        logger.info(response.message)
+
 def transcode_main(args):
     if args.gid is None:
         gid = str(uuid1())
     else:
         gid = args.gid
     if args.path and os.path.isdir(args.path):
         file_list = []
```

### Comparing `tator-1.0.5/tator/transcode/black.mp4` & `tator-1.1.0/tator/transcode/black.mp4`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/create_media.py` & `tator-1.1.0/tator/transcode/create_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,24 +36,22 @@
         'type': media_type,
         'section': section,
         'name': name,
         'md5': md5,
         'gid': gid,
         'uid': uid
     }
+
     if attributes:
         spec.update({'attributes': json.loads(attributes)})
     if url:
         spec.update({'url': url})
-    response = api.create_media_list(project, body=[spec])
 
-    assert isinstance(response, CreateResponse)
-    media_id = response.id
+    return api.create_media_list(project, body=[spec]).id[0] # pylint: disable=E1101
 
-    return media_id
 
 if __name__ == '__main__':
     args = parse_args()
     media_id = create_media(args.host, args.token, args.project, args.media_type,
                             args.section, args.name, args.md5, args.gid, args.uid, args.attributes)
     with open(args.output, 'w') as f:
         f.write(str(media_id))
```

### Comparing `tator-1.0.5/tator/transcode/delete_media.py` & `tator-1.1.0/tator/transcode/delete_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/determine_transcode.py` & `tator-1.1.0/tator/transcode/determine_transcode.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/make_fragment_info.py` & `tator-1.1.0/tator/transcode/make_fragment_info.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/make_thumbnails.py` & `tator-1.1.0/tator/transcode/make_thumbnails.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/prepare.py` & `tator-1.1.0/tator/transcode/prepare.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/transcode/transcode.py` & `tator-1.1.0/tator/transcode/transcode.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,20 +173,31 @@
         "-select_streams", "v",
         path,
     ]
     output = subprocess.run(cmd, stdout=subprocess.PIPE, check=True).stdout
     video_info = json.loads(output)
     avg_frame_rate=video_info['streams'][0]['avg_frame_rate']
     input_pixel_format=video_info['streams'][0]['pix_fmt']
+    tags=video_info['streams'][0].get('tags')
+    rotation = 0
+    if tags is not None:
+        rotation = int(tags.get('rotate', "0")) % 360
+    transpose = "null"
+    if rotation == 90:
+        transpose = "transpose=2"
+    elif rotation == 180:
+        transpose = "hflip,vflip"
+    elif rotation == 270:
+        transpose = "transpose=1"
 
     vid_dims = [raw_height, raw_width]
     cmd = [
         "ffmpeg", "-y",
-        "-i", path,
-        "-i", os.path.join(os.path.dirname(os.path.abspath(__file__)), "black.mp4"),
+        "-noautorotate", "-i", path,
+        "-noautorotate", "-i", os.path.join(os.path.dirname(os.path.abspath(__file__)), "black.mp4"),
     ]
 
     vaapi_present = [c for c in codecs if find_best_encoder(c).find('vaapi') >= 0]
     print(codecs)
     print(vaapi_present)
     if vaapi_present:
         cmd.extend(['-init_hw_device', 'vaapi=hw',
@@ -214,23 +225,24 @@
 
         if codec.find('264') > 0:
             preset = preset if preset else 'fast'
             per_res.extend(["-preset", preset,
                             "-tune", "fastdecode"])
         if codec.find('libsvtav1') >= 0:
             preset = preset if preset else '5'
-            per_res.extend(['-preset', preset])
+            per_res.extend(['-preset', preset, "-tune", "fastdecode"])
 
         cmd.extend([*per_res,
                     "-vcodec", codec,
                     "-pix_fmt", pixel_format,
                     quality_flag, crfs[ridx],
                     "-filter_complex",
                     # Scale the black mp4 to the input resolution prior to concating and scaling back down.
-                    f"[0:v:0]yadif[a{ridx}];[a{ridx}]setsar=1[vid{ridx}];[1:v:0]scale={vid_dims[1]}:{vid_dims[0]},setsar=1[bv{ridx}];[vid{ridx}][bv{ridx}]concat=n=2:v=1:a=0[rv{ridx}];[rv{ridx}]scale=-2:{resolution}[catv{ridx}];[catv{ridx}]pad=ceil(iw/2)*2:ceil(ih/2)*2[norate{ridx}];[norate{ridx}]fps={avg_frame_rate}{hw_upload}[outv{ridx}]",
+                    f"[0:v:0]{transpose}[rot0];[rot0]yadif[a{ridx}];[a{ridx}]setsar=1[vid{ridx}];[1:v:0]scale={vid_dims[1]}:{vid_dims[0]},setsar=1[bv{ridx}];[vid{ridx}][bv{ridx}]concat=n=2:v=1:a=0[rv{ridx}];[rv{ridx}]scale=-2:{resolution}[catv{ridx}];[catv{ridx}]pad=ceil(iw/2)*2:ceil(ih/2)*2[norate{ridx}];[norate{ridx}]fps={avg_frame_rate}{hw_upload}[outv{ridx}]",
+                    "-metadata:s:v:0", "rotate=0",
                     "-map", f"[outv{ridx}]",
                     output_file])
 
     logger.info('ffmpeg cmd = {}'.format(cmd))
     _launch_and_monitor_resources(cmd)
 
     api = get_api(host, token)
```

### Comparing `tator-1.0.5/tator/util/__init__.py` & `tator-1.1.0/tator/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 from tator.util.clone_version import clone_version
 from tator.util.clone_membership import clone_membership
 from tator.util.concat import make_concat
 from tator.util.find_single_change import find_single_change
 from tator.util.get_paginator import get_paginator
 from tator.util.media_util import MediaUtil
 from tator.util.media_manipulation import supplement_video_to_media
-
+from tator.util.upload_generic_file import upload_generic_file
```

### Comparing `tator-1.0.5/tator/util/_download_file.py` & `tator-1.1.0/tator/util/_download_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/_upload_file.py` & `tator-1.1.0/tator/util/_upload_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/chunked_file_list.py` & `tator-1.1.0/tator/util/chunked_file_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_leaf_list.py` & `tator-1.1.0/tator/util/clone_leaf_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_leaf_type.py` & `tator-1.1.0/tator/util/clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_localization_list.py` & `tator-1.1.0/tator/util/clone_localization_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_localization_type.py` & `tator-1.1.0/tator/util/clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_media_list.py` & `tator-1.1.0/tator/util/clone_media_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,29 +82,29 @@
         dest_type = -1
         dest_section = 'My cloned media'
         created_ids = []
         generator = clone_media_list(src_api, query_params, dest_project, media_mapping,
                                      dest_type, dest_section, dest_api)
         for num_created, num_total, response, id_map in generator:
             print(f"Created {num_created} of {num_total} files...")
-            created_ids.append(response.id)
+            created_ids.append(response.id[0])
         print(f"Finished creating {num_created} files!")
 
     Example for same host:
 
     .. code-block:: python
 
         api = tator.get_api(host, token)
         query_params = {'media_id': [1]}
         dest_project = 1
         created_ids = []
         generator = clone_media_list(src_api, query_params, dest_project)
         for num_created, num_total, response, id_map in generator:
             print(f"Created {num_created} of {num_total} files...")
-            created_ids += response.id # This response is from the CloneMedia endpoint.
+            created_ids += response.id[0] # This response is from the CloneMedia endpoint.
         print(f"Finished creating {num_created} files!")
 
     :param src_api: :class:`tator.TatorApi` object corresponding to source host or only
         host if this is a clone on same host.
     :param query_params: Dictionary containing query parameters for source media list.
     :param dest_project: Unique integer identifying destination project.
     :param media_mapping: Mapping between source and destination media IDs. Only used
@@ -183,39 +183,39 @@
             if media.gid:
                 media_spec['gid'] = media.gid
             if media.uid:
                 media_spec['uid'] = media.uid
 
             # Create the media object.
             response = dest_api.create_media_list(dest_project, body=[media_spec])
-            id_map = {media.id: response.id}
+            id_map = {media.id: response.id[0]}
 
             # Transfer videos.
             if media.media_files:
                 media_files = media.media_files.to_dict()
                 for key in ['streaming', 'archival', 'audio', 'image', 'thumbnail', 'thumbnail_gif']:
                     if ignore_transfer:
                         continue
                     if media_files.get(key):
                         for item in media_files[key]:
                             media_def = {k: v for k, v in item.items()
                                          if v is not None}
                             src_path = media_def.pop('path', None)
-                            media_def['path'] = transfer(src_path, media_id=response.id)
+                            media_def['path'] = transfer(src_path, media_id=response.id[0])
                             if key == 'streaming':
                                 src_segments = media_def.pop('segment_info', None)
-                                media_def['segment_info'] = transfer(src_segments, media_id=response.id)
+                                media_def['segment_info'] = transfer(src_segments, media_id=response.id[0])
                             if key in ['streaming', 'archival']:
-                                dest_api.create_video_file(response.id, role=key,
+                                dest_api.create_video_file(response.id[0], role=key,
                                                            video_definition=media_def)
                             elif key in ['image', 'thumbnail', 'thumbnail_gif']:
-                                dest_api.create_image_file(response.id, role=key,
+                                dest_api.create_image_file(response.id[0], role=key,
                                                            image_definition=media_def)
                             elif key in ['audio']:
-                                dest_api.create_audio_file(response.id, role=key,
+                                dest_api.create_audio_file(response.id[0], role=key,
                                                            audio_definition=media_def)
                 if media.media_files.ids:
                     dest_ids = []
                     for id_ in media.media_files.ids:
                         if id_ in media_mapping:
                             dest_ids.append(media_mapping[id_])
                         else:
@@ -223,10 +223,10 @@
                                              "mapping! Individual videos should be migrated "
                                              "before multi videos.")
                     update = {'multi': {'ids': dest_ids}}
                     if media.media_files.layout:
                         update['multi']['layout'] = media.media_files.layout
                     if media.media_files.quality:
                         update['multi']['quality'] = media.media_files.quality
-                    dest_api.update_media(response.id, media_update=update)
-            created_ids.append(response.id)
+                    dest_api.update_media(response.id[0], media_update=update)
+            created_ids.append(response.id[0])
             yield (len(created_ids), total_files, response, id_map)
```

### Comparing `tator-1.0.5/tator/util/clone_media_type.py` & `tator-1.1.0/tator/util/clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_membership.py` & `tator-1.1.0/tator/util/clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_section.py` & `tator-1.1.0/tator/util/clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_state_list.py` & `tator-1.1.0/tator/util/clone_state_list.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_state_type.py` & `tator-1.1.0/tator/util/clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/clone_version.py` & `tator-1.1.0/tator/util/clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/concat.py` & `tator-1.1.0/tator/util/concat.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,31 +63,31 @@
                   'fps': media_obj.fps,
                   'num_frames': media_obj.num_frames,
                   'type': type_id,
                   'width': media_obj.width,
                   'height': media_obj.height}
 
     resp = api.create_media_list(project, [media_spec])
-    print(f"Created {resp.id}")
+    print(f"Created {resp.id[0]}")
 
     # Copy thumbnails from first media
     with tempfile.TemporaryDirectory() as d:
         thumb_path = os.path.join(d,'tiled_thumb.jpg')
         thumb_gif_path = os.path.join(d,'tiled_gif.gif')
 
         for progress in download_media(api, media_obj, thumb_path, None, 'thumbnail'):
             pass
         for progress in download_media(api, media_obj, thumb_gif_path, None, 'thumbnail_gif'):
             pass
 
         for progress, thumbnail_info in _upload_file(api, project, thumb_path,
-                                                     media_id=resp.id, filename='tiled_thumb.jpg'):
+                                                     media_id=resp.id[0], filename='tiled_thumb.jpg'):
             logger.info(f"Thumbnail upload progress: {progress}%")
         for progress, thumbnail_gif_info in _upload_file(api, project, thumb_gif_path,
-                                                         media_id=resp.id, filename='tiled_gif.gif'):
+                                                         media_id=resp.id[0], filename='tiled_gif.gif'):
             logger.info(f"Thumbnail gif upload progress: {progress}%")
 
         # Open images to get output resolution.
         thumb_image = Image.open(thumb_path)
         thumb_gif_image = Image.open(thumb_gif_path)
 
         # Create image definitions for thumbnails.
@@ -96,17 +96,17 @@
                      'resolution': [thumb_image.height, thumb_image.width],
                      'mime': f'image/{thumb_image.format.lower()}'}
         thumb_gif_def = {'path': thumbnail_gif_info.key,
                          'size': os.stat(thumb_gif_path).st_size,
                          'resolution': [thumb_gif_image.height, thumb_gif_image.width],
                          'mime': f'image/{thumb_gif_image.format.lower()}'}
 
-        response = api.create_image_file(resp.id, role='thumbnail', image_definition=thumb_def)
+        response = api.create_image_file(resp.id[0], role='thumbnail', image_definition=thumb_def)
         assert isinstance(response, MessageResponse)
-        response = api.create_image_file(resp.id, role='thumbnail_gif', image_definition=thumb_gif_def)
+        response = api.create_image_file(resp.id[0], role='thumbnail_gif', image_definition=thumb_gif_def)
         assert isinstance(response, MessageResponse)
 
     concat_def = [{"id": media_id, "timestampOffset": offset} for media_id,offset in zip(media_ids, offsets)]
-    api.update_media(resp.id, {"concat": concat_def})
+    api.update_media(resp.id[0], {"concat": concat_def})
 
     return resp
```

### Comparing `tator-1.0.5/tator/util/download_attachment.py` & `tator-1.1.0/tator/util/download_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/download_media.py` & `tator-1.1.0/tator/util/download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/download_temporary_file.py` & `tator-1.1.0/tator/util/download_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/find_single_change.py` & `tator-1.1.0/tator/util/find_single_change.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/full_state_graphic.py` & `tator-1.1.0/tator/util/full_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/get_api.py` & `tator-1.1.0/tator/util/get_api.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/get_images.py` & `tator-1.1.0/tator/util/get_images.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/import_media.py` & `tator-1.1.0/tator/util/import_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/live_stream.py` & `tator-1.1.0/tator/util/live_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,9 +48,9 @@
         "type": type_id,
         "section": section,
         "md5": md5_of_config,
     }
     create_resp = api.create_media_list(project, [media_spec])
 
     patch_object = {"live": {"layout": layout, "streams": feedInfo}}
-    return api.update_media(create_resp.id, patch_object)
+    return api.update_media(create_resp.id[0], patch_object)
```

### Comparing `tator-1.0.5/tator/util/md5sum.py` & `tator-1.1.0/tator/util/md5sum.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/media_manipulation.py` & `tator-1.1.0/tator/util/media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/media_util.py` & `tator-1.1.0/tator/util/media_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     self._height = None
     self._width = None
     self._start_bias_frame = None
     self._moof_data = None
 
   def load_from_url(self, video_url, segment_url, height, width, fps):
     """ Setup the MediaUtil instance with primitive types
+
     :param video_url: Publically accessible URL to the raw segmented mp4 file to use
     :param segment_url: Publically accessible URL for the segmentation map file. 
     :param height: The vertical resolution of the video
     :param width: The horizontal resolution of the video
     :param fps: The frames per second of the video
     """
     self._video_file = video_url
@@ -223,14 +224,15 @@
     else:
       output_file = os.path.join(self._temp_dir, f"0.{render_format}")
 
     return output_file
 
   def get_animation(self, frames, fps, roi=None, render_format='mp4', force_scale=None):
     """ Return an animation of frames at a given FPS.
+
         :param  frames: list of frames
         :param fps: FPS of output animation """
     if not self._generate_frame_images(frames, roi,
                                        render_format="jpg",
                                        force_scale=force_scale):
       return None
```

### Comparing `tator-1.0.5/tator/util/multi_stream.py` & `tator-1.1.0/tator/util/multi_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,21 @@
 
         media_spec = {'attributes': attributes,
                 'name': name,
                 'md5': md5,
                 'section': section_obj.name,
                 'type': type_id}
         resp = api.create_media_list(project, [media_spec])
-        print(f"Created {resp.id}")
+        print(f"Created {resp.id[0]}")
         
         for progress, thumbnail_info in _upload_file(api, project, thumb_path,
-                                                        media_id=resp.id, filename='tiled_thumb.jpg'):
+                                                        media_id=resp.id[0], filename='tiled_thumb.jpg'):
                 logger.info(f"Thumbnail upload progress: {progress}%")
         for progress, thumbnail_gif_info in _upload_file(api, project, thumb_gif_path,
-                                                        media_id=resp.id, filename='tiled_gif.gif'):
+                                                        media_id=resp.id[0], filename='tiled_gif.gif'):
             logger.info(f"Thumbnail gif upload progress: {progress}%")
 
         # Open images to get output resolution.
         thumb_image = Image.open(thumb_path)
         thumb_gif_image = Image.open(thumb_gif_path)
 
         # Create image definitions for thumbnails.
@@ -156,24 +156,24 @@
                      'resolution': [thumb_image.height, thumb_image.width],
                      'mime': f'image/{thumb_image.format.lower()}'}
         thumb_gif_def = {'path': thumbnail_gif_info.key,
                          'size': os.stat(thumb_gif_path).st_size,
                          'resolution': [thumb_gif_image.height, thumb_gif_image.width],
                          'mime': f'image/{thumb_gif_image.format.lower()}'}
 
-        response = api.create_image_file(resp.id, role='thumbnail', image_definition=thumb_def)
+        response = api.create_image_file(resp.id[0], role='thumbnail', image_definition=thumb_def)
         assert isinstance(response, MessageResponse)
-        response = api.create_image_file(resp.id, role='thumbnail_gif', image_definition=thumb_gif_def)
+        response = api.create_image_file(resp.id[0], role='thumbnail_gif', image_definition=thumb_gif_def)
         assert isinstance(response, MessageResponse)
 
         # Add the multi definition.
         multi_def = {"layout": layout,
                      "ids": media_ids}
         if quality:
             multi_def.update({"quality": quality})
         if frame_offset:
             assert len(frame_offset) == len(media_ids), "Length of frame offsets did not match length of media IDs!"
             multi_def.update({"frameOffset": frame_offset})
-        api.update_media(resp.id, {"multi": multi_def})
+        api.update_media(resp.id[0], {"multi": multi_def})
 
         return resp
```

### Comparing `tator-1.0.5/tator/util/register_algorithm.py` & `tator-1.1.0/tator/util/register_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/register_applet.py` & `tator-1.1.0/tator/util/register_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/tator-symbol.png` & `tator-1.1.0/tator/util/tator-symbol.png`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/to_dataframe.py` & `tator-1.1.0/tator/util/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/update_applet.py` & `tator-1.1.0/tator/util/update_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/upload_attachment.py` & `tator-1.1.0/tator/util/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/tator/util/upload_media.py` & `tator-1.1.0/tator/util/upload_media.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from urllib.parse import urljoin
 
 from ._upload_file import _upload_file
 from .md5sum import md5sum
 
 def upload_media(api, type_id, path, md5=None, section=None, fname=None,
                  upload_gid=None, upload_uid=None, chunk_size=10*1024*1024,
-                 attributes=None, media_id=None, timeout=30, max_workers=10):
+                 attributes=None, email_spec=None, media_id=None, timeout=30,
+                 max_workers=10):
     """ Uploads a single media file.
 
     Example:
 
     .. code-block:: python
 
         api = tator.get_api(host, token)
@@ -29,14 +30,15 @@
     :param section: [Optional] Section name. If a section with this name does
         not exist it will be created.
     :param fname: [Optional] Filename to use for upload.
     :param upload_gid: [Optional] Group ID of the upload.
     :param upload_uid: [Optional] Unique ID of the upload.
     :param chunk_size: [Optional] Chunk size in bytes. Default is 2MB.
     :param attributes: [Optional] Attributes to apply to media object.
+    :param email_spec: [Optional] Spec for email to be sent upon transcode completion.
     :param media_id: [Optional] Unique ID of existing media object.
     :param timeout: [Optional] Request timeout for each upload chunk in seconds. Default is 30.
     :param max_workers: [Optional] Max workers for concurrent requests.
     :returns: Generator that yields tuple containing progress (0-100) and a
         response. The response is `None` until the last yield, when the response
         is the response object from :meth:`tator.TatorApi.create_media_list` or
         :meth:`tator.TatorApi.transcode`.
@@ -80,11 +82,12 @@
         'md5': md5,
         'attributes': attributes,
         'media_id': media_id,
         'size': os.stat(path).st_size,
     }
     # Initiate transcode or save image.
     if mime.find('video') >= 0:
+        spec['email_spec'] = email_spec
         response = api.transcode(project_id, transcode_spec=spec)
     else:
         response = api.create_media_list(project_id, body=[spec])
     yield (100, response)
```

### Comparing `tator-1.0.5/tator/util/upload_temporary_file.py` & `tator-1.1.0/tator/util/upload_temporary_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import os
-import math
-from uuid import uuid1
-
-from urllib.parse import urljoin
-from urllib.parse import urlsplit
 
 from ._upload_file import _upload_file
-from .md5sum import md5sum
 
-def upload_temporary_file(api, project, path, lookup=None, hours=24,
-                          name=None, chunk_size=100*1024*1024):
+def upload_temporary_file(
+    api, project, path, lookup=None, hours=24, name=None, chunk_size=100*1024*1024
+):
     """ Upload a file to the temporary file storage location.
 
     Example:
 
     .. code-block:: python
 
         api = tator.get_api(host, token)
@@ -34,19 +29,15 @@
     """
     if name is None:
         name = os.path.basename(path)
 
     if lookup is None:
         lookup = name
 
-    for progress, upload_info in _upload_file(api, project, path):
+    for progress, upload_info in _upload_file(api, project, path, chunk_size=chunk_size):
         yield (progress, None)
     url = api.get_download_info(project, {'keys': [upload_info.key]})[0].url
 
-    response = api.create_temporary_file(project, temporary_file_spec={
-        "url": url,
-        "name": name,
-        "lookup": lookup,
-        "hours": 24,
-    })
+    response = api.create_temporary_file(
+        project, temporary_file_spec={"url": url, "name": name, "lookup": lookup, "hours": hours}
+    )
     yield (100, response)
-
```

### Comparing `tator-1.0.5/tator.egg-info/SOURCES.txt` & `tator-1.1.0/tator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 tator/openapi/tator_openapi/models/affiliation_spec.py
 tator/openapi/tator_openapi/models/affiliation_update.py
 tator/openapi/tator_openapi/models/algorithm.py
 tator/openapi/tator_openapi/models/algorithm_manifest.py
 tator/openapi/tator_openapi/models/algorithm_manifest_spec.py
 tator/openapi/tator_openapi/models/algorithm_parameter.py
 tator/openapi/tator_openapi/models/algorithm_spec.py
-tator/openapi/tator_openapi/models/analysis.py
-tator/openapi/tator_openapi/models/analysis_spec.py
 tator/openapi/tator_openapi/models/announcement.py
 tator/openapi/tator_openapi/models/applet.py
 tator/openapi/tator_openapi/models/applet_spec.py
 tator/openapi/tator_openapi/models/archive_config.py
 tator/openapi/tator_openapi/models/attribute_combinator_spec.py
 tator/openapi/tator_openapi/models/attribute_filter_spec.py
 tator/openapi/tator_openapi/models/attribute_operation_spec.py
@@ -92,14 +90,15 @@
 tator/openapi/tator_openapi/models/invitation_spec.py
 tator/openapi/tator_openapi/models/invitation_update.py
 tator/openapi/tator_openapi/models/job.py
 tator/openapi/tator_openapi/models/job_cluster.py
 tator/openapi/tator_openapi/models/job_cluster_spec.py
 tator/openapi/tator_openapi/models/job_node.py
 tator/openapi/tator_openapi/models/job_spec.py
+tator/openapi/tator_openapi/models/job_spec_failure_email_spec.py
 tator/openapi/tator_openapi/models/leaf.py
 tator/openapi/tator_openapi/models/leaf_bulk_update.py
 tator/openapi/tator_openapi/models/leaf_id_query.py
 tator/openapi/tator_openapi/models/leaf_spec.py
 tator/openapi/tator_openapi/models/leaf_suggestion.py
 tator/openapi/tator_openapi/models/leaf_type.py
 tator/openapi/tator_openapi/models/leaf_type_spec.py
@@ -220,27 +219,29 @@
 tator/util/multi_stream.py
 tator/util/register_algorithm.py
 tator/util/register_applet.py
 tator/util/tator-symbol.png
 tator/util/to_dataframe.py
 tator/util/update_applet.py
 tator/util/upload_attachment.py
+tator/util/upload_generic_file.py
 tator/util/upload_media.py
 tator/util/upload_temporary_file.py
 test/test_a_float_array.py
 test/test_algorithm.py
 test/test_algorithm_launch.py
 test/test_applet.py
 test/test_archive_date.py
 test/test_attachment.py
 test/test_attribute_type_addition.py
 test/test_attribute_type_deletion.py
 test/test_attribute_type_mutation.py
 test/test_attributes.py
 test/test_change_log.py
+test/test_chunked_create.py
 test/test_clone_leaf_type.py
 test/test_clone_localization_type.py
 test/test_clone_media.py
 test/test_clone_media_type.py
 test/test_clone_membership.py
 test/test_clone_section.py
 test/test_clone_state_type.py
```

### Comparing `tator-1.0.5/test/test_a_float_array.py` & `tator-1.1.0/test/test_a_float_array.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_algorithm.py` & `tator-1.1.0/test/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_algorithm_launch.py` & `tator-1.1.0/test/test_algorithm_launch.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_applet.py` & `tator-1.1.0/test/test_applet.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_archive_date.py` & `tator-1.1.0/test/test_archive_date.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_attachment.py` & `tator-1.1.0/test/test_attachment.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_attribute_type_addition.py` & `tator-1.1.0/test/test_attribute_type_addition.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_attribute_type_deletion.py` & `tator-1.1.0/test/test_attribute_type_deletion.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_attribute_type_mutation.py` & `tator-1.1.0/test/test_attribute_type_mutation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_attributes.py` & `tator-1.1.0/test/test_attributes.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_change_log.py` & `tator-1.1.0/test/test_change_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
             "attributes": {"test_int": random.randint(0, 100)},
         }
         for _ in range(num_media)
     ]
 
     # Create the media.
     media_ids = [
-        tator_api.create_media_list(project=project, body=[media_spec]).id
+        tator_api.create_media_list(project=project, body=[media_spec]).id[0]
         for media_spec in media_specs
     ]
 
     # Creation tests
     create_changes = []
     for media_id, media_spec in zip(media_ids, media_specs):
         changes = tator_api.get_change_log_list(
@@ -577,15 +577,15 @@
         "md5": str(uuid.uuid1())[:32],
         "section": "Test media change log",
         "attributes": {"test_int": test_int},
     }
 
 
     # Create the media.
-    media_id = tator_api.create_media_list(project=project, body=media_spec).id
+    media_id = tator_api.create_media_list(project=project, body=media_spec).id[0]
 
     # Look for change that shouldn't be there
     found_change = tator.util.find_single_change(
         tator_api, project, media_id, "test_int", new_value=test_int - 1
     )
     assert found_change is None
```

### Comparing `tator-1.0.5/test/test_clone_leaf_type.py` & `tator-1.1.0/test/test_clone_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_clone_localization_type.py` & `tator-1.1.0/test/test_clone_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_clone_media.py` & `tator-1.1.0/test/test_clone_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,56 +60,56 @@
     query_params = {'project': project, 'media_id': [multi]}
     section = 'Cloned media util same host'
     created_ids = []
     generator = tator.util.clone_media_list(tator_api, query_params, project, {}, multi_type,
                                             section)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} files...")
-        created_ids.append(response.id)
+        created_ids.append(response.id[0])
     print(f"Finished creating {num_created} files!")
     assert len(created_ids) == 1
 
 def test_clone_videos_util_same_host(host, token, project, video_type, video):
     tator_api = tator.get_api(host, token)
     query_params = {'project': project, 'media_id': [video]}
     section = 'Cloned media util same host'
     created_ids = []
     generator = tator.util.clone_media_list(tator_api, query_params, project, {}, video_type,
                                             section)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} files...")
-        created_ids.append(response.id)
+        created_ids.append(response.id[0])
     print(f"Finished creating {num_created} files!")
     assert len(created_ids) == 1
 
 def test_clone_images_util_same_host(host, token, project, image_type, image):
     tator_api = tator.get_api(host, token)
     query_params = {'project': project, 'media_id': [image]}
     section = 'Cloned media util same host'
     created_ids = []
     generator = tator.util.clone_media_list(tator_api, query_params, project, {}, image_type,
                                             section)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} files...")
-        created_ids.append(response.id)
+        created_ids.append(response.id[0])
     print(f"Finished creating {num_created} files!")
     assert len(created_ids) == 1
 
 def test_clone_multi_util_different_host(host, token, project, multi_type, multi, video):
     tator_api = tator.get_api(host, token)
     dest_api = tator.get_api(host, token)
     assert tator_api is not dest_api
     query_params = {'project': project, 'media_id': [multi]}
     section = 'Cloned media util different host'
     created_ids = []
     generator = tator.util.clone_media_list(tator_api, query_params, project, {video:video},
                                             multi_type, section, dest_api)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} files...")
-        created_ids.append(response.id)
+        created_ids.append(response.id[0])
     print(f"Finished creating {num_created} files!")
     tator.util.clone_media_list(tator_api, query_params, project, multi_type,
                                 'Cloned media util different host', tator_api)
     assert len(created_ids) == 1
 
 def test_clone_videos_util_different_host(host, token, project, video_type, video):
     tator_api = tator.get_api(host, token)
@@ -118,15 +118,15 @@
     query_params = {'project': project, 'media_id': [video]}
     section = 'Cloned media util different host'
     created_ids = []
     generator = tator.util.clone_media_list(tator_api, query_params, project, {}, video_type,
                                             section, dest_api)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} files...")
-        created_ids.append(response.id)
+        created_ids.append(response.id[0])
     print(f"Finished creating {num_created} files!")
     tator.util.clone_media_list(tator_api, query_params, project, video_type,
                                 'Cloned media util different host', tator_api)
     assert len(created_ids) == 1
 
 def test_clone_images_util_different_host(host, token, project, image_type, image):
     tator_api = tator.get_api(host, token)
@@ -135,10 +135,10 @@
     query_params = {'project': project, 'media_id': [image]}
     section = 'Cloned media util different host'
     created_ids = []
     generator = tator.util.clone_media_list(tator_api, query_params, project, {}, image_type,
                                             section, dest_api)
     for num_created, num_total, response, id_map in generator:
         print(f"Created {num_created} of {num_total} files...")
-        created_ids.append(response.id)
+        created_ids.append(response.id[0])
     print(f"Finished creating {num_created} files!")
     assert len(created_ids) == 1
```

### Comparing `tator-1.0.5/test/test_clone_media_type.py` & `tator-1.1.0/test/test_clone_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_clone_membership.py` & `tator-1.1.0/test/test_clone_membership.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_clone_section.py` & `tator-1.1.0/test/test_clone_section.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_clone_state_type.py` & `tator-1.1.0/test/test_clone_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_clone_version.py` & `tator-1.1.0/test/test_clone_version.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_collection.py` & `tator-1.1.0/test/test_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     }
     section = 'Media State Test'
     path = random.choice(paths)
     for progress, response in tator.util.upload_media(api, image_type, path,
                                                       attributes=attributes,
                                                       section=section):
         pass
-    return response.id, attributes, section
+    return response.id[0], attributes, section
 
 def random_state(project, collection_type, media_ids, post=False):
     attributes = {
         'test_bool': random.choice([False, True]),
         'test_int': random.randint(-1000, 1000),
         'test_float': random.uniform(-1000.0, 1000.0),
         'test_enum': random.choice(['a', 'b', 'c']),
```

### Comparing `tator-1.0.5/test/test_download_media.py` & `tator-1.1.0/test/test_download_media.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_extract.py` & `tator-1.1.0/test/test_extract.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_file.py` & `tator-1.1.0/test/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import logging
 import os
+import requests
 import tempfile
 
 import pytest
 import tator
 from tator.util._upload_file import _upload_file
 import json
 import base64
@@ -381,8 +382,45 @@
 
         for file_info in file_b_ids:
             if file_obj.id == file_info["file_id"]:
                 file_b_count += 1
                 break
 
     assert file_a_count == len(file_a_ids) - 2
-    assert file_b_count == len(file_b_ids) - 2
+    assert file_b_count == len(file_b_ids) - 2
+
+
+def test_upload_generic_file(host, token, project):
+    TEST_STR = b"foo"
+    # Setup the interface to Tator
+    tator_api = tator.get_api(host=host, token=token)
+
+    # Create a FileType
+    response = tator_api.create_file_type(
+        project=project,
+        file_type_spec={
+            "name": "generic_upload_file_type",
+            "project": project,
+            "attribute_types": [
+                {"name": "test", "dtype": "int", "default": 0, "minimum": -1000, "maximum": 1000}
+            ],
+        },
+    )
+    type_id = response.id
+
+    # Create a file locally and test uploading/downloading
+    with tempfile.NamedTemporaryFile() as temp_file:
+        path = temp_file.name
+        fname = os.path.basename(path)
+
+        temp_file.write(TEST_STR)
+        temp_file.flush()
+
+        for progress, response in tator.util.upload_generic_file(tator_api, type_id, path, "File description", fname):
+            print(f"Progress: {progress}%")
+    assert response.name == fname
+    download_info = tator_api.get_download_info(project=project, download_info_spec={"keys": [response.path]})
+
+    assert len(download_info) == 1
+    assert download_info[0].key == response.path
+    response = requests.get(download_info[0].url, stream=True)
+    assert response.content == TEST_STR
```

### Comparing `tator-1.0.5/test/test_file_type.py` & `tator-1.1.0/test/test_file_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_get_clip.py` & `tator-1.1.0/test/test_get_clip.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_getframe.py` & `tator-1.1.0/test/test_getframe.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_import_media.py` & `tator-1.1.0/test/test_import_media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tator
 import time
 
 def test_import_image(host, token, project, image_type):
     api = tator.get_api(host, token)
     url = 'https://www.cvisionai.com/static/74822662b430b97b6d86bb74beab1666/fb5f3/open-em-image.png'
     response = tator.util.import_media(api, image_type, url)
-    assert(isinstance(response, tator.models.CreateResponse))
+    assert(isinstance(response, tator.models.CreateListResponse))
 
 
 def wait_for_transcode(api, transcode_id):
     while True:
         transcode = api.get_transcode(uid=transcode_id)
         status = transcode.job.status.lower()
         if status == "succeeded":
```

### Comparing `tator-1.0.5/test/test_job_cancel.py` & `tator-1.1.0/test/test_job_cancel.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_job_cluster.py` & `tator-1.1.0/test/test_job_cluster.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_leaf.py` & `tator-1.1.0/test/test_leaf.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_leaf_type.py` & `tator-1.1.0/test/test_leaf_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_local_transcode.py` & `tator-1.1.0/test/test_local_transcode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 import time
 import subprocess
 
 import tator
 import uuid
 import json
-import subprocess
+
+
+def _assert_subprocess(cmd, desired_result=True):
+    out = subprocess.run(cmd, capture_output=True)
+
+    if desired_result:
+        assert out.returncode == 0, out.stderr
+    else:
+        assert out.returncode != 0, out.stdout
+
 
 def _get_stream_info(path):
     cmd = [
         "ffprobe",
         "-v","error",
         "-show_entries", "stream",
         "-print_format", "json",
@@ -25,16 +34,16 @@
         '--host', host,
         '--token', token,
         '--project', str(project),
         '--type', str(video_type),
         '--section', 'Locally transcoded',
         '--name', unique_name
     ]
-    subprocess.run(cmd, check=True)
-    subprocess.run(cmd, check=True)
+    _assert_subprocess(cmd)
+    _assert_subprocess(cmd)
     api = tator.get_api(host, token)
     media_obj = api.get_media_list(project, name=unique_name, presigned=3600)[0]
 
     stream_info = _get_stream_info(media_obj.media_files.archival[0].path)
     assert stream_info['pix_fmt'] == 'yuv420p'
     stream_info = _get_stream_info(media_obj.media_files.streaming[0].path)
     assert stream_info['pix_fmt'] == 'yuv420p'
@@ -46,38 +55,33 @@
         '--host', host,
         '--token', token,
         '--project', str(project),
         '--type', str(yuv444p_video_type),
         '--section', 'Locally transcoded (yuv444p)',
         '--name', unique_name
     ]
-    subprocess.run(cmd, check=True)
+    _assert_subprocess(cmd)
     api = tator.get_api(host, token)
     media_obj = api.get_media_list(project, name=unique_name, presigned=3600)[0]
 
     stream_info = _get_stream_info(media_obj.media_files.archival[0].path)
     assert stream_info['pix_fmt'] == 'yuv444p'
     stream_info = _get_stream_info(media_obj.media_files.streaming[0].path)
     assert stream_info['pix_fmt'] == 'yuv444p'
 
 def test_bad_file(host, token, project, video_type, image_file):
-    failed = False
-    try:
-        cmd = [
-            'python3', '-m', 'tator.transcode', image_file,
-            '--host', host,
-            '--token', token,
-            '--project', str(project),
-            '--type', str(video_type),
-            '--section', 'Bad transcodes',
-        ]
-        subprocess.run(cmd, check=True)
-    except subprocess.CalledProcessError as cpe:
-        failed = True
-    assert(failed)
+    cmd = [
+        'python3', '-m', 'tator.transcode', image_file,
+        '--host', host,
+        '--token', token,
+        '--project', str(project),
+        '--type', str(video_type),
+        '--section', 'Bad transcodes',
+    ]
+    _assert_subprocess(cmd, False)
     time.sleep(2)
     # Make sure media file is gone.
     api = tator.get_api(host, token)
     sections = api.get_section_list(project)
     section_obj = [s for s in sections if s.name == 'Bad transcodes'][0]
 
     medias = api.get_media_list(project, attribute=[f'tator_user_sections::{section_obj.tator_user_sections}'])
```

### Comparing `tator-1.0.5/test/test_localization.py` & `tator-1.1.0/test/test_localization.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_localization_graphic.py` & `tator-1.1.0/test/test_localization_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_localization_type.py` & `tator-1.1.0/test/test_localization_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_media.py` & `tator-1.1.0/test/test_media.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from datetime import datetime
 import os
+from random import randint
 import tempfile
 from time import sleep
+from urllib.parse import parse_qs, urlparse
 from uuid import uuid1
 
 import tator
 
 def test_get_file(host, token, project, video):
     tator_api = tator.get_api(host, token)
     video_obj = tator_api.get_media(video)
@@ -148,31 +150,114 @@
             "md5": "",
         }
         for idx in range(n_images)
     ]
 
     start = datetime.now()
     response = tator_api.create_media_list(project, body=media_specs)
+    created_ids = response.id
     duration = (datetime.now() - start).total_seconds()
     assert duration < 5
 
     assert str(len(media_specs)) in response.message
+    assert len(media_specs) == len(created_ids)
 
     new_project_media_count = -1
     desired_project_media_count = project_media_count + len(media_specs)
     for _ in range(30):
         sleep(1)
         new_project_media_count = tator_api.get_media_count(project, type=image_type)
         if new_project_media_count == desired_project_media_count:
             break
     assert new_project_media_count == desired_project_media_count
     for _ in range(30):
         sleep(1)
-        media_list = tator_api.get_media_list(project, type=image_type)
+        media_list = tator_api.get_media_list(project, type=image_type, media_id=created_ids)
 
         n_with_media_files = 0
         for media in media_list:
             if media.name.startswith(uuid) and media.media_files is not None:
                 n_with_media_files += 1
         if n_with_media_files == n_images:
             break
     assert n_with_media_files == n_images
+
+
+def parse_url(url):
+    parsed_url = urlparse(url)
+    return parsed_url.path, parse_qs(parsed_url.query)
+
+
+def parse_media_files(media):
+    return dict(
+        parse_url(spec["path"])
+        for file_type, file_specs in media.media_files.to_dict().items()
+        if file_specs is not None
+        for spec in file_specs
+        if "path" in spec
+    )
+
+
+def test_presigned_no_cache(host, token, project, video_type, video_file):
+    expires_key = "X-Amz-Expires"
+
+    # Set up new video to ensure a clean cache
+    tator_api = tator.get_api(host, token)
+    uuid_val = str(uuid1())
+    attributes = {"test_string": uuid_val}
+    for progress, response in tator.util.upload_media(
+            tator_api, video_type, video_file, attributes=attributes
+    ):
+        print(f"Upload video progress: {progress}%")
+    print(response.message)
+
+    while True:
+        response = tator_api.get_media_list(
+            project,
+            name='AudioVideoSyncTest_BallastMedia.mp4',
+            attribute=[f"test_string::{uuid_val}"],
+        )
+        print("Waiting for transcode...")
+        sleep(2.5)
+        if len(response) == 0:
+            continue
+        if response[0].media_files is None:
+            continue
+        streaming = response[0].media_files.streaming
+        have_archival = response[0].media_files.archival is not None
+        if streaming and have_archival and len(streaming) == 4:
+            video_id = response[0].id
+            break
+
+    # Get initial presigned url
+    original_presigned_duration = new_presigned_duration = randint(8640, 86400)
+    while new_presigned_duration == original_presigned_duration:
+        new_presigned_duration = randint(8640, 86400)
+
+    video_obj = tator_api.get_media(video_id, presigned=original_presigned_duration)
+
+    init_presigned_url = parse_media_files(video_obj)
+
+    # Request a new duration without the `no_cache` flag and assert it returns the same urls
+    video_obj = tator_api.get_media(video_id, presigned=new_presigned_duration, no_cache=False)
+    no_cache_false_presigned_url = parse_media_files(video_obj)
+
+    for path, query_params in no_cache_false_presigned_url.items():
+        assert path in init_presigned_url
+        assert int(query_params[expires_key][0]) == original_presigned_duration
+
+    # Request a new duration with the `no_cache` flag and assert it returns new urls
+    video_obj = tator_api.get_media(video_id, presigned=new_presigned_duration, no_cache=True)
+    no_cache_false_presigned_url = parse_media_files(video_obj)
+
+    for path, query_params in no_cache_false_presigned_url.items():
+        assert path in init_presigned_url
+        assert int(query_params[expires_key][0]) == new_presigned_duration
+
+    # Request a new duration without the `no_cache` flag again and assert it returns the original
+    # cached urls and not the ones from the new duration
+    video_obj = tator_api.get_media(video_id, presigned=original_presigned_duration, no_cache=False)
+    no_cache_false_presigned_url = parse_media_files(video_obj)
+
+    for path, query_params in no_cache_false_presigned_url.items():
+        assert path in init_presigned_url
+        assert int(query_params[expires_key][0]) == original_presigned_duration
```

### Comparing `tator-1.0.5/test/test_media_type.py` & `tator-1.1.0/test/test_media_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_pagination.py` & `tator-1.1.0/test/test_chunked_create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from datetime import datetime
-from pprint import pprint
 import random
-from time import sleep
-from types import GeneratorType
 from uuid import uuid1
 
+import pytest
 import tator
 
 
-def make_image(tator_api, project, image_type, image_file, test_string):
+def make_image(tator_api, image_type, image_file, test_string):
     attributes = {"test_string": test_string}
-    for progress, response in tator.util.upload_media(tator_api, image_type, image_file, attributes=attributes):
+    for progress, response in tator.util.upload_media(
+        tator_api, image_type, image_file, attributes=attributes
+    ):
         print(f"Upload image progress: {progress}%")
-    return response.id
+    return response.id[0]
+
 
-def random_localization(project, box_type, image_obj, test_string, post=False):
+def random_localization(project, box_type, image_obj, test_string):
     x = random.uniform(0.0, 1.0)
     y = random.uniform(0.0, 1.0)
     w = random.uniform(0.0, 1.0 - x)
     h = random.uniform(0.0, 1.0 - y)
     attributes = {
         "test_bool": random.choice([False, True]),
         "test_int": random.randint(-1000, 1000),
@@ -34,86 +35,104 @@
         "y": y,
         "width": w,
         "height": h,
         "project": project,
         "type": box_type,
         "media_id": image_obj.id,
         "frame": 0,
-        "attributes": attributes
+        "attributes": attributes,
     }
 
     return {**out}
 
 
-def _assert_pagination(api, function_name, batch_size, total, **kwargs):
-    # Get paginator for `get_localization_list`
-    paginator = tator.util.get_paginator(api, function_name, batch_size=batch_size)
-    page_iter = paginator.paginate(**kwargs)
-    assert type(page_iter) == GeneratorType
-
-    # Check the batch size
-    all_objects = []
-    expect_stop_iteration = False
-    while True:
-        try:
-            response = next(page_iter)
-        except StopIteration:
-            assert expect_stop_iteration
-            break
-        else:
-            assert expect_stop_iteration == False
-            all_objects += response
-            if len(response) < batch_size:
-                expect_stop_iteration = True
-            else:
-                assert len(response) == batch_size
-
-    assert len(all_objects) == total
-
-
-def test_localization_pagination(host, token, project, image_type, image_file, box_type):
+def test_localization_chunked_create(host, token, project, image_type, image_file, box_type):
     test_string = str(uuid1())
     tator_api = tator.get_api(host, token)
-    image = make_image(tator_api, project, image_type, image_file, test_string)
+    image = make_image(tator_api, image_type, image_file, test_string)
     image_obj = tator_api.get_media(image)
 
-    batch_size = 100
-    num_localizations = 2222  # Should not be a multiple of batch_size
+    num_localizations = 1111
     boxes = [
-        random_localization(project, box_type, image_obj, test_string, post=True)
+        random_localization(project, box_type, image_obj, test_string)
         for _ in range(num_localizations)
     ]
+
+    # Default chunk_size
+    box_ids = [
+        new_id
+        for response in tator.util.chunked_create(
+            tator_api.create_localization_list, project, body=boxes
+        )
+        for new_id in response.id
+    ]
+    assert len(box_ids) == len(boxes)
+
+    # Small chunk_size
+    box_ids = [
+        new_id
+        for response in tator.util.chunked_create(
+            tator_api.create_localization_list, project, chunk_size=100, body=boxes
+        )
+        for new_id in response.id
+    ]
+    assert len(box_ids) == len(boxes)
+
+    # Huge chunk_size
+    box_ids = [
+        new_id
+        for response in tator.util.chunked_create(
+            tator_api.create_localization_list, project, chunk_size=1000, body=boxes
+        )
+        for new_id in response.id
+    ]
+    assert len(box_ids) == len(boxes)
+
+    tator_api.delete_media(image)
+
+
+def helper(api, project, boxes, chunk_size=None):
+    kwargs = {}
+    if chunk_size:
+        kwargs["chunk_size"] = chunk_size
     box_ids = []
     for response in tator.util.chunked_create(
-        tator_api.create_localization_list, project, body=boxes
+        api.create_localization_list, project, body=boxes, **kwargs
     ):
         box_ids += response.id
+        print(f"Created {len(response.id)} boxes")
     assert len(box_ids) == len(boxes)
-    assert len(box_ids) % 100 != 0
-    print(f"Created {len(box_ids)} boxes!")
 
-    # Verify list is the right length
-    response = tator_api.get_localization_list(project, type=box_type, media_id=[image])
-    assert len(response) == num_localizations
-
-    # Check `get_localization_list`
-    _assert_pagination(
-        tator_api,
-        "get_localization_list",
-        batch_size,
-        num_localizations,
-        project=project,
-        type=box_type,
-        media_id=[image],
-    )
-
-    # Check `get_localization_list_by_id`
-    _assert_pagination(
-        tator_api,
-        "get_localization_list_by_id",
-        batch_size,
-        num_localizations,
-        project=project,
-        localization_id_query={"media_ids": [image]},
-    )
+
+def test_localization_chunked_create(host, token, project, image_type, image_file, box_type):
+    test_string = str(uuid1())
+    tator_api = tator.get_api(host, token)
+    image = make_image(tator_api, image_type, image_file, test_string)
+    image_obj = tator_api.get_media(image)
+
+    num_localizations = 1111
+    boxes = [
+        random_localization(project, box_type, image_obj, test_string)
+        for _ in range(num_localizations)
+    ]
+
+    # Default chunk_size
+    print("using default chunk size")
+    helper(tator_api, project, boxes)
+
+    # Small chunk_size
+    print("using small chunk size (100)")
+    helper(tator_api, project, boxes, chunk_size=100)
+
+    # Huge chunk_size
+    print("using huge chunk size (1000)")
+    helper(tator_api, project, boxes, chunk_size=1000)
+
+    # Give bad func to force a failure to create
+    with pytest.raises(RuntimeError) as exc:
+        for _ in tator.util.chunked_create(lambda _: True, project, body=boxes):
+            pass
+
+    n_boxes = len(boxes)
+    assert str(exc.value) == f"Was not able to create {n_boxes} of {n_boxes} objects"
 
     tator_api.delete_media(image)
```

### Comparing `tator-1.0.5/test/test_poly.py` & `tator-1.1.0/test/test_poly.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_search.py` & `tator-1.1.0/test/test_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,19 @@
         'test_string': str(uuid.uuid1()),
         'test_datetime': datetime.datetime.now().isoformat(),
         'test_geopos': [random.uniform(-180.0, 180.0), random.uniform(-90.0, 90.0)],
         'test_float_array': [random.uniform(-1.0, 1.0) for _ in range(3)],
     }
     section = random.choice(['Search Section A', 'Search Section B'])
     path = random.choice(paths)
-    for progress, response in tator.util.upload_media(api, image_type, path,
-                                                      attributes=attributes,
-                                                      section=section):
+    for _, response in tator.util.upload_media(
+        api, image_type, path, attributes=attributes, section=section
+    ):
         pass
-    return response.id, attributes, section
+    return response.id[0], attributes, section
 
 def random_search(sections=None):
     """ Runs a random query and compares results with ES enabled and disabled.
     """
     bool_value = random.choice([True, False])
     int_lower = random.randint(-1000, 0)
     int_upper = random.randint(0, 1000)
```

### Comparing `tator-1.0.5/test/test_state.py` & `tator-1.1.0/test/test_state.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_state_graphic.py` & `tator-1.1.0/test/test_state_graphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_state_type.py` & `tator-1.1.0/test/test_state_type.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_stategraphic.py` & `tator-1.1.0/test/test_stategraphic.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_temporary_file.py` & `tator-1.1.0/test/test_temporary_file.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_tracks.py` & `tator-1.1.0/test/test_tracks.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_transcode.py` & `tator-1.1.0/test/test_transcode.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         "section": section,
         "md5": md5,
     }
 
 
     # Create the media.
     response = tator_api.create_media_list(project=project, body=media_spec)
-    print(f"Transcoding video with existing media ID {response.id}...")
+    print(f"Transcoding video with existing media ID {response.id[0]}...")
     for progress, response in tator.util.upload_media(tator_api, video_type, video_file,
-                                                      media_id=response.id):
+                                                      media_id=response.id[0]):
         print(f"Upload video progress: {progress}%")
     print(response.message)
     print(response.id)
     while True:
         transcode = tator_api.get_transcode(response.id)
         status = transcode.job.status.lower()
         if status == 'succeeded':
@@ -89,20 +89,20 @@
     other_gid = str(uuid1())
     for idx in range(5):
         media_spec['uid'] = str(uuid1())
         if idx > 2:
             # On last two transcodes, change the group ID
             media_spec['gid'] = other_gid
         response = tator_api.create_media_list(project=project, body=[media_spec])
-        media_ids.append(response.id)
-        print(f"Transcoding video with existing media ID {response.id}...")
+        media_ids.append(response.id[0])
+        print(f"Transcoding video with existing media ID {response.id[0]}...")
         for progress, response in tator.util.upload_media(tator_api, video_type, video_file,
                                                           upload_uid=media_spec['uid'],
                                                           upload_gid=media_spec['gid'],
-                                                          media_id=response.id):
+                                                          media_id=response.id[0]):
             print(f"Upload video progress: {progress}%")
         uids.append(response.id)
 
     # Get all transcodes for the two groups
     transcodes1 = tator_api.get_transcode_list(project, gid=upload_gid)
     transcodes2 = tator_api.get_transcode_list(project, gid=other_gid)
     assert(len(transcodes1) + len(transcodes2) == 5)
```

### Comparing `tator-1.0.5/test/test_util_media_manipulation.py` & `tator-1.1.0/test/test_util_media_manipulation.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_util_media_util.py` & `tator-1.1.0/test/test_util_media_util.py`

 * *Files identical despite different names*

### Comparing `tator-1.0.5/test/test_version.py` & `tator-1.1.0/test/test_version.py`

 * *Files identical despite different names*

