# Comparing `tmp/mido-1.2.9.tar.gz` & `tmp/mido-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mido-1.2.9.tar", last modified: Fri Oct  5 11:10:21 2018, max compression
+gzip compressed data, was "G:\raph\Documents\GitHub\mido-1.3.0\dist\.tmp-kiwmxm4w\mido-1.3.0.tar", last modified: Fri Jul 21 20:10:17 2023, max compression
```

## Comparing `mido-1.2.9.tar` & `mido-1.3.0.tar`

### file list

```diff
@@ -1,146 +1,168 @@
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/tests/
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/tests/midifiles/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4727 2018-10-04 21:07:07.000000 mido-1.2.9/tests/midifiles/test_midifiles.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      483 2018-10-04 21:07:07.000000 mido-1.2.9/tests/midifiles/test_tracks.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1393 2018-10-04 21:07:07.000000 mido-1.2.9/tests/midifiles/test_meta.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      744 2018-10-04 21:07:07.000000 mido-1.2.9/tests/midifiles/test_units.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3348 2018-10-04 21:07:07.000000 mido-1.2.9/tests/test_parser.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/tests/backends/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      264 2018-10-04 21:07:07.000000 mido-1.2.9/tests/backends/test_backend.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      762 2018-10-04 21:07:07.000000 mido-1.2.9/tests/backends/test_rtmidi.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1299 2018-10-04 21:07:07.000000 mido-1.2.9/tests/test_syx.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/tests/messages/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3302 2018-10-04 21:07:07.000000 mido-1.2.9/tests/messages/test_messages.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      685 2018-10-04 21:07:07.000000 mido-1.2.9/tests/messages/test_encode.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      559 2018-10-04 21:07:07.000000 mido-1.2.9/tests/messages/test_checks.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1011 2018-10-04 21:07:07.000000 mido-1.2.9/tests/messages/test_decode.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      754 2018-10-04 21:07:07.000000 mido-1.2.9/tests/messages/test_strings.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      938 2018-10-04 21:07:07.000000 mido-1.2.9/tests/test_frozen.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2168 2018-10-04 21:07:07.000000 mido-1.2.9/tests/test_ports.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1517 2018-10-04 21:07:07.000000 mido-1.2.9/tests/test_tokenizer.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1316 2018-10-04 21:07:07.000000 mido-1.2.9/tests/test_sockets.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      217 2018-10-04 21:07:07.000000 mido-1.2.9/tox.ini
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)     1803 2018-10-04 21:07:07.000000 mido-1.2.9/setup.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/docs/
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/docs/_static/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)       56 2017-10-11 16:19:26.000000 mido-1.2.9/docs/_static/PLACEHOLDER
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     6533 2018-08-21 16:04:41.000000 mido-1.2.9/docs/implementing_ports.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     7355 2018-10-04 21:07:07.000000 mido-1.2.9/docs/ports.rst
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/docs/backends/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1014 2018-08-21 16:04:41.000000 mido-1.2.9/docs/backends/amidi.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3635 2018-08-21 16:04:41.000000 mido-1.2.9/docs/backends/rtmidi.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      497 2018-08-21 16:04:41.000000 mido-1.2.9/docs/backends/rtmidi_python.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      223 2018-08-21 16:04:41.000000 mido-1.2.9/docs/backends/pygame.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2230 2018-08-21 16:04:41.000000 mido-1.2.9/docs/backends/index.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      920 2018-08-21 16:04:41.000000 mido-1.2.9/docs/backends/portmidi.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     7877 2018-08-21 16:03:24.000000 mido-1.2.9/docs/conf.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      239 2018-10-04 21:07:07.000000 mido-1.2.9/docs/acknowledgements.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4094 2018-08-21 16:04:41.000000 mido-1.2.9/docs/messages.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     6118 2018-10-04 21:07:07.000000 mido-1.2.9/docs/roadmap.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3857 2018-08-21 16:04:41.000000 mido-1.2.9/docs/socket_ports.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2962 2018-08-21 16:04:41.000000 mido-1.2.9/docs/about_midi.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      864 2018-10-04 21:07:07.000000 mido-1.2.9/docs/syx.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)    22739 2018-10-05 11:01:06.000000 mido-1.2.9/docs/changes.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1115 2018-08-21 16:03:24.000000 mido-1.2.9/docs/license.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2080 2018-08-21 16:04:41.000000 mido-1.2.9/docs/parsing.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2507 2018-08-21 16:04:41.000000 mido-1.2.9/docs/message_types.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1384 2018-08-21 16:04:41.000000 mido-1.2.9/docs/frozen_messages.rst
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/docs/images/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)    20327 2018-08-21 16:04:41.000000 mido-1.2.9/docs/images/midi_time.svg
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3224 2018-08-21 16:04:41.000000 mido-1.2.9/docs/string_encoding.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2286 2018-10-04 21:07:07.000000 mido-1.2.9/docs/contributing.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     7037 2018-08-21 16:04:41.000000 mido-1.2.9/docs/midi_files.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)       74 2018-08-21 16:03:24.000000 mido-1.2.9/docs/authors.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     9075 2018-10-04 21:07:07.000000 mido-1.2.9/docs/meta_message_types.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     5123 2018-08-21 16:04:41.000000 mido-1.2.9/docs/intro.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1142 2018-08-21 16:04:41.000000 mido-1.2.9/docs/freezing.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1365 2018-08-21 16:03:24.000000 mido-1.2.9/docs/bin.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1824 2018-10-04 21:07:07.000000 mido-1.2.9/docs/index.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1220 2018-08-21 16:03:24.000000 mido-1.2.9/docs/implementing_backends.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1660 2018-08-21 16:03:24.000000 mido-1.2.9/docs/resources.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2345 2018-08-21 16:04:41.000000 mido-1.2.9/docs/lib.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     5092 2017-10-11 16:19:26.000000 mido-1.2.9/docs/make.bat
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      755 2018-08-21 16:04:41.000000 mido-1.2.9/docs/installing.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     5556 2017-10-11 16:19:26.000000 mido-1.2.9/docs/Makefile
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      454 2018-10-04 21:07:07.000000 mido-1.2.9/MANIFEST.in
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1092 2017-10-11 16:19:26.000000 mido-1.2.9/LICENSE
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4827 2018-10-05 11:10:21.000000 mido-1.2.9/PKG-INFO
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3134 2018-10-04 21:07:07.000000 mido-1.2.9/README.rst
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      128 2018-10-05 11:10:21.000000 mido-1.2.9/setup.cfg
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/mido.egg-info/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)        5 2018-10-05 11:10:21.000000 mido-1.2.9/mido.egg-info/top_level.txt
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2918 2018-10-05 11:10:21.000000 mido-1.2.9/mido.egg-info/SOURCES.txt
--rw-rw-r--   0 olemb     (1000) olemb     (1000)        1 2018-10-05 11:10:21.000000 mido-1.2.9/mido.egg-info/dependency_links.txt
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4827 2018-10-05 11:10:21.000000 mido-1.2.9/mido.egg-info/PKG-INFO
--rw-rw-r--   0 olemb     (1000) olemb     (1000)        1 2018-01-15 14:21:07.000000 mido-1.2.9/mido.egg-info/not-zip-safe
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      111 2018-10-05 11:10:21.000000 mido-1.2.9/mido.egg-info/requires.txt
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/bin/
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      857 2017-10-11 16:19:26.000000 mido-1.2.9/bin/mido-connect
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)     2279 2018-08-21 16:04:41.000000 mido-1.2.9/bin/mido-play
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      766 2018-08-21 16:04:41.000000 mido-1.2.9/bin/mido-ports
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      916 2017-10-11 16:19:26.000000 mido-1.2.9/bin/mido-serve
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/extras/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     6845 2018-08-21 16:04:41.000000 mido-1.2.9/extras/hid_joystick.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      279 2018-08-21 16:04:41.000000 mido-1.2.9/extras/README.rst
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/examples/
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/examples/midifiles/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      347 2018-10-04 21:07:07.000000 mido-1.2.9/examples/midifiles/midifile_to_json.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      135 2017-10-11 16:19:26.000000 mido-1.2.9/examples/midifiles/test.sh
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      452 2018-08-21 16:04:41.000000 mido-1.2.9/examples/midifiles/print_midi_file.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      559 2018-10-04 21:07:07.000000 mido-1.2.9/examples/midifiles/create_midi_file.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      520 2018-10-04 21:07:07.000000 mido-1.2.9/examples/midifiles/play_midi_file.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/examples/backends/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      537 2018-10-04 21:07:07.000000 mido-1.2.9/examples/backends/use_printer.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3057 2018-10-04 21:07:07.000000 mido-1.2.9/examples/backends/rtm.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      576 2018-10-04 21:07:07.000000 mido-1.2.9/examples/backends/printer.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      674 2018-10-04 21:07:07.000000 mido-1.2.9/examples/using_rtmidi_directly.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/examples/sockets/
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      500 2017-10-11 16:19:26.000000 mido-1.2.9/examples/sockets/forward_ports.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      900 2017-10-11 16:19:26.000000 mido-1.2.9/examples/sockets/simple_client.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      504 2018-10-04 21:07:07.000000 mido-1.2.9/examples/sockets/simple_server.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      822 2017-10-11 16:19:26.000000 mido-1.2.9/examples/sockets/serve_ports.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/examples/ports/
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      863 2018-10-04 21:07:07.000000 mido-1.2.9/examples/ports/input_filter.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      838 2018-08-21 16:04:41.000000 mido-1.2.9/examples/ports/send.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      849 2018-10-04 21:07:07.000000 mido-1.2.9/examples/ports/queue_port.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      428 2017-10-11 16:19:26.000000 mido-1.2.9/examples/ports/multi_receive.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      518 2018-08-21 16:04:41.000000 mido-1.2.9/examples/ports/receive.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      581 2018-10-04 21:07:07.000000 mido-1.2.9/examples/ports/nonblocking_receive.py
--rwxrwxr-x   0 olemb     (1000) olemb     (1000)      397 2018-10-04 21:07:07.000000 mido-1.2.9/examples/ports/list_ports.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/mido/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2344 2018-10-04 21:07:07.000000 mido-1.2.9/mido/frozen.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/mido/midifiles/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3170 2018-10-04 21:07:07.000000 mido-1.2.9/mido/midifiles/tracks.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1256 2018-08-21 16:04:41.000000 mido-1.2.9/mido/midifiles/units.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)    13653 2018-10-04 21:07:07.000000 mido-1.2.9/mido/midifiles/midifiles.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)    15974 2018-10-04 21:07:07.000000 mido-1.2.9/mido/midifiles/meta.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      211 2018-10-04 21:07:07.000000 mido-1.2.9/mido/midifiles/__init__.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/mido/backends/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     6721 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/backend.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     8893 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/portmidi.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     5330 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/rtmidi.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3705 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/pygame.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4281 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/portmidi_init.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2105 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/_parser_queue.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3860 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/rtmidi_python.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3089 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/amidi.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1351 2018-10-04 21:07:07.000000 mido-1.2.9/mido/backends/rtmidi_utils.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)        0 2018-08-21 16:03:24.000000 mido-1.2.9/mido/backends/__init__.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4496 2018-10-04 21:07:07.000000 mido-1.2.9/mido/sockets.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1629 2018-08-21 16:04:41.000000 mido-1.2.9/mido/syx.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      160 2018-10-05 11:02:19.000000 mido-1.2.9/mido/__about__.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      684 2018-10-04 21:07:07.000000 mido-1.2.9/mido/py2.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)    11809 2018-10-04 21:07:07.000000 mido-1.2.9/mido/ports.py
-drwxrwxr-x   0 olemb     (1000) olemb     (1000)        0 2018-10-05 11:10:21.000000 mido-1.2.9/mido/messages/
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1606 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/strings.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2821 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/decode.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     1700 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/encode.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     3376 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/specs.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     7069 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/messages.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2879 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/checks.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      293 2018-10-04 21:07:07.000000 mido-1.2.9/mido/messages/__init__.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)      503 2018-10-04 21:07:07.000000 mido-1.2.9/mido/version.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2847 2018-10-04 21:07:07.000000 mido-1.2.9/mido/tokenizer.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     2832 2018-10-04 21:07:07.000000 mido-1.2.9/mido/parser.py
--rw-rw-r--   0 olemb     (1000) olemb     (1000)     4310 2018-10-04 21:07:07.000000 mido-1.2.9/mido/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/
+-rw-rw-rw-   0        0        0      222 2023-07-21 20:07:59.000000 mido-1.3.0/.flake8
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/.github/
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0     1065 2023-07-21 20:07:59.000000 mido-1.3.0/.github/workflows/documentation.yml
+-rw-rw-rw-   0        0        0     2718 2023-07-21 20:07:59.000000 mido-1.3.0/.github/workflows/release.yml
+-rw-rw-rw-   0        0        0     3185 2023-07-21 20:07:59.000000 mido-1.3.0/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0      334 2023-07-21 20:07:59.000000 mido-1.3.0/.gitignore
+-rw-rw-rw-   0        0        0      559 2023-07-21 20:07:59.000000 mido-1.3.0/.readthedocs.yaml
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/.reuse/
+-rw-rw-rw-   0        0        0      296 2023-07-21 20:07:59.000000 mido-1.3.0/.reuse/dep5
+-rw-rw-rw-   0        0        0     1078 2023-07-21 20:07:59.000000 mido-1.3.0/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/LICENSES/
+-rw-rw-rw-   0        0        0    17023 2023-07-21 20:07:59.000000 mido-1.3.0/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0        0        0    21305 2023-07-21 20:07:59.000000 mido-1.3.0/LICENSES/CC-BY-SA-3.0.txt
+-rw-rw-rw-   0        0        0     7048 2023-07-21 20:07:59.000000 mido-1.3.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0        0        0     1078 2023-07-21 20:07:59.000000 mido-1.3.0/LICENSES/MIT.txt
+-rw-rw-rw-   0        0        0      708 2023-07-21 20:07:59.000000 mido-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3896 2023-07-21 20:10:17.000000 mido-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2682 2023-07-21 20:07:59.000000 mido-1.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/
+-rw-rw-rw-   0        0        0     5668 2023-07-21 20:07:59.000000 mido-1.3.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/_static/
+-rw-rw-rw-   0        0        0       56 2023-07-21 20:07:59.000000 mido-1.3.0/docs/_static/.gitkeep
+-rw-rw-rw-   0        0        0     2719 2023-07-21 20:07:59.000000 mido-1.3.0/docs/about_midi.rst
+-rw-rw-rw-   0        0        0      368 2023-07-21 20:07:59.000000 mido-1.3.0/docs/acknowledgements.rst
+-rw-rw-rw-   0        0        0     3121 2023-07-21 20:07:59.000000 mido-1.3.0/docs/api.rst
+-rw-rw-rw-   0        0        0      552 2023-07-21 20:07:59.000000 mido-1.3.0/docs/authors.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/backends/
+-rw-rw-rw-   0        0        0     1353 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/amidi.rst
+-rw-rw-rw-   0        0        0     1357 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/custom.rst
+-rw-rw-rw-   0        0        0     3041 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/index.rst
+-rw-rw-rw-   0        0        0     1110 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/portmidi.rst
+-rw-rw-rw-   0        0        0      547 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/pygame.rst
+-rw-rw-rw-   0        0        0     4266 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/rtmidi.rst
+-rw-rw-rw-   0        0        0      742 2023-07-21 20:07:59.000000 mido-1.3.0/docs/backends/rtmidi_python.rst
+-rw-rw-rw-   0        0        0     1736 2023-07-21 20:07:59.000000 mido-1.3.0/docs/binaries.rst
+-rw-rw-rw-   0        0        0    26430 2023-07-21 20:07:59.000000 mido-1.3.0/docs/changes.rst
+-rw-rw-rw-   0        0        0     6069 2023-07-21 20:07:59.000000 mido-1.3.0/docs/code_of_conduct.rst
+-rw-rw-rw-   0        0        0     9319 2023-07-21 20:07:59.000000 mido-1.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0     8523 2023-07-21 20:07:59.000000 mido-1.3.0/docs/contributing.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/files/
+-rw-rw-rw-   0        0        0      160 2023-07-21 20:07:59.000000 mido-1.3.0/docs/files/index.rst
+-rw-rw-rw-   0        0        0     8048 2023-07-21 20:07:59.000000 mido-1.3.0/docs/files/midi.rst
+-rw-rw-rw-   0        0        0     1003 2023-07-21 20:07:59.000000 mido-1.3.0/docs/files/syx.rst
+-rw-rw-rw-   0        0        0     1282 2023-07-21 20:07:59.000000 mido-1.3.0/docs/freezing_exe.rst
+-rw-rw-rw-   0        0        0     2252 2023-07-21 20:07:59.000000 mido-1.3.0/docs/glossary.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/images/
+-rw-rw-rw-   0        0        0    20327 2023-07-21 20:07:59.000000 mido-1.3.0/docs/images/midi_time.svg
+-rw-rw-rw-   0        0        0      108 2023-07-21 20:07:59.000000 mido-1.3.0/docs/images/midi_time.svg.license
+-rw-rw-rw-   0        0        0     2606 2023-07-21 20:07:59.000000 mido-1.3.0/docs/index.rst
+-rw-rw-rw-   0        0        0     1401 2023-07-21 20:07:59.000000 mido-1.3.0/docs/installing.rst
+-rw-rw-rw-   0        0        0     5255 2023-07-21 20:07:59.000000 mido-1.3.0/docs/intro.rst
+-rw-rw-rw-   0        0        0      984 2023-07-21 20:07:59.000000 mido-1.3.0/docs/licenses.rst
+-rwxrwxrwx   0        0        0     5210 2023-07-21 20:07:59.000000 mido-1.3.0/docs/make.bat
+-rw-rw-rw-   0        0        0     2328 2023-07-21 20:07:59.000000 mido-1.3.0/docs/message_types.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/messages/
+-rw-rw-rw-   0        0        0     1418 2023-07-21 20:07:59.000000 mido-1.3.0/docs/messages/frozen.rst
+-rw-rw-rw-   0        0        0     4643 2023-07-21 20:07:59.000000 mido-1.3.0/docs/messages/index.rst
+-rw-rw-rw-   0        0        0     2366 2023-07-21 20:07:59.000000 mido-1.3.0/docs/messages/parsing.rst
+-rw-rw-rw-   0        0        0     3450 2023-07-21 20:07:59.000000 mido-1.3.0/docs/messages/serializing.rst
+-rw-rw-rw-   0        0        0     9229 2023-07-21 20:07:59.000000 mido-1.3.0/docs/meta_message_types.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/ports/
+-rw-rw-rw-   0        0        0     6720 2023-07-21 20:07:59.000000 mido-1.3.0/docs/ports/custom.rst
+-rw-rw-rw-   0        0        0     7718 2023-07-21 20:07:59.000000 mido-1.3.0/docs/ports/index.rst
+-rw-rw-rw-   0        0        0     4318 2023-07-21 20:07:59.000000 mido-1.3.0/docs/ports/socket.rst
+-rw-rw-rw-   0        0        0     1583 2023-07-21 20:07:59.000000 mido-1.3.0/docs/resources.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/docs/shared/
+-rw-rw-rw-   0        0        0      594 2023-07-21 20:07:59.000000 mido-1.3.0/docs/shared/licenses_logos.rst
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/examples/
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/examples/backends/
+-rw-rw-rw-   0        0        0      676 2023-07-21 20:07:59.000000 mido-1.3.0/examples/backends/printer.py
+-rw-rw-rw-   0        0        0     3112 2023-07-21 20:07:59.000000 mido-1.3.0/examples/backends/rtm.py
+-rw-rw-rw-   0        0        0      629 2023-07-21 20:07:59.000000 mido-1.3.0/examples/backends/use_printer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/examples/midifiles/
+-rw-rw-rw-   0        0        0      945 2023-07-21 20:07:59.000000 mido-1.3.0/examples/midifiles/create_midi_file.py
+-rw-rw-rw-   0        0        0      455 2023-07-21 20:07:59.000000 mido-1.3.0/examples/midifiles/midifile_to_json.py
+-rw-rw-rw-   0        0        0      806 2023-07-21 20:07:59.000000 mido-1.3.0/examples/midifiles/play_midi_file.py
+-rw-rw-rw-   0        0        0      547 2023-07-21 20:07:59.000000 mido-1.3.0/examples/midifiles/print_midi_file.py
+-rw-rw-rw-   0        0        0      379 2023-07-21 20:07:59.000000 mido-1.3.0/examples/midifiles/show_midifile.py
+-rw-rw-rw-   0        0        0      243 2023-07-21 20:07:59.000000 mido-1.3.0/examples/midifiles/test.sh
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/examples/ports/
+-rw-rw-rw-   0        0        0      920 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/input_filter.py
+-rw-rw-rw-   0        0        0      461 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/list_ports.py
+-rw-rw-rw-   0        0        0      522 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/multi_receive.py
+-rw-rw-rw-   0        0        0      638 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/nonblocking_receive.py
+-rw-rw-rw-   0        0        0      886 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/queue_port.py
+-rw-rw-rw-   0        0        0      575 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/receive.py
+-rw-rw-rw-   0        0        0      886 2023-07-21 20:07:59.000000 mido-1.3.0/examples/ports/send.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:16.000000 mido-1.3.0/examples/sockets/
+-rw-rw-rw-   0        0        0      604 2023-07-21 20:07:59.000000 mido-1.3.0/examples/sockets/forward_ports.py
+-rw-rw-rw-   0        0        0      926 2023-07-21 20:07:59.000000 mido-1.3.0/examples/sockets/serve_ports.py
+-rw-rw-rw-   0        0        0     1004 2023-07-21 20:07:59.000000 mido-1.3.0/examples/sockets/simple_client.py
+-rw-rw-rw-   0        0        0      608 2023-07-21 20:07:59.000000 mido-1.3.0/examples/sockets/simple_server.py
+-rw-rw-rw-   0        0        0      782 2023-07-21 20:07:59.000000 mido-1.3.0/examples/using_rtmidi_directly.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/extras/
+-rw-rw-rw-   0        0        0      396 2023-07-21 20:07:59.000000 mido-1.3.0/extras/README.rst
+-rw-rw-rw-   0        0        0     6920 2023-07-21 20:07:59.000000 mido-1.3.0/extras/hid_joystick.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/mido/
+-rw-rw-rw-   0        0        0     4226 2023-07-21 20:07:59.000000 mido-1.3.0/mido/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/mido/backends/
+-rw-rw-rw-   0        0        0      107 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/__init__.py
+-rw-rw-rw-   0        0        0     1407 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/_parser_queue.py
+-rw-rw-rw-   0        0        0     3189 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/amidi.py
+-rw-rw-rw-   0        0        0     6775 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/backend.py
+-rw-rw-rw-   0        0        0     8999 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/portmidi.py
+-rw-rw-rw-   0        0        0     4550 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/portmidi_init.py
+-rw-rw-rw-   0        0        0     3753 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/pygame.py
+-rw-rw-rw-   0        0        0     5634 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/rtmidi.py
+-rw-rw-rw-   0        0        0     3853 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/rtmidi_python.py
+-rw-rw-rw-   0        0        0     1459 2023-07-21 20:07:59.000000 mido-1.3.0/mido/backends/rtmidi_utils.py
+-rw-rw-rw-   0        0        0     2403 2023-07-21 20:07:59.000000 mido-1.3.0/mido/frozen.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/mido/messages/
+-rw-rw-rw-   0        0        0      401 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/__init__.py
+-rw-rw-rw-   0        0        0     2924 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/checks.py
+-rw-rw-rw-   0        0        0     2773 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/decode.py
+-rw-rw-rw-   0        0        0     1808 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/encode.py
+-rw-rw-rw-   0        0        0     7893 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/messages.py
+-rw-rw-rw-   0        0        0     3476 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/specs.py
+-rw-rw-rw-   0        0        0     1696 2023-07-21 20:07:59.000000 mido-1.3.0/mido/messages/strings.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/mido/midifiles/
+-rw-rw-rw-   0        0        0      319 2023-07-21 20:07:59.000000 mido-1.3.0/mido/midifiles/__init__.py
+-rw-rw-rw-   0        0        0    16326 2023-07-21 20:07:59.000000 mido-1.3.0/mido/midifiles/meta.py
+-rw-rw-rw-   0        0        0    14898 2023-07-21 20:07:59.000000 mido-1.3.0/mido/midifiles/midifiles.py
+-rw-rw-rw-   0        0        0     3470 2023-07-21 20:07:59.000000 mido-1.3.0/mido/midifiles/tracks.py
+-rw-rw-rw-   0        0        0     1701 2023-07-21 20:07:59.000000 mido-1.3.0/mido/midifiles/units.py
+-rw-rw-rw-   0        0        0     2790 2023-07-21 20:07:59.000000 mido-1.3.0/mido/parser.py
+-rw-rw-rw-   0        0        0    11848 2023-07-21 20:07:59.000000 mido-1.3.0/mido/ports.py
+-rw-rw-rw-   0        0        0     4494 2023-07-21 20:07:59.000000 mido-1.3.0/mido/sockets.py
+-rw-rw-rw-   0        0        0     1604 2023-07-21 20:07:59.000000 mido-1.3.0/mido/syx.py
+-rw-rw-rw-   0        0        0     2885 2023-07-21 20:07:59.000000 mido-1.3.0/mido/tokenizer.py
+-rw-rw-rw-   0        0        0      516 2023-07-21 20:07:59.000000 mido-1.3.0/mido/version.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/mido.egg-info/
+-rw-rw-rw-   0        0        0     3896 2023-07-21 20:10:16.000000 mido-1.3.0/mido.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3332 2023-07-21 20:10:16.000000 mido-1.3.0/mido.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 20:10:16.000000 mido-1.3.0/mido.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      168 2023-07-21 20:10:16.000000 mido-1.3.0/mido.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      547 2023-07-21 20:10:16.000000 mido-1.3.0/mido.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-21 20:10:16.000000 mido-1.3.0/mido.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2930 2023-07-21 20:07:59.000000 mido-1.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/scripts/
+-rw-rw-rw-   0        0        0      107 2023-07-21 20:07:59.000000 mido-1.3.0/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1058 2023-07-21 20:07:59.000000 mido-1.3.0/scripts/mido_connect.py
+-rw-rw-rw-   0        0        0     2280 2023-07-21 20:07:59.000000 mido-1.3.0/scripts/mido_play.py
+-rw-rw-rw-   0        0        0      907 2023-07-21 20:07:59.000000 mido-1.3.0/scripts/mido_ports.py
+-rw-rw-rw-   0        0        0     1113 2023-07-21 20:07:59.000000 mido-1.3.0/scripts/mido_serve.py
+-rw-rw-rw-   0        0        0       42 2023-07-21 20:10:17.000000 mido-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/tests/
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/tests/backends/
+-rw-rw-rw-   0        0        0      372 2023-07-21 20:07:59.000000 mido-1.3.0/tests/backends/test_backend.py
+-rw-rw-rw-   0        0        0      870 2023-07-21 20:07:59.000000 mido-1.3.0/tests/backends/test_rtmidi.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/tests/messages/
+-rw-rw-rw-   0        0        0      459 2023-07-21 20:07:59.000000 mido-1.3.0/tests/messages/test_checks.py
+-rw-rw-rw-   0        0        0     1119 2023-07-21 20:07:59.000000 mido-1.3.0/tests/messages/test_decode.py
+-rw-rw-rw-   0        0        0      793 2023-07-21 20:07:59.000000 mido-1.3.0/tests/messages/test_encode.py
+-rw-rw-rw-   0        0        0     3549 2023-07-21 20:07:59.000000 mido-1.3.0/tests/messages/test_messages.py
+-rw-rw-rw-   0        0        0      678 2023-07-21 20:07:59.000000 mido-1.3.0/tests/messages/test_strings.py
+drwxrwxrwx   0        0        0        0 2023-07-21 20:10:17.000000 mido-1.3.0/tests/midifiles/
+-rw-rw-rw-   0        0        0     2962 2023-07-21 20:07:59.000000 mido-1.3.0/tests/midifiles/test_meta.py
+-rw-rw-rw-   0        0        0     5466 2023-07-21 20:07:59.000000 mido-1.3.0/tests/midifiles/test_midifiles.py
+-rw-rw-rw-   0        0        0      949 2023-07-21 20:07:59.000000 mido-1.3.0/tests/midifiles/test_tracks.py
+-rw-rw-rw-   0        0        0     3603 2023-07-21 20:07:59.000000 mido-1.3.0/tests/midifiles/test_units.py
+-rw-rw-rw-   0        0        0     1716 2023-07-21 20:07:59.000000 mido-1.3.0/tests/test_frozen.py
+-rw-rw-rw-   0        0        0     3419 2023-07-21 20:07:59.000000 mido-1.3.0/tests/test_parser.py
+-rw-rw-rw-   0        0        0     2276 2023-07-21 20:07:59.000000 mido-1.3.0/tests/test_ports.py
+-rw-rw-rw-   0        0        0     1424 2023-07-21 20:07:59.000000 mido-1.3.0/tests/test_sockets.py
+-rw-rw-rw-   0        0        0     1398 2023-07-21 20:07:59.000000 mido-1.3.0/tests/test_syx.py
+-rw-rw-rw-   0        0        0     1638 2023-07-21 20:07:59.000000 mido-1.3.0/tests/test_tokenizer.py
```

### Comparing `mido-1.2.9/tests/midifiles/test_midifiles.py` & `mido-1.3.0/tests/midifiles/test_midifiles.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 import io
 from pytest import raises
 from mido.messages import Message
