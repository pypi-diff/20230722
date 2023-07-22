# Comparing `tmp/newcalls-0.0.1.tar.gz` & `tmp/newcalls-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "newcalls-0.0.1.tar", last modified: Sat Jul 22 15:42:05 2023, max compression
+gzip compressed data, was "newcalls-0.0.2.tar", last modified: Sat Jul 22 16:02:55 2023, max compression
```

## Comparing `newcalls-0.0.1.tar` & `newcalls-0.0.2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.364314 newcalls-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     7652 2023-07-22 15:41:16.000000 newcalls-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5398 2023-07-22 15:42:05.364314 newcalls-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4520 2023-07-22 15:41:16.000000 newcalls-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.340313 newcalls-0.0.1/newcalls/
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/__version__.py
--rw-r--r--   0 root         (0) root         (0)     8957 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/binding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.344313 newcalls-0.0.1/newcalls/custom_api/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/custom_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3295 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/custom_api/custom_api.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/environment.py
--rw-r--r--   0 root         (0) root         (0)     6961 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3818 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/ffprobe.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/file_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.344313 newcalls-0.0.1/newcalls/handlers/
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/handlers/handlers_holder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.344313 newcalls-0.0.1/newcalls/media_devices/
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/media_devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)      485 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/media_devices/device_info.py
--rw-r--r--   0 root         (0) root         (0)     3149 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/media_devices/media_devices.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/media_devices/screen_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.344313 newcalls-0.0.1/newcalls/methods/
--rw-r--r--   0 root         (0) root         (0)      284 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.344313 newcalls-0.0.1/newcalls/methods/core/
--rw-r--r--   0 root         (0) root         (0)      292 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/core/binding_runner.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/core/join_voice_call.py
--rw-r--r--   0 root         (0) root         (0)      437 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/core/leave_voice_call.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/core/set_video_call_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.348313 newcalls-0.0.1/newcalls/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)      463 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_closed_voice_chat.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_group_call_invite.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_kicked.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_left.py
--rw-r--r--   0 root         (0) root         (0)     1003 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_participants_change.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_raw_update.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/decorators/on_stream_end.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.348313 newcalls-0.0.1/newcalls/methods/groups/
--rw-r--r--   0 root         (0) root         (0)      489 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/active_calls.py
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/calls.py
--rw-r--r--   0 root         (0) root         (0)     2492 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/change_volume_call.py
--rw-r--r--   0 root         (0) root         (0)     1480 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/get_active_call.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/get_call.py
--rw-r--r--   0 root         (0) root         (0)     1584 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/get_participants.py
--rw-r--r--   0 root         (0) root         (0)    11245 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/join_group_call.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/groups/leave_group_call.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.348313 newcalls-0.0.1/newcalls/methods/handlers/
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/handlers/raw_update_handler.py
--rw-r--r--   0 root         (0) root         (0)      725 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/handlers/stream_ended_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.348313 newcalls-0.0.1/newcalls/methods/stream/
--rw-r--r--   0 root         (0) root         (0)      361 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9881 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/change_stream.py
--rw-r--r--   0 root         (0) root         (0)     2593 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/mute_stream.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/pause_stream.py
--rw-r--r--   0 root         (0) root         (0)     2357 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/played_time.py
--rw-r--r--   0 root         (0) root         (0)     2824 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/resume_stream.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/stream/unmute_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.352313 newcalls-0.0.1/newcalls/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/cache_peer.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/get_max_voice_chat.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/is_connected.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/mtproto_handler.py
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/ping.py
--rw-r--r--   0 root         (0) root         (0)      985 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     1095 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/methods/utilities/start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.352313 newcalls-0.0.1/newcalls/mtproto/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/mtproto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/mtproto/bridged_client.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/mtproto/client_cache.py
--rw-r--r--   0 root         (0) root         (0)     5095 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/mtproto/mtproto_client.py
--rw-r--r--   0 root         (0) root         (0)    15884 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/mtproto/newgram_client.py
--rw-r--r--   0 root         (0) root         (0)    14816 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/mtproto/telethon_client.py
--rw-r--r--   0 root         (0) root         (0)     2207 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/newcalls.py
--rw-r--r--   0 root         (0) root         (0)     2728 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/newcalls_session.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/scaffold.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/stream_type.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.356314 newcalls-0.0.1/newcalls/types/
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/browsers.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/cache.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/call_holder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.356314 newcalls-0.0.1/newcalls/types/groups/
--rw-r--r--   0 root         (0) root         (0)      909 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/__init__.py
--rw-r--r--   0 root         (0) root         (0)      161 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/already_joined.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/error_during_join.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/group_call.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/group_call_participant.py
--rw-r--r--   0 root         (0) root         (0)      783 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/joined_group_call_participant.py
--rw-r--r--   0 root         (0) root         (0)      163 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/joined_voice_chat.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/left_group_call_participant.py
--rw-r--r--   0 root         (0) root         (0)      375 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/left_voice_chat.py
--rw-r--r--   0 root         (0) root         (0)      157 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/muted_call.py
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/not_in_group_call.py
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/updated_group_call_participant.py
--rw-r--r--   0 root         (0) root         (0)      161 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/groups/upgrade_needed.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.360314 newcalls-0.0.1/newcalls/types/input_stream/
--rw-r--r--   0 root         (0) root         (0)      930 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/audio_image_piped.py
--rw-r--r--   0 root         (0) root         (0)      438 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/audio_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/audio_piped.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/audio_video_piped.py
--rw-r--r--   0 root         (0) root         (0)     1580 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/capture_audio_device.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/capture_av_desktop.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/capture_av_device_desktop.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/capture_video_desktop.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/input_audio_stream.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/input_stream.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/input_video_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.360314 newcalls-0.0.1/newcalls/types/input_stream/quality/
--rw-r--r--   0 root         (0) root         (0)      459 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/__init__.py
--rw-r--r--   0 root         (0) root         (0)      291 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/high_quality_audio.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/high_quality_video.py
--rw-r--r--   0 root         (0) root         (0)      289 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/low_quality_audio.py
--rw-r--r--   0 root         (0) root         (0)      421 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/low_quality_video.py
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/medium_quality_audio.py
--rw-r--r--   0 root         (0) root         (0)      427 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/quality/medium_quality_video.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/video_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/video_piped.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/input_stream/video_tools.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/list.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/object.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/participant_list.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/py_object.py
--rw-r--r--   0 root         (0) root         (0)      881 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.364314 newcalls-0.0.1/newcalls/types/stream/
--rw-r--r--   0 root         (0) root         (0)      586 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/changed_stream.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/muted_stream.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/paused_stream.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/resumed_stream.py
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/stream_audio_endend.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/stream_deleted.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/stream_time.py
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/stream_video_endend.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/stream/unmuted_stream.py
--rw-r--r--   0 root         (0) root         (0)      360 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/update.py
--rw-r--r--   0 root         (0) root         (0)      769 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/update_solver.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/types/user_agent.py
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-22 15:41:16.000000 newcalls-0.0.1/newcalls/version_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 15:42:05.344313 newcalls-0.0.1/newcalls.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5398 2023-07-22 15:42:05.000000 newcalls-0.0.1/newcalls.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5151 2023-07-22 15:42:05.000000 newcalls-0.0.1/newcalls.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 15:42:05.000000 newcalls-0.0.1/newcalls.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 15:42:05.000000 newcalls-0.0.1/newcalls.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-22 15:42:05.000000 newcalls-0.0.1/newcalls.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-22 15:42:05.000000 newcalls-0.0.1/newcalls.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 15:42:05.364314 newcalls-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4840 2023-07-22 15:41:16.000000 newcalls-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.368260 newcalls-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-07-22 16:02:29.000000 newcalls-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-07-22 16:02:55.368260 newcalls-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4520 2023-07-22 16:02:29.000000 newcalls-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     8957 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/binding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls/custom_api/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/custom_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3295 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/custom_api/custom_api.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/environment.py
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3818 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/ffprobe.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/file_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls/handlers/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/handlers/handlers_holder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls/media_devices/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/media_devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      485 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/media_devices/device_info.py
+-rw-r--r--   0 root         (0) root         (0)     3149 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/media_devices/media_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/media_devices/screen_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls/methods/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls/methods/core/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/core/binding_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/core/join_voice_call.py
+-rw-r--r--   0 root         (0) root         (0)      437 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/core/leave_voice_call.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/core/set_video_call_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.356259 newcalls-0.0.2/newcalls/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)      463 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_closed_voice_chat.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_group_call_invite.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_kicked.py
+-rw-r--r--   0 root         (0) root         (0)      943 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_left.py
+-rw-r--r--   0 root         (0) root         (0)     1003 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_participants_change.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_raw_update.py
+-rw-r--r--   0 root         (0) root         (0)      947 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/decorators/on_stream_end.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.356259 newcalls-0.0.2/newcalls/methods/groups/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/active_calls.py
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/calls.py
+-rw-r--r--   0 root         (0) root         (0)     2492 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/change_volume_call.py
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/get_active_call.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/get_call.py
+-rw-r--r--   0 root         (0) root         (0)     1584 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/get_participants.py
+-rw-r--r--   0 root         (0) root         (0)    11245 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/join_group_call.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/groups/leave_group_call.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.356259 newcalls-0.0.2/newcalls/methods/handlers/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/handlers/raw_update_handler.py
+-rw-r--r--   0 root         (0) root         (0)      725 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/handlers/stream_ended_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.356259 newcalls-0.0.2/newcalls/methods/stream/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9881 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/change_stream.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/mute_stream.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/pause_stream.py
+-rw-r--r--   0 root         (0) root         (0)     2357 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/played_time.py
+-rw-r--r--   0 root         (0) root         (0)     2824 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/resume_stream.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/stream/unmute_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.356259 newcalls-0.0.2/newcalls/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/cache_peer.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/get_max_voice_chat.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/is_connected.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/mtproto_handler.py
+-rw-r--r--   0 root         (0) root         (0)      156 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/ping.py
+-rw-r--r--   0 root         (0) root         (0)      985 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/methods/utilities/start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.360259 newcalls-0.0.2/newcalls/mtproto/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/mtproto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/mtproto/bridged_client.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/mtproto/client_cache.py
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/mtproto/mtproto_client.py
+-rw-r--r--   0 root         (0) root         (0)    15884 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/mtproto/newgram_client.py
+-rw-r--r--   0 root         (0) root         (0)    14816 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/mtproto/telethon_client.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/newcalls.py
+-rw-r--r--   0 root         (0) root         (0)     2728 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/newcalls_session.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/scaffold.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/stream_type.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.360259 newcalls-0.0.2/newcalls/types/
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/browsers.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/call_holder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.360259 newcalls-0.0.2/newcalls/types/groups/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/already_joined.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/error_during_join.py
+-rw-r--r--   0 root         (0) root         (0)      915 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/group_call.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/joined_group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)      163 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/joined_voice_chat.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/left_group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/left_voice_chat.py
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/muted_call.py
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/not_in_group_call.py
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/updated_group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)      161 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/groups/upgrade_needed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.364260 newcalls-0.0.2/newcalls/types/input_stream/
+-rw-r--r--   0 root         (0) root         (0)      930 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/audio_image_piped.py
+-rw-r--r--   0 root         (0) root         (0)      438 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/audio_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/audio_piped.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/audio_video_piped.py
+-rw-r--r--   0 root         (0) root         (0)     1580 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/capture_audio_device.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/capture_av_desktop.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/capture_av_device_desktop.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/capture_video_desktop.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/input_audio_stream.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/input_stream.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/input_video_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.364260 newcalls-0.0.2/newcalls/types/input_stream/quality/
+-rw-r--r--   0 root         (0) root         (0)      459 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/high_quality_audio.py
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/high_quality_video.py
+-rw-r--r--   0 root         (0) root         (0)      289 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/low_quality_audio.py
+-rw-r--r--   0 root         (0) root         (0)      421 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/low_quality_video.py
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/medium_quality_audio.py
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/quality/medium_quality_video.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/video_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/video_piped.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/input_stream/video_tools.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/list.py
+-rw-r--r--   0 root         (0) root         (0)     1842 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/object.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/participant_list.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/py_object.py
+-rw-r--r--   0 root         (0) root         (0)      881 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.364260 newcalls-0.0.2/newcalls/types/stream/
+-rw-r--r--   0 root         (0) root         (0)      586 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/changed_stream.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/muted_stream.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/paused_stream.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/resumed_stream.py
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/stream_audio_endend.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/stream_deleted.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/stream_time.py
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/stream_video_endend.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/stream/unmuted_stream.py
+-rw-r--r--   0 root         (0) root         (0)      360 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/update.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/update_solver.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/types/user_agent.py
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-22 16:02:29.000000 newcalls-0.0.2/newcalls/version_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-22 16:02:55.352259 newcalls-0.0.2/newcalls.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-07-22 16:02:55.000000 newcalls-0.0.2/newcalls.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5151 2023-07-22 16:02:55.000000 newcalls-0.0.2/newcalls.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 16:02:55.000000 newcalls-0.0.2/newcalls.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-22 16:02:55.000000 newcalls-0.0.2/newcalls.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-22 16:02:55.000000 newcalls-0.0.2/newcalls.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-22 16:02:55.000000 newcalls-0.0.2/newcalls.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-22 16:02:55.368260 newcalls-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4840 2023-07-22 16:02:29.000000 newcalls-0.0.2/setup.py
```

### Comparing `newcalls-0.0.1/LICENSE` & `newcalls-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/PKG-INFO` & `newcalls-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcalls
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/jokokendi/newcalls
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: newcalls Version: 0.0.1 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: newcalls Version: 0.0.2 Summary: UNKNOWN Home-page:
 https://github.com/jokokendi/newcalls Author: jokokendi Author-email:
 ajual7832@gmail.com License: LGPL-3.0 Platform: UNKNOWN Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `newcalls-0.0.1/README.md` & `newcalls-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/binding.py` & `newcalls-0.0.2/newcalls/binding.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/custom_api/custom_api.py` & `newcalls-0.0.2/newcalls/custom_api/custom_api.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/environment.py` & `newcalls-0.0.2/newcalls/environment.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/exceptions.py` & `newcalls-0.0.2/newcalls/exceptions.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/ffprobe.py` & `newcalls-0.0.2/newcalls/ffprobe.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/file_manager.py` & `newcalls-0.0.2/newcalls/file_manager.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/handlers/handlers_holder.py` & `newcalls-0.0.2/newcalls/handlers/handlers_holder.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/media_devices/media_devices.py` & `newcalls-0.0.2/newcalls/media_devices/media_devices.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/media_devices/screen_info.py` & `newcalls-0.0.2/newcalls/media_devices/screen_info.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/core/binding_runner.py` & `newcalls-0.0.2/newcalls/methods/core/binding_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 
-from ...NewCalls_session import NewCallsSession
+from ...newcalls_session import NewCallsSession
 from ...scaffold import Scaffold
 
 
 class BindingRunner(Scaffold):
     async def _start_binding(self):
         @self._binding.on_update()
         async def update_handler(data: dict):
```

