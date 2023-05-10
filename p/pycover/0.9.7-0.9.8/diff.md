# Comparing `tmp/pycover-0.9.7.tar.gz` & `tmp/pycover-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycover-0.9.7.tar", last modified: Fri Dec 23 20:05:32 2022, max compression
+gzip compressed data, was "pycover-0.9.8.tar", last modified: Wed May 10 07:36:58 2023, max compression
```

## Comparing `pycover-0.9.7.tar` & `pycover-0.9.8.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.447533 pycover-0.9.7/
--rw-rw-rw-   0        0        0     7817 2022-12-23 18:59:54.000000 pycover-0.9.7/LICENSE
--rw-rw-rw-   0        0        0     5489 2022-12-23 20:05:32.446532 pycover-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0     4631 2022-12-23 18:59:54.000000 pycover-0.9.7/README.md
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.135537 pycover-0.9.7/pycover/
--rw-rw-rw-   0        0        0      210 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/__init__.py
--rw-rw-rw-   0        0        0       23 2022-12-23 20:05:09.000000 pycover-0.9.7/pycover/__version__.py
--rw-rw-rw-   0        0        0     9184 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/binding.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.171534 pycover-0.9.7/pycover/custom_api/
--rw-rw-rw-   0        0        0       63 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/custom_api/__init__.py
--rw-rw-rw-   0        0        0     3404 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/custom_api/custom_api.py
--rw-rw-rw-   0        0        0     2283 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/environment.py
--rw-rw-rw-   0        0        0     7145 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/exceptions.py
--rw-rw-rw-   0        0        0     3925 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/ffprobe.py
--rw-rw-rw-   0        0        0     1486 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/file_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.175532 pycover-0.9.7/pycover/handlers/
--rw-rw-rw-   0        0        0       78 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/handlers/__init__.py
--rw-rw-rw-   0        0        0      854 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/handlers/handlers_holder.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.185534 pycover-0.9.7/pycover/media_devices/
--rw-rw-rw-   0        0        0      192 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/media_devices/__init__.py
--rw-rw-rw-   0        0        0      505 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/media_devices/device_info.py
--rw-rw-rw-   0        0        0     3248 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/media_devices/media_devices.py
--rw-rw-rw-   0        0        0     1080 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/media_devices/screen_info.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.187531 pycover-0.9.7/pycover/methods/
--rw-rw-rw-   0        0        0      301 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.201530 pycover-0.9.7/pycover/methods/core/
--rw-rw-rw-   0        0        0      305 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/core/__init__.py
--rw-rw-rw-   0        0        0     1787 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/core/binding_runner.py
--rw-rw-rw-   0        0        0     1381 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/core/join_voice_call.py
--rw-rw-rw-   0        0        0      457 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/core/leave_voice_call.py
--rw-rw-rw-   0        0        0      922 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/core/set_video_call_status.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.221530 pycover-0.9.7/pycover/methods/decorators/
--rw-rw-rw-   0        0        0      482 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/__init__.py
--rw-rw-rw-   0        0        0      980 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_closed_voice_chat.py
--rw-rw-rw-   0        0        0     1026 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_group_call_invite.py
--rw-rw-rw-   0        0        0     1004 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_kicked.py
--rw-rw-rw-   0        0        0      978 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_left.py
--rw-rw-rw-   0        0        0     1039 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_participants_change.py
--rw-rw-rw-   0        0        0      963 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_raw_update.py
--rw-rw-rw-   0        0        0      983 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/decorators/on_stream_end.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.245535 pycover-0.9.7/pycover/methods/groups/
--rw-rw-rw-   0        0        0      510 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/__init__.py
--rw-rw-rw-   0        0        0      159 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/active_calls.py
--rw-rw-rw-   0        0        0      139 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/calls.py
--rw-rw-rw-   0        0        0     2567 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/change_volume_call.py
--rw-rw-rw-   0        0        0     1533 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/get_active_call.py
--rw-rw-rw-   0        0        0     1491 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/get_call.py
--rw-rw-rw-   0        0        0     1638 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/get_participants.py
--rw-rw-rw-   0        0        0    11531 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/join_group_call.py
--rw-rw-rw-   0        0        0     3194 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/groups/leave_group_call.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.252529 pycover-0.9.7/pycover/methods/handlers/
--rw-rw-rw-   0        0        0      187 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/handlers/__init__.py
--rw-rw-rw-   0        0        0     1955 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/handlers/raw_update_handler.py
--rw-rw-rw-   0        0        0      752 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/handlers/stream_ended_handler.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.269531 pycover-0.9.7/pycover/methods/stream/
--rw-rw-rw-   0        0        0      378 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/__init__.py
--rw-rw-rw-   0        0        0    10122 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/change_stream.py
--rw-rw-rw-   0        0        0     2670 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/mute_stream.py
--rw-rw-rw-   0        0        0     2895 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/pause_stream.py
--rw-rw-rw-   0        0        0     2423 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/played_time.py
--rw-rw-rw-   0        0        0     2907 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/resume_stream.py
--rw-rw-rw-   0        0        0     2682 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/stream/unmute_stream.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.292533 pycover-0.9.7/pycover/methods/utilities/
--rw-rw-rw-   0        0        0      386 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/__init__.py
--rw-rw-rw-   0        0        0      152 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/cache_peer.py
--rw-rw-rw-   0        0        0      935 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/get_max_voice_chat.py
--rw-rw-rw-   0        0        0     1863 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/idle.py
--rw-rw-rw-   0        0        0      153 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/is_connected.py
--rw-rw-rw-   0        0        0     3091 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/mtproto_handler.py
--rw-rw-rw-   0        0        0      163 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/ping.py
--rw-rw-rw-   0        0        0     1014 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/run.py
--rw-rw-rw-   0        0        0     1130 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/methods/utilities/start.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.306533 pycover-0.9.7/pycover/mtproto/
--rw-rw-rw-   0        0        0      134 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/mtproto/__init__.py
--rw-rw-rw-   0        0        0     2304 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/mtproto/bridged_client.py
--rw-rw-rw-   0        0        0     6689 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/mtproto/client_cache.py
--rw-rw-rw-   0        0        0    16282 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/mtproto/fipper_client.py
--rw-rw-rw-   0        0        0     5265 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/mtproto/mtproto_client.py
--rw-rw-rw-   0        0        0    15219 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/mtproto/telethon_client.py
--rw-rw-rw-   0        0        0     2277 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/pycover.py
--rw-rw-rw-   0        0        0     2681 2022-12-23 20:05:09.000000 pycover-0.9.7/pycover/pycover_session.py
--rw-rw-rw-   0        0        0     1229 2022-12-23 19:49:08.000000 pycover-0.9.7/pycover/scaffold.py
--rw-rw-rw-   0        0        0     1115 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/stream_type.py
--rw-rw-rw-   0        0        0     2741 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/sync.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.335532 pycover-0.9.7/pycover/types/
--rw-rw-rw-   0        0        0     2723 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/__init__.py
--rw-rw-rw-   0        0        0     9925 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/browsers.py
--rw-rw-rw-   0        0        0     1096 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/cache.py
--rw-rw-rw-   0        0        0     1338 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/call_holder.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.366533 pycover-0.9.7/pycover/types/groups/
--rw-rw-rw-   0        0        0      936 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/__init__.py
--rw-rw-rw-   0        0        0      170 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/already_joined.py
--rw-rw-rw-   0        0        0      395 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/error_during_join.py
--rw-rw-rw-   0        0        0      948 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/group_call.py
--rw-rw-rw-   0        0        0     2128 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/group_call_participant.py
--rw-rw-rw-   0        0        0      808 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/joined_group_call_participant.py
--rw-rw-rw-   0        0        0      172 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/joined_voice_chat.py
--rw-rw-rw-   0        0        0      801 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/left_group_call_participant.py
--rw-rw-rw-   0        0        0      395 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/left_voice_chat.py
--rw-rw-rw-   0        0        0      166 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/muted_call.py
--rw-rw-rw-   0        0        0      171 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/not_in_group_call.py
--rw-rw-rw-   0        0        0      813 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/updated_group_call_participant.py
--rw-rw-rw-   0        0        0      170 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/groups/upgrade_needed.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.402533 pycover-0.9.7/pycover/types/input_stream/
--rw-rw-rw-   0        0        0      959 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/__init__.py
--rw-rw-rw-   0        0        0     3664 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/audio_image_piped.py
--rw-rw-rw-   0        0        0      459 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/audio_parameters.py
--rw-rw-rw-   0        0        0     2257 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/audio_piped.py
--rw-rw-rw-   0        0        0     3273 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/audio_video_piped.py
--rw-rw-rw-   0        0        0     1619 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/capture_audio_device.py
--rw-rw-rw-   0        0        0     2958 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/capture_av_desktop.py
--rw-rw-rw-   0        0        0     2585 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/capture_av_device_desktop.py
--rw-rw-rw-   0        0        0     1738 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/capture_video_desktop.py
--rw-rw-rw-   0        0        0     1059 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/input_audio_stream.py
--rw-rw-rw-   0        0        0     1192 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/input_stream.py
--rw-rw-rw-   0        0        0     1065 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/input_video_stream.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.420531 pycover-0.9.7/pycover/types/input_stream/quality/
--rw-rw-rw-   0        0        0      474 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/__init__.py
--rw-rw-rw-   0        0        0      306 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/high_quality_audio.py
--rw-rw-rw-   0        0        0      446 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/high_quality_video.py
--rw-rw-rw-   0        0        0      304 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/low_quality_audio.py
--rw-rw-rw-   0        0        0      442 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/low_quality_video.py
--rw-rw-rw-   0        0        0      310 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/medium_quality_audio.py
--rw-rw-rw-   0        0        0      448 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/quality/medium_quality_video.py
--rw-rw-rw-   0        0        0      733 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/video_parameters.py
--rw-rw-rw-   0        0        0     2596 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/video_piped.py
--rw-rw-rw-   0        0        0     1969 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/input_stream/video_tools.py
--rw-rw-rw-   0        0        0       89 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/list.py
--rw-rw-rw-   0        0        0     1893 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/object.py
--rw-rw-rw-   0        0        0     1782 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/participant_list.py
--rw-rw-rw-   0        0        0      738 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/py_object.py
--rw-rw-rw-   0        0        0      910 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/session.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.443534 pycover-0.9.7/pycover/types/stream/
--rw-rw-rw-   0        0        0      607 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/__init__.py
--rw-rw-rw-   0        0        0      403 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/changed_stream.py
--rw-rw-rw-   0        0        0      399 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/muted_stream.py
--rw-rw-rw-   0        0        0      401 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/paused_stream.py
--rw-rw-rw-   0        0        0      403 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/resumed_stream.py
--rw-rw-rw-   0        0        0      397 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/stream_audio_endend.py
--rw-rw-rw-   0        0        0      423 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/stream_deleted.py
--rw-rw-rw-   0        0        0      328 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/stream_time.py
--rw-rw-rw-   0        0        0      397 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/stream_video_endend.py
--rw-rw-rw-   0        0        0      403 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/stream/unmuted_stream.py
--rw-rw-rw-   0        0        0      380 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/update.py
--rw-rw-rw-   0        0        0      797 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/update_solver.py
--rw-rw-rw-   0        0        0     1127 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/types/user_agent.py
--rw-rw-rw-   0        0        0      308 2022-12-23 18:59:55.000000 pycover-0.9.7/pycover/version_manager.py
-drwxrwxrwx   0        0        0        0 2022-12-23 20:05:32.166530 pycover-0.9.7/pycover.egg-info/
--rw-rw-rw-   0        0        0     5489 2022-12-23 20:05:31.000000 pycover-0.9.7/pycover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5016 2022-12-23 20:05:31.000000 pycover-0.9.7/pycover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-23 20:05:31.000000 pycover-0.9.7/pycover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-23 19:12:25.000000 pycover-0.9.7/pycover.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2022-12-23 20:05:31.000000 pycover-0.9.7/pycover.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-23 20:05:31.000000 pycover-0.9.7/pycover.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-23 20:05:32.447533 pycover-0.9.7/setup.cfg
--rw-rw-rw-   0        0        0     4999 2022-12-23 20:05:09.000000 pycover-0.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.707234 pycover-0.9.8/
+-rw-rw-rw-   0        0        0     7817 2023-05-10 06:33:42.000000 pycover-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0     5489 2023-05-10 07:36:58.706232 pycover-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4631 2023-05-10 06:33:42.000000 pycover-0.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.658349 pycover-0.9.8/pycover/
+-rw-rw-rw-   0        0        0      210 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-10 07:17:01.000000 pycover-0.9.8/pycover/__version__.py
+-rw-rw-rw-   0        0        0     9184 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/binding.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.734809 pycover-0.9.8/pycover/custom_api/
+-rw-rw-rw-   0        0        0       63 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/custom_api/__init__.py
+-rw-rw-rw-   0        0        0     3404 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/custom_api/custom_api.py
+-rw-rw-rw-   0        0        0     2283 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/environment.py
+-rw-rw-rw-   0        0        0     7145 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/exceptions.py
+-rw-rw-rw-   0        0        0     3925 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/ffprobe.py
+-rw-rw-rw-   0        0        0     1486 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/file_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.759795 pycover-0.9.8/pycover/handlers/
+-rw-rw-rw-   0        0        0       78 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/handlers/__init__.py
+-rw-rw-rw-   0        0        0      854 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/handlers/handlers_holder.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.799770 pycover-0.9.8/pycover/media_devices/
+-rw-rw-rw-   0        0        0      192 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/media_devices/__init__.py
+-rw-rw-rw-   0        0        0      505 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/media_devices/device_info.py
+-rw-rw-rw-   0        0        0     3248 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/media_devices/media_devices.py
+-rw-rw-rw-   0        0        0     1080 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/media_devices/screen_info.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.804767 pycover-0.9.8/pycover/methods/
+-rw-rw-rw-   0        0        0      301 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.868728 pycover-0.9.8/pycover/methods/core/
+-rw-rw-rw-   0        0        0      305 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/core/__init__.py
+-rw-rw-rw-   0        0        0     1787 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/core/binding_runner.py
+-rw-rw-rw-   0        0        0     1381 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/core/join_voice_call.py
+-rw-rw-rw-   0        0        0      457 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/core/leave_voice_call.py
+-rw-rw-rw-   0        0        0      922 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/core/set_video_call_status.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.923694 pycover-0.9.8/pycover/methods/decorators/
+-rw-rw-rw-   0        0        0      482 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/__init__.py
+-rw-rw-rw-   0        0        0      980 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_closed_voice_chat.py
+-rw-rw-rw-   0        0        0     1026 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_group_call_invite.py
+-rw-rw-rw-   0        0        0     1004 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_kicked.py
+-rw-rw-rw-   0        0        0      978 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_left.py
+-rw-rw-rw-   0        0        0     1039 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_participants_change.py
+-rw-rw-rw-   0        0        0      963 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_raw_update.py
+-rw-rw-rw-   0        0        0      983 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/decorators/on_stream_end.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.998649 pycover-0.9.8/pycover/methods/groups/
+-rw-rw-rw-   0        0        0      510 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/active_calls.py
+-rw-rw-rw-   0        0        0      139 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/calls.py
+-rw-rw-rw-   0        0        0     2567 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/change_volume_call.py
+-rw-rw-rw-   0        0        0     1533 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/get_active_call.py
+-rw-rw-rw-   0        0        0     1491 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/get_call.py
+-rw-rw-rw-   0        0        0     1638 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/get_participants.py
+-rw-rw-rw-   0        0        0    11531 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/join_group_call.py
+-rw-rw-rw-   0        0        0     3194 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/groups/leave_group_call.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.025632 pycover-0.9.8/pycover/methods/handlers/
+-rw-rw-rw-   0        0        0      187 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1955 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/handlers/raw_update_handler.py
+-rw-rw-rw-   0        0        0      752 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/handlers/stream_ended_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.091591 pycover-0.9.8/pycover/methods/stream/
+-rw-rw-rw-   0        0        0      378 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/__init__.py
+-rw-rw-rw-   0        0        0    10122 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/change_stream.py
+-rw-rw-rw-   0        0        0     2670 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/mute_stream.py
+-rw-rw-rw-   0        0        0     2895 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/pause_stream.py
+-rw-rw-rw-   0        0        0     2423 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/played_time.py
+-rw-rw-rw-   0        0        0     2907 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/resume_stream.py
+-rw-rw-rw-   0        0        0     2682 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/stream/unmute_stream.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.169544 pycover-0.9.8/pycover/methods/utilities/
+-rw-rw-rw-   0        0        0      386 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/cache_peer.py
+-rw-rw-rw-   0        0        0      935 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/get_max_voice_chat.py
+-rw-rw-rw-   0        0        0     1863 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/idle.py
+-rw-rw-rw-   0        0        0      153 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/is_connected.py
+-rw-rw-rw-   0        0        0     3091 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/mtproto_handler.py
+-rw-rw-rw-   0        0        0      163 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/ping.py
+-rw-rw-rw-   0        0        0     1014 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/run.py
+-rw-rw-rw-   0        0        0     1130 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/methods/utilities/start.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.230505 pycover-0.9.8/pycover/mtproto/
+-rw-rw-rw-   0        0        0      134 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/mtproto/__init__.py
+-rw-rw-rw-   0        0        0     2304 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/mtproto/bridged_client.py
+-rw-rw-rw-   0        0        0     6689 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/mtproto/client_cache.py
+-rw-rw-rw-   0        0        0    16282 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/mtproto/fipper_client.py
+-rw-rw-rw-   0        0        0     5265 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/mtproto/mtproto_client.py
+-rw-rw-rw-   0        0        0    15219 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/mtproto/telethon_client.py
+-rw-rw-rw-   0        0        0     2277 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/pycover.py
+-rw-rw-rw-   0        0        0     2680 2023-05-10 07:17:01.000000 pycover-0.9.8/pycover/pycover_session.py
+-rw-rw-rw-   0        0        0     1229 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/scaffold.py
+-rw-rw-rw-   0        0        0     1115 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/stream_type.py
+-rw-rw-rw-   0        0        0     2741 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/sync.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.325447 pycover-0.9.8/pycover/types/
+-rw-rw-rw-   0        0        0     2723 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/__init__.py
+-rw-rw-rw-   0        0        0     9925 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/browsers.py
+-rw-rw-rw-   0        0        0     1096 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/cache.py
+-rw-rw-rw-   0        0        0     1338 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/call_holder.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.447372 pycover-0.9.8/pycover/types/groups/
+-rw-rw-rw-   0        0        0      936 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/already_joined.py
+-rw-rw-rw-   0        0        0      395 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/error_during_join.py
+-rw-rw-rw-   0        0        0      948 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/group_call.py
+-rw-rw-rw-   0        0        0     2128 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/group_call_participant.py
+-rw-rw-rw-   0        0        0      808 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/joined_group_call_participant.py
+-rw-rw-rw-   0        0        0      172 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/joined_voice_chat.py
+-rw-rw-rw-   0        0        0      801 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/left_group_call_participant.py
+-rw-rw-rw-   0        0        0      395 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/left_voice_chat.py
+-rw-rw-rw-   0        0        0      166 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/muted_call.py
+-rw-rw-rw-   0        0        0      171 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/not_in_group_call.py
+-rw-rw-rw-   0        0        0      813 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/updated_group_call_participant.py
+-rw-rw-rw-   0        0        0      170 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/groups/upgrade_needed.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.563300 pycover-0.9.8/pycover/types/input_stream/
+-rw-rw-rw-   0        0        0      959 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/__init__.py
+-rw-rw-rw-   0        0        0     3664 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/audio_image_piped.py
+-rw-rw-rw-   0        0        0      459 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/audio_parameters.py
+-rw-rw-rw-   0        0        0     2257 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/audio_piped.py
+-rw-rw-rw-   0        0        0     3273 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/audio_video_piped.py
+-rw-rw-rw-   0        0        0     1619 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/capture_audio_device.py
+-rw-rw-rw-   0        0        0     2958 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/capture_av_desktop.py
+-rw-rw-rw-   0        0        0     2585 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/capture_av_device_desktop.py
+-rw-rw-rw-   0        0        0     1738 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/capture_video_desktop.py
+-rw-rw-rw-   0        0        0     1059 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/input_audio_stream.py
+-rw-rw-rw-   0        0        0     1192 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/input_stream.py
+-rw-rw-rw-   0        0        0     1065 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/input_video_stream.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.601278 pycover-0.9.8/pycover/types/input_stream/quality/
+-rw-rw-rw-   0        0        0      474 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/high_quality_audio.py
+-rw-rw-rw-   0        0        0      446 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/high_quality_video.py
+-rw-rw-rw-   0        0        0      304 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/low_quality_audio.py
+-rw-rw-rw-   0        0        0      442 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/low_quality_video.py
+-rw-rw-rw-   0        0        0      310 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/medium_quality_audio.py
+-rw-rw-rw-   0        0        0      448 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/quality/medium_quality_video.py
+-rw-rw-rw-   0        0        0      733 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/video_parameters.py
+-rw-rw-rw-   0        0        0     2596 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/video_piped.py
+-rw-rw-rw-   0        0        0     1969 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/input_stream/video_tools.py
+-rw-rw-rw-   0        0        0       89 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/list.py
+-rw-rw-rw-   0        0        0     1893 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/object.py
+-rw-rw-rw-   0        0        0     1782 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/participant_list.py
+-rw-rw-rw-   0        0        0      738 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/py_object.py
+-rw-rw-rw-   0        0        0      910 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/session.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:58.702235 pycover-0.9.8/pycover/types/stream/
+-rw-rw-rw-   0        0        0      607 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/__init__.py
+-rw-rw-rw-   0        0        0      403 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/changed_stream.py
+-rw-rw-rw-   0        0        0      399 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/muted_stream.py
+-rw-rw-rw-   0        0        0      401 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/paused_stream.py
+-rw-rw-rw-   0        0        0      403 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/resumed_stream.py
+-rw-rw-rw-   0        0        0      397 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/stream_audio_endend.py
+-rw-rw-rw-   0        0        0      423 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/stream_deleted.py
+-rw-rw-rw-   0        0        0      328 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/stream_time.py
+-rw-rw-rw-   0        0        0      397 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/stream_video_endend.py
+-rw-rw-rw-   0        0        0      403 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/stream/unmuted_stream.py
+-rw-rw-rw-   0        0        0      380 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/update.py
+-rw-rw-rw-   0        0        0      797 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/update_solver.py
+-rw-rw-rw-   0        0        0     1127 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/types/user_agent.py
+-rw-rw-rw-   0        0        0      308 2023-05-10 06:33:43.000000 pycover-0.9.8/pycover/version_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-10 07:36:57.715314 pycover-0.9.8/pycover.egg-info/
+-rw-rw-rw-   0        0        0     5489 2023-05-10 07:36:56.000000 pycover-0.9.8/pycover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5016 2023-05-10 07:36:56.000000 pycover-0.9.8/pycover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 07:36:56.000000 pycover-0.9.8/pycover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-10 07:36:56.000000 pycover-0.9.8/pycover.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-05-10 07:36:56.000000 pycover-0.9.8/pycover.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-10 07:36:56.000000 pycover-0.9.8/pycover.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 07:36:58.708232 pycover-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     4999 2023-05-10 07:17:01.000000 pycover-0.9.8/setup.py
```

### Comparing `pycover-0.9.7/LICENSE` & `pycover-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/PKG-INFO` & `pycover-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycover
-Version: 0.9.7
+Version: 0.9.8
 Home-page: https://github.com/AyiinXd/pycover
 Author: AyiinXd
 Author-email: buayadanau4@gmail.com
 License: LGPL-3.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycover Version: 0.9.7 Home-page: https://