-from mido.midifiles.midifiles import MidiFile
+from mido.midifiles.midifiles import MidiFile, MidiTrack
 from mido.midifiles.meta import MetaMessage, KeySignatureError
 
 HEADER_ONE_TRACK = """
 4d 54 68 64  # MThd
 00 00 00 06  # Chunk size
       00 01  # Type 1
       00 01  # 1 track
@@ -159,7 +163,23 @@
         MetaMessage('midi_port', port=0),
 
         MetaMessage('sequence_number', number=1),
         MetaMessage('midi_port', port=1),
 
         MetaMessage('end_of_track'),
     ]
+
+
+def test_midifile_repr():
+    midifile = MidiFile(type=1, ticks_per_beat=123, tracks=[
+        MidiTrack([
+            Message('note_on', channel=1, note=2, time=3),
+            Message('note_off', channel=1, note=2, time=3)]),
+        MidiTrack([
+            MetaMessage('sequence_number', number=5),
+            Message('note_on', channel=2, note=6, time=9),
+            Message('note_off', channel=2, note=6, time=9)]),
+    ])
+    midifile_eval = eval(repr(midifile))
+    for track, track_eval in zip(midifile.tracks, midifile_eval.tracks):
+        for m1, m2 in zip(track, track_eval):
+            assert m1 == m2
```

### Comparing `mido-1.2.9/tests/test_parser.py` & `mido-1.3.0/tests/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-from __future__ import print_function
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 import random
+
 from pytest import raises
 
 from mido.messages import Message, specs
 from mido.parser import Parser, parse, parse_all
 
 
 def test_parse():
```

### Comparing `mido-1.2.9/tests/test_syx.py` & `mido-1.3.0/tests/test_syx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,40 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from pytest import raises
 from mido.messages import Message
 from mido.syx import read_syx_file, write_syx_file
 
 
 def test_read(tmpdir):
     path = tmpdir.join("test.syx").strpath
     msg = Message('sysex', data=(1, 2, 3))
 
     with open(path, 'wb') as outfile:
         outfile.write(msg.bin())
 
     assert read_syx_file(path) == [msg]
 
-    with open(path, 'wt') as outfile:
+    with open(path, 'w') as outfile:
         outfile.write(msg.hex())
     assert read_syx_file(path) == [msg]
 
-    with open(path, 'wt') as outfile:
+    with open(path, 'w') as outfile:
         outfile.write('NOT HEX')
 
     with raises(ValueError):
         read_syx_file(path)
 
 
 def test_handle_any_whitespace(tmpdir):
     path = tmpdir.join("test.syx").strpath
 
-    with open(path, 'wt') as outfile:
+    with open(path, 'w') as outfile:
         outfile.write('F0 01 02 \t F7\n   F0 03 04 F7\n')
     assert read_syx_file(path) == [Message('sysex', data=[1, 2]),
                                    Message('sysex', data=[3, 4])]
 
 
 def test_write(tmpdir):
     # p = tmpdir.mkdir("sub").join("hello.txt")
@@ -38,9 +42,9 @@
     msg = Message('sysex', data=(1, 2, 3))
 
     write_syx_file(path, [msg])
     with open(path, 'rb') as infile:
         assert infile.read() == msg.bin()
 
     write_syx_file(path, [msg], plaintext=True)
-    with open(path, 'rt') as infile:
+    with open(path) as infile:
         assert infile.read().strip() == msg.hex()
```

### Comparing `mido-1.2.9/tests/messages/test_messages.py` & `mido-1.3.0/tests/messages/test_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from pytest import raises
-from mido.messages.specs import MIN_PITCHWHEEL, MAX_PITCHWHEEL, MIN_SONGPOS, MAX_SONGPOS
+from mido.messages.specs import MIN_PITCHWHEEL, MAX_PITCHWHEEL, \
+    MIN_SONGPOS, MAX_SONGPOS
 from mido.messages.messages import Message, SysexData
 
 
 def test_msg_time_equality():
     # Since 1.1.18 time is included in comparison.
     assert Message('clock', time=0) == Message('clock', time=0)
     assert Message('clock', time=0) != Message('clock', time=1)
@@ -104,7 +109,13 @@
     assert data == {'type': 'sysex', 'data': [1, 2, 3], 'time': 0}
     assert isinstance(data['data'], list)
 
 
 def test_from_hex_sysex_data_type():
     msg = Message.from_hex('F0 01 02 03 F7')
     assert isinstance(msg.data, SysexData)
+
+
+def test_repr():
+    msg = Message('note_on', channel=1, note=2, time=3)
+    msg_eval = eval(repr(msg))
+    assert msg == msg_eval
```

### Comparing `mido-1.2.9/tests/messages/test_encode.py` & `mido-1.3.0/tests/messages/test_encode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from mido.messages.specs import SPEC_BY_STATUS
 from mido.messages.encode import encode_message
 from mido.messages.decode import decode_message
 
 
 def test_encode_decode_all():
     """Encode and then decode all messages on all channels.
```

### Comparing `mido-1.2.9/tests/messages/test_decode.py` & `mido-1.3.0/tests/messages/test_decode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from pytest import raises
 from mido.messages.decode import decode_message
 
 
 def sysex(data):
     """Make sysex data."""
     return [0xf0] + list(data) + [0xf7]
```

### Comparing `mido-1.2.9/tests/messages/test_strings.py` & `mido-1.3.0/tests/messages/test_strings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,13 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from pytest import raises
+
 from mido.messages import Message
 
 
 def test_decode_sysex():
     assert Message.from_str('sysex data=(1,2,3)').data == (1, 2, 3)
 
 
@@ -12,13 +17,7 @@
 
 
 def test_encode_sysex():
     assert str(Message('sysex', data=())) == 'sysex data=() time=0'
     # This should not have an extra comma.
     assert str(Message('sysex', data=(1,))) == 'sysex data=(1) time=0'
     assert str(Message('sysex', data=(1, 2, 3))) == 'sysex data=(1,2,3) time=0'
-
-
-def test_encode_long_int():
-    # Make sure Python 2 doesn't stick an 'L' at the end of a long
-    # integer.
-    assert 'L' not in str(Message('clock', time=1231421984983298432948))
```

### Comparing `mido-1.2.9/tests/test_ports.py` & `mido-1.3.0/tests/test_ports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 import pytest
 from mido.messages import Message
 from mido.ports import BaseIOPort
 
 
 class TestIOPort:
     class Port(BaseIOPort):
```

### Comparing `mido-1.2.9/tests/test_tokenizer.py` & `mido-1.3.0/tests/test_tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from mido.tokenizer import Tokenizer
 
+
 def tokenize(midi_bytes):
     return list(Tokenizer(midi_bytes))
 
 
 def test_channel_message():
     assert tokenize([0x90, 1, 2]) == [[0x90, 1, 2]]
 
