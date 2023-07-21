# Comparing `tmp/py_ptsl-101.0.0.tar.gz` & `tmp/py_ptsl-101.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ptsl-101.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_ptsl-101.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_ptsl-101.0.0.tar` & `py_ptsl-101.1.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1498 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/LICENSE
--rw-r--r--   0        0        0     2270 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/README.md
--rw-r--r--   0        0        0    53243 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/PTSL_pb2.py
--rw-r--r--   0        0        0    74192 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/PTSL_pb2.pyi
--rw-r--r--   0        0        0     4008 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/PTSL_pb2_grpc.py
--rw-r--r--   0        0        0     1075 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/__init__.py
--rw-r--r--   0        0        0     3926 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/builders/create_session_builder.py
--rw-r--r--   0        0        0     4277 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/builders/export_text_builder.py
--rw-r--r--   0        0        0     4611 2023-07-20 19:07:05.689377 py_ptsl-101.0.0/ptsl/builders/import_builder.py
--rw-r--r--   0        0        0    11768 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/client.py
--rw-r--r--   0        0        0    25162 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/engine.py
--rw-r--r--   0        0        0     1416 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/errors.py
--rw-r--r--   0        0        0     3654 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/__init__.py
--rw-r--r--   0        0        0       80 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/authorize_connection.py
--rw-r--r--   0        0        0       66 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/clear.py
--rw-r--r--   0        0        0       73 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/clear_special.py
--rw-r--r--   0        0        0       73 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/close_session.py
--rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/consolidate_clip.py
--rw-r--r--   0        0        0       65 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/copy.py
--rw-r--r--   0        0        0       72 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/copy_special.py
--rw-r--r--   0        0        0       87 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/create_fades_based_on_preset.py
--rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/create_session.py
--rw-r--r--   0        0        0       64 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/cut.py
--rw-r--r--   0        0        0       71 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/cut_special.py
--rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_clips_as_files.py
--rw-r--r--   0        0        0       70 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_mix.py
--rw-r--r--   0        0        0       89 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_selected_tracks_as_aaf_omf.py
--rw-r--r--   0        0        0      300 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/export_session_info_as_text.py
--rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/extend_selection_to_target_tracks.py
--rw-r--r--   0        0        0       81 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_dyamic_properties.py
--rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_file_location.py
--rw-r--r--   0        0        0      695 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_playback_mode.py
--rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_ptsl_version.py
--rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_record_mode.py
--rw-r--r--   0        0        0       82 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_audio_format.py
--rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_audio_rate_pull_settings.py
--rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_bit_depth.py
--rw-r--r--   0        0        0       85 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_feet_frames_rate.py
--rw-r--r--   0        0        0      537 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_interleaved_state.py
--rw-r--r--   0        0        0       77 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_length.py
--rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_name.py
--rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_path.py
--rw-r--r--   0        0        0      631 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_sample_rate.py
--rw-r--r--   0        0        0       80 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_start_time.py
--rw-r--r--   0        0        0       83 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_time_code_rate.py
--rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_session_video_rate_pull_settings.py
--rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_task_status.py
--rw-r--r--   0        0        0      774 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_track_list.py
--rw-r--r--   0        0        0       78 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_transport_armed.py
--rw-r--r--   0        0        0       78 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/get_transport_state.py
--rw-r--r--   0        0        0       75 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/host_ready_check.py
--rw-r--r--   0        0        0       69 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/import_command.py
--rw-r--r--   0        0        0      127 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/memory_locations.py
--rw-r--r--   0        0        0       72 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/open_session.py
--rw-r--r--   0        0        0     2771 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/operation.py
--rw-r--r--   0        0        0       66 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/paste.py
--rw-r--r--   0        0        0       73 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/paste_special.py
--rw-r--r--   0        0        0       89 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/refresh_all_modified_audio_files.py
--rw-r--r--   0        0        0       84 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/refresh_target_audio_files.py
--rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/register_connection.py
--rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/rename_selected_clip.py
--rw-r--r--   0        0        0       77 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/rename_target_clip.py
--rw-r--r--   0        0        0       78 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/rename_target_track.py
--rw-r--r--   0        0        0       72 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/save_session.py
--rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/save_session_as.py
--rw-r--r--   0        0        0       82 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/select_all_clips_on_track.py
--rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_playback_mode.py
--rw-r--r--   0        0        0       74 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_record_mode.py
--rw-r--r--   0        0        0       82 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_audio_format.py
--rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_audio_rate_pull_settings.py
--rw-r--r--   0        0        0       79 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_bit_depth.py
--rw-r--r--   0        0        0       85 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_feet_frames_rate.py
--rw-r--r--   0        0        0       87 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_interleaved_state.py
--rw-r--r--   0        0        0       77 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_length.py
--rw-r--r--   0        0        0       80 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_start_time.py
--rw-r--r--   0        0        0       83 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_time_code_rate.py
--rw-r--r--   0        0        0       92 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/set_session_video_rate_pull_settings.py
--rw-r--r--   0        0        0       65 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/spot.py
--rw-r--r--   0        0        0      212 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/toggle_play_state.py
--rw-r--r--   0        0        0       76 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/ops/trim_to_selection.py
--rw-r--r--   0        0        0     4821 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/ptsl/util.py
--rw-r--r--   0        0        0     1759 2023-07-20 19:07:05.693378 py_ptsl-101.0.0/pyproject.toml
--rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 py_ptsl-101.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/LICENSE
+-rw-r--r--   0        0        0     2270 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/README.md
+-rw-r--r--   0        0        0    53243 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/PTSL_pb2.py
+-rw-r--r--   0        0        0    74192 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/PTSL_pb2.pyi
+-rw-r--r--   0        0        0     4008 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/PTSL_pb2_grpc.py
+-rw-r--r--   0        0        0     1075 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/__init__.py
+-rw-r--r--   0        0        0     3926 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/builders/create_session_builder.py
+-rw-r--r--   0        0        0     4277 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/builders/export_text_builder.py
+-rw-r--r--   0        0        0     4611 2023-07-21 18:35:13.707434 py_ptsl-101.1.0/ptsl/builders/import_builder.py
+-rw-r--r--   0        0        0    11768 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/client.py
+-rw-r--r--   0        0        0    25347 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/engine.py
+-rw-r--r--   0        0        0     1416 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/errors.py
+-rw-r--r--   0        0        0     3654 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/__init__.py
+-rw-r--r--   0        0        0       80 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/authorize_connection.py
+-rw-r--r--   0        0        0       66 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/clear.py
+-rw-r--r--   0        0        0       73 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/clear_special.py
+-rw-r--r--   0        0        0       73 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/close_session.py
+-rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/consolidate_clip.py
+-rw-r--r--   0        0        0       65 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/copy.py
+-rw-r--r--   0        0        0       72 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/copy_special.py
+-rw-r--r--   0        0        0       87 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/create_fades_based_on_preset.py
+-rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/create_session.py
+-rw-r--r--   0        0        0       64 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/cut.py
+-rw-r--r--   0        0        0       71 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/cut_special.py
+-rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_clips_as_files.py
+-rw-r--r--   0        0        0       70 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_mix.py
+-rw-r--r--   0        0        0       89 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_selected_tracks_as_aaf_omf.py
+-rw-r--r--   0        0        0       84 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/export_session_info_as_text.py
+-rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/extend_selection_to_target_tracks.py
+-rw-r--r--   0        0        0       81 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_dyamic_properties.py
+-rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_file_location.py
+-rw-r--r--   0        0        0      695 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_playback_mode.py
+-rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_ptsl_version.py
+-rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_record_mode.py
+-rw-r--r--   0        0        0       82 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_audio_format.py
+-rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_audio_rate_pull_settings.py
+-rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_bit_depth.py
+-rw-r--r--   0        0        0       85 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_feet_frames_rate.py
+-rw-r--r--   0        0        0      537 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_interleaved_state.py
+-rw-r--r--   0        0        0       77 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_length.py
+-rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_name.py
+-rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_path.py
+-rw-r--r--   0        0        0      631 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_sample_rate.py
+-rw-r--r--   0        0        0       80 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_start_time.py
+-rw-r--r--   0        0        0       83 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_time_code_rate.py
+-rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_session_video_rate_pull_settings.py
+-rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_task_status.py
+-rw-r--r--   0        0        0      774 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_track_list.py
+-rw-r--r--   0        0        0       78 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_transport_armed.py
+-rw-r--r--   0        0        0       78 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/get_transport_state.py
+-rw-r--r--   0        0        0       75 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/host_ready_check.py
+-rw-r--r--   0        0        0       69 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/import_command.py
+-rw-r--r--   0        0        0      127 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/memory_locations.py
+-rw-r--r--   0        0        0       72 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/open_session.py
+-rw-r--r--   0        0        0     2771 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/operation.py
+-rw-r--r--   0        0        0       66 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/paste.py
+-rw-r--r--   0        0        0       73 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/paste_special.py
+-rw-r--r--   0        0        0       89 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/refresh_all_modified_audio_files.py
+-rw-r--r--   0        0        0       84 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/refresh_target_audio_files.py
+-rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/register_connection.py
+-rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/rename_selected_clip.py
+-rw-r--r--   0        0        0       77 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/rename_target_clip.py
+-rw-r--r--   0        0        0       78 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/rename_target_track.py
+-rw-r--r--   0        0        0       72 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/save_session.py
+-rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/save_session_as.py
+-rw-r--r--   0        0        0       82 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/select_all_clips_on_track.py
+-rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_playback_mode.py
+-rw-r--r--   0        0        0       74 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_record_mode.py
+-rw-r--r--   0        0        0       82 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_audio_format.py
+-rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_audio_rate_pull_settings.py
+-rw-r--r--   0        0        0       79 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_bit_depth.py
+-rw-r--r--   0        0        0       85 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_feet_frames_rate.py
+-rw-r--r--   0        0        0       87 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_interleaved_state.py
+-rw-r--r--   0        0        0       77 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_length.py
+-rw-r--r--   0        0        0       80 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_start_time.py
+-rw-r--r--   0        0        0       83 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_time_code_rate.py
+-rw-r--r--   0        0        0       92 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/set_session_video_rate_pull_settings.py
+-rw-r--r--   0        0        0       65 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/spot.py
+-rw-r--r--   0        0        0      212 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/toggle_play_state.py
+-rw-r--r--   0        0        0       76 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/ops/trim_to_selection.py
+-rw-r--r--   0        0        0     4821 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/ptsl/util.py
+-rw-r--r--   0        0        0     1759 2023-07-21 18:35:13.711434 py_ptsl-101.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 py_ptsl-101.1.0/PKG-INFO
```

### Comparing `py_ptsl-101.0.0/LICENSE` & `py_ptsl-101.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/README.md` & `py_ptsl-101.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/PTSL_pb2.py` & `py_ptsl-101.1.0/ptsl/PTSL_pb2.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/PTSL_pb2.pyi` & `py_ptsl-101.1.0/ptsl/PTSL_pb2.pyi`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/PTSL_pb2_grpc.py` & `py_ptsl-101.1.0/ptsl/PTSL_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/__init__.py` & `py_ptsl-101.1.0/ptsl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
 """
 
 from .client import Client
 from .engine import Engine, open_engine
 from .errors import CommandError
 
-__version__ = '101.0.0'
+__version__ = '101.1.0'
```