+Metadata-Version: 2.1 Name: pycover Version: 0.9.8 Home-page: https://
 github.com/AyiinXd/pycover Author: AyiinXd Author-email: buayadanau4@gmail.com
 License: LGPL-3.0 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pycover-0.9.7/README.md` & `pycover-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/binding.py` & `pycover-0.9.8/pycover/binding.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/custom_api/custom_api.py` & `pycover-0.9.8/pycover/custom_api/custom_api.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/environment.py` & `pycover-0.9.8/pycover/environment.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/exceptions.py` & `pycover-0.9.8/pycover/exceptions.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/ffprobe.py` & `pycover-0.9.8/pycover/ffprobe.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/file_manager.py` & `pycover-0.9.8/pycover/file_manager.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/handlers/handlers_holder.py` & `pycover-0.9.8/pycover/handlers/handlers_holder.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/media_devices/media_devices.py` & `pycover-0.9.8/pycover/media_devices/media_devices.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/media_devices/screen_info.py` & `pycover-0.9.8/pycover/media_devices/screen_info.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/core/binding_runner.py` & `pycover-0.9.8/pycover/methods/core/binding_runner.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/core/join_voice_call.py` & `pycover-0.9.8/pycover/methods/core/join_voice_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/core/set_video_call_status.py` & `pycover-0.9.8/pycover/methods/core/set_video_call_status.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_closed_voice_chat.py` & `pycover-0.9.8/pycover/methods/decorators/on_closed_voice_chat.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_group_call_invite.py` & `pycover-0.9.8/pycover/methods/decorators/on_group_call_invite.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_kicked.py` & `pycover-0.9.8/pycover/methods/decorators/on_kicked.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_left.py` & `pycover-0.9.8/pycover/methods/decorators/on_left.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_participants_change.py` & `pycover-0.9.8/pycover/methods/decorators/on_participants_change.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_raw_update.py` & `pycover-0.9.8/pycover/methods/decorators/on_raw_update.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/decorators/on_stream_end.py` & `pycover-0.9.8/pycover/methods/decorators/on_stream_end.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/groups/change_volume_call.py` & `pycover-0.9.8/pycover/methods/groups/change_volume_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/groups/get_active_call.py` & `pycover-0.9.8/pycover/methods/groups/get_active_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/groups/get_call.py` & `pycover-0.9.8/pycover/methods/groups/get_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/groups/get_participants.py` & `pycover-0.9.8/pycover/methods/groups/get_participants.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/groups/join_group_call.py` & `pycover-0.9.8/pycover/methods/groups/join_group_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/groups/leave_group_call.py` & `pycover-0.9.8/pycover/methods/groups/leave_group_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/handlers/raw_update_handler.py` & `pycover-0.9.8/pycover/methods/handlers/raw_update_handler.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/handlers/stream_ended_handler.py` & `pycover-0.9.8/pycover/methods/handlers/stream_ended_handler.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/stream/change_stream.py` & `pycover-0.9.8/pycover/methods/stream/change_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/stream/mute_stream.py` & `pycover-0.9.8/pycover/methods/stream/mute_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/stream/pause_stream.py` & `pycover-0.9.8/pycover/methods/stream/pause_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/stream/played_time.py` & `pycover-0.9.8/pycover/methods/stream/played_time.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/stream/resume_stream.py` & `pycover-0.9.8/pycover/methods/stream/resume_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/stream/unmute_stream.py` & `pycover-0.9.8/pycover/methods/stream/unmute_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/utilities/get_max_voice_chat.py` & `pycover-0.9.8/pycover/methods/utilities/get_max_voice_chat.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/utilities/idle.py` & `pycover-0.9.8/pycover/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/utilities/mtproto_handler.py` & `pycover-0.9.8/pycover/methods/utilities/mtproto_handler.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/utilities/run.py` & `pycover-0.9.8/pycover/methods/utilities/run.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/methods/utilities/start.py` & `pycover-0.9.8/pycover/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/mtproto/bridged_client.py` & `pycover-0.9.8/pycover/mtproto/bridged_client.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/mtproto/client_cache.py` & `pycover-0.9.8/pycover/mtproto/client_cache.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/mtproto/fipper_client.py` & `pycover-0.9.8/pycover/mtproto/fipper_client.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/mtproto/mtproto_client.py` & `pycover-0.9.8/pycover/mtproto/mtproto_client.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/mtproto/telethon_client.py` & `pycover-0.9.8/pycover/mtproto/telethon_client.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/pycover.py` & `pycover-0.9.8/pycover/pycover.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/pycover_session.py` & `pycover-0.9.8/pycover/pycover_session.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                 f'PyCover v{__version__}, Copyright (C) '
                 f'2021-2022 Laky-64 <https://github.com/Laky-64>\n'
                 'Licensed under the terms of the GNU Lesser '
                 'General Public License v3 or later (LGPLv3+)\n',
             )
             try:
                 remote_stable_ver = await self._remote_version('master')