@@ -31,15 +36,15 @@
 
 def test_realtime_inside_sysex():
     """Realtime messages are allowed inside sysex.
 
     The sysex messages should be delivered first.
 
     This is the only case where a message is allowed inside another message.
-    """ 
+    """
     assert tokenize([0xf0, 1, 0xf8, 2, 0xf7]) == [[0xf8], [0xf0, 1, 2, 0xf7]]
     assert tokenize([0xf0, 0xf8, 0xf7]) == [[0xf8], [0xf0, 0xf7]]
 
 
 def test_message_inside_sysex():
     """Non-realtime message inside sysex should reset the parser."""
     assert tokenize([0xf0, 0x90, 1, 2, 0xf7]) == [[0x90, 1, 2]]
@@ -48,8 +53,9 @@
 def test_sysex_inside_sysex():
     """Sysex inside sysex should reset the parser."""
     assert tokenize([0xf0, 1, 0xf0, 2, 0xf7]) == [[0xf0, 2, 0xf7]]
 
 
 def test_stray_data_bytes():
     """Data bytes outside messages should be ignored."""
-    assert tokenize([0, 1, 0x90, 2, 3, 4, 5, 0xf8, 6]) == [[0x90, 2, 3], [0xf8]]
+    assert tokenize([0, 1, 0x90, 2, 3, 4, 5, 0xf8, 6]) == \
+           [[0x90, 2, 3], [0xf8]]
```

### Comparing `mido-1.2.9/tests/test_sockets.py` & `mido-1.3.0/tests/test_sockets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 import pytest
 from mido.sockets import parse_address
 
 
 class TestParseAddress:
     @pytest.mark.parametrize('input_str, expected',
                              [(':8080', ('', 8080)),
```

### Comparing `mido-1.2.9/docs/implementing_ports.rst` & `mido-1.3.0/docs/ports/custom.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-Writing a New Port
-==================
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
+Writing a New or Custom Port
+----------------------------
 
 The Mido port API allows you to write new ports to do practically
 anything.
 
 A new port type can be defined by subclassing one of the base classes
 and overriding one or more methods. Here's an example::
 
@@ -18,15 +22,15 @@
     note_on channel=0 note=0 velocity=64 time=0
 
 ``_send()`` will be called by ``send()``, and is responsible for
 actually sending the message somewhere (or in this case print it out).
 
 
 Overridable Methods
--------------------
+^^^^^^^^^^^^^^^^^^^
 
 There are four overridable methods (all of them default to doing
 nothing)::
 
 ``_open(self, **kwargs)``
 
     Should do whatever is necessary to initialize the port (for
@@ -89,15 +93,15 @@
 about that.
 
 The base classes are ``BaseInput``, ``BaseOutput`` and ``BaseIOPort``
 (which is a subclass of the other two.)
 
 
 Locking
--------
+^^^^^^^
 
 The calls to ``_receive()`` and ``_send()`` will are protected by a
 lock, ``left.lock``. As a result all send and receive will be thread
 safe.
 
 .. note:: If your ``_receive()`` function actually blocks instead of
           letting the parent class handle it ``poll()`` will not
@@ -114,60 +118,59 @@
 
         ...
 
 An example of this is ``mido.backends.rtmidi`` where the callback is
 used to feed an internal queue that ``receive()`` reads from.
 
 
-
 Examples
---------
+^^^^^^^^
 
 An full example of a device port for the imaginary MIDI library
 ``fjopp``::
 
     import fjopp
     from mido.ports import BaseIOPort
 
     # This defines an I/O port.
     class FjoppPort(BaseIOPort):
         def _open(self, **kwargs):
-	    self._device = fjopp.open_device(self.name)
+        self._device = fjopp.open_device(self.name)
 
-	def _close(self):
+    def _close(self):
             self._device.close()
 
         def _send(self, message):
             self.device.write(message.bytes())
 
         def _receive(self, block=True):
             while True:
-	        data = self.device.read()
-	        if data:
-	            self._parser.feed(data)
+            data = self.device.read()
+            if data:
+                self._parser.feed(data)
                 else:
                     return
 
 If ``fjopp`` supports blocking read, you can do this to actually block
 on the device instead of letting ``receive()`` and friends poll and
 wait for you::
 
     def _receive(self, block=True):
         if block:
             # Actually block on the device.
-	    # (``read_blocking()`` will always return some data.)
-	    while not ``self._messages``:
-	        data = self._device.read_blocking()
-		self._parser.feed(data)
+        # (``read_blocking()`` will always return some data.)
+        while not ``self._messages``:
+            data = self._device.read_blocking()
+        self._parser.feed(data)
         else:
-	    # Non-blocking read like above.
+        # Non-blocking read like above.
             while True:
-	        data = self.device.read()
-		if data:
-		     self._parser.feed(data)
+            data = self.device.read()
+        if data:
+             self._parser.feed(data)
 
 This can be used for any kind of port that wants to block on a pipe,
 an socket or another input source. Note that Mido will still use
 polling and waiting when receiving from multiple ports (for example in
 a ``MultiPort``).
 
 If you want separate input and output classes, but the ``_open()`` and
@@ -176,25 +179,25 @@
 
 Sometimes it's useful to know inside the methods whether the port
 supports input or output. The way to do this is to check for the
 methods ```send()`` and ``receive()``, for example::
 
     def _open(self, **kwargs):
         if hasattr(self, 'send'):
-	    # This is an output port.
+        # This is an output port.
 
         if hasattr(self, 'receive'):
             # This is an input port.
 
         if hasattr(self, 'send') and hasattr(self, 'receive'):
             # This is an I/O port.
 
 
 Attributes
-----------
+^^^^^^^^^^
 
 A port has some attributes that can be useful inside your methods.
 
 ``name``
 
     The name of the port. The value is device specific and does not
     have to be unique. It can have any value, but must be a string or
```

### Comparing `mido-1.2.9/docs/ports.rst` & `mido-1.3.0/docs/ports/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Ports
 =====
 
-A Mido port is an object that can send or receive messages (or both).
+A Mido :term:`port` is an *object* that can *send* and/or *receive* messages.
 
-You can open a port by calling one of the open methods, for example::
+You can open a :term:`port` by calling one of the *open methods*, for example::
 
     >>> inport = mido.open_input('SH-201')
     >>> outport = mido.open_output('Integra-7')
 
-Now you can receive messages on the input port and send messages on
-the output port::
+Now you can *receive* messages on the *input port* and *send* messages on
+the *output port*::
 
     >>> msg = inport.receive()
     >>> outport.send(msg)
 
 The message is copied by ``send()``, so you can safely modify your
 original message without causing breakage in other parts of the
 system.
 
 In this case, the ports are device ports, and are connected to some
 sort of (physical or virtual) MIDI device, but a port can be
-anything. For example, you can use a ``MultiPort`` receive messages
+anything. For example, you can use a ``MultiPort`` to receive messages
 from multiple ports as if they were one::
 
     from mido.ports import MultiPort
 
     ...
     multi = MultiPort([inport1, inport2, inport3])
     for msg in multi:
@@ -34,76 +38,77 @@
 example is a socket port, which is a wrapper around a TCP/IP socket.
 
 No matter how the port is implemented internally or what it does, it
 will look and behave like any other Mido port, so all kinds of ports
 can be used interchangeably.
 
 
-.. note:: Sending and receiving messages is thread safe. Opening and
+.. warning:: Sending and receiving messages is thread safe. Opening and
           closing ports and listing port names are not.
 
 
-Common Things
--------------
+Common
+------
 
-How to open a port depends on the port type. Device ports (PortMidi,
+How to open a :term:`port` depends on the port type. Device ports (PortMidi,
 RtMidi and others defined in backends) are opened with the open
 functions, for example::
 
     port = mido.open_output()
 
 Input and I/O ports (which support both input and output) are opened
 with ``open_input()`` and ``open_ioport()`` respectively. If you call
-these without a port name like above, you will get the (system
-specific) default port. You can override this by setting the
+these without a port name like above, you will get the - system
+specific - default port. You can override this by setting the
 ``MIDO_DEFAULT_OUTPUT`` etc. environment variables.
 
-To get a list of available ports, you can do::
+To get a *list* of available ports, you can do::
 
     >>> mido.get_output_names()
     ['SH-201', 'Integra-7']
 
 and then::
 
     >>> port = mido.open_output('Integra-7')
 
-There are corresponding function for input and I/O ports.
+There are corresponding functions for input and I/O ports.
 
-To learn how to open other kinds of ports, see the documentation for
-the port type in question.
+To learn how to open other kinds of ports, see documentation of
+the relevant port type.
 
-The port name is available in ``port.name``.
+The *port name* is available in ``port.name``.
 
-To close a port, call::
+To *close* a port, call::
 
     port.close()
 
 or use the ``with`` statement to have the port closed automatically::
 
     with mido.open_input() as port:
         for message in port:
             do_something_with(message)
 
-You can check if the port is closed with::
+You can check if the *port is closed* with::
 
     if port.closed:
         print("Yup, it's closed.")
 
 If the port is already closed, calling ``close()`` will simply do nothing.
 
 
-Output Ports
-------------
+Output
+------
 
-Output ports basically have only one method::
+Output :term:`ports` basically only have one method::
 
     outport.send(message)
 
-This will send the message immediately. (Well, the port can choose to
-do whatever it wants with the message, but at least it's sent.)
+This will *send* the message immediately. (Well, the port can choose to
+do whatever it wants with the message, but at least it's sent from Mido's
+point of view.)
 
 There are also a couple of utility methods::
 
     outport.reset()
 
 This will send "all notes off" and "reset all controllers" on every
 channel. This is used to reset everything to the default state, for
@@ -125,160 +130,167 @@
     outport.panic()
 
 This will not reset controllers. Unlike ``reset()``, the notes will
 not be turned off gracefully, but will stop immediately with no regard
 to decay time.
 
 
-Input Ports
------------
+Input
+-----
 
-To iterate over incoming messages:::
+To *iterate* over *incoming messages*::
 
     for msg in port:
         print(msg)
 
 This will iterate over messages as they arrive on the port until the
 port closes. (So far only socket ports actually close by
 themselves. This happens if the other end disconnects.)
 
-You can also do non-blocking iteration::
+You can also do *non-blocking iteration*::
 
     for msg in port.iter_pending():
         print(msg)
 
 This will iterate over all messages that have already arrived. It is
 typically used in main loops where you want to do something else while
 you wait for messages::
 
     while True:
         for msg in port.iter_pending():
             print(msg)
 
         do_other_stuff()
 
-In an event based system like a GUI where you don't write the main
-loop you can install a handler that's called periodically. Here's an
+In an *event based system* like a GUI where you don't write the main
+loop you can install a *handler* that's called periodically. Here's an
 example for GTK::
 
     def callback(self):
         for msg in self.inport:
             print(msg)
 
     gobject.timeout_add_seconds(timeout, callback)
 
-To get a bit more control you can receive messages one at a time::
+To get a bit more control you can receive messages *one at a time*::
 
     msg = port.receive()
 
-This will block until a message arrives. To get a message only if one
+This will *block* until a message arrives. To get a message only if one
 is available, you can use `poll()`::
 
     msg = port.poll()
 
-This will return ``None`` if no message is available.
+This will return ``None`` immediately if *no message is available*.
+
+.. deprecated:: 1.2
+
+    There used to be a ``pending()`` method which returned the number of
+    pending messages.
 
-.. note:: There used to be a ``pending()`` method which returned the
-          number of pending messages. It was removed in 1.2.0 for
-          three reasons:
+    It was removed for three reasons:
           
-          * with ``poll()`` and ``iter_pending()`` it is no longer
-            necessary
+    * with ``poll()`` and ``iter_pending()`` it is no longer
+      necessary
 
-          * it was unreliable when multithreading and for some ports
-            it doesn't even make sense
+    * it was unreliable when multithreading and for some ports
+      it doesn't even make sense
 
-          * it made the internal method API confusing. `_send()` sends
-            a message so `_receive()` should receive a message.
+    * it made the internal method API confusing. `_send()` sends
+      a message so `_receive()` should receive a message.
 
 
 Callbacks
 ---------
 
-Instead of reading from the port you can install a callback function
-which will be called for every message that arrives.
+Instead of manually reading from the :term:`port` you can install a
+:term:`callback` function which will be called for every message that arrives.
 
 Here's a simple callback function::
 
     def print_message(message):
         print(message)
 
-To install the callback you can either pass it when you create the
+To *install* the callback you can either pass it when you create the
 port or later by setting the ``callback`` attribute::
 
     port = mido.open_input(callback=print_message)
     port.callback = print_message
     ...
     port.callback = another_function
 
-.. note::
+.. warning::
 
-    Since the callback runs in a different thread you may need to use
+    Since the :term:`callback` runs in a different thread you may need to use
     locks or other synchronization mechanisms to keep your main program and
     the callback from stepping on each other's toes.
 
-Calling ``receive()``, ``__iter__()``, or ``iter_pending()`` on a port
-with a callback will raise an exception::
+Calling ``receive()``, ``__iter__()``, or ``iter_pending()`` on a :term:`port`
+with a :term:`callback` will raise an exception::
 
     ValueError: a callback is set for this port
 
-To clear the callback::
+To *clear* the :term:`callback`::
 
     port.callback = None
 
-This will return the port to normal.
+This will return the :term:`port` to normal.
+
+
+API
+---
 
+.. todo:: Add abstract code to describe these interfaces.
 
-Port API
---------
 
 Common Methods and Attributes
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 ``close()``
 
-Close the port. If the port is already closed this will simply do
-nothing.
+Closes the :term:`port`. If the :term:`port` is already closed this will
+simply do nothing.
+
 
 ``name``
 
-Name of the port or None.
+Name of the port or ``None``.
 
 
 ``closed``
 
-True if the port is closed.
+``True`` if the port is closed.
 
 
 Output Port Methods
 ^^^^^^^^^^^^^^^^^^^
 
 ``send(message)``
 
-Send a message.
+Sends a message.
 
 
 ``reset()``
 
-Sends "all notes off" and "reset all controllers on all channels.
+Sends "all notes off" and "reset all controllers" on all channels.
 
 
 ``panic()``
 
 Sends "all sounds off" on all channels. This will abruptly end all
 sounding notes.
 
 
 Input Port Methods
 ^^^^^^^^^^^^^^^^^^
 
 ``receive(block=True)``
 
-Receive a message. This will block until it returns a message. If
-``block=True`` is passed it will instead return ``None`` if there is
+Receives a message. This will block until it returns a message. If
+``block=False`` is passed it will instead return ``None`` if there is
 no message.
 
 
 ``poll()``
 
 Returns a message, or ``None`` if there are no pending messages.
 
@@ -286,9 +298,14 @@
 ``iter_pending()``
 
 Iterates through pending messages.
 
 
 ``__iter__()``
 
-Iterates through messages as they arrive on the port until the port
-closes.
+Iterates through messages as they arrive on the :term:`port` until the
+:term:`port` closes.
+
+
+.. include:: socket.rst
+
+.. include:: custom.rst
```

### Comparing `mido-1.2.9/docs/backends/rtmidi.rst` & `mido-1.3.0/docs/backends/rtmidi.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,64 @@
+.. SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 RtMidi (Default, Recommended)
 -----------------------------
 
 Name: ``mido.backends.rtmidi``
 
+Resources:
+
+* `python-rtmidi Python Library <https://pypi.org/project/python-rtmidi/>`_
+* `RtMidi C Library <https://www.music.mcgill.ca/~gary/rtmidi/>`_
+
 The RtMidi backend is a thin wrapper around `python-rtmidi
-<https://pypi.python.org/pypi/python-rtmidi/>`_
+<https://pypi.org/project/python-rtmidi/>`_.
 
 
-Features:
+Features
+^^^^^^^^
 
 * callbacks
 
-* true blocking ``receive()`` in Python 3 (using a callback and a
-  queue)
+* true blocking ``receive()`` in Python 3 (using a *callback* and a
+  *queue*)
 
-* virtual ports
+* virtual ports (Except on Microsoft Windows)
 
-* ports can be opened multiple times, each will receive a copy of each message
+* ports can be opened multiple times, each will receive a copy of all messages
 
-* client name can be specified when opening a virtual port
+* a *client name* can be specified when opening a virtual port
 
-* sends but doesn't receive active sensing
+* sends but doesn't receive active sensing (By default)
 
 * port list is always up to date
 
 * all methods but ``close()`` are thread safe
 
 
-Port Names (Linux/ALSA
-^^^^^^^^^^^^^^^^^^^^^^
+Port Names (Linux/ALSA)
+^^^^^^^^^^^^^^^^^^^^^^^
 
 When you're using Linux/ALSA the port names include client name and
 ALSA client and port numbers, for example:
 
 .. code-block:: python
 
     >>> mido.get_output_names()
     ['TiMidity:TiMidity port 0 128:0']
 
-The ALSA client and port numbers ("128:0" in this case) can change
+The ALSA client and port numbers ("``128:0``" in this case) can change
 from session to session, making it hard to hard code port names or use
-them in config files.
+them in configuration files.
 
-To get around this the RtMidi backend allows you to leave out the the
+To get around this the RtMidi backend allows you to leave out the
 port number of port number and client names. These lines will all open
-the port above:
+the same port as above:
 
 .. code-block:: python
 
     mido.open_output('TiMidity port 0')
 
 .. code-block:: python
 
@@ -74,60 +84,71 @@
     >>> port
     <open input 'New Port' (RtMidi/LINUX_ALSA)>
 
 Other applications can now connect to this port. (One oddity is that,
 at least in Linux, RtMidi can't see its own virtual ports, while
 PortMidi can see them.)
 
+.. note::
+
+    Virtual Ports are **not** available under Microsoft Windows. An alternative
+    is to use third party software such as Tobias Erichsen's `loopMIDI
+    <https://www.tobias-erichsen.de/software/loopmidi.html>`_.
+
 
 Client Name
 ^^^^^^^^^^^
 
-You can specify a client name for the port:  (New in 1.2.0.)
+.. versionadded:: 1.2
+
+You can specify a client name for the port:
 
 .. code-block:: python
 
     >>> port = mido.open_input('New Port', client_name='My Client')
 
-This requires python-rtmidi >= 1.0rc1. If ``client_name`` is passed
-the port will be a virtal port.
+This requires ``python-rtmidi >= 1.0rc1``. If ``client_name`` is passed
+the port will be a virtual port.
 
-.. note:: Unfortunately, at least with ALSA, opening two ports with
-          the same ``client_name`` creates two clients with the same
-          name instead of one client with two ports.
+.. note::
+
+    Unfortunately, at least with ALSA, opening two ports with the same
+    ``client_name`` creates two clients with the same name instead of one
+    client with two ports.
 
 There are a couple of problems with port names in Linux. First, RtMidi
 can't see some software ports such as ``amSynth MIDI IN``. PortMidi
 uses the same ALSA sequencer API, so this is problem in RtMidi.
 
 Second, in some versions of RtMidi ports are named inconsistently. For
-example, the input port 'Midi Through 14:0' has a corresponding output
-named 'Midi Through:0'. Unless this was intended, it is a bug in
+example, the input port '``Midi Through 14:0``' has a corresponding output
+named '``Midi Through:0``'. Unless this was intended, it is a bug in
 RtMidi's ALSA implementation.
 
 
-Choosing API
-^^^^^^^^^^^^
+Choosing an API
+^^^^^^^^^^^^^^^
+
+The RtMidi library can be compiled with support for more than one API.
 
-The RtMidi library can be compiled with support for more than one
-API. You can select API by adding it after the module name, either in
+To get a list of all available APIs at runtime::
+
+    >>> mido.backend.module.get_api_names()
+    ['LINUX_ALSA', 'UNIX_JACK']
+
+You can select the API by adding it after the module name, either in
 the environment variable::
 
     $ export MIDO_BACKEND=mido.backends.rtmidi/LINUX_ALSA
     $ export MIDO_BACKEND=mido.backends.rtmidi/UNIX_JACK
 
-or in one of these::
+or within the program using one of these::
 
     >>> mido.set_backend('mido.backends.rtmidi/LINUX_ALSA')
     >>> mido.backend
     <backend mido.backends.rtmidi/LINUX_ALSA (not loaded)>
 
     >>> mido.Backend('mido.backends.rtmidi/UNIX_JACK')
     <backend mido.backends.rtmidi/UNIX_JACK (not loaded)>
 
 This allows you to, for example, use both ALSA and JACK ports in the
 same program.
-
-To get a list of available APIs::
-
-    >>> mido.backend.module.get_api_names()
-    ['LINUX_ALSA', 'UNIX_JACK']
```

### Comparing `mido-1.2.9/docs/backends/index.rst` & `mido-1.3.0/docs/backends/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,60 @@
+.. SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Backends
 ========
 
-.. toctree::
-   :maxdepth: 1
+A backend provides the interface between Mido and the operating system level
+MIDI stack.
 
-   rtmidi
-   portmidi
-   pygame
-   rtmidi_python
-   amidi
+Some Mido features are only available with select backends.
 
+Mido's backend subsystem has been designed to be extensible so you can add
+your own backends if required. See :doc:`custom`.
+
+Providing platform specific Python-native backends is currently evaluated.
+See: https://github.com/mido/mido/issues/506
+
+.. todo:: Insert a stack diagram to clear things up.
 
-Choosing a Backend
-------------------
+
+Choice
+------
 
 Mido comes with five backends:
 
-* :doc:`RtMidi <rtmidi>` is the recommended backends. It has all the
-  features of the other ones and more and is usually easier to
-  install.
-
-* :doc:`PortMidi <portmidi>` was the default backend up until 1.2. It
-  uses the ``portmidi`` shared library and can be difficult to install
-  on some systems.
+* :doc:`RtMidi <rtmidi>` is the *default* and *recommended* backend. It has all
+  the features of the other ones and more plus it is usually easier to install.
+
+* :doc:`PortMidi <portmidi>` was the default backend up until version 1.2. It
+  uses the ``portmidi`` shared library and can be difficult to install on some
+  systems.
 
-* :doc:`Pygame <pygame>` uses the ``pygame.midi``.
+* :doc:`Pygame <pygame>` uses the ``pygame.midi`` module.
 
 * :doc:`rtmidi-python <rtmidi_python>` uses the ``rtmidi_python`` package, an
   alternative wrapper for PortMidi. It is currently very basic but
   easier to install on some Windows systems.
 
 * :doc:`Amidi <amidi>` is an experimental backend for Linux/ALSA
   that uses the command ``amidi`` to send and receive messages.
 
-If you want to use another than the RtMidi you can override this with
-the ``MIDO_BACKEND`` environment variable, for example::
-
-    $ MIDO_BACKEND=mido.backends.portmidi ./program.py
+You can set the backend using an environment variable: See :ref:`env_vars`.
 
 Alternatively, you can set the backend from within your program::
 
     >>> mido.set_backend('mido.backends.portmidi')
     >>> mido.backend
     <backend mido.backends.portmidi (not loaded)>
 
-This will override the environment variable.
+.. note::
+
+    This will override the environment variable.
 
 If you want to use more than one backend at a time, you can do::
 
     rtmidi = mido.Backend('mido.backends.rtmidi')
     portmidi = mido.Backend('mido.backends.portmidi')
 
     input = rtmidi.open_input()
@@ -56,30 +62,59 @@
     for message in input:
         output.send(message)
 
 The backend will not be loaded until you call one of the ``open_`` or
 ``get_`` methods. You can pass ``load=True`` to have it loaded right
 away.
 
-If you pass ``use_environ=True`` the module will use the environment
+If you pass ``use_environ=True``, the module will use the environment
 variables ``MIDO_DEFAULT_INPUT`` etc. for default ports.
 
 
+.. _env_vars:
+
 Environment Variables
 ---------------------
 
+
+Select Backend
+^^^^^^^^^^^^^^
+
+If you want to use a backend other than RtMidi you can override this with
+the ``MIDO_BACKEND`` environment variable, for example::
+
+    $ MIDO_BACKEND=mido.backends.portmidi ./program.py
+
+
+Set Default ports
+^^^^^^^^^^^^^^^^^
+
 You can override the backend's choice of default ports with these
 three environment variables::
 
     MIDO_DEFAULT_INPUT
     MIDO_DEFAULT_OUTPUT
     MIDO_DEFAULT_IOPORT
 
 For example::
 
-    $ MIDO_DEFAULT_INPUT='SH-201' python program.py
+    $ MIDO_DEFAULT_INPUT='SH-201' python3 program.py
 
 or::
 
     $ export MIDO_DEFAULT_OUTPUT='Integra-7'
-    $ python program1.py
-    $ python program2.py
+    $ python3 program1.py
+    $ python3 program2.py
+
+
+Available Backends
+------------------
+
+.. toctree::
+
+   rtmidi
+   portmidi
+   pygame
+   rtmidi_python
+   amidi
+
+.. include:: custom.rst
```

### Comparing `mido-1.2.9/docs/backends/portmidi.rst` & `mido-1.3.0/docs/backends/portmidi.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,50 @@
+.. SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 PortMidi
 --------
 
 Name: ``mido.backends.portmidi``
 
+Resources:
+
+* `PortMidi C Library <https://github.com/PortMidi/portmidi>`_
+
 
 Installing
 ^^^^^^^^^^
 
 The PortMidi backend requires the ``portmidi`` shared library.
 
 `Ubuntu <https://www.ubuntu.com/>`_::
 
     apt install libportmidi-dev
 
-`Homebrew <http://mxcl.github.io/homebrew/>`_::
+`Homebrew <https://mxcl.dev/homebrew/>`_::
 
     brew install portmidi
 
-`MacPorts <http://www.macports.org/>`_::
+`MacPorts <https://www.macports.org/>`_::
 
     port install portmidi
 
 The backend will look for::
 
     portmidi.so      (Linux)
-    portmidi.dll     (Windows)
     portmidi.dynlib  (macOS)
+    portmidi.dll     (Windows)
 
 
 Features
 ^^^^^^^^
 
-Can send but doesn't receive ``active_sensing`` messages.
+* Can send but doesn't receive ``active_sensing`` messages.
 
-PortMidi has no callback mechanism, so callbacks are implemented in
-Python with threads. Each port with a callback has a dedicated thread
-doing blocking reads from the device.
-
-Due to limitations in PortMidi the port list will not be up-to-date if
-there are any ports open. (The refresh is implemented by
-re-initalizing PortMidi which would break any open ports.)
+* No callback mechanism so callbacks are implemented in
+  Python with threads. Each port with a callback has a dedicated thread
+  doing blocking reads from the device.
+
+* Due to limitations in PortMidi the port list will not be up-to-date if
+  there are any ports open. (The refresh is implemented by
+  re-initializing PortMidi which would break any open ports.)
```

### Comparing `mido-1.2.9/docs/conf.py` & `mido-1.3.0/docs/conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,244 +1,303 @@
-# -*- coding: utf-8 -*-
+#
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: CC0-1.0
 #
 # Mido documentation build configuration file, created by
 # sphinx-quickstart on Wed Jun 26 16:58:08 2013.
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys, os
+import os
+import sys
+
+try:
+    # Python 3.8+
+    import importlib.metadata as importlib_metadata
+except ImportError:
+    # <Python 3.7 and lower
+    import importlib_metadata
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
-import mido
-from mido import __version__
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
-#needs_sphinx = '1.0'
+# needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.doctest', 'sphinx.ext.todo', 'sphinx.ext.coverage', 'sphinx.ext.ifconfig']
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.doctest',
+    'sphinx.ext.todo',
+    'sphinx.ext.coverage',
+    'sphinx.ext.ifconfig',
+    'sphinx.ext.imgconverter',  # To support SVG in LaTeX PDFs
+    'sphinx_rtd_theme',
+]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
-#source_encoding = 'utf-8-sig'
+# source_encoding = 'utf-8-sig'
 
-# The master toctree document.
-master_doc = 'index'
+# The main toctree document.
+root_doc = 'index'
 
 # General information about the project.
-project = u'Mido'
-copyright = u'Ole Martin Bjørndalen'
+project = 'Mido'
+copyright = 'Ole Martin Bjørndalen\nRaphaël Doursenaud'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = __version__
 # The full version, including alpha/beta/rc tags.
-release = __version__
+release = importlib_metadata.version('mido')
+# The short X.Y version.
+version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
-#language = None
+# language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
-#today = ''
+# today = ''
 # Else, today_fmt is used as the format for a strftime call.
-#today_fmt = '%B %d, %Y'
+# today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 exclude_patterns = ['_build']
 
 # The reST default role (used for this markup: `text`) to use for all documents.
-#default_role = None
+# default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
-#add_function_parentheses = True
+# add_function_parentheses = True
 
 # If true, the current module name will be prepended to all description
 # unit titles (such as .. function::).
-#add_module_names = True
+# add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
-#show_authors = False
+# show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
-#modindex_common_prefix = []
+# modindex_common_prefix = []
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'default'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-#html_theme_options = {}
+html_theme_options = {
+    'navigation_depth': 3,
+    'vcs_pageview_mode': 'edit',
+    'style_external_links': True,
+    'prev_next_buttons_location': 'both',
+}
+
+html_context = {
+    'display_github': True,
+    'github_user': 'mido',
+    'github_repo': 'mido',
+    'github_version': 'main',
+    'conf_py_path': '/docs/',
+}
 
 # Add any paths that contain custom themes here, relative to this directory.
-#html_theme_path = []
+# html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
-#html_title = None
+# html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
-#html_short_title = None
+# html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+html_logo = '../logo/mido.svg'
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
-#html_favicon = None
+# html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
-#html_last_updated_fmt = '%b %d, %Y'
+# html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
-#html_use_smartypants = True
+# html_use_smartypants = True
 
 # Custom sidebar templates, maps document names to template names.
-#html_sidebars = {}
+# html_sidebars = {}
 
 # Additional templates that should be rendered to pages, maps page names to
 # template names.
-#html_additional_pages = {}
+# html_additional_pages = {}
 
 # If false, no module index is generated.
-#html_domain_indices = True
+# html_domain_indices = True
 
 # If false, no index is generated.
-#html_use_index = True
+# html_use_index = True
 
 # If true, the index is split into individual pages for each letter.
-#html_split_index = False
+# html_split_index = False
 
 # If true, links to the reST sources are added to the pages.
-#html_show_sourcelink = True
+# html_show_sourcelink = True
 
 # If true, "Created using Sphinx" is shown in the HTML footer. Default is True.
-#html_show_sphinx = True
+# html_show_sphinx = True
 
 # If true, "(C) Copyright ..." is shown in the HTML footer. Default is True.
-#html_show_copyright = True
+# html_show_copyright = True
 
 # If true, an OpenSearch description file will be output, and all pages will
 # contain a <link> tag referring to it.  The value of this option must be the
 # base URL from which the finished HTML is served.
-#html_use_opensearch = ''
+# html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
-#html_file_suffix = None
+# html_file_suffix = None
+
+html_base_url = 'https://mido.readthedocs.org/'
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'Midodoc'
 
-
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-#'papersize': 'letterpaper',
+    # The paper size ('letterpaper' or 'a4paper').
+    'papersize': 'a4paper',
 
-# The font size ('10pt', '11pt' or '12pt').
-#'pointsize': '10pt',
+    # The font size ('10pt', '11pt' or '12pt').
+    'pointsize': '10pt',
 
-# Additional stuff for the LaTeX preamble.
-#'preamble': '',
+    # Additional stuff for the LaTeX preamble.
+    # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'Mido.tex', u'Mido Documentation',
-   u'Ole Martin Bjørndalen', 'manual'),
+    (
+        'index',
+        'Mido.tex',
+        'Mido Documentation',
+        'Ole Martin Bjørndalen, Raphaël Doursenaud',
+        'manual'
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
-#latex_logo = None
+latex_logo = '../logo/mido.png'
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
-#latex_use_parts = False
+latex_use_parts = False
 
 # If true, show page references after internal links.
-#latex_show_pagerefs = False
+latex_show_pagerefs = True
 
 # If true, show URL addresses after external links.
-#latex_show_urls = False
+latex_show_urls = 'true'
 
 # Documents to append as an appendix to all manuals.
-#latex_appendices = []
+# latex_appendices = []
 
 # If false, no module index is generated.
-#latex_domain_indices = True
+# latex_domain_indices = True
 
 
 # -- Options for manual page output --------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'mido', u'Mido Documentation',
-     [u'Ole Martin Bjørndalen'], 1)
+    (
+        'index',
+        'mido',
+        'Mido Documentation',
+        ['Ole Martin Bjørndalen', 'Raphaël Doursenaud'],
+        1
+     )
 ]
 
 # If true, show URL addresses after external links.
-#man_show_urls = False
+# man_show_urls = False
 
 
 # -- Options for Texinfo output ------------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-  ('index', 'Mido', u'Mido Documentation',
-   u'Ole Martin Bjørndalen', 'Mido', 'MIDI Objects for Python',
-   'Miscellaneous'),
+    (
+        'index',
+        'Mido',
+        'Mido Documentation',
+        'Ole Martin Bjørndalen, Raphaël Doursenaud',
+        'Mido',
+        'MIDI Objects for Python',
+        'Miscellaneous'
+    ),
 ]
 
 # Documents to append as an appendix to all manuals.
-#texinfo_appendices = []
+# texinfo_appendices = []
 
 # If false, no module index is generated.
-#texinfo_domain_indices = True
+# texinfo_domain_indices = True
 
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
-#texinfo_show_urls = 'footnote'
+# texinfo_show_urls = 'footnote'
+
+# -- Options for sphinx.ext.todo -----------------------------------------------
+
+todo_include_todos = True
+
+# -- Options for the linkcheck builder -----------------------------------------
+
+linkcheck_ignore = [
+    r'https://wiki.ccarh.org',  # Has aggressive anti-DDoS and will fail often
+    r'https://www.ccarh.org',  # Has aggressive anti-DDoS and will fail often
+    r'https://www.sweetwater.com',  # Issues 403 for robots
+]
```

### Comparing `mido-1.2.9/docs/messages.rst` & `mido-1.3.0/docs/messages/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,30 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Messages
 ========
 
 A Mido message is a Python object with methods and attributes. The
 attributes will vary depending on message type.
 
 To create a new message::
 
     >>> mido.Message('note_on')
-    <message note_on channel=0 note=0 velocity=64 time=0>
+    Message('note_on', channel=0, note=0, velocity=64, time=0)
 
 You can pass attributes as keyword arguments::
 
     >>> mido.Message('note_on', note=100, velocity=3, time=6.2)
-    <message note_on channel=0 note=100 velocity=3 time=6.2>
+    Message('note_on', channel=0, note=100, velocity=3, time=6.2)
 
-All attributes will default to 0. The exceptions are ``velocity``,
-which defaults to 64 (middle velocity) and ``data`` which defaults to
-``()``.
+All attributes will default to ``0``.
+The exceptions are ``velocity``, which defaults to ``64`` (middle velocity)
+and ``data`` which defaults to ``()``.
 
 You can set and get attributes as you would expect::
 
     >>> msg = mido.Message('note_on')
     >>> msg.note
     0
 
@@ -29,78 +33,98 @@
     >>> msg.type
     'note_on'
 
 Attributes are also settable but it's always better to use
 ``msg.copy()``::
 
     >>> msg.copy(note=99, time=100.0)
-    <message note_on channel=0 note=99 velocity=64 time=100.0>
+    Message('note_on', channel=0, note=99, velocity=64, time=100.0)
 
 .. note:: Mido always makes a copy of messages instead of modifying
           them so if you do the same you have immutable messages in
           practice. (Third party libraries may not follow the same
           rule.)
 
-.. note:: :doc:`/frozen_messages` are a variant of messages that are
+.. note:: :doc:`frozen` are a variant of messages that are
           hashable and can be used as dictionary keys. They are also
           safe from tampering by third party libraries. You can freely
           convert between the two and use frozen messages wherever
           normal messages are allowed.
 
-Mido supports all message types defined by the MIDI standard. For a
-full list of messages and their attributes, see :doc:`/message_types`.
+Mido supports all message types defined by the :term:`MIDI` standard. For a
+full list of messages and their attributes, see :doc:`../message_types`.
+
+
+Control Changes
+---------------
+
+.. code-block:: python
+
+    if msg.is_cc():
+        print('Control change message received')
+
+    if msg.is_cc(7):
+        print('Volume changed to', msg.value)
+
 
+Converting To & From Bytes
+--------------------------
 
-Converting To Bytes
--------------------
+To Bytes
+^^^^^^^^
 
-You can convert a message to MIDI bytes with one of these methods:
+You can convert a message to :term:`MIDI` ``bytes`` with one of these methods:
 
     >>> msg = mido.Message('note_on')
     >>> msg
-    <message note_on channel=0 note=0 velocity=64 time=0>
+    Message('note_on', channel=0, note=0, velocity=64, time=0)
     >>> msg.bytes()
     [144, 0, 64]
     >>> msg.bin()
     bytearray(b'\x90\x00@')
     >>> msg.hex()
     '90 00 40'
 
 
-Converting From Bytes
----------------------
+From Bytes
+^^^^^^^^^^
 
-You can turn bytes back into messages with the :doc:`/parser <parsing>`.
+You can turn ``bytes`` back into messages with the :doc:`parser <parsing>`.
 
-You can also create a message from bytes using class methods (new in
-1.2):
+.. versionadded:: 1.2
+
+You can also create a message from ``bytes`` using class methods:
 
 .. code-block:: python
 
    msg1 = mido.Message.from_bytes([0x90, 0x40, 0x60])
    msg2 = mido.Message.from_hex('90, 40 60')
 
-The bytes must contain exactly one complete message. If not
+The ``bytes`` must contain exactly one complete message. If not
 ``ValueError`` is raised.
 
 
 
 The Time Attribute
 ------------------
 
 Each message has a ``time`` attribute, which can be set to any value
-of type ``int`` or ``float`` (and in Python 2 also ``long``). What you
-do with this value is entirely up to you.
+of type ``int`` or ``float``.
+
+Some parts of Mido use the attribute for special purposes. In ``MIDI file``
+tracks, it is used as delta time (in :term:`ticks`), and it must be a
+non-negative integer.
 
-Some parts of Mido use the attribute for special purposes. In MIDI
-file tracks, it is used as delta time (in ticks).
+In other parts of Mido, this value is ignored.
 
-.. note:: Before 1.1.18 the ``time`` attribute was not included in
-          comparisons. If you want the old behavior the easies way is
-          ``msg1.bytes()`` == ``msg2.bytes()``.
+.. versionchanged:: 1.1.18
+
+    In earlier versions, the ``time`` attribute was not included in
+    comparisons. If you want the old behavior the easiest way is
+    ``msg1.bytes() == msg2.bytes()``.
 
 To sort messages on time you can do::
 
     messages.sort(key=lambda message: message.time)
 
 or::
 
@@ -108,41 +132,50 @@
 
     messages.sort(key=operator.attrgetter('time'))
 
 
 System Exclusive Messages
 -------------------------
 
-System Exclusive (SysEx) messages are used to send device specific
-data. The ``data`` attribute is a tuple of data bytes which serves as
+:term:`System Exclusive` (aka :term:`SysEx`) messages are used to send device
+specific data. The ``data`` attribute is a tuple of data bytes which serves as
 the payload of the message::
 
     >>> msg = Message('sysex', data=[1, 2, 3])
     >>> msg
-    <message sysex data=(1, 2, 3) time=0>
+    Message('sysex', data=(1, 2, 3), time=0)
     >>> msg.hex()
     'F0 01 02 03 F7'
 
 You can also extend the existing data::
 
    >>> msg = Message('sysex', data=[1, 2, 3])
    >>> msg.data += [4, 5]
    >>> msg.data += [6, 7, 8]
    >>> msg
-   <message sysex data=(1, 2, 3, 4, 5, 6, 7, 8) time=0>
+   Message('sysex', data=(1, 2, 3, 4, 5, 6, 7, 8), time=0)
+
+Any sequence of integers between `0` and `127` is allowed, and type and range
+checking is applied to each data byte.
 
-Any sequence of integers is allowed, and type and range checking is
-applied to each data byte. These are all valid::
+These are all valid::
 
     (65, 66, 67)
     [65, 66, 67]
     (i + 65 for i in range(3))
     (ord(c) for c in 'ABC')
     bytearray(b'ABC')
     b'ABC'  # Python 3 only.
 
 For example::
 
     >>> msg = Message('sysex', data=bytearray(b'ABC'))
     >>> msg.data += bytearray(b'DEF')
     >>> msg
-    <message sysex data=(65, 66, 67, 68, 69, 70) time=0>
+    Message('sysex', data=(65, 66, 67, 68, 69, 70), time=0)
+
+
+.. include:: frozen.rst
+
+.. include:: parsing.rst
+
+.. include:: serializing.rst
```

### Comparing `mido-1.2.9/docs/socket_ports.rst` & `mido-1.3.0/docs/ports/socket.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,45 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Socket Ports - MIDI over TCP/IP
-===============================
+-------------------------------
+
 
-About Socket Ports
-------------------
+About
+^^^^^
 
-Socket ports allow you to send MIDI messages over a computer
+Socket :term:`ports` allows you to send :term:`MIDI` messages over a computer
 network.
 
-The protocol is standard MIDI bytes over a TCP stream.
+The protocol is a simple MIDI bytes stream over :term:`TCP`.
+
+.. warning::
+
+    It is **not** :term:`rtpmidi`!
 
 
 Caveats
--------
+^^^^^^^
 
-The data is sent over an unencrypted channel. Also, the default server
-allows connections from any host and also accepts arbitrary sysex
+The data is sent over an *unencrypted channel*. Also, the default server
+allows connections from any host and also accepts arbitrary :term:`sysex`
 messages, which could allow anyone to for example overwrite patches on
-your synths (or worse). Use only on trusted networks.
+your synths (or **worse**). Use **only** on *trusted networks*.
 
-If you need more security, you can build a custom server with a white
-list of clients that are allowed to connect.
+If you need more security, you can build a *custom server* with a whitelist
+of clients allowed to connect.
 
-If timing is critical, latency and jitter (especially on wireless
-networks) may make socket ports unusable.
+If *timing* is critical, *latency* and *jitter* (especially on *wireless
+networks*) may make socket ports *unusable*.
 
 
 Sending Messages to a Server
-----------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 First, let's import some things::
 
     from mido.sockets import PortServer, connect
 
 After that, a simple server is only two lines::
 
@@ -41,21 +50,26 @@
 
     output = connect('localhost', 8080):
     output.send(message)
 
 Each end of the connection behaves like a normal Mido I/O port, with
 all the usual methods.
 
-The host may be a DNS host name or IP address (as a string). It may
-also be '', in which case connections are accepted on any ip address
-on the computer.
+The host may be an host name or IP address (as a string). It may also be '',
+in which case connections are accepted from any IP address on the computer.
+
+.. todo::
+
+    Test and clarify "Any IP address on the computer".
+    Does this mean only local adresses can connect or that any connection
+    from any network is allowed?
 
 
 Turning Things on their Head
-----------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 If you want the server to send messages the client, you can instead
 do::
 
     server = PortServer('localhost', 8080):
     while True:
         server.send(message)
@@ -68,40 +82,42 @@
 
 The client will now print any message that the server sends. Each
 message that the server sends will be received by all connected
 clients.
 
 
 Under the Hood
---------------
+^^^^^^^^^^^^^^
 
-The examples above use the server and client ports as normal I/O
+The examples above use the server and client ports as normal Mido I/O
 ports. This makes it easy to write simple servers, but you don't have
-any control connections and the way messages are sent and received.
+any control on connections and the way messages are sent and received.
 
-To get more control, you can ignore all the other methods of the
+To get more control,you can ignore all the other methods of the
 ``PortServer`` object and use only ``accept()``. Here's a simple
 server implemented this way::
 
     with PortServer('localhost', 8080) as server:
         while True:
             client = server.accept()
             for message in client:
                 print(message)
 
-``accept()`` waits for a client to connect, and returns a SocketPort
-object which is connected to the SocketPort object returned by
-``connect()`` at the other end.
+``accept()`` waits for a client to connect, and returns a ``SocketPort``
+object which is connected to the ``SocketPort`` object returned by
+``connect()`` on the other end.
 
-The server above has one weakness: it allows only one connection at a
+The server above has one weakness: it only allows one connection at a
 time. You can get around this by using ``accept(block=False)``. This
-will return a SocketPort if there is a connection waiting and None if
+will return a ``SocketPort`` if there's a connection waiting and ``None`` if
 there is connection yet.
 
-Using this, you can write the server any way you like, for example::
+.. todo:: Clarify "Connection waiting" vs "There is a connection yet".
+
+Using this you can write the server any way you like, for example::
 
     with PortServer('localhost', 8080) as server:
         clients = []
         while True:
             # Handle connections.
             client = server.accept(block=False)
             if client:
@@ -119,12 +135,12 @@
                     print('Received {} from {}'.format(message, client))
 
             # Do other things
             ...
 
 
 Possible Future Additions
--------------------------
+^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Optional HTTP-style headers could be added. As long as these are 7-bit
-ASCII, they will be counted as data bytes and ignored by clients or
+:term:`ASCII`, they will be counted as data bytes and ignored by clients or
 servers who don't expect them.
```

### Comparing `mido-1.2.9/docs/about_midi.rst` & `mido-1.3.0/docs/about_midi.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 About MIDI
 ==========
 
 A Short Introduction To MIDI
 ----------------------------
 
 MIDI is a simple binary protocol for communicating with synthesizers
@@ -13,59 +17,66 @@
 sequencers, and with them the electronic home studio. Although many
 attempts have been made to replace it, it is still the industry
 standard.
 
 MIDI was designed for the 8-bit micro controllers found in synthesizers
 at the beginning of the 80's. As such, it is a very minimal
 byte-oriented protocol. The message for turning a note on is only
-three bytes long (here shown in hexadecimal)::
+three bytes long (here shown in hexadecimal):
+
+.. code-block:: text
 
     92 3C 64
 
-This message consists of::
+This message consists of:
+
+.. code-blocK:: text
 
     92 -- 9 == message type note on
           2 == channel 2
 
     3C -- note 60 (middle C)
 
     64 -- velocity (how hard the note is hit)
 
-The first byte is called a status byte. It has the upper bit set,
-which is how you can tell it apart from the following data
-bytes. Data bytes are thus only 7 bits (0..127).
+The first byte is called a ``status`` byte. It has the upper bit set,
+which is how you can tell it apart from the following ``data``
+bytes. Data bytes are thus *always* 7 bits (Values: 0..127).
 
 Each message type has a given number of data bytes, the exception
-being the System Exclusive message which has a start and a stop byte
-and any number of data bytes in-between these two::
+being the :term:`System Exclusive` message which has a start (``SOX``) and a
+stop (``EOX``) byte and any number of data bytes in-between these two:
+
+.. code-block:: text
 
     F0 ... F7
 
 Messages can be divided into four groups:
 
-* Channel messages. These are used to turn notes on and off, to change
+* Channel Messages. These are used to turn notes on and off, to change
   patches, and change controllers (pitch bend, modulation wheel, pedal
   and many others). There are 16 channels, and the channel number is
-  encoded in the lower 4 bits of the status byte. Each synth can
-  choose which channel (or channels) it responds to. This can typically
-  be configured.
-
-* System common messages.
-
-* System real time messages, the include start, stop, continue, song
-  position (for playback of songs) and reset.
-
-* System Exclusive messages (often called Sysex messages). These are
-  used for sending and receiving device specific such as patch data.
+  encoded in the lower 4 bits (aka :term:`nibble`) of the status byte.
+  Each synth can choose which channel (or channels) it responds to. This can
+  typically be configured.
+
+* System Common Messages.
+
+* System Real Time Messages, includes ``start``, ``stop``, ``continue``,
+  ``song position`` (for playback of songs) and ``reset``.
+
+* System Exclusive Messages (often called :term:`SysEx` messages) are
+  used for sending and receiving *device specific* data such as patches and
+  proprietary controls.
 
 
 Some Examples of Messages
 -------------------------
 
-::
+.. code-block:: text
 
     # Turn on middle C on channel 2:
     92 3C 64
 
     # Turn it back off:
     82 3C 64
 
@@ -73,23 +84,7 @@
     C2 04
 
     # Continue (Starts a song that has been paused):
     FB
 
     # Sysex data request for the Roland SH-201 synthesizer:
     F0 41 10 00 00 16 11 20 00 00 00 00 00 00 21 3F F7
-
-
-Further Reading
----------------
-
-* `An Introduction to MIDI <https://www.midi.org/articles/an-intro-to-midi>`_
-
-* `MIDI Basics <http://download.yamaha.com/api/asset/file/?language=pt&site=br.yamaha.com&asset_id=13088>`_ (by Yamaha)
-
-* `Wikipedia's page on MIDI <http://en.wikipedia.org/wiki/Midi>`_
-
-* `MIDI Manufacturers Association <http://www.midi.org/>`_
-
-* `A full table of MIDI messages <http://www.midi.org/techspecs/midimessages.php>`_
-
-* `Essentials of the MIDI protocol <https://ccrma.stanford.edu/~craig/articles/linuxmidi/misc/essenmidi.html>`_
```

### Comparing `mido-1.2.9/docs/syx.rst` & `mido-1.3.0/docs/files/syx.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
+.. SPDX-FileCopyrightText: 2014 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 SYX Files
 =========
 
-SYX files are used to store SysEx messages, usually for patch
-data.
+SYX files are used to store :term:`SysEx` messages, usually for patch data.
 
 
 Reading and Writing
 -------------------
 
-To read a SYX file::
+To read a ``SYX`` file::
 
     messages = mido.read_syx_file('patch.syx')
 
-To write a SYX file::
+To write a ``SYX`` file::
 
     mido.write_syx_file('patch.syx', messages)
 
 Non-sysex messages will be ignored.
 
 
 Plain Text Format
 -----------------
 
-Mido also supports plain text SYX files. These are read in exactly the
+Mido also supports *plain text* SYX files. These are read in exactly the
 same way::
 
     messages = mido.read_syx_file('patch.txt')
 
 ``read_syx_file()`` determines which format the file is by looking at
-the first byte.  It Raises ValueError if file is plain text and byte
+the first byte.  It raises ``ValueError`` if file is plain text and byte
 is not a 2-digit hex number.
 
 To write plain text::
 
     mido.write_syx_file('patch.txt', messages, plaintext=True)
 
-This will write the messages as hex encoded bytes with one message per
-line::
+This will write the messages as hex encoded bytes with one message per line::
 
     F0 00 01 5D 02 00 F7
     F0 00 01 5D 03 00 F7
```

### Comparing `mido-1.2.9/docs/changes.rst` & `mido-1.3.0/docs/changes.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,128 @@
-Changes
-=======
+.. SPDX-FileCopyrightText: 2014 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
 
-(See :doc:`roadmap` for future plans.)
+Version Changes
+===============
+
+This project uses `Semantic Versioning <https://semver.org>`_.
+
+.. seealso::
+
+    The `Future <https://github.com/mido/mido/milestone/2>`_ milestone on
+    Github for future plans.
 
 
 Release History
 ---------------
 
+
+1.3.0 (2023-07-21)
+^^^^^^^^^^^^^^^^^^
+
+.. warning::
+
+    This release drops support for Python 2 and is only compatible with 3.7
+    onwards.
+
+* Bugfix Backends/rtmidi: Prevent virtual port name mangling (@rdoursenaud,
+  thanks to @digitalsignalperson for reporting)
+
+* Bugfix Backends/rtmidi: Remove callback before closing the port to avoid a
+  race condition (@rdoursenaud)
+
+* Bugfix MidiFile: Properly decode/encode SMPTE hours in the SMPTE offset Meta
+  (Thanks to @laori93 for reporting and @heilei for investigating. Issue #156)
+
+* Installation: support the "extras" syntax to install optional dependencies
+  (@rdoursenaud)
+
+* Documentation: updated, overhauled and proofread (@rdoursenaud, nomadbyte,
+  @superbock)
+
+* Bugfix: Backends/Portmidi (@akx, pull request #483)
+
+* MidiFile: Move merging track out of ``__iter__()`` to prevent hanging on
+  first call (@Frnot, pull request #470)
+
+* MidiFile: ``play()`` can now use an optional custom clock source
+  (@almostimplemented, pull request #153)
+
+* The project is now REUSE compliant. See https://reuse.software/ for details
+  (@rdoursenaud)
+
+* Packaging is now PEP-518 compliant (@rdoursenaud)
+
+* Backends/Socket: Disable buffering (@m-vo, pull request #342)
+
+* Removed support for Python 2.7. * Mido now requires Python 3.7 or
+  higher. (Ole Martin Bjørndalen, pull request #408, with additional cleanup
+  from @rdoursenaud)
+
+* Backends: The ``rtmidi`` and ``python-rtmidi`` 1.2.10 sometimes returned
+  duplicate port names. (Bug introduced in 1.2.10. Fix by Maciej
+  Sokołowski, pull request #321)
+
+* Bugfix Backends/Socket: In Python 3, PortServer used to crashe when a socket
+  client disconnects. (issue #290) (@kyleclaassen, pull request #291)
+
+* MidiFile: Make ``UnknownMetaMessage`` robust to faulty MIDI files (@sonovice,
+  pull request #286)
+
+* Bugfix MIDIFile: BPM <-> MIDI tempo conversions (@superbock, pull request
+  #114)
+
+* MidiFile: Added ``from_bytes()`` to ``MetaMessage`` (@gulaki, pull request
+  #149)
+
+1.2.10 (2021-05-10)
+^^^^^^^^^^^^^^^^^^^
+
+* New ``repr()`` format for messages, tracks and MIDI file
+  objects. (Implemented by John Belmonte, pull request #164.)
+
+* added new example ``midifiles/show_midifile.py`` based on the
+  new ``repr()`` format.
+
+* Added ``msg.is_cc()`` method. Checks if message is a control change.
+  Can also be used to check for a specific control change number, for
+  example ``msg.is_cc(7)``.
+
+* Fixed memory leaks in RtMidi backend (issue #256, fix by The Other Days,
+  pull request #264.)
+
+* clip now works with sysex messages (Fix by  Avatar Timo Stüber, pull request
+  #229.)
+
+* Improved docs and error message for time attribute in a message.
+  (tomerv, pull request #249.)
+
+* Improved MidiFile.play to avoid time drift. (Implemented by John
+  Belmonte, pull request #161.)
+
+* bugfix: MIDO_DEFAULT_INPUT was misspelled in mido-ports causing it
+  to be show as 'not set' even though it was set. (Fix by Bernhard
+  Wagner, pull request #192.)
+
+* Now only copies ports once in ports.multi_receive() (Tom Ritchford, pull
+  request #191.)
+
+* Ports lists returned from ``get_input_names()`` and friends are no
+  longer sorted. (Suggested and implemented by Ryan McCampbell, issue
+  #298.)
+
+* Updated linke in docs to point to the new home github.com/mido/
+  (Fixed by Joshua Mayers, pull request #177.)
+
+* thanks to Christopher Arndt, Kathryn DiPippo and Timo Stüber for fixing
+  flake8 issues.
+
+
+
 1.2.9 (2018-10-05)
 ^^^^^^^^^^^^^^^^^^
 
 * rewrote ``Parser`` class around a MIDI tokenizer. Should lead to
   slight speedup and much cleaner code.
 
 * bugfix: `data` attribute was missing for `UnknownMetaMessage`
@@ -576,15 +688,15 @@
 
 * bugfix: package didn't work with easy_install.
   (Issue #14, reported by netchose.)
 
 * bugfix: 100% memory consumption when calling blocking receive()
   on a PortMidi input. (Issue #15, reported by Francesco Ceruti.)
 
-* added wheel support: http://pythonwheels.com/
+* added wheel support: https://pythonwheels.com/
 
 
 1.1.5 (2014-04-18)
 ^^^^^^^^^^^^^^^^^^
 
 * removed the 'mode' attribute from key_signature messages. Minor keys
   now have an 'm' appended, for example 'Cm'.
```

### Comparing `mido-1.2.9/docs/license.rst` & `mido-1.3.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-License
-=======
+The MIT License
 
-The MIT License (MIT)
+Copyright (c) Ole Martin Bjørndalen
 
-Copyright (c) 2013-infinity Ole Martin Bjørndalen
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
 
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mido-1.2.9/docs/parsing.rst` & `mido-1.3.0/docs/messages/parsing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,57 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Parsing MIDI Bytes
-==================
+------------------
+
+The MIDI protocol is a *binary protocol*. Each message is encoded as a *status*
+byte followed by up to three *data* bytes. (Except :term:`SysEx` messages
+which can have an arbitrary number of *data* bytes immediately followed by an
+EOX status byte.)
 
-MIDI is a binary protocol. Each each message is encoded as a status byte
-followed by up to three data bytes. (Sysex messages can have any number of
-data bytes and use a stop byte instead.)
+.. versionadded:: 1.2 ``mido.Message.from_hex()``
 
 .. note:: To parse a single message you can use the class methods
-          ``mido.Message.from_bytes()`` and
-          ``mido.Message.from_hex()`` (new in 1.2).
+          ``mido.Message.from_bytes()`` and ``mido.Message.from_hex()``
+
+
 
-Mido comes with a parser that turns MIDI bytes into messages. You can create a parser object, or call one of the utility functions::
+Mido comes with a *parser* that turns MIDI bytes into messages. You can create
+a *parser object* or call one of the *utility functions*::
 
     >>> mido.parse([0x92, 0x10, 0x20])
-    <message note_on channel=0 note=16 velocity=32 time=0>
+    Message('note_on', channel=2, note=16, velocity=32, time=0)
 
     >>> mido.parse_all([0x92, 0x10, 0x20, 0x82, 0x10, 0x20])
-    [<message note_on channel=2 note=16 velocity=32 time=0>,
-     <message note_off channel=2 note=16 velocity=32 time=0>]
+    [Message('note_on', channel=2, note=16, velocity=32, time=0),
+     Message('note_off', channel=2, note=16, velocity=32, time=0)]
 
 These functions are just shortcuts for the full ``Parser`` class. This
-is the parser used inside input ports to parse incoming messages.
+is the same parser as used inside input ports to parse incoming messages.
 Here are a few examples of how it can be used::
 
     >>> p = mido.Parser()
     >>> p.feed([0x90, 0x10, 0x20])
     >>> p.pending()
     1
     >>> p.get_message()
-    <message note_on channel=0 note=16 velocity=32 time=0>
+    Message('note_on', channel=0, note=16, velocity=32, time=0)
 
     >>> p.feed_byte(0x90)
     >>> p.feed_byte(0x10)
     >>> p.feed_byte(0x20)
     >>> p.feed([0x80, 0x10, 0x20])
-    <message note_on channel=0 note=16 velocity=32 time=0>
+    >>> p.pending()
+    2
+    >>> p.get_message()
+    Message('note_on', channel=0, note=16, velocity=32, time=0)
+    >>> p.get_message()
+    Message('note_off', channel=0, note=16, velocity=32, time=0)
 
 ``feed()`` accepts any iterable that generates integers in 0..255. The
 parser will skip and stray status bytes or data bytes, so you can
 safely feed it random data and see what comes out the other end.
 
 ``get_message()`` will return ``None`` if there are no messages ready
 to be gotten.
@@ -47,11 +61,8 @@
 
     >>> p.feed([0x92, 0x10, 0x20, 0x82, 0x10, 0x20])
     >>> for message in p:
     ...    print(message)
     note_on channel=2 note=16 velocity=32 time=0
     note_off channel=2 note=16 velocity=32 time=0
 
-The messages are available in `p.messages` (a `collections.deque`).
-
-For the full table of MIDI binary encoding, see:
-`<http://www.midi.org/techspecs/midimessages.php>`_
+The messages are available in ``p.messages`` (a ``collections.deque``).
```

### Comparing `mido-1.2.9/docs/message_types.rst` & `mido-1.3.0/docs/message_types.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,15 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Message Types
 =============
 
+
 Supported Messages
 ------------------
 
 ==============  ==============================
 Name            Keyword Arguments / Attributes
 ==============  ==============================
 note_off        channel note velocity
@@ -23,16 +28,15 @@
 start
 continue
 stop
 active_sensing
 reset
 ==============  ==============================
 
-``quarter_frame`` is used for SMPTE time codes. See:
-http://www.electronics.dit.ie/staff/tscarff/Music_technology/midi/MTC.htm
+``quarter_frame`` is used for SMPTE time codes.
 
 
 Parameter Types
 ---------------
 
 ===========  ======================  ================
 Name         Valid Range             Default Value
@@ -59,21 +63,15 @@
     1 when communicating with the user.
 
 ``velocity`` is how fast the note was struck or released. It defaults
 to 64 so that if you don't set it, you will still get a reasonable
 value. (64 is the recommended default for devices that don't support
 it attack or release velocity.)
 
-The ``time`` parameter is not included in the encoded message, and is
-(currently) not used by Mido in any way. You can use it for whatever
-purpose you wish.
+The ``time`` is used in MIDI files as delta time.
 
 The ``data`` parameter accepts any iterable that generates numbers in
 0..127. This includes::
 
     mido.Message('sysex', data=[1, 2, 3])
     mido.Message('sysex', data=range(10))
     mido.Message('sysex', data=(i for i in range(10) if i % 2 == 0))
-
-For details about the binary encoding of a MIDI message, see:
-
-http://www.midi.org/techspecs/midimessages.php
```

### Comparing `mido-1.2.9/docs/frozen_messages.rst` & `mido-1.3.0/docs/messages/frozen.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,58 @@
+.. SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Frozen Messages
 ---------------
 
-(New in 1.2.)
+.. versionadded:: 1.2
 
-Since Mido messages are mutable (can change) they can not be hashed or
+Since Mido messages are *mutable* (can change) they can not be hashed or
 put in dictionaries. This makes it hard to use them for things like
 Markov chains.
 
-In these situations you can use frozen messages:
+In these situations you can use *frozen messages*:
 
 .. code-block:: python
 
     from mido.frozen import FrozenMessage
 
     msg = FrozenMessage('note_on')
     d = {msg: 'interesting'}
 
-Frozen messages are used and behave in exactly the same way as normal
-messages with one exception: attributes are not settable.
+*Frozen messages* are used and behave in exactly the same way as normal
+messages with one exception: **attributes are not settable**.
 
 There are also variants for meta messages (``FrozenMetaMessage`` and
 ``FrozenUnknownMetaMessage``).
 
-You can freeze and thaw messages with:
+You can *freeze* and *thaw* messages with:
 
 .. code-block:: python
 
     from mido.frozen import freeze_message, thaw_message
 
     frozen = freeze_message(msg)
     thawed = thaw_message(frozen)
 
-``thaw_message()`` will always return a copy. Passing a frozen message
+``thaw_message()`` will always return a *copy*. Passing a *frozen message*
 to ``freeze_message()`` will return the original message.
 
 Both functions return ``None`` if you pass ``None`` which is handy for
 things like:
 
 .. code-block:: python
 
     msg = freeze_message(port.receive())
 
-    # Python 3 only:
     for msg in map(freeze_message, port):
         ...
 
-    # Python 2 and 3:
-    for msg in (freeze_message(msg) for msg in port):
-        ...
-
-To check if a message is frozen:
+To check if a message is *frozen*:
 
 .. code-block:: python
 
     from mido.frozen import is_frozen
 
     if is_frozen(msg):
         ...
-
```

### Comparing `mido-1.2.9/docs/images/midi_time.svg` & `mido-1.3.0/docs/images/midi_time.svg`

 * *Files identical despite different names*

### Comparing `mido-1.2.9/docs/string_encoding.rst` & `mido-1.3.0/docs/messages/serializing.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
+
+Serializing
+-----------
+
 String Encoding
-===============
+^^^^^^^^^^^^^^^
 
 Mido messages can be serialized to a text format, which can be used to
 safely store messages in text files, send them across sockets or embed
 them in JSON, among other things.
 
-To encode a message, simply call ``str()`` on it::
+To *encode* a message, simply call ``str()`` on it::
 
     >>> cc = control_change(channel=9, control=1, value=122, time=60)
     >>> str(cc)
     'control_change channel=9 control=1 value=122 time=60'
 
 To convert the other way (new method in 1.2)::
 
     >>> mido.Message.from_str('control_change control=1 value=122')
-    <message control_change channel=0 control=1 value=122 time=0>
+    Message('control_change', channel=0, control=1, value=122, time=0)
 
 Alternatively, you can call the ``format_as_string`` function directly:
 
     >>> mido.format_as_string(cc)
     'control_change channel=9 control=1 value=122 time=60'
 
 If you don't need the time attribute or you want to store it elsewhere, you
@@ -27,49 +35,49 @@
     >>> mido.format_as_string(cc)
     'control_change channel=9 control=1 value=122'
 
 (This option is also available in ``mido.Message.from_str()``.)
 
 
 Format
-------
+^^^^^^
 
 The format is simple::
 
     MESSAGE_TYPE [PARAMETER=VALUE ...]
 
 These are the same as the arguments to ``mido.Message()``. The order
-of parameters doesn't matter, but each one can only appear once.
+of parameters doesn't matter but each one can only appear once.
 
-Only these character will ever occur in a string encoded Mido message::
+Only these characters will ever occur in a string encoded Mido message::
 
     [a-z][0-9][ =_.+()]
 
 or written out::
 
     'abcdefghijklmnopqrstuvwxyz0123456789 =_.+()'
 
 This means the message can be embedded in most text formats without
 any form of escaping.
 
 
 Parsing
--------
+^^^^^^^
 
-To parse a message, you can use ``mido.parse_string()``::
+To *parse* a message, you can use ``mido.parse_string()``::
 
     >>> parse_string('control_change control=1 value=122 time=0.5')
-    <message control_change channel=0 control=1 value=122 time=0.5>
+    Message('control_change', channel=0, control=1, value=122, time=0.5)
 
 Parameters that are left out are set to their default
 values. ``ValueError`` is raised if the message could not be
-parsed. Extra whitespace is ignored::
+parsed. *Extra whitespace is ignored*::
 
     >>> parse_string('  control_change   control=1  value=122')
-    <message control_change channel=0 control=1 value=122 time=0>
+    Message('control_change', channel=0, control=1, value=122, time=0)
 
 To parse messages from a stream, you can use
 ``mido.messages.parse_string_stream()``::
 
     for (message, error) in parse_string_stream(open('some_music.text')):
         if error:
             print(error)
@@ -81,30 +89,34 @@
 message describing what went wrong, as well as the line number where
 the error occurred.
 
 The argument to ``parse_string_stream()`` can be any object that
 generates strings when iterated over, such as a file or a list.
 
 ``parse_string_stream()`` will ignore blank lines and comments (which
-start with a # and go to the end of the line). An example of valid
+start with a ``#`` and go to the end of the line). An example of valid
 input::
 
     # A very short song with an embedded sysex message.
     note_on channel=9 note=60 velocity=120 time=0
     # Send some data
 
     sysex data=(1,2,3) time=0.5
 
     pitchwheel pitch=4000  # bend the not a little time=0.7
     note_off channel=9 note=60 velocity=60 time=1.0
 
 
 Examples
---------
+^^^^^^^^
+
+An example of messages embedded into JSON:
 
-And example of messages embedded in JSON::
+.. code-block:: json
 
-    {'messages': [
-       '0.0 note_on channel=9 note=60 velocity=120',
-       '0.5 sysex data=(1,2,3)',
-       ...
-    ])
+    {
+        "messages": [
+            "0.0 note_on channel=9 note=60 velocity=120",
+            "0.5 sysex data=(1,2,3)",
+            "...",
+        ]
+    }
```

### Comparing `mido-1.2.9/docs/midi_files.rst` & `mido-1.3.0/docs/files/midi.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,47 @@
-MIDI Files
-==========
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
 
-MidiFile objects can be used to read, write and play back MIDI
-files.
+Standard MIDI Files
+===================
 
+``MidiFile`` objects can be used to *read*, *write* and *play back* MIDI files.
 
-Opening a File
---------------
+
+Opening
+-------
 
 You can open a file with::
 
     from mido import MidiFile
 
     mid = MidiFile('song.mid')
 
-.. note:: Sysex dumps such as patch data are often stored in SYX files
-   rather than MIDI files. If you get "MThd not found. Probably not a
-   MIDI file" try ``mido.read_syx_file()``. (See :doc:`syx` for more.)
-   
+.. note::
+
+    :term:`SysEx` dumps such as patch data are often stored in ``SYX``
+    files rather than MIDI files. If you get "MThd not found. Probably not a
+    MIDI file" try ``mido.read_syx_file()``.
+    (See :doc:`syx` for more.)
+
 The ``tracks`` attribute is a list of tracks. Each track is a list of
 messages and meta messages, with the ``time`` attribute of each
 messages set to its delta time (in ticks). (See Tempo and Beat
 Resolution below for more on delta times.)
 
 To print out all messages in the file, you can do::
 
     for i, track in enumerate(mid.tracks):
         print('Track {}: {}'.format(i, track.name))
         for msg in track:
             print(msg)
 
 The entire file is read into memory. Thus you can freely modify tracks
-and messages, and save the file back by calling the ``save()``
+and messages and save the file back by calling the ``save()``
 method. (More on this below.)
 
 
 Iterating Over Messages
 -----------------------
 
 Iterating over a ``MidiFile`` object will generate all MIDI messages
@@ -45,82 +51,83 @@
 
 Meta messages will also be included. If you want to filter them out,
 you can do::
 
     if msg.is_meta:
         ...
 
-This makes it easy to play back a MIDI file on a port::
+This makes it easy to play back a MIDI file on a port (though this simple
+implementation is subject to time drift)::
 
     for msg in MidiFile('song.mid'):
         time.sleep(msg.time)
         if not msg.is_meta:
             port.send(msg)
 
 This is so useful that there's a method for it::
 
     for msg in MidiFile('song.mid').play():
         port.send(msg)
 
-This does the sleeping and filtering for you. If you pass
-``meta_messages=True`` you will also get meta messages. These can not
-be sent on ports, which is why they are off by default.
+This does the sleeping and filtering for you (while avoiding drift). If you
+pass ``meta_messages=True`` you will also get meta messages. These **cannot**
+be sent on ports, which is why they are ``off`` by default.
 
 
 
 Creating a New File
 -------------------
 
-You can create a new file by calling MidiFile without the ``filename``
+You can create a new file by calling ``MidiFile`` without the ``filename``
 argument. The file can then be saved by calling the ``save()`` method::
 
     from mido import Message, MidiFile, MidiTrack
 
     mid = MidiFile()
     track = MidiTrack()
     mid.tracks.append(track)
 
     track.append(Message('program_change', program=12, time=0))
     track.append(Message('note_on', note=64, velocity=64, time=32))
     track.append(Message('note_off', note=64, velocity=127, time=32))
-    
+
     mid.save('new_song.mid')
 
 The ``MidiTrack`` class is a subclass of list, so you can use all the
 usual methods.
 
 All messages must be tagged with delta time (in ticks). (A delta time
 is how long to wait before the next message.)
 
-If there is no 'end_of_track' message at the end of a track, one will
+If there is no ``end_of_track`` message at the end of a track, one will
 be written anyway.
 
 A complete example can be found in ``examples/midifiles/``.
 
 The ``save`` method takes either a filename (``str``) or, using the ``file``
-keyword parameter, a file object such as an in-memory binary file (an
+keyword parameter, a file-like object such as an in-memory binary file (an
 ``io.BytesIO``). If you pass a file object, ``save`` does not close it.
 Similarly, the ``MidiFile`` constructor can take either a filename, or
 a file object by using the ``file`` keyword parameter. if you pass a file
 object to ``MidiFile`` as a context manager, the file is not closed when
-the context manager exits. Examples can be found in ``test_midifiles2.py``.
-
+the context manager exits.
+Examples can be found in ``test_midifiles2.py``.
 
 
 File Types
 ----------
 
 There are three types of MIDI files:
 
 * type 0 (single track): all messages are saved in one track
 * type 1 (synchronous): all tracks start at the same time
 * type 2 (asynchronous): each track is independent of the others
 
 When creating a new file, you can select type by passing the ``type``
-keyword argument, or by setting the ``type`` attribute::
+keyword argument or by setting the ``type`` attribute::
 
    mid = MidiFile(type=2)
    mid.type = 1
 
 Type 0 files must have exactly one track. A ``ValueError`` is raised
 if you attempt to save a file with no tracks or with more than one
 track.
@@ -143,32 +150,32 @@
 -------------
 
 Meta messages behave like normal messages and can be created in the
 usual way, for example::
 
     >>> from mido import MetaMessage
     >>> MetaMessage('key_signature', key='C#', mode='major')
-    <meta message key_signature key='C#' mode='major' time=0>
+    MetaMessage('key_signature', key='C#', mode='major', time=0)
 
 You can tell meta messages apart from normal messages with::
 
     if msg.is_meta:
         ...
 
 or if you know the message type you can use the ``type`` attribute::
 
     if msg.type == 'key_signature':
         ...
     elif msg.type == 'note_on':
         ...
 
-Meta messages can not be sent on ports.
+Meta messages **cannot** be sent on ports.
 
 For a list of supported meta messages and their attributes, and also
-how to implement new meta messages, see :doc:`meta_message_types`.
+how to implement new meta messages, see :doc:`../meta_message_types`.
 
 
 About the Time Attribute
 ------------------------
 
 The ``time`` attribute is used in several different ways:
 
@@ -176,51 +183,65 @@
 
 * in messages yielded from ``play()``, it is delta time in seconds
   (time elapsed since the last yielded message)
 
 * (only important to implementers) inside certain methods it is
   used for absolute time in ticks or seconds
 
+.. todo: Review implementation to separate concerns and units into dedicated
+         attributes.
 
-Tempo and Beat Resolution
+
+Tempo and Time Resolution
 -------------------------
 
-.. image:: images/midi_time.svg
+.. image:: ../images/midi_time.svg
+
+Timing in MIDI files is centered around ticks. Each message in a MIDI file has
+a delta time, which tells how many ticks have passed since the last message.
+
+A tick is the smallest unit of time in MIDI and remains fixed throughout the
+song. Each quarter notes is divided into a certain number of ticks, often
+referred as the resolution of the file or pulses per quarter note (PPQN). This
+resolution is stored as ``ticks_per_beat`` in MidiFile objects.
 
-Timing in MIDI files is centered around ticks and beats. A beat is the same as 
-a quarter note. Beats are divided into ticks, the smallest unit of time in 
-MIDI.
-
-Each message in a MIDI file has a delta time, which tells how many ticks have 
-passed since the last message. The length of a tick is defined in ticks per 
-beat. This value is stored as ``ticks_per_beat`` in MidiFile objects and 
-remains fixed throughout the song.
+The meaning of this ``ticks_per_beat`` in terms of absolute timing depends on
+the tempo and time signature of the file.
 
 
 MIDI Tempo vs. BPM
 ^^^^^^^^^^^^^^^^^^
 
-Unlike music, tempo in MIDI is not given as beats per minute, but rather in 
-microseconds per beat.
+Unlike music, tempo in MIDI is not given as beats per minute (BPM), but rather
+in microseconds per quarter note, with a default tempo of 500000 microseconds
+per quarter note. Given a default 4/4 time signature where a beat is exactly a
+quarter note, this corresponds to 120 beats per minute.
+
+In case of different time signatures, the length of a beat depends on the
+denominator of the time signature. E.g. in 2/2 time signature a beat has a
+length of a half note, i.e. two quarter notes. Thus the default MIDI tempo of
+500000 corresponds to a beat length of 1 second which is 60 BPM.
 
-The default tempo is 500000 microseconds per beat, which is 120 beats per 
-minute. The meta message 'set_tempo' can be used to change tempo during a song.
+The meta messages 'set_tempo' and 'time_signature' can be used to change
+the tempo and time signature during a song, respectively.
 
-You can use :py:func:`bpm2tempo` and :py:func:`tempo2bpm` to convert to and 
-from beats per minute. Note that :py:func:`tempo2bpm` may return a floating 
+You can use :py:func:`bpm2tempo` and :py:func:`tempo2bpm` to convert to and
+from beats per minute. Note that :py:func:`tempo2bpm` may return a floating
 point number.
 
+
 Converting Between Ticks and Seconds
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-To convert from MIDI time to absolute time in seconds, the number of beats per 
-minute (BPM) and ticks per beat (often called pulses per quarter note or PPQ, 
-for short) have to be decided upon.
+To convert from MIDI time to absolute time in seconds, the tempo (either
+in number of beats per minute (BPM) or microseconds per quarter note, see
+`MIDI Tempo vs. BPM`_ above) and ticks per per quarter note have to be decided
+upon.
 
 You can use :py:func:`tick2second` and :py:func:`second2tick` to convert to
-and from seconds and ticks. Note that integer rounding of the result might be 
+and from seconds and ticks. Note that integer rounding of the result might be
 necessary because MIDI files require ticks to be integers.
 
-If you have a lot of rounding errors you should increase the time resolution 
-with more ticks per beat, by setting MidiFile.ticks_per_beat to a large number.
-Typical values range from 96 to 480 but some use even more ticks per beat.
-
+If you have a lot of rounding errors you should increase the time resolution
+with more ticks per quarter note, by setting MidiFile.ticks_per_beat to a
+large number. Typical values range from 96 to 480 but some use even more ticks
+per quarter note.
```

### Comparing `mido-1.2.9/docs/meta_message_types.rst` & `mido-1.3.0/docs/meta_message_types.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Meta Message Types
 ==================
 
 Supported Messages
 ------------------
 
 sequence_number (0x00)
@@ -194,33 +198,35 @@
 
 Time signature of:
 
 4/4 : MetaMessage('time_signature', numerator=4, denominator=4)
 
 3/8 : MetaMessage('time_signature', numerator=3, denominator=8)
 
-.. note:: From 1.2.9 time signature message have the correct default
-          value of 4/4. In earlier versions the default value was 2/4
-          due to a typo in the code.
+.. versionadded:: 1.2.9
+
+    Time signature message have the correct default value of 4/4. In earlier
+    versions the default value was 2/4 due to a typo in the code.
 
 
 key_signature (0x59)
 ^^^^^^^^^^^^^^^^^^^^
 
 =========  ==================  ========
 Attribute  Values              Default
 =========  ==================  ========
 key        'C', 'F#m', ...     'C'
 =========  ==================  ========
 
 Valid values: A A#m Ab Abm Am B Bb Bbm Bm C C# C#m Cb Cm D D#m Db Dm E
 Eb Ebm Em F F# F#m Fm G G#m Gb Gm
 
-Note: the mode attribute was removed in 1.1.5. Instead, an 'm' is
-appended to minor keys.
+.. versionchanged:: 1.1.5
+
+    The mode attribute was removed. Instead, an 'm' is appended to minor keys.
 
 
 sequencer_specific (0x7f)
 ^^^^^^^^^^^^^^^^^^^^^^^^^
 
 ==============  ==============  ========
 Attribute       Values          Default
@@ -239,32 +245,33 @@
 back to the file exactly as they came out.
 
 Code that depends on ``UnknownMetaMessage`` may break if the message
 in question is ever implemented, so it's best to only use these to
 learn about the format of the new message and then implement it as
 described below.
 
-``UnknownMetaMessage`` have two attributes::
+``UnknownMetaMessage`` have two attributes:
+
+* ``type_byte`` - a byte which uniquely identifies this message type
 
-    ``type_byte`` - a byte which uniquely identifies this message type
-    ``data`` - the message data as a list of bytes
+* ``data`` - the message data as a list of bytes
 
 These are also visible in the ``repr()`` string::
 
-    <unknown meta message type_byte=0x## data=[...], time=0>
+    UnknownMetaMessage(type_byte=251, data=(1, 2, 3), time=0)
 
 
-Implementing New Meta Messages
-------------------------------
+Implementing New or Custom Meta Messages
+----------------------------------------
 
-If you come across a meta message which is not implemented, or you
+If you come across a meta message which is not implemented or you
 want to use a custom meta message, you can add it by writing a new
 meta message spec::
 
-    from mido.midifiles import MetaSpec, add_meta_spec
+    from mido.midifiles.meta import MetaSpec, add_meta_spec
 
     class MetaSpec_light_color(MetaSpec):
         type_byte = 0xf0
         attributes = ['r', 'g', 'b']
         defaults = [0, 0, 0]
 
     def decode(self, message, data):
@@ -296,15 +303,15 @@
 
     add_meta_spec(MetaSpec_light_color)
 
 and create messages in the usual way::
 
     >>> from mido import MetaMessage
     >>> MetaMessage('light_color', r=120, g=60, b=10)
-    <meta message light_color r=120 g=60 b=10 time=0>
+    MetaMessage('light_color', r=120, g=60, b=10, time=0)
 
 and the new message type will now work when reading and writing MIDI
 files.
 
 Some additional functions are available::
 
     encode_string(unicode_string)
@@ -322,8 +329,8 @@
 
     class MetaSpec_instrument_name(MetaSpec_track_name):
         type_byte = 0x04
 
 This allows you to skip everything but ``type_byte``, since the rest
 is inherited.
 
-See the existing MetaSpec classes for further examples.
+See the existing ``MetaSpec`` classes for further examples.
```

### Comparing `mido-1.2.9/docs/intro.rst` & `mido-1.3.0/docs/intro.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Introduction (Basic Concepts)
 =============================
 
-Mido is all about messages and ports.
+Mido is all about messages, ports and files.
 
 
 Messages
 --------
 
 Mido allows you to work with MIDI messages as Python objects. To
 create a new message::
 
     >>> from mido import Message
     >>> msg = Message('note_on', note=60)
     >>> msg
-    <message note_on channel=0 note=60 velocity=64 time=0>
+    Message('note_on', channel=0, note=60, velocity=64, time=0)
 
 .. note::
 
-    Mido numbers channels 0 to 15 instead of 1 to 16. This makes them
-    easier to work with in Python but you may want to add and subtract
-    1 when communicating with the user.
+    Mido numbers channels ``0`` to ``15`` instead of ``1`` to ``16``. This makes
+    them easier to work with from Python but you may want to add and subtract
+    ``1`` when communicating with the user.
 
 A list of all supported message types and their parameters can be
 found in :doc:`message_types`.
 
 The values can now be accessed as attributes::
 
     >>> msg.type
@@ -33,25 +37,25 @@
     >>> msg.velocity
     64
 
 Attributes are also settable but this should be avoided. It's better
 to use ``msg.copy()``::
 
     >>> msg.copy(note=100, velocity=127)
-    <message note_on channel=2 note=100 velocity=127 time=0)
+    Message('note_on', channel=0, note=100, velocity=127, time=0)
 
 Type and value checks are done when you pass parameters or assign to
 attributes, and the appropriate exceptions are raised. This ensures
 that the message is always valid.
 
-For more about messages, see :doc:`messages`.
+For more about messages, see :doc:`messages/index`.
 
 
 Type and Value Checking
------------------------
+^^^^^^^^^^^^^^^^^^^^^^^
 
 Mido messages come with type and value checking built in::
 
     >>> import mido
     >>> mido.Message('note_on', channel=2092389483249829834)
     Traceback (most recent call last):
       File "<stdin>", line 1, in <module>
@@ -104,57 +108,66 @@
 
     for msg in inport:
         ...
 
 You can also receive and iterate over messages in a non-blocking
 way.
 
-For more about ports, see :doc:`ports`.
+For more about ports, see :doc:`ports/index`.
 
 
 All Ports are Ports
--------------------
+^^^^^^^^^^^^^^^^^^^
 
 The input and output ports used above are device ports, which
-communicate with a (physical or virtual) MIDI device.
+communicate with a physical or virtual MIDI device.
 
 Other port types include:
 
-* ``MultiPort``, which wraps around a set of ports and allow you to send to all of them or receive from all of them as if they were one.
+* ``MultiPort``, which wraps around a set of ports and allows you to send to
+  all of them or receive from all of them as if they were one.
 
-* ``SocketPort``, which communicates with another port over a TCP/IP (network) connection.
+* ``SocketPort``, which communicates with another port over a TCP/IP (network)
+  connection.
 
-* ``IOPort``, which wraps around an input and an output port and allows you to send and receive messages as if the two were the same port.
+* ``IOPort``, which wraps around an input and an output port and allows you to
+  send and receive messages as if the two were the same port.
 
 Ports of all types look and behave the same way, so they can be used
 interchangeably.
 
-It's easy to write new port types. See :doc:`implementing_ports`.
+It's easy to write new port types. See :doc:`ports/custom`.
 
 
 Virtual Ports
--------------
+^^^^^^^^^^^^^
 
-Virtual ports allow you to create new ports that other applications
+Virtual ports allows you to create new ports that other applications
 can connect to::
 
     with mido.open_input('New Port', virtual=True) as inport:
         for message in inport:
             print(message)
 
-The port should now appear to other applications as "New Port".
+The port should now appear to other applications as "``New Port``".
+
+
+.. warning::
 
-Unfortunately virtual ports are not supported by PortMidi and Pygame
-so this only works with RtMidi.
+    Unfortunately virtual ports are not supported by PortMidi and Pygame
+    so this only works with RtMidi.
 
+    Furthermore, RtMidi's virtual ports are not available under Microsoft
+    Windows. See: :doc:`backends/rtmidi` for details.
 
-Parsing MIDI Bytes
-------------------
 
-Mido comes with a parser that allows you to turn bytes into
+Raw MIDI Bytes Parser
+---------------------
+
+Mido comes with a parser that allows you to turn ``bytes`` into
 messages. You can create a new parser::
 
     >>> p = mido.Parser()
     >>> p.feed([0x90, 0x40])
     >>> p.feed_byte(0x60)
 
 You can then fetch messages out of the parser::
@@ -162,27 +175,20 @@
     >>> p.pending()
     1
     >>> for message in p:
     ...    print(message)
     ...
     note_on channel=0 note=64 velocity=96 time=0
 
-For more on parsers and parsing see :doc:`parsing`.
+For more on parsers and parsing see :doc:`messages/parsing`.
+
+.. versionadded:: 1.2
 
-You can also create a message from bytes using class methods (new in
-1.2):
+You can also create a message from ``bytes`` using class methods:
 
 .. code-block:: python
 
    msg1 = mido.Message.from_bytes([0x90, 0x40, 0x60])
    msg2 = mido.Message.from_hex('90, 40 60')
 
-The bytes must contain exactly one complete message. If not
+The ``bytes`` must contain exactly one complete message. If not
 ``ValueError`` is raised.
-
-
-Backends
---------
-
-Mido comes with backends for RtMidi and PortMidi and Pygame. The
-default is RtMidi. You can select another backend or even use multiple
-backends at the same time. For more on this, see :doc:`backends/index`.
```

### Comparing `mido-1.2.9/docs/freezing.rst` & `mido-1.3.0/docs/freezing_exe.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+.. SPDX-FileCopyrightText: 2014 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Freezing to EXE File
 ====================
 
 PyInstaller
 -----------
 
 When you build an executable with PyInstaller and run it you may get
@@ -22,15 +26,15 @@
 
     $ pyinstaller --onefile midotest.py
     $ ./dist/midotest 
     [u'Midi Through Port-0']
 
 If you don't want to change the program, you can instead declare the
 backend module as a `hidden import
-<http://pythonhosted.org/PyInstaller/#listing-hidden-imports>`_.
+<https://pyinstaller.org/en/stable/when-things-go-wrong.html#listing-hidden-imports>`_.
 
 
 bbFreeze, py2exe, cx_Freeze, py2app, etc.
 -----------------------------------------
 
 I suspect the same is true for these, but I have not had a chance to
 try it out yet.
```

### Comparing `mido-1.2.9/docs/bin.rst` & `mido-1.3.0/docs/binaries.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,39 @@
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 Included Programs
 =================
 
-These are installed with Mido.
+A few sample programs are installed with Mido and available directly from the
+:term:`CLI`.
 
+.. warning::
 
-mido-play
----------
-
-Plays back one or more MIDI files::
-
-    $ mido-play song1.mid song2.mid
+    These are intended to demonstrate the capabilities of Mido and used as a
+    template for your own programs. These are not fully fledged and may miss
+    crucial features.
 
 
 mido-ports
 ----------
 
-Lists available input and output ports and shows environment variables
+Lists all available input and output ports, shows environment variables
 and the current backend module.
 
 
+mido-play
+---------
+
+Plays back one or more MIDI files::
+
+    $ mido-play song1.mid [song2.mid]
+
+
 mido-serve
 ----------
 
 Serves one or more ports over the network, for example::
 
     $ mido-serve :9080 'Integra-7'
```

### Comparing `mido-1.2.9/docs/implementing_backends.rst` & `mido-1.3.0/docs/backends/custom.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-Writing a New Backend
-=====================
+.. SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
+Writing a New or Custom Backend
+-------------------------------
 
 A backend is a Python module with one or more of these::
 
     Input -- an input port class
     Output -- an output port class
     IOPort -- an I/O port class
     get_devices() -- returns a list of devices
```

### Comparing `mido-1.2.9/docs/make.bat` & `mido-1.3.0/docs/make.bat`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+REM SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+REM
+REM SPDX-License-Identifier: CC0-1.0
+
 @ECHO OFF
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
```

### Comparing `mido-1.2.9/docs/Makefile` & `mido-1.3.0/docs/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: CC0-1.0
+
 # Makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line.
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 PAPER         =
```

### Comparing `mido-1.2.9/LICENSE` & `mido-1.3.0/LICENSES/MIT.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-The MIT License
+MIT License
 
-Copyright (c) 2013-infinity Ole Martin Bjørndalen
+Copyright (c) <year> <copyright holders>
 
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
-TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
-SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mido-1.2.9/mido.egg-info/SOURCES.txt` & `mido-1.3.0/mido.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,98 @@
+.flake8
+.gitignore
+.readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
-setup.py
-tox.ini
-bin/mido-connect
-bin/mido-play
-bin/mido-ports
-bin/mido-serve
+pyproject.toml
+.github/workflows/documentation.yml
+.github/workflows/release.yml
+.github/workflows/test.yml
+.reuse/dep5
+LICENSES/CC-BY-4.0.txt
+LICENSES/CC-BY-SA-3.0.txt
+LICENSES/CC0-1.0.txt
+LICENSES/MIT.txt
 docs/Makefile
 docs/about_midi.rst
 docs/acknowledgements.rst
+docs/api.rst
 docs/authors.rst
-docs/bin.rst
+docs/binaries.rst
 docs/changes.rst
+docs/code_of_conduct.rst
 docs/conf.py
 docs/contributing.rst
-docs/freezing.rst
-docs/frozen_messages.rst
-docs/implementing_backends.rst
-docs/implementing_ports.rst
+docs/freezing_exe.rst
+docs/glossary.rst
 docs/index.rst
 docs/installing.rst
 docs/intro.rst
-docs/lib.rst
-docs/license.rst
+docs/licenses.rst
 docs/make.bat
 docs/message_types.rst
-docs/messages.rst
 docs/meta_message_types.rst
-docs/midi_files.rst
-docs/parsing.rst
-docs/ports.rst
 docs/resources.rst
-docs/roadmap.rst
-docs/socket_ports.rst
-docs/string_encoding.rst
-docs/syx.rst
-docs/_static/PLACEHOLDER
+docs/_static/.gitkeep
 docs/backends/amidi.rst
+docs/backends/custom.rst
 docs/backends/index.rst
 docs/backends/portmidi.rst
 docs/backends/pygame.rst
 docs/backends/rtmidi.rst
 docs/backends/rtmidi_python.rst
+docs/files/index.rst
+docs/files/midi.rst
+docs/files/syx.rst
 docs/images/midi_time.svg
+docs/images/midi_time.svg.license
+docs/messages/frozen.rst
+docs/messages/index.rst
+docs/messages/parsing.rst
+docs/messages/serializing.rst
+docs/ports/custom.rst
+docs/ports/index.rst
+docs/ports/socket.rst
+docs/shared/licenses_logos.rst
 examples/using_rtmidi_directly.py
 examples/backends/printer.py
 examples/backends/rtm.py
 examples/backends/use_printer.py
 examples/midifiles/create_midi_file.py
 examples/midifiles/midifile_to_json.py
 examples/midifiles/play_midi_file.py
 examples/midifiles/print_midi_file.py
+examples/midifiles/show_midifile.py
 examples/midifiles/test.sh
 examples/ports/input_filter.py
 examples/ports/list_ports.py
 examples/ports/multi_receive.py
 examples/ports/nonblocking_receive.py
 examples/ports/queue_port.py
 examples/ports/receive.py
 examples/ports/send.py
 examples/sockets/forward_ports.py
 examples/sockets/serve_ports.py
 examples/sockets/simple_client.py
 examples/sockets/simple_server.py
 extras/README.rst
 extras/hid_joystick.py
-mido/__about__.py
 mido/__init__.py
 mido/frozen.py
 mido/parser.py
 mido/ports.py
-mido/py2.py
 mido/sockets.py
 mido/syx.py
 mido/tokenizer.py
 mido/version.py
 mido.egg-info/PKG-INFO
 mido.egg-info/SOURCES.txt
 mido.egg-info/dependency_links.txt
-mido.egg-info/not-zip-safe
+mido.egg-info/entry_points.txt
 mido.egg-info/requires.txt
 mido.egg-info/top_level.txt
 mido/backends/__init__.py
 mido/backends/_parser_queue.py
 mido/backends/amidi.py
 mido/backends/backend.py
 mido/backends/portmidi.py
@@ -101,14 +109,19 @@
 mido/messages/specs.py
 mido/messages/strings.py
 mido/midifiles/__init__.py
 mido/midifiles/meta.py
 mido/midifiles/midifiles.py
 mido/midifiles/tracks.py
 mido/midifiles/units.py
+scripts/__init__.py
+scripts/mido_connect.py
+scripts/mido_play.py
+scripts/mido_ports.py
+scripts/mido_serve.py
 tests/test_frozen.py
 tests/test_parser.py
 tests/test_ports.py
 tests/test_sockets.py
 tests/test_syx.py
 tests/test_tokenizer.py
 tests/backends/test_backend.py
```

### Comparing `mido-1.2.9/bin/mido-connect` & `mido-1.3.0/scripts/mido_serve.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,50 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
-Forward all messages from one or more ports to server.
+Serve one or more output ports. Every message received on any of the
+connected sockets will be sent to every output port.
 """
 import argparse