### Comparing `py_ptsl-101.0.0/ptsl/builders/create_session_builder.py` & `py_ptsl-101.1.0/ptsl/builders/create_session_builder.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/builders/export_text_builder.py` & `py_ptsl-101.1.0/ptsl/builders/export_text_builder.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/builders/import_builder.py` & `py_ptsl-101.1.0/ptsl/builders/import_builder.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/client.py` & `py_ptsl-101.1.0/ptsl/client.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/engine.py` & `py_ptsl-101.1.0/ptsl/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     TimeProperties, CL_ClipLocation
 
 
 @contextmanager
 def open_engine(*args, **kwargs):
     """
     Open a ptsl engine. Engine will close with the context.
+    :param company_name: The company name to register.
+    :param application_name: The application name to register.
+    :param certificate_path: A path to a certificate (deprecated).
     """
     engine = Engine(*args, **kwargs)
 
     try:
         yield engine
     finally:
         engine.close()
```

### Comparing `py_ptsl-101.0.0/ptsl/errors.py` & `py_ptsl-101.1.0/ptsl/errors.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/ops/__init__.py` & `py_ptsl-101.1.0/ptsl/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/ops/get_playback_mode.py` & `py_ptsl-101.1.0/ptsl/ops/get_playback_mode.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/ops/get_session_interleaved_state.py` & `py_ptsl-101.1.0/ptsl/ops/get_session_interleaved_state.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/ops/get_session_sample_rate.py` & `py_ptsl-101.1.0/ptsl/ops/get_session_sample_rate.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/ops/get_track_list.py` & `py_ptsl-101.1.0/ptsl/ops/get_track_list.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/ops/operation.py` & `py_ptsl-101.1.0/ptsl/ops/operation.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/ptsl/util.py` & `py_ptsl-101.1.0/ptsl/util.py`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/pyproject.toml` & `py_ptsl-101.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_ptsl-101.0.0/PKG-INFO` & `py_ptsl-101.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ptsl
-Version: 101.0.0
+Version: 101.1.0
 Summary: Native Python PTSL (Pro Tools Scripting Library) RPC interface
 Keywords: pro tools,scripting,grpc,automation,avid
 Author-email: Jamie Hardt <jamiehardt@me.com>
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