-                remote_dev_ver = await self._remote_version('dev')
+                remote_dev_ver = await self._remote_version('master')
                 remote_test_ver = remote_stable_ver + '.99'
                 if VersionManager.version_tuple(__version__) > \
                         VersionManager.version_tuple(remote_test_ver):
                     remote_ver = remote_readable_ver = remote_dev_ver
                     my_ver = __version__
                 else:
                     remote_readable_ver = remote_stable_ver
@@ -56,13 +56,13 @@
                 return result_text
             finally:
                 await session.close()
         result = re.findall(
             '__version__ = \'(.*?)\'', (
                 await get_async(
                     f'https://raw.githubusercontent.com/'
-                    f'AyiinXd/pytgcalls/{branch}'
-                    f'/pycover/__version__.py',
+                    f'AyiinXd/reforestation/{branch}'
+                    f'/__version__.py',
                 )
             ),
         )
         return result[0] if len(result) > 0 else __version__
```

### Comparing `pycover-0.9.7/pycover/scaffold.py` & `pycover-0.9.8/pycover/scaffold.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/stream_type.py` & `pycover-0.9.8/pycover/stream_type.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/sync.py` & `pycover-0.9.8/pycover/sync.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/__init__.py` & `pycover-0.9.8/pycover/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/browsers.py` & `pycover-0.9.8/pycover/types/browsers.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/cache.py` & `pycover-0.9.8/pycover/types/cache.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/call_holder.py` & `pycover-0.9.8/pycover/types/call_holder.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/groups/__init__.py` & `pycover-0.9.8/pycover/types/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/groups/group_call.py` & `pycover-0.9.8/pycover/types/groups/group_call.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/groups/group_call_participant.py` & `pycover-0.9.8/pycover/types/groups/group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/groups/joined_group_call_participant.py` & `pycover-0.9.8/pycover/types/groups/joined_group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/groups/left_group_call_participant.py` & `pycover-0.9.8/pycover/types/groups/left_group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/groups/updated_group_call_participant.py` & `pycover-0.9.8/pycover/types/groups/updated_group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/__init__.py` & `pycover-0.9.8/pycover/types/input_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/audio_image_piped.py` & `pycover-0.9.8/pycover/types/input_stream/audio_image_piped.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/audio_piped.py` & `pycover-0.9.8/pycover/types/input_stream/audio_piped.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/audio_video_piped.py` & `pycover-0.9.8/pycover/types/input_stream/audio_video_piped.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/capture_audio_device.py` & `pycover-0.9.8/pycover/types/input_stream/capture_audio_device.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/capture_av_desktop.py` & `pycover-0.9.8/pycover/types/input_stream/capture_av_desktop.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/capture_av_device_desktop.py` & `pycover-0.9.8/pycover/types/input_stream/capture_av_device_desktop.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/capture_video_desktop.py` & `pycover-0.9.8/pycover/types/input_stream/capture_video_desktop.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/input_audio_stream.py` & `pycover-0.9.8/pycover/types/input_stream/input_audio_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/input_stream.py` & `pycover-0.9.8/pycover/types/input_stream/input_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/input_video_stream.py` & `pycover-0.9.8/pycover/types/input_stream/input_video_stream.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/video_parameters.py` & `pycover-0.9.8/pycover/types/input_stream/video_parameters.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/video_piped.py` & `pycover-0.9.8/pycover/types/input_stream/video_piped.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/input_stream/video_tools.py` & `pycover-0.9.8/pycover/types/input_stream/video_tools.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/object.py` & `pycover-0.9.8/pycover/types/object.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/participant_list.py` & `pycover-0.9.8/pycover/types/participant_list.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/py_object.py` & `pycover-0.9.8/pycover/types/py_object.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/session.py` & `pycover-0.9.8/pycover/types/session.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/stream/__init__.py` & `pycover-0.9.8/pycover/types/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/update_solver.py` & `pycover-0.9.8/pycover/types/update_solver.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover/types/user_agent.py` & `pycover-0.9.8/pycover/types/user_agent.py`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/pycover.egg-info/PKG-INFO` & `pycover-0.9.8/pycover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycover
-Version: 0.9.7
+Version: 0.9.8
 Home-page: https://github.com/AyiinXd/pycover
 Author: AyiinXd
 Author-email: buayadanau4@gmail.com
 License: LGPL-3.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycover Version: 0.9.7 Home-page: https://
+Metadata-Version: 2.1 Name: pycover Version: 0.9.8 Home-page: https://
 github.com/AyiinXd/pycover Author: AyiinXd Author-email: buayadanau4@gmail.com
 License: LGPL-3.0 Classifier: License :: OSI Approved :: GNU Lesser General
 Public License v3 (LGPLv3) Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pycover-0.9.7/pycover.egg-info/SOURCES.txt` & `pycover-0.9.8/pycover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycover-0.9.7/setup.py` & `pycover-0.9.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 
 with open(os.path.join(base_path, 'README.md'), encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='pycover',
-    version='0.9.7',
+    version='0.9.8',
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://github.com/AyiinXd/pycover',
     author='AyiinXd',
     author_email='buayadanau4@gmail.com',
     license='LGPL-3.0',
     license_file='LICENSE',
```