+
 import mido
+from mido import sockets
+from mido.ports import MultiPort
+
 
 def parse_args():
     parser = argparse.ArgumentParser(description=__doc__)
     arg = parser.add_argument
 
     arg('address',
         metavar='ADDRESS',
-        help='host:port to connect to')
+        help='host:port to serve on')
 
     arg('ports',
         metavar='PORT',
         nargs='+',
-        help='input ports to listen to')
+        help='output port to serve')
 
     return parser.parse_args()
 
-args = parse_args()
 
-try:
-    hostname, port = mido.sockets.parse_address(args.address)
-    ports = [mido.open_input(name) for name in args.ports]
-
-    with mido.sockets.connect(hostname, port) as server_port:
-        print('Connected.')
-        for message in mido.ports.multi_receive(ports):
-            print('Sending {}'.format(message))
-            server_port.send(message)
-except KeyboardInterrupt:
-    pass
+def main():
+    args = parse_args()
+
+    try:
+        out = MultiPort([mido.open_output(name) for name in args.ports])
+
+        (hostname, port) = sockets.parse_address(args.address)
+        with sockets.PortServer(hostname, port) as server:
+            for message in server:
+                print(f'Received {message}')
+                out.send(message)
+    except KeyboardInterrupt:
+        pass
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `mido-1.2.9/bin/mido-play` & `mido-1.3.0/scripts/mido_play.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-#!/usr/bin/env python
-"""                                                                            
+#!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
+"""
 Play MIDI file on output port.
 
 Example:
 
     mido-play some_file.mid
 
 Todo:
 
   - add option for printing messages
 """
-from __future__ import print_function, division
-import sys
 import argparse
+import sys
+
 import mido
 from mido import MidiFile, Message, tempo2bpm
 
+
 def parse_args():
     parser = argparse.ArgumentParser(description=__doc__)
     arg = parser.add_argument
 
     arg('-o', '--output-port',
         help='Mido port to send output to')
 
@@ -40,24 +46,24 @@
         nargs='+',
         help='MIDI file to play')
 
     return parser.parse_args()
 
 
 def play_file(output, filename, print_messages):
-    midi_file = MidiFile(filename) 
+    midi_file = MidiFile(filename)
 
-    print('Playing {}.'.format(midi_file.filename))
+    print(f'Playing {midi_file.filename}.')
     length = midi_file.length
     print('Song length: {} minutes, {} seconds.'.format(
-            int(length / 60),
-            int(length % 60)))
+        int(length / 60),
+        int(length % 60)))
     print('Tracks:')
     for i, track in enumerate(midi_file.tracks):
-        print('  {:2d}: {!r}'.format(i, track.name.strip()))
+        print(f'  {i:2d}: {track.name.strip()!r}')
 
     for message in midi_file.play(meta_messages=True):
         if print_messages:
             sys.stdout.write(repr(message) + '\n')
             sys.stdout.flush()
 
         if isinstance(message, Message):
@@ -66,27 +72,29 @@
             print('Tempo changed to {:.1f} BPM.'.format(
                 tempo2bpm(message.tempo)))
 
     print()
 
 
 def main():
+    args = parse_args()
+
+    if args.quiet:
+        def print(*args):
+            pass
+
     try:
         with mido.open_output(args.output_port) as output:
-            print('Using output {!r}.'.format(output.name))
+            print(f'Using output {output.name!r}.')
             output.reset()
             try:
                 for filename in args.files:
                     play_file(output, filename, args.print_messages)
             finally:
                 print()
                 output.reset()
     except KeyboardInterrupt:
         pass
 
-args = parse_args()
-
-if args.quiet:
-    def print(*args):
-        pass
 
-main()
+if __name__ == '__main__':
+    main()
```