### Comparing `newcalls-0.0.1/newcalls/methods/core/join_voice_call.py` & `newcalls-0.0.2/newcalls/methods/core/join_voice_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/core/set_video_call_status.py` & `newcalls-0.0.2/newcalls/methods/core/set_video_call_status.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_closed_voice_chat.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_closed_voice_chat.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_group_call_invite.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_group_call_invite.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_kicked.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_kicked.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_left.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_left.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_participants_change.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_participants_change.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_raw_update.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/decorators/on_stream_end.py` & `newcalls-0.0.2/newcalls/methods/decorators/on_stream_end.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/groups/change_volume_call.py` & `newcalls-0.0.2/newcalls/methods/groups/change_volume_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/groups/get_active_call.py` & `newcalls-0.0.2/newcalls/methods/groups/get_active_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/groups/get_call.py` & `newcalls-0.0.2/newcalls/methods/groups/get_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/groups/get_participants.py` & `newcalls-0.0.2/newcalls/methods/groups/get_participants.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/groups/join_group_call.py` & `newcalls-0.0.2/newcalls/methods/groups/join_group_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/groups/leave_group_call.py` & `newcalls-0.0.2/newcalls/methods/groups/leave_group_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/handlers/raw_update_handler.py` & `newcalls-0.0.2/newcalls/methods/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/handlers/stream_ended_handler.py` & `newcalls-0.0.2/newcalls/methods/handlers/stream_ended_handler.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/stream/change_stream.py` & `newcalls-0.0.2/newcalls/methods/stream/change_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/stream/mute_stream.py` & `newcalls-0.0.2/newcalls/methods/stream/mute_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/stream/pause_stream.py` & `newcalls-0.0.2/newcalls/methods/stream/pause_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/stream/played_time.py` & `newcalls-0.0.2/newcalls/methods/stream/played_time.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/stream/resume_stream.py` & `newcalls-0.0.2/newcalls/methods/stream/resume_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/stream/unmute_stream.py` & `newcalls-0.0.2/newcalls/methods/stream/unmute_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/utilities/get_max_voice_chat.py` & `newcalls-0.0.2/newcalls/methods/utilities/get_max_voice_chat.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/utilities/idle.py` & `newcalls-0.0.2/newcalls/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/utilities/mtproto_handler.py` & `newcalls-0.0.2/newcalls/methods/utilities/mtproto_handler.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/utilities/run.py` & `newcalls-0.0.2/newcalls/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/methods/utilities/start.py` & `newcalls-0.0.2/newcalls/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/mtproto/bridged_client.py` & `newcalls-0.0.2/newcalls/mtproto/bridged_client.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/mtproto/client_cache.py` & `newcalls-0.0.2/newcalls/mtproto/client_cache.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/mtproto/mtproto_client.py` & `newcalls-0.0.2/newcalls/mtproto/mtproto_client.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/mtproto/newgram_client.py` & `newcalls-0.0.2/newcalls/mtproto/newgram_client.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/mtproto/telethon_client.py` & `newcalls-0.0.2/newcalls/mtproto/telethon_client.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/newcalls.py` & `newcalls-0.0.2/newcalls/newcalls.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/newcalls_session.py` & `newcalls-0.0.2/newcalls/newcalls_session.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/scaffold.py` & `newcalls-0.0.2/newcalls/scaffold.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/stream_type.py` & `newcalls-0.0.2/newcalls/stream_type.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/sync.py` & `newcalls-0.0.2/newcalls/sync.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/__init__.py` & `newcalls-0.0.2/newcalls/types/__init__.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/browsers.py` & `newcalls-0.0.2/newcalls/types/browsers.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/cache.py` & `newcalls-0.0.2/newcalls/types/cache.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/call_holder.py` & `newcalls-0.0.2/newcalls/types/call_holder.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/groups/__init__.py` & `newcalls-0.0.2/newcalls/types/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/groups/group_call.py` & `newcalls-0.0.2/newcalls/types/groups/group_call.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/groups/group_call_participant.py` & `newcalls-0.0.2/newcalls/types/groups/group_call_participant.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/groups/joined_group_call_participant.py` & `newcalls-0.0.2/newcalls/types/groups/joined_group_call_participant.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/groups/left_group_call_participant.py` & `newcalls-0.0.2/newcalls/types/groups/left_group_call_participant.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/groups/updated_group_call_participant.py` & `newcalls-0.0.2/newcalls/types/groups/updated_group_call_participant.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/__init__.py` & `newcalls-0.0.2/newcalls/types/input_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/audio_image_piped.py` & `newcalls-0.0.2/newcalls/types/input_stream/audio_image_piped.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/audio_piped.py` & `newcalls-0.0.2/newcalls/types/input_stream/audio_piped.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/audio_video_piped.py` & `newcalls-0.0.2/newcalls/types/input_stream/audio_video_piped.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/capture_audio_device.py` & `newcalls-0.0.2/newcalls/types/input_stream/capture_audio_device.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/capture_av_desktop.py` & `newcalls-0.0.2/newcalls/types/input_stream/capture_av_desktop.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/capture_av_device_desktop.py` & `newcalls-0.0.2/newcalls/types/input_stream/capture_av_device_desktop.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/capture_video_desktop.py` & `newcalls-0.0.2/newcalls/types/input_stream/capture_video_desktop.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/input_audio_stream.py` & `newcalls-0.0.2/newcalls/types/input_stream/input_audio_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/input_stream.py` & `newcalls-0.0.2/newcalls/types/input_stream/input_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/input_video_stream.py` & `newcalls-0.0.2/newcalls/types/input_stream/input_video_stream.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/video_parameters.py` & `newcalls-0.0.2/newcalls/types/input_stream/video_parameters.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/video_piped.py` & `newcalls-0.0.2/newcalls/types/input_stream/video_piped.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/input_stream/video_tools.py` & `newcalls-0.0.2/newcalls/types/input_stream/video_tools.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/object.py` & `newcalls-0.0.2/newcalls/types/object.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/participant_list.py` & `newcalls-0.0.2/newcalls/types/participant_list.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/py_object.py` & `newcalls-0.0.2/newcalls/types/py_object.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/session.py` & `newcalls-0.0.2/newcalls/types/session.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/stream/__init__.py` & `newcalls-0.0.2/newcalls/types/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/update_solver.py` & `newcalls-0.0.2/newcalls/types/update_solver.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls/types/user_agent.py` & `newcalls-0.0.2/newcalls/types/user_agent.py`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/newcalls.egg-info/PKG-INFO` & `newcalls-0.0.2/newcalls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newcalls
-Version: 0.0.1
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/jokokendi/newcalls
 Author: jokokendi
 Author-email: ajual7832@gmail.com
 License: LGPL-3.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: newcalls Version: 0.0.1 Summary: UNKNOWN Home-page:
+Metadata-Version: 2.1 Name: newcalls Version: 0.0.2 Summary: UNKNOWN Home-page:
 https://github.com/jokokendi/newcalls Author: jokokendi Author-email:
 ajual7832@gmail.com License: LGPL-3.0 Platform: UNKNOWN Classifier: License ::
 OSI Approved :: GNU Lesser General Public License v3 (LGPLv3) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `newcalls-0.0.1/newcalls.egg-info/SOURCES.txt` & `newcalls-0.0.2/newcalls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newcalls-0.0.1/setup.py` & `newcalls-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
 
 with open(os.path.join(base_path, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='newcalls',
-    version='0.0.1',
+    version='0.0.2',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/jokokendi/newcalls',
     author='jokokendi',
     author_email='ajual7832@gmail.com',
     license='LGPL-3.0',
     license_file='LICENSE',
```