### Comparing `mido-1.2.9/extras/hid_joystick.py` & `mido-1.3.0/extras/hid_joystick.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """Read from /dev/input/js0 and return as dictionaries.
 
 If you have pygame it is easier and more portable to do something
 like::
 
     import pygame.joystick
     from pygame.event import event_name
@@ -39,15 +43,15 @@
 f0 fb 37 09 00 00 82 00
 f0 fb 37 09 00 00 82 01
 f0 fb 37 09 00 00 82 02
 f0 fb 37 09 00 00 82 03
 f0 fb 37 09 00 00 82 04
 f0 fb 37 09 00 00 82 05
             --+--  |
-              |    1 = button, 2 = 
+              |    1 = button, 2 =
               |
             value (little endian unsigned)
 
         button down
              |
 98 f0 2f 09 01 00 01 00   1 down
 08 fa 2f 09 00 00 01 00   1 up
@@ -77,54 +81,57 @@
 import struct
 import select
 
 JS_EVENT_BUTTON = 0x1
 JS_EVENT_AXIS = 0x2
 JS_EVENT_INIT = 0x80
 
+
 def read_event(device):
     data = device.read(8)
 
     event = {}
 
     (event['time'],
      event['value'],
      event['type'],
      event['number']) = struct.unpack('IhBB', data)
 
     event['init'] = bool(event['type'] & JS_EVENT_INIT)
     event['type'] &= 0x7f  # Strip away the flag bits (JS_EVENT_INIT etc.)
     if event['type'] != JS_EVENT_BUTTON:
-        
         event['normalized_value'] = \
             float(event['value']) / 0x7fff  # Normalize to -1..1
 
     event['type'] = {1: 'button', 2: 'axis'}[event['type']]
-    
+
     return event
 
+
 def read_events(device_name):
     with open(device_name, 'rb') as device:
         while True:
             yield read_event(device)
 
+
 def panic(port):
     """
     Send "All Notes Off" and "Reset All Controllers" on
     all channels.
     """
     for channel in range(16):
         for control in [121, 123]:
             message = mido.Message('control_change',
                                    channel=channel,
                                    control=control, value=0)
             print(message)
             port.send(message)
 
-class Monophonic(object):
+
+class Monophonic:
     # Todo: this assumes everything is on channel 0!
 
     def __init__(self, output, channel=0):
         self.output = output
         self.notes = set()
         self.current_note = None
         self.channel = channel
@@ -197,14 +204,15 @@
 
         # elif event['type'] == 'axis':
         #     if event['number'] == 0:
         #         pitch_scale = mido.messages.MAX_PITCHWHEEL
         #         pitch = int(event['normalized_value'] * pitch_scale)
         #         out.send(mido.Message('pitchwheel', pitch=pitch))
 
+
 def play_drums(dev, out):
     # http://www.midi.org/techspecs/gm1sound.php
     note_mapping = {
         2: 35,  # Acoustic Bass Drum
         6: 38,  # Acoustic Snare
         1: 41,  # Low Floor Tom
         4: 47,  # Low Mid Tom
@@ -212,15 +220,15 @@
         8: 51,  # Ride Cymbal
 
         5: 42,  # Closed Hi Hat
         7: 46,  # Open Hi Hat
 
         9: 52,  # Chinese Cymbal
         10: 55,  # Splash Cymbal
-        }
+    }
 
     while True:
         event = read_event(dev)
         if event['init']:
             continue
 
         if event['type'] == 'button':
@@ -230,15 +238,15 @@
             if button not in note_mapping:
                 continue
 
             if event['value']:
                 type_ = 'note_on'
             else:
                 type_ = 'note_off'
-            
+
             note = note_mapping[button]
 
             message = mido.Message(type_, channel=9, note=note, velocity=64)
             print(message)
             out.send(message)
```

### Comparing `mido-1.2.9/examples/midifiles/play_midi_file.py` & `mido-1.3.0/examples/midifiles/play_midi_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,38 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Play MIDI file on output port.
 
 Run with (for example):
 
     ./play_midi_file.py 'SH-201 MIDI 1' 'test.mid'
 """
 import sys
+import time
+
 import mido
 from mido import MidiFile
 
 filename = sys.argv[1]
 if len(sys.argv) == 3:
     portname = sys.argv[2]
 else:
     portname = None
 
 with mido.open_output(portname) as output:
     try:
-        for message in MidiFile(filename).play():
+        midifile = MidiFile(filename)
+        t0 = time.time()
+        for message in midifile.play():
             print(message)
             output.send(message)
+        print('play time: {:.2f} s (expected {:.2f})'.format(
+            time.time() - t0, midifile.length))
 
     except KeyboardInterrupt:
         print()
         output.reset()
```

### Comparing `mido-1.2.9/examples/backends/use_printer.py` & `mido-1.3.0/examples/backends/use_printer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+# SPDX-FileCopyrightText: 2014 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Try out the new printer port backend.
 
 It also works with MIDO_BACKEND, so you can do:
 
     $ MIDO_BACKEND=printer python
     >>> import mido
     >>> mido.get_output_names()
     ['The Printer Port']
 """
 import mido
 
 mido.set_backend('printer')
 
-print('Available outputs: {!r}'.format(mido.get_output_names()))
+print(f'Available outputs: {mido.get_output_names()!r}')
 
 with mido.open_output() as port:
-    print('Using {}.'.format(port))
+    print(f'Using {port}.')
 
     port.send(mido.Message('program_change', program=10))
     for i in [1, 2, 3]:
         port.send(mido.Message('control_change', control=1, value=i))
```

### Comparing `mido-1.2.9/examples/backends/rtm.py` & `mido-1.3.0/examples/backends/rtm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Experimental backend for rtmidi-python:
 
 http://github.com/superquadratic/rtmidi-python
 
 - Doesn't work with Python 3.3:
 
@@ -12,16 +16,16 @@
 - Virtual ports don't show up, so other programs can't connect to them.
 
 - There is no way to select API.
 
 Other than that, it works exactly like the included python-rtmidi
 backend.
 """
-from __future__ import absolute_import
 import rtmidi_python as rtmidi
+
 from mido.ports import BaseInput, BaseOutput
 
 
 def get_devices():
     devices = []
 
     input_names = set(rtmidi.MidiIn().ports)
@@ -33,67 +37,68 @@
             'is_input': name in input_names,
             'is_output': name in output_names,
         })
 
     return devices
 
 
-class PortCommon(object):
+class PortCommon:
     def _open(self, virtual=False, callback=None):
         opening_input = hasattr(self, 'receive')
 
         if opening_input:
             self._rt = rtmidi.MidiIn()
             self._rt.ignore_types(False, False, False)
             if callback:
                 def callback_wrapper(message, delta_time):
                     self._parser.feed(message)
                     for message in self._parser:
                         callback(message)
+
                 self._rt.callback = self._callback = callback_wrapper
                 self._has_callback = True
             else:
                 self._has_callback = False
         else:
             self._rt = rtmidi.MidiOut()
             # Turn of ignore of sysex, time and active_sensing.
 
         ports = self._rt.ports
 
         if virtual:
             if self.name is None:
-                raise IOError('virtual port must have a name')
+                raise OSError('virtual port must have a name')
             self._rt.open_virtual_port(self.name)
         else:
             if self.name is None:
                 # Todo: this could fail if list is empty.
                 # In RtMidi, the default port is the first port.
                 try:
                     self.name = ports[0]
                 except IndexError:
-                    raise IOError('no ports available')
+                    raise OSError('no ports available')
 
             try:
                 port_id = ports.index(self.name)
             except ValueError:
-                raise IOError('unknown port {!r}'.format(self.name))
+                raise OSError(f'unknown port {self.name!r}')
 
             self._rt.open_port(port_id)
 
         self._device_type = 'rtmidi_python'
 
     def _close(self):
         self._rt.close_port()
 
 
 class Input(PortCommon, BaseInput):
     # Todo: sysex messages do not arrive here.
     def _receive(self, block=True):
         if self._has_callback:
-            raise IOError('a callback is currently set for this port')
+            raise OSError('a callback is currently set for this port')
 
         while True:
             (message, delta_time) = self._rt.get_message()
             if message is None:
                 break
             else:
                 self._parser.feed(message)
```

### Comparing `mido-1.2.9/examples/backends/printer.py` & `mido-1.3.0/examples/backends/printer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 A simple custom backend with an output port type which prints messages
 to stdout.
 """
 from mido.ports import BaseOutput
 
 
@@ -14,11 +18,11 @@
 class Output(BaseOutput):
     def _open(self, **kwargs):
         device = get_devices()[0]
 
         if self.name is None:
             self.name = device['name']
         elif self.name != device['name']:
-            raise ValueError('unknown port {!r}'.format(self.name))
+            raise ValueError(f'unknown port {self.name!r}')
 
     def _send(self, message):
         print(message)
```

### Comparing `mido-1.2.9/examples/ports/send.py` & `mido-1.3.0/examples/ports/send.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Send random notes to the output port.
 """
 
-from __future__ import print_function
+import random
 import sys
 import time
-import random
+
 import mido
 from mido import Message
 
-
 if len(sys.argv) > 1:
     portname = sys.argv[1]
 else:
     portname = None  # Use default port
 
 # A pentatonic scale
 notes = [60, 62, 64, 67, 69, 72]
 
 try:
     with mido.open_output(portname, autoreset=True) as port:
-        print('Using {}'.format(port))
+        print(f'Using {port}')
         while True:
             note = random.choice(notes)
 
             on = Message('note_on', note=note)
-            print('Sending {}'.format(on))
+            print(f'Sending {on}')
             port.send(on)
             time.sleep(0.05)
 
             off = Message('note_off', note=note)
-            print('Sending {}'.format(off))
+            print(f'Sending {off}')
             port.send(off)
             time.sleep(0.1)
 except KeyboardInterrupt:
     pass
 
 print()
```

### Comparing `mido-1.2.9/examples/ports/queue_port.py` & `mido-1.3.0/examples/ports/queue_port.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """A port interface around a queue.
 
 This allows you to create internal ports to send messages between threads.
 """
+import queue
+
 import mido
 from mido import ports
 
-try:
-    import queue
-except ImportError:
-    # Python 2.
-    import Queue as queue
-
 
 class QueuePort(ports.BaseIOPort):
     # We don't need locking since the queue takes care of that.
     _locking = False
 
     def _open(self):
         self.queue = queue.Queue()
```

### Comparing `mido-1.2.9/examples/ports/nonblocking_receive.py` & `mido-1.3.0/examples/ports/nonblocking_receive.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Example of non-blocking reception from input port.
 """
-from __future__ import print_function
 import sys
 import time
+
 import mido
 
 if len(sys.argv) > 1:
     portname = sys.argv[1]
 else:
     portname = None  # Use default port
 
 try:
     with mido.open_input(portname) as port:
-        print('Using {}'.format(port))
+        print(f'Using {port}')
         while True:
             for message in port.iter_pending():
-                print('Received {}'.format(message))
+                print(f'Received {message}')
 
             print('Doing something else for a while...')
             time.sleep(0.5)
 except KeyboardInterrupt:
     pass
```

### Comparing `mido-1.2.9/mido/frozen.py` & `mido-1.3.0/mido/frozen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from .messages import Message
 from .midifiles import MetaMessage, UnknownMetaMessage
 
 
-class Frozen(object):
-    def __repr__(self):
-        text = super(Frozen, self).__repr__()
-        return '<frozen {}'.format(text[1:])
-
+class Frozen:
     def __setattr__(self, *_):
         raise ValueError('frozen message is immutable')
 
     def __hash__(self):
         return hash(tuple(sorted(vars(self).items())))
 
 
@@ -19,15 +19,16 @@
 
 
 class FrozenMetaMessage(Frozen, MetaMessage):
     pass
 
 
 class FrozenUnknownMetaMessage(Frozen, UnknownMetaMessage):
-    pass
+    def __repr__(self):
+        return 'Frozen' + UnknownMetaMessage.__repr__(self)
 
 
 def is_frozen(msg):
     """Return True if message is frozen, otherwise False."""
     return isinstance(msg, Frozen)
```

### Comparing `mido-1.2.9/mido/midifiles/tracks.py` & `mido-1.3.0/mido/midifiles/tracks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from .meta import MetaMessage
 
 
 class MidiTrack(list):
     @property
     def name(self):
         """Name of the track.
@@ -47,15 +51,21 @@
     def __add__(self, other):
         return self.__class__(list.__add__(self, other))
 
     def __mul__(self, other):
         return self.__class__(list.__mul__(self, other))
 
     def __repr__(self):
-        return '<midi track {!r} {} messages>'.format(self.name, len(self))
+        if len(self) == 0:
+            messages = ''
+        elif len(self) == 1:
+            messages = f'[{self[0]}]'
+        else:
+            messages = '[\n  {}]'.format(',\n  '.join(repr(m) for m in self))
+        return f'{self.__class__.__name__}({messages})'
 
 
 def _to_abstime(messages):
     """Convert messages to absolute time."""
     now = 0
     for msg in messages:
         now += msg.time
```

### Comparing `mido-1.2.9/mido/midifiles/midifiles.py` & `mido-1.3.0/mido/midifiles/midifiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 MIDI file reading and playback.
 
 References:
 
 http://home.roadrunner.com/~jgglatt/
 http://home.roadrunner.com/~jgglatt/tech/miditech.htm
@@ -11,27 +15,25 @@
 http://www.ccarh.org/courses/253/assignment/midifile/
 https://code.google.com/p/binasc/wiki/mainpage
 http://stackoverflow.com/questions/2984608/midi-delta-time
 http://www.recordingblogs.com/sa/tabid/82/EntryId/44/MIDI-Part-XIII-Delta-time-a
 http://www.sonicspot.com/guide/midifiles.html
 """
 
-from __future__ import print_function, division
 import io
-import time
 import string
 import struct
+import time
 from numbers import Integral
 
-from ..messages import Message, SPEC_BY_STATUS
 from .meta import (MetaMessage, build_meta_message, meta_charset,
                    encode_variable_int)
-
 from .tracks import MidiTrack, merge_tracks, fix_end_of_track
 from .units import tick2second
+from ..messages import Message, SPEC_BY_STATUS
 
 # The default tempo is 120 BPM.
 # (500000 microseconds per beat (quarter note).)
 DEFAULT_TEMPO = 500000
 DEFAULT_TICKS_PER_BEAT = 480
 
 # Maximum message length to attempt to read.
@@ -39,30 +41,25 @@
 
 
 def print_byte(byte, pos=0):
     char = chr(byte)
     if char.isspace() or char not in string.printable:
         char = '.'
 
-    print('  {:06x}: {:02x}  {}'.format(pos, byte, char))
+    print(f'  {pos:06x}: {byte:02x}  {char}')
 
 
-class DebugFileWrapper(object):
+class DebugFileWrapper:
     def __init__(self, file):
         self.file = file
 
     def read(self, size):
         data = self.file.read(size)
 
         for byte in data:
-            # Iterating gives us byte strings instead of ints in
-            # Python 2.
-            if isinstance(byte, str):
-                byte = ord(byte)
-
             print_byte(byte, self.file.tell())
 
         return data
 
     def tell(self):
         return self.file.tell()
 
@@ -73,15 +70,15 @@
         raise EOFError
     else:
         return ord(byte)
 
 
 def read_bytes(infile, size):
     if size > MAX_MESSAGE_LENGTH:
-        raise IOError('Message length {} exceeds maximum length {}'.format(
+        raise OSError('Message length {} exceeds maximum length {}'.format(
             size, MAX_MESSAGE_LENGTH))
     return [read_byte(infile) for _ in range(size)]
 
 
 def _dbg(text=''):
     print(text)
 
@@ -104,55 +101,58 @@
     return struct.unpack('>4sL', header)
 
 
 def read_file_header(infile):
     name, size = read_chunk_header(infile)
 
     if name != b'MThd':
-        raise IOError('MThd not found. Probably not a MIDI file')
+        raise OSError('MThd not found. Probably not a MIDI file')
     else:
         data = infile.read(size)
 
         if len(data) < 6:
             raise EOFError
 
         return struct.unpack('>hhh', data[:6])
 
 
 def read_message(infile, status_byte, peek_data, delta, clip=False):
     try:
         spec = SPEC_BY_STATUS[status_byte]
     except LookupError:
-        raise IOError('undefined status byte 0x{:02x}'.format(status_byte))
+        raise OSError(f'undefined status byte 0x{status_byte:02x}')
 
     # Subtract 1 for status byte.
     size = spec['length'] - 1 - len(peek_data)
     data_bytes = peek_data + read_bytes(infile, size)
 
     if clip:
         data_bytes = [byte if byte < 127 else 127 for byte in data_bytes]
     else:
         for byte in data_bytes:
             if byte > 127:
-                raise IOError('data byte must be in range 0..127')
+                raise OSError('data byte must be in range 0..127')
 
     return Message.from_bytes([status_byte] + data_bytes, time=delta)
 
 
-def read_sysex(infile, delta):
+def read_sysex(infile, delta, clip=False):
     length = read_variable_int(infile)
     data = read_bytes(infile, length)
 
     # Strip start and end bytes.
     # TODO: is this necessary?
     if data and data[0] == 0xf0:
         data = data[1:]
     if data and data[-1] == 0xf7:
         data = data[:-1]
 
+    if clip:
+        data = [byte if byte < 127 else 127 for byte in data]
+
     return Message('sysex', data=data, time=delta)
 
 
 def read_variable_int(infile):
     delta = 0
 
     while True:
@@ -171,18 +171,18 @@
 
 def read_track(infile, debug=False, clip=False):
     track = MidiTrack()
 
     name, size = read_chunk_header(infile)
 
     if name != b'MTrk':
-        raise IOError('no MTrk header at start of track')
+        raise OSError('no MTrk header at start of track')
 
     if debug:
-        _dbg('-> size={}'.format(size))
+        _dbg(f'-> size={size}')
         _dbg()
 
     start = infile.tell()
     last_status = None
 
     while True:
         # End of track reached.
@@ -191,42 +191,42 @@
 
         if debug:
             _dbg('Message:')
 
         delta = read_variable_int(infile)
 
         if debug:
-            _dbg('-> delta={}'.format(delta))
+            _dbg(f'-> delta={delta}')
 
         status_byte = read_byte(infile)
 
         if status_byte < 0x80:
             if last_status is None:
-                raise IOError('running status without last_status')
+                raise OSError('running status without last_status')
             peek_data = [status_byte]
             status_byte = last_status
         else:
             if status_byte != 0xff:
                 # Meta messages don't set running status.
                 last_status = status_byte
             peek_data = []
 
         if status_byte == 0xff:
             msg = read_meta_message(infile, delta)
         elif status_byte in [0xf0, 0xf7]:
             # TODO: I'm not quite clear on the difference between
             # f0 and f7 events.
-            msg = read_sysex(infile, delta)
+            msg = read_sysex(infile, delta, clip)
         else:
             msg = read_message(infile, status_byte, peek_data, delta, clip)
 
         track.append(msg)
 
         if debug:
-            _dbg('-> {!r}'.format(msg))
+            _dbg(f'-> {msg!r}')
             _dbg()
 
     return track
 
 
 def write_chunk(outfile, name, data):
     """Write an IFF chunk to the file.
@@ -240,14 +240,16 @@
 def write_track(outfile, track):
     data = bytearray()
 
     running_status_byte = None
     for msg in fix_end_of_track(track):
         if not isinstance(msg.time, Integral):
             raise ValueError('message time must be int in MIDI file')
+        if msg.time < 0:
+            raise ValueError('message time must be non-negative in MIDI file')
 
         if msg.is_realtime:
             raise ValueError('realtime messages are not allowed in MIDI files')
 
         data.extend(encode_variable_int(msg.time))
 
         if msg.is_meta:
@@ -284,51 +286,62 @@
     # this is:
     #
     #    (500000 / 1000000) / 480 == 0.5 / 480 == 0.0010417
     #
     return (tempo / 1000000.0) / ticks_per_beat
 
 
-class MidiFile(object):
+class MidiFile:
     def __init__(self, filename=None, file=None,
                  type=1, ticks_per_beat=DEFAULT_TICKS_PER_BEAT,
                  charset='latin1',
                  debug=False,
-                 clip=False
+                 clip=False,
+                 tracks=None
                  ):
 
         self.filename = filename
         self.type = type
         self.ticks_per_beat = ticks_per_beat
         self.charset = charset
         self.debug = debug
         self.clip = clip
 
         self.tracks = []
 
         if type not in range(3):
             raise ValueError(
-                'invalid format {} (must be 0, 1 or 2)'.format(format))
+                f'invalid format {format} (must be 0, 1 or 2)')
 
-        if file is not None:
+        if tracks is not None:
+            self.tracks = tracks
+        elif file is not None:
             self._load(file)
         elif self.filename is not None:
-            with io.open(filename, 'rb') as file:
+            with open(filename, 'rb') as file:
                 self._load(file)
+        # merge tracks at load time to prevent timing error on
+        # first call to __iter__()
+        if self.type != 2:
+            self.merged_track = merge_tracks(self.tracks)
 
     def add_track(self, name=None):
         """Add a new track to the file.
 
         This will create a new MidiTrack object and append it to the
         track list.
         """
         track = MidiTrack()
         if name is not None:
             track.name = name
         self.tracks.append(track)
+        # merge new track immediately to prevent timing error on
+        # first call to __iter__()
+        if self.type != 2:
+            self.merged_track = merge_tracks(self.tracks)
         return track
 
     def _load(self, infile):
         if self.debug:
             infile = DebugFileWrapper(infile)
 
         with meta_charset(self.charset):
@@ -342,15 +355,15 @@
             if self.debug:
                 _dbg('-> type={}, tracks={}, ticks_per_beat={}'.format(
                     self.type, num_tracks, self.ticks_per_beat))
                 _dbg()
 
             for i in range(num_tracks):
                 if self.debug:
-                    _dbg('Track {}:'.format(i))
+                    _dbg(f'Track {i}:')
 
                 self.tracks.append(read_track(infile,
                                               debug=self.debug,
                                               clip=self.clip))
                 # TODO: used to ignore EOFError. I hope things still work.
 
     @property
@@ -369,46 +382,57 @@
     def __iter__(self):
         # The tracks of type 2 files are not in sync, so they can
         # not be played back like this.
         if self.type == 2:
             raise TypeError("can't merge tracks in type 2 (asynchronous) file")
 
         tempo = DEFAULT_TEMPO
-        for msg in merge_tracks(self.tracks):
+        for msg in self.merged_track:
             # Convert message time from absolute time
             # in ticks to relative time in seconds.
             if msg.time > 0:
                 delta = tick2second(msg.time, self.ticks_per_beat, tempo)
             else:
                 delta = 0
 
             yield msg.copy(time=delta)
 
             if msg.type == 'set_tempo':
                 tempo = msg.tempo
 
-    def play(self, meta_messages=False):
+    def play(self, meta_messages=False, now=time.time):
         """Play back all tracks.
 
         The generator will sleep between each message by
         default. Messages are yielded with correct timing. The time
         attribute is set to the number of seconds slept since the
         previous message.
 
         By default you will only get normal MIDI messages. Pass
         meta_messages=True if you also want meta messages.
 
         You will receive copies of the original messages, so you can
         safely modify them without ruining the tracks.
 
+        By default the system clock is used for the timing of yielded
+        MIDI events. To use a different clock (e.g. to synchronize to
+        an audio stream), pass now=time_fn where time_fn is a zero
+        argument function that yields the current time in seconds.
         """
-        sleep = time.sleep
+        start_time = now()
+        input_time = 0.0
 
         for msg in self:
-            sleep(msg.time)
+            input_time += msg.time
+
+            playback_time = now() - start_time
+            duration_to_next_event = input_time - playback_time
+
+            if duration_to_next_event > 0.0:
+                time.sleep(duration_to_next_event)
 
             if isinstance(msg, MetaMessage) and not meta_messages:
                 continue
             else:
                 yield msg
 
     def save(self, filename=None, file=None):
@@ -424,15 +448,15 @@
         """
         if self.type == 0 and len(self.tracks) != 1:
             raise ValueError('type 0 file must have exactly 1 track')
 
         if file is not None:
             self._save(file)
         elif filename is not None:
-            with io.open(filename, 'wb') as file:
+            with open(filename, 'wb') as file:
                 self._save(file)
         else:
             raise ValueError('requires filename or file')
 
     def _save(self, outfile):
         with meta_charset(self.charset):
             header = struct.pack('>hhh', self.type,
@@ -450,25 +474,35 @@
         May take argument meta_only to show only meta messages.
 
         Use:
         print_tracks() -> will print all messages
         print_tracks(meta_only=True) -> will print only MetaMessages
         """
         for i, track in enumerate(self.tracks):
-            print('=== Track {}'.format(i))
+            print(f'=== Track {i}')
             for msg in track:
                 if not isinstance(msg, MetaMessage) and meta_only:
                     pass
                 else:
-                    print('{!r}'.format(msg))
+                    print(f'{msg!r}')
 
     def __repr__(self):
-        return '<midi file {!r} type {}, {} tracks, {} messages>'.format(
-            self.filename, self.type, len(self.tracks),
-            sum([len(track) for track in self.tracks]))
+        if self.tracks:
+            tracks_str = ',\n'.join(repr(track) for track in self.tracks)
+            tracks_str = '  ' + tracks_str.replace('\n', '\n  ')
+            tracks_str = f', tracks=[\n{tracks_str}\n]'
+        else:
+            tracks_str = ''
+
+        return '{}(type={}, ticks_per_beat={}{})'.format(
+            self.__class__.__name__,
+            self.type,
+            self.ticks_per_beat,
+            tracks_str,
+        )
 
     # The context manager has no purpose but is kept around since it was
     # used in examples in the past.
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
```

### Comparing `mido-1.2.9/mido/midifiles/meta.py` & `mido-1.3.0/mido/midifiles/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Meta messages for MIDI files.
 
 TODO:
      - what if an unknown meta message is implemented and someone depends on
        the 'data' attribute?
      - is 'type_byte' a good name?
      - 'values' is not a good name for a dictionary.
      - type and value safety?
      - copy().
      - expose _key_signature_encode/decode?
 """
-from __future__ import print_function, division
 import math
 import struct
-from numbers import Integral
 from contextlib import contextmanager
+from numbers import Integral
+
 from ..messages import BaseMessage, check_time
-from ..py2 import PY2
 
 _charset = 'latin1'
 
 
 class KeySignatureError(Exception):
     """ Raised when key cannot be converted from key/mode to key letter """
     pass
@@ -82,38 +85,38 @@
                'ushort': 'hH',
                'ulong': 'lL'
                }
 
     try:
         pack_format, unpack_format = formats[to_type]
     except KeyError:
-        raise ValueError('invalid integer type {}'.format(to_type))
+        raise ValueError(f'invalid integer type {to_type}')
 
     try:
         packed = struct.pack(pack_format, n)
         return struct.unpack(unpack_format, packed)[0]
     except struct.error as err:
         raise ValueError(*err.args)
 
 
 def unsigned(to_type, n):
-    return signed('u{}'.format(to_type), n)
+    return signed(f'u{to_type}', n)
 
 
 def encode_variable_int(value):
     """Encode variable length integer.
 
     Returns the integer as a list of bytes,
     where the last byte is < 128.
 
     This is used for delta times and meta message payload
     length.
     """
     if not isinstance(value, Integral) or value < 0:
-        raise ValueError('variable int must be a positive integer')
+        raise ValueError('variable int must be a non-negative integer')
 
     bytes = []
     while value:
         bytes.append(value & 0x7f)
         value >>= 7
 
     if bytes:
@@ -123,14 +126,28 @@
         for i in range(len(bytes) - 1):
             bytes[i] |= 0x80
         return bytes
     else:
         return [0]
 
 
+def decode_variable_int(value):
+    """Decode a list to a variable length integer.
+
+    Does the opposite of encode_variable_int(value)
+    """
+    for i in range(len(value) - 1):
+        value[i] &= ~0x80
+    val = 0
+    for i in value:
+        val <<= 7
+        val |= i
+    return val
+
+
 def encode_string(string):
     return list(bytearray(string.encode(_charset)))
 
 
 def decode_string(data):
     return bytearray(data).decode(_charset)
 
@@ -144,29 +161,23 @@
     _charset = old
 
 
 def check_int(value, low, high):
     if not isinstance(value, Integral):
         raise TypeError('attribute must be an integer')
     elif not low <= value <= high:
-        raise ValueError('attribute must be in range {}..{}'.format(low, high))
-
-
-if PY2:
-    _STRING_TYPE = (str, unicode)  # noqa: F821
-else:
-    _STRING_TYPE = str
+        raise ValueError(f'attribute must be in range {low}..{high}')
 
 
 def check_str(value):
-    if not isinstance(value, _STRING_TYPE):
+    if not isinstance(value, str):
         raise TypeError('attribute must be a string')
 
 
-class MetaSpec(object):
+class MetaSpec:
     # The default is to do no checks.
     def check(self, name, value):
         pass
 
 
 class MetaSpec_sequence_number(MetaSpec):
     type_byte = 0x00
@@ -311,34 +322,34 @@
                   'frames',
                   'sub_frames'
                   ]
     # TODO: What are some good defaults?
     defaults = [24, 0, 0, 0, 0, 0]
 
     def decode(self, message, data):
-        message.frame_rate = _smpte_framerate_decode[(data[0] >> 6)]
-        message.hours = (data[0] & 0x3f)
+        message.frame_rate = _smpte_framerate_decode[(data[0] >> 5)]
+        message.hours = (data[0] & 0b0001_1111)
         message.minutes = data[1]
         message.seconds = data[2]
         message.frames = data[3]
         message.sub_frames = data[4]
 
     def encode(self, message):
-        frame_rate_lookup = _smpte_framerate_encode[message.frame_rate] << 6
+        frame_rate_lookup = _smpte_framerate_encode[message.frame_rate] << 5
         return [frame_rate_lookup | message.hours,
                 message.minutes,
                 message.seconds,
                 message.frames,
                 message.sub_frames]
 
     def check(self, name, value):
         if name == 'frame_rate':
             if value not in _smpte_framerate_encode:
                 valid = ', '.join(sorted(_smpte_framerate_encode.keys()))
-                raise ValueError('frame_rate must be one of {}'.format(valid))
+                raise ValueError(f'frame_rate must be one of {valid}')
         elif name == 'hours':
             check_int(value, 0, 255)
         elif name in ['minutes', 'seconds']:
             check_int(value, 0, 59)
         elif name == 'frames':
             check_int(value, 0, 255)
         elif name == 'sub_frames':
@@ -402,15 +413,15 @@
 
     def encode(self, message):
         key, mode = _key_signature_encode[message.key]
         return [unsigned('byte', key), mode]
 
     def check(self, name, value):
         if value not in _key_signature_encode:
-            raise ValueError('invalid key {!r}'.format(value))
+            raise ValueError(f'invalid key {value!r}')
 
 
 class MetaSpec_sequencer_specific(MetaSpec):
     type_byte = 0x7f
     attributes = ['data']
     defaults = [[]]
 
@@ -516,65 +527,70 @@
             if name == 'time':
                 check_time(value)
             else:
                 spec.check(name, value)
             self_vars[name] = value
 
         elif name in self_vars:
-            raise AttributeError('{} attribute is read only'.format(name))
+            raise AttributeError(f'{name} attribute is read only')
         else:
             raise AttributeError(
-                '{} message has no attribute {}'.format(self.type, name))
+                f'{self.type} message has no attribute {name}')
 
     __setattr__ = _setattr
 
     def bytes(self):
         spec = _META_SPEC_BY_TYPE[self.type]
         data = spec.encode(self)
 
-        return ([0xff, spec.type_byte] +
-                encode_variable_int(len(data)) +
-                data)
+        return ([0xff, spec.type_byte] + encode_variable_int(len(data)) + data)
 
-    def __repr__(self):
-        spec = _META_SPEC_BY_TYPE[self.type]
-        attributes = []
-        for name in spec.attributes:
-            attributes.append('{}={!r}'.format(name, getattr(self, name)))
-        attributes = ' '.join(attributes)
-        if attributes:
-            attributes = (' {}'.format(attributes))
+    @classmethod
+    def from_bytes(cls, msg_bytes):
+        if msg_bytes[0] != 0xff:
+            raise ValueError('bytes does not correspond to a MetaMessage.')
+        scan_end = 2
+        data = []
+        flag = True
+        while flag and scan_end < len(msg_bytes):
+            scan_end += 1
+            length_data = msg_bytes[2:scan_end]
+            length = decode_variable_int(length_data)
+            data = msg_bytes[scan_end:]
+            if length == len(data):
+                flag = False
+        if flag:
+            raise ValueError('Bad data. Cannot be converted to message.')
+        msg = build_meta_message(msg_bytes[1], data)
+        return msg
 
-        return '<meta message {}{} time={}>'.format(self.type,
-                                                    attributes, self.time)
+    def _get_value_names(self):
+        """Used by BaseMessage.__repr__()."""
+        spec = _META_SPEC_BY_TYPE[self.type]
+        return spec.attributes + ['time']
 
 
 class UnknownMetaMessage(MetaMessage):
-    def __init__(self, type_byte, data=None, time=0):
+    def __init__(self, type_byte, data=None, time=0, type='unknown_meta'):
         if data is None:
             data = ()
         else:
             data = tuple(data)
 
         vars(self).update({
-            'type': 'unknown_meta',
+            'type': type,
             'type_byte': type_byte,
             'data': data,
             'time': time})
 
     def __repr__(self):
-        return ('<unknown meta message'
-                ' type_byte=0x{:02x} '
-                'data={!r} time={}>').format(self.type_byte,
-                                             self.data,
-                                             self.time
-                                             )
+        fmt = 'UnknownMetaMessage(type_byte={}, data={}, time={})'
+        return fmt.format(self.type_byte, self.data, self.time)
 
     def __setattr__(self, name, value):
         # This doesn't do any checking.
         # It probably should.
         vars(self)[name] = value
 
     def bytes(self):
-        return ([0xff, self.type_byte] +
-                encode_variable_int(len(self.data)) +
-                list(self.data))
+        length = encode_variable_int(len(self.data))
+        return ([0xff, self.type_byte] + length + list(self.data))
```

### Comparing `mido-1.2.9/mido/backends/backend.py` & `mido-1.3.0/mido/backends/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+# SPDX-FileCopyrightText: 2014 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 import os
 import importlib
 from .. import ports
 
 DEFAULT_BACKEND = 'mido.backends.rtmidi'
 
 
-class Backend(object):
+class Backend:
     """
     Wrapper for backend module.
 
     A backend module implements classes for input and output ports for
     a specific MIDI library. The Backend object wraps around the
     object and provides convenient 'open_*()' and 'get_*_names()'
     functions.
@@ -68,15 +72,15 @@
             kwargs['api'] = self.api
         return kwargs
 
     def open_input(self, name=None, virtual=False, callback=None, **kwargs):
         """Open an input port.
 
         If the environment variable MIDO_DEFAULT_INPUT is set,
-        if will override the default port.
+        it will override the default port.
 
         virtual=False
           Passing True opens a new port that other applications can
           connect to. Raises IOError if not supported by the backend.
 
         callback=None
           A callback function to be called when a new message arrives.
@@ -90,15 +94,15 @@
 
         return self.module.Input(name, **self._add_api(kwargs))
 
     def open_output(self, name=None, virtual=False, autoreset=False, **kwargs):
         """Open an output port.
 
         If the environment variable MIDO_DEFAULT_OUTPUT is set,
-        if will override the default port.
+        it will override the default port.
 
         virtual=False
           Passing True opens a new port that other applications can
           connect to. Raises IOError if not supported by the backend.
 
         autoreset=False
           Automatically send all_notes_off and reset_all_controllers
@@ -112,15 +116,15 @@
         return self.module.Output(name, **self._add_api(kwargs))
 
     def open_ioport(self, name=None, virtual=False,
                     callback=None, autoreset=False, **kwargs):
         """Open a port for input and output.
 
         If the environment variable MIDO_DEFAULT_IOPORT is set,
-        if will override the default port.
+        it will override the default port.
 
         virtual=False
           Passing True opens a new port that other applications can
           connect to. Raises IOError if not supported by the backend.
 
         callback=None
           A callback function to be called when a new message arrives.
@@ -161,37 +165,38 @@
     def _get_devices(self, **kwargs):
         if hasattr(self.module, 'get_devices'):
             return self.module.get_devices(**self._add_api(kwargs))
         else:
             return []
 
     def get_input_names(self, **kwargs):
-        """Return a sorted list of all input port names."""
+        """Return a list of all input port names."""
         devices = self._get_devices(**self._add_api(kwargs))
         names = [device['name'] for device in devices if device['is_input']]
-        return list(sorted(names))
+        return names
 
     def get_output_names(self, **kwargs):
-        """Return a sorted list of all output port names."""
+        """Return a list of all output port names."""
         devices = self._get_devices(**self._add_api(kwargs))
         names = [device['name'] for device in devices if device['is_output']]
-        return list(sorted(names))
+        return names
 
     def get_ioport_names(self, **kwargs):
-        """Return a sorted list of all I/O port names."""
+        """Return a list of all I/O port names."""
         devices = self._get_devices(**self._add_api(kwargs))
         inputs = [device['name'] for device in devices if device['is_input']]
-        outputs = [device['name'] for device in devices if device['is_output']]
-        return sorted(set(inputs) & set(outputs))
+        outputs = {
+            device['name'] for device in devices if device['is_output']}
+        return [name for name in inputs if name in outputs]
 
     def __repr__(self):
         if self.loaded:
             status = 'loaded'
         else:
             status = 'not loaded'
 
         if self.api:
-            name = '{}/{}'.format(self.name, self.api)
+            name = f'{self.name}/{self.api}'
         else:
             name = self.name
 
-        return '<backend {} ({})>'.format(name, status)
+        return f'<backend {name} ({status})>'
```

### Comparing `mido-1.2.9/mido/backends/portmidi.py` & `mido-1.3.0/mido/backends/portmidi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Input and Output ports for PortMidi.
 
 There is no need to use this module directly. All you need is
 available in the toplevel module.
 
 PortMidi documentation:
 http://portmedia.sourceforge.net/portmidi/doxygen/
 """
+import ctypes
 import threading
 from ..ports import BaseInput, BaseOutput, sleep
 from . import portmidi_init as pm
 
 _state = {'port_count': 0}
 
 
@@ -25,24 +30,24 @@
 
 def _check_error(return_value):
     """Raise IOError if return_value < 0.
 
     The exception will be raised with the error message from PortMidi.
     """
     if return_value == pm.pmHostError:
-        raise IOError('PortMidi Host Error: '
+        raise OSError('PortMidi Host Error: '
                       '{}'.format(pm.get_host_error_message()))
     elif return_value < 0:
-        raise IOError(pm.lib.Pm_GetErrorText(return_value))
+        raise OSError(pm.lib.Pm_GetErrorText(return_value))
 
 
 def _get_device(device_id):
     info_pointer = pm.lib.Pm_GetDeviceInfo(device_id)
     if not info_pointer:
-        raise IOError('PortMidi device with id={} not found'.format(
+        raise OSError('PortMidi device with id={} not found'.format(
             device_id))
     info = info_pointer.contents
 
     return {
         'id': device_id,
         'interface': info.interface.decode('utf-8'),
         'name': info.name.decode('utf-8'),
@@ -55,15 +60,15 @@
 def _get_default_device(get_input):
     if get_input:
         device_id = pm.lib.Pm_GetDefaultInputDeviceID()
     else:
         device_id = pm.lib.Pm_GetDefaultOutputDeviceID()
 
     if device_id < 0:
-        raise IOError('no default port found')
+        raise OSError('no default port found')
 
     return _get_device(device_id)
 
 
 def _get_named_device(name, get_input):
     # Look for the device by name and type (input / output)
     for device in get_devices():
@@ -75,28 +80,28 @@
             if not device['is_input']:
                 continue
         else:
             if not device['is_output']:
                 continue
 
         if device['opened']:
-            raise IOError('port already opened: {!r}'.format(name))
+            raise OSError(f'port already opened: {name!r}')
 
         return device
     else:
-        raise IOError('unknown port {!r}'.format(name))
+        raise OSError(f'unknown port {name!r}')
 
 
 def get_devices(**kwargs):
     """Return a list of devices as dictionaries."""
     _refresh_port_list()
     return [_get_device(i) for i in range(pm.lib.Pm_CountDevices())]
 
 
-class PortCommon(object):
+class PortCommon:
     """
     Mixin with common things for input and output ports.
     """
     def _open(self, **kwargs):
         _refresh_port_list()
 
         if kwargs.get('virtual'):
@@ -112,28 +117,28 @@
             device = _get_named_device(self.name, self.is_input)
 
         if device['opened']:
             if self.is_input:
                 devtype = 'input'
             else:
                 devtype = 'output'
-            raise IOError('{} port {!r} is already open'.format(devtype,
+            raise OSError('{} port {!r} is already open'.format(devtype,
                                                                 self.name))
 
         if self.is_input:
             _check_error(pm.lib.Pm_OpenInput(
-                         pm.byref(self._stream),
+                         ctypes.byref(self._stream),
                          device['id'],  # Input device
                          pm.null,       # Input driver info
                          1000,          # Buffer size
                          pm.NullTimeProcPtr,  # Time callback
                          pm.null))      # Time info
         else:
             _check_error(pm.lib.Pm_OpenOutput(
-                         pm.byref(self._stream),
+                         ctypes.byref(self._stream),
                          device['id'],  # Output device
                          pm.null,       # Output diver info
                          0,             # Buffer size
                                         # (ignored when latency == 0?)
                          pm.NullTimeProcPtr,  # Default to internal clock
                          pm.null,       # Time info
                          0))            # Latency
```

### Comparing `mido-1.2.9/mido/backends/rtmidi.py` & `mido-1.3.0/mido/backends/rtmidi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """Backend for python-rtmidi:
 
 http://pypi.python.org/pypi/python-rtmidi/
 """
-from __future__ import absolute_import
 import threading
 
 import rtmidi
-from .. import ports
-from ..messages import Message
 from ._parser_queue import ParserQueue
 from .rtmidi_utils import expand_alsa_port_name
+from .. import ports
+from ..messages import Message
 
 
 def _get_api_lookup():
     api_to_name = {}
     name_to_api = {}
 
     for name in dir(rtmidi):
@@ -32,81 +35,87 @@
 def _get_api_id(name=None):
     if name is None:
         return rtmidi.API_UNSPECIFIED
 
     try:
         api = _name_to_api[name]
     except KeyError:
-        raise ValueError('unknown API {}'.format(name))
+        raise ValueError(f'unknown API {name}')
 
     if name in get_api_names():
         return api
     else:
-        raise ValueError('API {} not compiled in'.format(name))
+        raise ValueError(f'API {name} not compiled in')
 
 
 def get_devices(api=None, **kwargs):
-    devices = []
+    devices = {}
 
     rtapi = _get_api_id(api)
 
-    input_names = set(rtmidi.MidiIn(rtapi=rtapi).get_ports())
-    output_names = set(rtmidi.MidiOut(rtapi=rtapi).get_ports())
-
-    for name in sorted(input_names | output_names):
-        devices.append({'name': name,
-                        'is_input': name in input_names,
-                        'is_output': name in output_names,
-                        })
-
-    return devices
+    mi = rtmidi.MidiIn(rtapi=rtapi)
+    mo = rtmidi.MidiOut(rtapi=rtapi)
+    input_names = mi.get_ports()
+    output_names = mo.get_ports()
+
+    for name in input_names + output_names:
+        if name not in devices:
+            devices[name] = {
+                'name': name,
+                'is_input': name in input_names,
+                'is_output': name in output_names,
+            }
+
+    mi.delete()
+    mo.delete()
+    return list(devices.values())
 
 
 def get_api_names():
     return [_api_to_name[n] for n in rtmidi.get_compiled_api()]
 
 
 def _open_port(rt, name=None, client_name=None, virtual=False, api=None):
-
-    if api == 'LINUX_ALSA':
-        name = expand_alsa_port_name(rt.get_ports(), name)
-
     if client_name is not None:
         virtual = True
 
     if virtual:
         if name is None:
-            raise IOError('virtual port must have a name')
+            raise OSError('virtual port must have a name')
 
         rt.open_virtual_port(name)
         return name
 
+    if api == 'LINUX_ALSA':
+        name = expand_alsa_port_name(rt.get_ports(), name)
+
     port_names = rt.get_ports()
     if len(port_names) == 0:
-        raise IOError('no ports available')
+        raise OSError('no ports available')
 
     if name is None:
         name = port_names[0]
         port_id = 0
     elif name in port_names:
         port_id = port_names.index(name)
     else:
-        raise IOError('unknown port {!r}'.format(name))
+        raise OSError(f'unknown port {name!r}')
 
     try:
         rt.open_port(port_id)
     except RuntimeError as err:
-        raise IOError(*err.args)
+        raise OSError(*err.args)
 
     return name
 
 
-class PortCommon(object):
+class PortCommon:
     def _close(self):
         self._rt.close_port()
+        self._rt.delete()
 
 
 class Input(PortCommon, ports.BaseInput):
     _locking = False
 
     def _open(self, client_name=None, virtual=False,
               api=None, callback=None, **kwargs):
@@ -115,24 +124,30 @@
         self._callback_lock = threading.RLock()
         self._queue = ParserQueue()
 
         rtapi = _get_api_id(api)
         self._rt = rtmidi.MidiIn(name=client_name, rtapi=rtapi)
 
         self.api = _api_to_name[self._rt.get_current_api()]
-        self._device_type = 'RtMidi/{}'.format(self.api)
+        self._device_type = f'RtMidi/{self.api}'
 
         self.name = _open_port(self._rt, self.name, client_name=client_name,
                                virtual=virtual, api=self.api)
         self._rt.ignore_types(False, False, True)
         self.closed = False
 
         # We need to do this last when everything is set up.
         self.callback = callback
 
+    def _close(self):
+        # Deregister the callback before closing the port
+        # to prevent crashing another thread.
+        self.callback = None
+        super()._close()
+
     # We override receive() and poll() instead of _receive() and
     # _poll() to bypass locking.
     def receive(self, block=True):
         if block:
             return self._queue.get()
         else:
             return self._queue.poll()
@@ -172,23 +187,22 @@
 
 
 class Output(PortCommon, ports.BaseOutput):
     _locking = False
 
     def _open(self, client_name=None, virtual=False,
               api=None, callback=None, **kwargs):
-
         self.closed = True
         self._send_lock = threading.RLock()
 
         rtapi = _get_api_id(api)
         self._rt = rtmidi.MidiOut(name=client_name, rtapi=rtapi)
 
         self.api = _api_to_name[self._rt.get_current_api()]
-        self._device_type = 'RtMidi/{}'.format(self.api)
+        self._device_type = f'RtMidi/{self.api}'
 
         self.name = _open_port(self._rt, self.name, client_name=client_name,
                                virtual=virtual, api=self.api)
         self.closed = False
 
     # We override send() instead of _send() to bypass locking.
     def send(self, msg):
```

### Comparing `mido-1.2.9/mido/backends/pygame.py` & `mido-1.3.0/mido/backends/pygame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Mido ports for pygame.midi.
 
 Pygame uses PortMidi, so this is perhaps not very useful.
 
 http://www.pygame.org/docs/ref/midi.html
 """
 
-from __future__ import absolute_import
 from pygame import midi
 from ..ports import BaseInput, BaseOutput
 
 
 def _get_device(device_id):
     keys = ['interface', 'name', 'is_input', 'is_output', 'opened']
     info = dict(zip(keys, midi.get_device_info(device_id)))
@@ -23,15 +26,15 @@
 def _get_default_device(get_input):
     if get_input:
         device_id = midi.get_default_input_id()
     else:
         device_id = midi.get_default_output_id()
 
     if device_id < 0:
-        raise IOError('no default port found')
+        raise OSError('no default port found')
 
     return _get_device(device_id)
 
 
 def _get_named_device(name, get_input):
     # Look for the device by name and type (input / output)
     for device in get_devices():
@@ -43,30 +46,31 @@
             if device['is_output']:
                 continue
         else:
             if device['is_input']:
                 continue
 
         if device['opened']:
-            raise IOError('port already opened: {!r}'.format(name))
+            raise OSError(f'port already opened: {name!r}')
 
         return device
     else:
-        raise IOError('unknown port: {!r}'.format(name))
+        raise OSError(f'unknown port: {name!r}')
 
 
 def get_devices(**kwargs):
     midi.init()
     return [_get_device(device_id) for device_id in range(midi.get_count())]
 
 
-class PortCommon(object):
+class PortCommon:
     """
     Mixin with common things for input and output ports.
     """
+
     def _open(self, **kwargs):
         if kwargs.get('virtual'):
             raise ValueError('virtual ports are not supported'
                              ' by the Pygame backend')
         elif kwargs.get('callback'):
             raise ValueError('callbacks are not supported'
                              ' by the Pygame backend')
@@ -80,15 +84,15 @@
             device = _get_named_device(self.name, self.is_input)
 
         if device['opened']:
             if self.is_input:
                 devtype = 'input'
             else:
                 devtype = 'output'
-            raise IOError('{} port {!r} is already open'.format(devtype,
+            raise OSError('{} port {!r} is already open'.format(devtype,
                                                                 self.name))
         if self.is_input:
             self._port = midi.Input(device['id'])
         else:
             self._port = midi.Output(device['id'])
 
         self._device_type = 'Pygame/{}'.format(device['interface'])
@@ -97,28 +101,30 @@
         self._port.close()
 
 
 class Input(PortCommon, BaseInput):
     """
     PortMidi Input port
     """
+
     def _receive(self, block=True):
         # I get hanging notes if MAX_EVENTS > 1, so I'll have to
         # resort to calling Pm_Read() in a loop until there are no
         # more pending events.
 
         while self._port.poll():
             bytes, time = self._port.read(1)[0]
             self._parser.feed(bytes)
 
 
 class Output(PortCommon, BaseOutput):
     """
     PortMidi output port
     """
+
     def _send(self, message):
         if message.type == 'sysex':
             # Python 2 version of Pygame accepts a bytes or list here
             # while Python 3 version requires bytes.
             # According to the docs it should accept both so this may be
             # a bug in Pygame:
             # https://www.pygame.org/docs/ref/midi.html#pygame.midi.Output.write_sys_ex
```

### Comparing `mido-1.2.9/mido/backends/rtmidi_python.py` & `mido-1.3.0/mido/backends/rtmidi_python.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """Backend for rtmidi-python:
 
 https://pypi.python.org/pypi/rtmidi-python
 
 To use this backend copy (or link) it to somewhere in your Python path
 and call:
 
@@ -13,43 +17,40 @@
 
 * add support for APIs.
 
 * active_sensing is still filtered. (The same is true for
   mido.backends.rtmidi.)There may be a way to remove this filtering.
 
 """
-from __future__ import absolute_import
+import queue
+
 import rtmidi_python as rtmidi
 # TODO: change this to a relative import if the backend is included in
 # the package.
 from ..ports import BaseInput, BaseOutput
-from ..py2 import PY2
-
-if PY2:
-    import Queue as queue
-else:
-    import queue
 
 
 def get_devices(api=None, **kwargs):
-    devices = []
+    devices = {}
 
-    input_names = set(rtmidi.MidiIn().ports)
-    output_names = set(rtmidi.MidiOut().ports)
+    input_names = rtmidi.MidiIn().ports
+    output_names = rtmidi.MidiOut().ports
 
-    for name in sorted(input_names | output_names):
-        devices.append({'name': name,
-                        'is_input': name in input_names,
-                        'is_output': name in output_names,
-                        })
+    for name in input_names + output_names:
+        if name not in devices:
+            devices[name] = {
+                'name': name,
+                'is_input': name in input_names,
+                'is_output': name in output_names,
+            }
 
-    return devices
+    return list(devices.values())
 
 
-class PortCommon(object):
+class PortCommon:
     def _open(self, virtual=False, **kwargs):
 
         self._queue = queue.Queue()
         self._callback = None
 
         # rtapi = _get_api_id(api)
         opening_input = hasattr(self, 'receive')
@@ -62,40 +63,40 @@
             self._rt = rtmidi.MidiOut()  # rtapi=rtapi)
             # Turn of ignore of sysex, time and active_sensing.
 
         ports = self._rt.ports
 
         if virtual:
             if self.name is None:
-                raise IOError('virtual port must have a name')
+                raise OSError('virtual port must have a name')
             self._rt.open_virtual_port(self.name)
         else:
             if self.name is None:
                 # TODO: this could fail if list is empty.
                 # In RtMidi, the default port is the first port.
                 try:
                     self.name = ports[0]
                 except IndexError:
-                    raise IOError('no ports available')
+                    raise OSError('no ports available')
 
             try:
                 port_id = ports.index(self.name)
             except ValueError:
-                raise IOError('unknown port {!r}'.format(self.name))
+                raise OSError(f'unknown port {self.name!r}')
 
             try:
                 self._rt.open_port(port_id)
             except RuntimeError as err:
-                raise IOError(*err.args)
+                raise OSError(*err.args)
 
         # api = _api_to_name[self._rt.get_current_api()]
         api = ''
-        self._device_type = 'RtMidi/{}'.format(api)
+        self._device_type = f'RtMidi/{api}'
         if virtual:
-            self._device_type = 'virtual {}'.format(self._device_type)
+            self._device_type = f'virtual {self._device_type}'
 
     @property
     def callback(self):
         return self._callback
 
     @callback.setter
     def callback(self, func):
```

### Comparing `mido-1.2.9/mido/backends/amidi.py` & `mido-1.3.0/mido/backends/amidi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """Mido amidi backend
 
 Very experimental backend using amidi to access the ALSA rawmidi
 interface.
 
 TODO:
 
@@ -41,15 +45,15 @@
 
 
 def _get_device(name, mode):
     for dev in get_devices():
         if name == dev['name'] and dev[mode]:
             return dev
     else:
-        raise IOError('unknown port {!r}'.format(name))
+        raise OSError(f'unknown port {name!r}')
 
 
 class Input(PortMethods, InputMethods):
     def __init__(self, name=None, **kwargs):
         self.name = name
         self.closed = False
```

### Comparing `mido-1.2.9/mido/backends/rtmidi_utils.py` & `mido-1.3.0/mido/backends/rtmidi_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """Utility functions for RtMidi backend.
 
 These are in a separate file so they can be tested without
 the `python-rtmidi` package.
 
 """
```

### Comparing `mido-1.2.9/mido/sockets.py` & `mido-1.3.0/mido/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 MIDI over TCP/IP.
 """
 import socket
 import select
 from .parser import Parser
 from .ports import MultiPort, BaseIOPort
-from .py2 import PY2
 
 
 def _is_readable(socket):
     """Return True if there is data to be read on the socket."""
 
     timeout = 0
     (rlist, wlist, elist) = select.select(
@@ -83,48 +86,45 @@
         if conn is None:
             self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self._socket.setblocking(True)
             self._socket.connect((host, portno))
         else:
             self._socket = conn
 
-        if PY2:
-            kwargs = {'bufsize': 0}
-        else:
-            kwargs = {'buffering': None}
+        kwargs = {'buffering': 0}
 
         self._rfile = self._socket.makefile('rb', **kwargs)
         self._wfile = self._socket.makefile('wb', **kwargs)
 
     def _get_device_type(self):
         return 'socket'
 
     def _receive(self, block=True):
         while _is_readable(self._socket):
             try:
                 byte = self._rfile.read(1)
-            except socket.error as err:
-                raise IOError(err.args[1])
-            if byte == '':
+            except OSError as err:
+                raise OSError(err.args[1])
+            if len(byte) == 0:
                 # The other end has disconnected.
                 self.close()
                 break
             else:
                 self._parser.feed_byte(ord(byte))
 
     def _send(self, message):
         try:
             self._wfile.write(message.bin())
             self._wfile.flush()
-        except socket.error as err:
+        except OSError as err:
             if err.errno == 32:
                 # Broken pipe. The other end has disconnected.
                 self.close()
 
-            raise IOError(err.args[1])
+            raise OSError(err.args[1])
 
     def _close(self):
         self._socket.close()
 
 
 def connect(host, portno):
     """Connect to a socket port server.
@@ -155,8 +155,8 @@
     if not 0 < port < (2**16):
         raise ValueError('port number out of range')
 
     return (host, port)
 
 
 def format_address(host, portno):
-    return '{}{:d}'.format(host, portno)
+    return f'{host}{portno:d}'
```

### Comparing `mido-1.2.9/mido/syx.py` & `mido-1.3.0/mido/syx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+# SPDX-FileCopyrightText: 2014 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Read and write SYX file format
 """
-from __future__ import print_function
 import re
+
 from .parser import Parser
 
 
 def read_syx_file(filename):
     """Read sysex messages from SYX file.
 
     Returns a list of sysex messages.
@@ -21,17 +25,15 @@
 
     if len(data) == 0:
         # Empty file.
         return []
 
     parser = Parser()
 
-    # data[0] will give a byte string in Python 2 and an integer in
-    # Python 3.
-    if data[0] in (b'\xf0', 240):
+    if data[0] == 240:
         # Binary format.
         parser.feed(data)
     else:
         text = data.decode('latin1')
         data = bytearray.fromhex(re.sub(r'\s', ' ', text))
         parser.feed(data)
 
@@ -46,15 +48,15 @@
     By default this will write the binary format.  Pass
     ``plaintext=True`` to write the plain text format (hex encoded
     ASCII text).
     """
     messages = [m for m in messages if m.type == 'sysex']
 
     if plaintext:
-        with open(filename, 'wt') as outfile:
+        with open(filename, 'w') as outfile:
             for message in messages:
                 outfile.write(message.hex())
                 outfile.write('\n')
     else:
         with open(filename, 'wb') as outfile:
             for message in messages:
                 outfile.write(message.bin())
```

### Comparing `mido-1.2.9/mido/ports.py` & `mido-1.3.0/mido/ports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 Useful tools for working with ports
 """
-from __future__ import unicode_literals
+import random
 import threading
 import time
-import random
-from .parser import Parser
+
 from .messages import Message
+from .parser import Parser
 
 # How many seconds to sleep before polling again.
 _DEFAULT_SLEEP_TIME = 0.001
 _sleep_time = _DEFAULT_SLEEP_TIME
 
 
 # TODO: document this more.
@@ -51,23 +55,23 @@
     """
     ALL_SOUNDS_OFF = 120
     for channel in range(16):
         yield Message('control_change',
                       channel=channel, control=ALL_SOUNDS_OFF)
 
 
-class DummyLock(object):
+class DummyLock:
     def __enter__(self):
         return self
 
     def __exit__(self, *_):
         return False
 
 
-class BasePort(object):
+class BasePort:
     """
     Abstract base class for Input and Output ports.
     """
     is_input = False
     is_output = False
     _locking = True
 
@@ -100,15 +104,15 @@
         is garbage collected.
         """
         with self._lock:
             if not self.closed:
                 if hasattr(self, 'autoreset') and self.autoreset:
                     try:
                         self.reset()
-                    except IOError:
+                    except OSError:
                         pass
 
                 self._close()
                 self.closed = True
 
     def __del__(self):
         self.close()
@@ -214,15 +218,15 @@
                     return msg
 
                 if self._messages:
                     return self._messages.popleft()
                 elif not block:
                     return None
                 elif self.closed:
-                    raise IOError('port closed during receive()')
+                    raise OSError('port closed during receive()')
 
             sleep()
 
     def poll(self):
         """Receive the next pending message or None
 
         This is the same as calling `receive(block=False)`."""
@@ -233,15 +237,15 @@
         # This could have simply called receive() in a loop, but that
         # could result in a "port closed during receive()" error which
         # is hard to catch here.
         self._check_callback()
         while True:
             try:
                 yield self.receive()
-            except IOError:
+            except OSError:
                 if self.closed:
                     # The port closed before or inside receive().
                     # (This makes the assumption that this is the reason,
                     # at the risk of masking other errors.)
                     return
                 else:
                     raise
@@ -327,15 +331,15 @@
     _locking = False
 
     def __init__(self, input, output):
         self.input = input
         self.output = output
 
         # We use str() here in case name is None.
-        self.name = '{} + {}'.format(str(input.name), str(output.name))
+        self.name = f'{str(input.name)} + {str(output.name)}'
         self._messages = self.input._messages
         self.closed = False
         self._lock = DummyLock()
 
     def _close(self):
         self.input.close()
         self.output.close()
@@ -380,17 +384,17 @@
     yielded before moving on to the next port.
 
     If yield_ports=True, (port, message) is yielded instead of just
     the message.
 
     If block=False only pending messages will be yielded.
     """
+    ports = list(ports)
     while True:
         # Make a shuffled copy of the port list.
-        ports = list(ports)
         random.shuffle(ports)
 
         for port in ports:
             if not port.closed:
                 for message in port.iter_pending():
                     if yield_ports:
                         yield port, message
```

### Comparing `mido-1.2.9/mido/messages/strings.py` & `mido-1.3.0/mido/messages/strings.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from .specs import SPEC_BY_TYPE, make_msgdict
 
 
 def msg2str(msg, include_time=True):
     type_ = msg['type']
     spec = SPEC_BY_TYPE[type_]
 
     words = [type_]
 
     for name in spec['value_names']:
         value = msg[name]
 
         if name == 'data':
             value = '({})'.format(','.join(str(byte) for byte in value))
-        words.append('{}={}'.format(name, value))
+        words.append(f'{name}={value}')
 
     if include_time:
         words.append('time={}'.format(msg['time']))
 
     return str.join(' ', words)
 
 
@@ -28,15 +32,15 @@
         pass
 
     try:
         return float(value)
     except ValueError:
         pass
 
-    raise ValueError('invalid time {!r}'.format(value))
+    raise ValueError(f'invalid time {value!r}')
 
 
 def _parse_data(value):
     if not value.startswith('(') and value.endswith(')'):
         raise ValueError('missing parentheses in data message')
 
     try:
```

### Comparing `mido-1.2.9/mido/messages/decode.py` & `mido-1.3.0/mido/messages/decode.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from collections import deque
-from numbers import Integral
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from .specs import (SYSEX_START, SYSEX_END,
                     SPEC_BY_STATUS, CHANNEL_MESSAGES,
                     MIN_PITCHWHEEL)
 from .checks import check_data
-from ..py2 import convert_py2_bytes
 
 
 def _decode_sysex_data(data):
     return {'data': tuple(data)}
 
 
 def _decode_quarter_frame_data(data):
@@ -63,41 +64,40 @@
 
     Raises ValueError if the bytes are out of range or the message is
     invalid.
 
     This is not a part of the public API.
     """
     # TODO: this function is getting long.
-    msg_bytes = convert_py2_bytes(msg_bytes)
 
     if len(msg_bytes) == 0:
         raise ValueError('message is 0 bytes long')
 
     status_byte = msg_bytes[0]
     data = msg_bytes[1:]
 
     try:
         spec = SPEC_BY_STATUS[status_byte]
     except KeyError:
-        raise ValueError('invalid status byte {!r}'.format(status_byte))
+        raise ValueError(f'invalid status byte {status_byte!r}')
 
     msg = {
         'type': spec['type'],
         'time': time,
     }
 
     # Sysex.
     if status_byte == SYSEX_START:
         if len(data) < 1:
             raise ValueError('sysex without end byte')
 
         end = data[-1]
         data = data[:-1]
         if end != SYSEX_END:
-            raise ValueError('invalid sysex end byte {!r}'.format(end))
+            raise ValueError(f'invalid sysex end byte {end!r}')
 
     if check:
         check_data(data)
 
     if status_byte in _SPECIAL_CASES:
         if status_byte in CHANNEL_MESSAGES:
             msg['channel'] = status_byte & 0x0f
```

### Comparing `mido-1.2.9/mido/messages/encode.py` & `mido-1.3.0/mido/messages/encode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from .specs import CHANNEL_MESSAGES, SPEC_BY_TYPE, MIN_PITCHWHEEL
 
 
 def _encode_pitchwheel(msg):
     pitch = msg['pitch'] - MIN_PITCHWHEEL
     return [0xe0 | msg['channel'], pitch & 0x7f, pitch >> 7]
```

### Comparing `mido-1.2.9/mido/messages/specs.py` & `mido-1.3.0/mido/messages/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """Definitions and lookup tables for MIDI messages.
 
 TODO:
 
     * add lookup functions for messages definitions by type and status
       byte.
 """
@@ -116,15 +120,15 @@
 
     No type or value checking is done.  The caller is responsible for
     calling check_msgdict().
     """
     if type_ in SPEC_BY_TYPE:
         spec = SPEC_BY_TYPE[type_]
     else:
-        raise LookupError('Unknown message type {!r}'.format(type_))
+        raise LookupError(f'Unknown message type {type_!r}')
 
     msg = {'type': type_, 'time': DEFAULT_VALUES['time']}
 
     for name in spec['value_names']:
         msg[name] = DEFAULT_VALUES[name]
 
     msg.update(overrides)
```

### Comparing `mido-1.2.9/mido/messages/messages.py` & `mido-1.3.0/mido/messages/messages.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,43 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 import re
-from .specs import make_msgdict, SPEC_BY_TYPE, REALTIME_TYPES
+
 from .checks import check_msgdict, check_value, check_data
 from .decode import decode_message
 from .encode import encode_message
+from .specs import make_msgdict, SPEC_BY_TYPE, REALTIME_TYPES
 from .strings import msg2str, str2msg
-from ..py2 import convert_py2_bytes
 
 
-class BaseMessage(object):
+class BaseMessage:
     """Abstract base class for messages."""
     is_meta = False
 
     def copy(self):
-        raise NotImplemented
+        raise NotImplementedError
 
     def bytes(self):
-        raise NotImplemented
+        raise NotImplementedError
 
     def bin(self):
         """Encode message and return as a bytearray.
 
         This can be used to write the message to a file.
         """
         return bytearray(self.bytes())
 
     def hex(self, sep=' '):
         """Encode message and return as a string of hex numbers,
 
         Each number is separated by the string sep.
         """
-        return sep.join('{:02X}'.format(byte) for byte in self.bytes())
+        return sep.join(f'{byte:02X}' for byte in self.bytes())
 
     def dict(self):
         """Returns a dictionary containing the attributes of the message.
 
         Example: {'type': 'sysex', 'data': [1, 2], 'time': 0}
 
         Sysex data will be returned as a list.
@@ -42,53 +46,79 @@
         if data['type'] == 'sysex':
             # Make sure we return a list instead of a SysexData object.
             data['data'] = list(data['data'])
 
         return data
 
     @classmethod
-    def from_dict(cl, data):
+    def from_dict(cls, data):
         """Create a message from a dictionary.
 
         Only "type" is required. The other will be set to default
         values.
         """
-        return cl(**data)
+        return cls(**data)
+
+    def _get_value_names(self):
+        # This is overridden by MetaMessage.
+        return list(SPEC_BY_TYPE[self.type]['value_names']) + ['time']
+
+    def __repr__(self):
+        items = [repr(self.type)]
+        for name in self._get_value_names():
+            items.append(f'{name}={getattr(self, name)!r}')
+        return '{}({})'.format(type(self).__name__, ', '.join(items))
 
     @property
     def is_realtime(self):
         """True if the message is a system realtime message."""
         return self.type in REALTIME_TYPES
 
+    def is_cc(self, control=None):
+        """Return True if the message is of type 'control_change'.
+
+        The optional control argument can be used to test for a specific
+        control number, for example:
+
+        if msg.is_cc(7):
+            # Message is control change 7 (channel volume).
+        """
+        if self.type != 'control_change':
+            return False
+        elif control is None:
+            return True
+        else:
+            return self.control == control
+
     def __delattr__(self, name):
         raise AttributeError('attribute cannot be deleted')
 
     def __setattr__(self, name, value):
         raise AttributeError('message is immutable')
 
     def __eq__(self, other):
         if not isinstance(other, BaseMessage):
-            raise TypeError('can\'t compare message to {}'.format(type(other)))
+            raise TypeError(f'can\'t compare message to {type(other)}')
 
         # This includes time in comparison.
         return vars(self) == vars(other)
 
 
 class SysexData(tuple):
     """Special kind of tuple accepts and converts any sequence in +=."""
     def __iadd__(self, other):
         check_data(other)
-        return self + SysexData(convert_py2_bytes(other))
+        return self + SysexData(other)
 
 
 class Message(BaseMessage):
     def __init__(self, type, **args):
         msgdict = make_msgdict(type, args)
         if type == 'sysex':
-            msgdict['data'] = SysexData(convert_py2_bytes(msgdict['data']))
+            msgdict['data'] = SysexData(msgdict['data'])
         check_msgdict(msgdict)
         vars(self).update(msgdict)
 
     def copy(self, **overrides):
         """Return a copy of the message.
 
         Attributes will be overridden by the passed keyword arguments.
@@ -158,17 +188,14 @@
             return 2 + len(self.data)
         else:
             return SPEC_BY_TYPE[self.type]['length']
 
     def __str__(self):
         return msg2str(vars(self))
 
-    def __repr__(self):
-        return '<message {}>'.format(str(self))
-
     def _setattr(self, name, value):
         if name == 'type':
             raise AttributeError('type attribute is read only')
         elif name not in vars(self):
             raise AttributeError('{} message has no '
                                  'attribute {}'.format(self.type,
                                                        name))
@@ -194,22 +221,22 @@
 
     Raises ValueError if the string could not be parsed.
     """
     return Message.from_str(text)
 
 
 def parse_string_stream(stream):
-    """Parse a stram of messages and yield (message, error_message)
+    """Parse a stream of messages and yield (message, error_message)
 
     stream can be any iterable that generates text strings, where each
     string is a string encoded message.
 
     If a string can be parsed, (message, None) is returned. If it
-    can't be parsed (None, error_message) is returned. The error
-    message containes the line number where the error occurred.
+    can't be parsed, (None, error_message) is returned. The error
+    message contains the line number where the error occurred.
     """
     line_number = 1
     for line in stream:
         try:
             line = line.split('#')[0].strip()
             if line:
                 yield parse_string(line), None
```

### Comparing `mido-1.2.9/mido/messages/checks.py` & `mido-1.3.0/mido/messages/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# SPDX-FileCopyrightText: 2016 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from numbers import Integral, Real
 from .specs import (SPEC_BY_TYPE, MIN_SONGPOS, MAX_SONGPOS,
                     MIN_PITCHWHEEL, MAX_PITCHWHEEL)
-from ..py2 import convert_py2_bytes
 
 
 def check_type(type_):
     if type_ not in SPEC_BY_TYPE:
-        raise ValueError('invalid message type {!r}'.format(type_))
+        raise ValueError(f'invalid message type {type_!r}')
 
 
 def check_channel(channel):
     if not isinstance(channel, Integral):
         raise TypeError('channel must be int')
     elif not 0 <= channel <= 15:
         raise ValueError('channel must be in range 0..15')
@@ -29,15 +32,15 @@
         raise TypeError('pichwheel value must be int')
     elif not MIN_PITCHWHEEL <= pitch <= MAX_PITCHWHEEL:
         raise ValueError('pitchwheel value must be in range {}..{}'.format(
                          MIN_PITCHWHEEL, MAX_PITCHWHEEL))
 
 
 def check_data(data_bytes):
-    for byte in convert_py2_bytes(data_bytes):
+    for byte in data_bytes:
         check_data_byte(byte)
 
 
 def check_frame_type(value):
     if not isinstance(value, Integral):
         raise TypeError('frame_type must be int')
     elif not 0 <= value <= 7:
```

### Comparing `mido-1.2.9/mido/tokenizer.py` & `mido-1.3.0/mido/tokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+# SPDX-FileCopyrightText: 2017 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 from collections import deque
 from numbers import Integral
 from .messages.specs import SYSEX_START, SYSEX_END, SPEC_BY_STATUS
-from .py2 import convert_py2_bytes
 
 
-class Tokenizer(object):
+class Tokenizer:
     """
     Splits a MIDI byte stream into messages.
     """
     def __init__(self, data=None):
         """Create a new decoder."""
 
         self._status = 0
@@ -74,22 +77,22 @@
 
         if 0 <= byte <= 255:
             if byte <= 127:
                 return self._feed_data_byte(byte)
             else:
                 return self._feed_status_byte(byte)
         else:
-            raise ValueError('invalid byte value {!r}'.format(byte))
+            raise ValueError(f'invalid byte value {byte!r}')
 
     def feed(self, data):
         """Feed MIDI bytes to the decoder.
 
         Takes an iterable of ints in in range [0..255].
         """
-        for byte in convert_py2_bytes(data):
+        for byte in data:
             self.feed_byte(byte)
 
     def __len__(self):
         return len(self._messages)
 
     def __iter__(self):
         """Yield messages that have been parsed so far."""
```

### Comparing `mido-1.2.9/mido/parser.py` & `mido-1.3.0/mido/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 MIDI Parser
 
 There is no need to use this module directly. All you need is
 available in the top level module.
 """
 from collections import deque
+
 from .messages import Message
 from .tokenizer import Tokenizer
 
-# TODO: make sure the method signatures are as before.
-# TODO: add doc strings.
-
 
-class Parser(object):
+class Parser:
     """
     MIDI byte stream parser
 
     Parses a stream of MIDI bytes and produces messages.
 
     Data can be put into the parser in the form of
     integers, byte arrays or byte strings.
@@ -40,15 +42,14 @@
         range 0..255, such as:
 
             [0, 1, 2]
             (0, 1, 2)
             [for i in range(256)]
             (for i in range(256)]
             bytearray()
-            b''  # Will be converted to integers in Python 2.
         """
         self._tok.feed(data)
         self._decode()
 
     def feed_byte(self, byte):
         """Feed one MIDI byte into the parser.
```

### Comparing `mido-1.2.9/mido/__init__.py` & `mido-1.3.0/mido/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# -*- coding: utf-8 -*-
+# SPDX-FileCopyrightText: 2013 Ole Martin Bjorndalen <ombdalen@gmail.com>
+#
+# SPDX-License-Identifier: MIT
+
 """
 MIDI Objects for Python
 
 Mido is a library for working with MIDI messages and ports. It's
 designed to be as straight forward and Pythonic as possible.
 
 Creating messages:
@@ -85,30 +88,28 @@
     >>>
     >>> for message in default_input:
     ...     output.send(message)
 
     >>> get_input_names()
     ['MPK mini MIDI 1', 'SH-201']
 """
-from __future__ import absolute_import
 import os
-from .backends.backend import Backend
+
 from . import ports, sockets
+from .backends.backend import Backend
 from .messages import (Message, parse_string, parse_string_stream,
                        format_as_string, MIN_PITCHWHEEL, MAX_PITCHWHEEL,
                        MIN_SONGPOS, MAX_SONGPOS)
-from .parser import Parser, parse, parse_all
 from .midifiles import (MidiFile, MidiTrack, merge_tracks,
                         MetaMessage, UnknownMetaMessage,
                         bpm2tempo, tempo2bpm, tick2second, second2tick,
                         KeySignatureError)
+from .parser import Parser, parse, parse_all
 from .syx import read_syx_file, write_syx_file
 from .version import version_info
-from .__about__ import (__version__, __author__, __author_email__,
-                        __url__, __license__)
 
 # Prevent splat import.
 __all__ = []
 
 
 def set_backend(name=None, load=False):
     """Set current backend.
@@ -133,8 +134,8 @@
     for name in dir(backend):
         if name.split('_')[0] in ['open', 'get']:
             glob[name] = getattr(backend, name)
 
 
 set_backend()
 
-del os, absolute_import
+del os
```

