# Comparing `tmp/iqmotion-0.9.2.tar.gz` & `tmp/iqmotion-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iqmotion-0.9.2.tar", last modified: Mon Jun 29 17:15:54 2020, max compression
+gzip compressed data, was "dist/iqmotion-0.9.3.tar", last modified: Mon Jun 29 17:45:04 2020, max compression
```

## Comparing `iqmotion-0.9.2.tar` & `iqmotion-0.9.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.511437 iqmotion-0.9.2/
--rw-rw-rw-   0 root         (0) root         (0)      106 2020-06-29 17:15:41.000000 iqmotion-0.9.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4972 2020-06-29 17:15:54.511437 iqmotion-0.9.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3300 2020-06-29 17:15:41.000000 iqmotion-0.9.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.503437 iqmotion-0.9.2/iqmotion/
--rwxrwxrwx   0 root         (0) root         (0)      378 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.504437 iqmotion-0.9.2/iqmotion/client_entries/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/client_entries/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/client_entries/client_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/client_entries/client_entry_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3264 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/client_entries/dictionary_client_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/client_entries/process_client_entry.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.505437 iqmotion-0.9.2/iqmotion/clients/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.507437 iqmotion-0.9.2/iqmotion/clients/client_files/
--rwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/anticogging.json
--rw-rw-rw-   0 root         (0) root         (0)     3601 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/brushless_drive.json
--rw-rw-rw-   0 root         (0) root         (0)      748 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/buzzer_control.json
--rw-rw-rw-   0 root         (0) root         (0)      766 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/esc_propeller_input_parser.json
--rw-rw-rw-   0 root         (0) root         (0)      187 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/hobby_input.json
--rw-rw-rw-   0 root         (0) root         (0)     2994 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/multi_turn_angle_control.json
--rw-rw-rw-   0 root         (0) root         (0)      171 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/persistent_memory.json
--rw-rw-rw-   0 root         (0) root         (0)     1322 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/power_monitor.json
--rw-rw-rw-   0 root         (0) root         (0)     1959 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/propeller_motor_control.json
--rw-rw-rw-   0 root         (0) root         (0)       88 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/serial_interface.json
--rw-rw-rw-   0 root         (0) root         (0)      301 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/servo_input_parser.json
--rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/step_direction_input.json
--rw-rw-rw-   0 root         (0) root         (0)     1964 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/system_control.json
--rw-rw-rw-   0 root         (0) root         (0)      591 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/temperature_estimator.json
--rw-rw-rw-   0 root         (0) root         (0)      508 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_files/temperature_monitor_uc.json
--rw-rw-rw-   0 root         (0) root         (0)     3966 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/clients/client_with_entries.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.508437 iqmotion-0.9.2/iqmotion/communication/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6077 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/circular_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1233 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/communicator.py
--rwxrwxrwx   0 root         (0) root         (0)      961 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/crc.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/packet_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      829 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/packet_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1523 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/packet_state.py
--rw-rw-rw-   0 root         (0) root         (0)     5491 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/serial_communicator.py
--rw-rw-rw-   0 root         (0) root         (0)     4144 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/serial_packet_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     9076 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/communication/serial_packet_states.py
--rwxrwxrwx   0 root         (0) root         (0)     1449 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/custom_errors.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.510437 iqmotion-0.9.2/iqmotion/iq_devices/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.510437 iqmotion-0.9.2/iqmotion/iq_devices/common_commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/common_commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2254 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/common_commands/ramper.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/custom_iq_module.py
--rw-rw-rw-   0 root         (0) root         (0)    18045 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/iq_module.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/iq_module_json_parser.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.510437 iqmotion-0.9.2/iqmotion/iq_devices/module_files/
--rw-rw-rw-   0 root         (0) root         (0)      375 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/module_files/servo.json
--rwxrwxrwx   0 root         (0) root         (0)      374 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/module_files/speed.json
--rw-rw-rw-   0 root         (0) root         (0)      375 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/module_files/step_direction.json
--rw-rw-rw-   0 root         (0) root         (0)      636 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/servo_module.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/speed_module.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/iq_devices/step_dir_module.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.511437 iqmotion-0.9.2/iqmotion/message_making/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/message_making/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/message_making/client_with_entries_message.py
--rw-rw-rw-   0 root         (0) root         (0)     4359 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/message_making/dictionary_message_maker.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/message_making/message.py
--rw-rw-rw-   0 root         (0) root         (0)      322 2020-06-29 17:15:41.000000 iqmotion-0.9.2/iqmotion/message_making/message_maker.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:15:54.503437 iqmotion-0.9.2/iqmotion.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4972 2020-06-29 17:15:54.000000 iqmotion-0.9.2/iqmotion.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2526 2020-06-29 17:15:54.000000 iqmotion-0.9.2/iqmotion.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-29 17:15:54.000000 iqmotion-0.9.2/iqmotion.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2020-06-29 17:15:54.000000 iqmotion-0.9.2/iqmotion.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2020-06-29 17:15:54.000000 iqmotion-0.9.2/iqmotion.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      108 2020-06-29 17:15:54.512437 iqmotion-0.9.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1199 2020-06-29 17:15:54.000000 iqmotion-0.9.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.456956 iqmotion-0.9.3/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2020-06-29 17:44:53.000000 iqmotion-0.9.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4972 2020-06-29 17:45:04.456956 iqmotion-0.9.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3300 2020-06-29 17:44:53.000000 iqmotion-0.9.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.448956 iqmotion-0.9.3/iqmotion/
+-rwxrwxrwx   0 root         (0) root         (0)      378 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.449956 iqmotion-0.9.3/iqmotion/client_entries/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/client_entries/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/client_entries/client_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/client_entries/client_entry_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3264 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/client_entries/dictionary_client_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/client_entries/process_client_entry.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.450956 iqmotion-0.9.3/iqmotion/clients/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.452956 iqmotion-0.9.3/iqmotion/clients/client_files/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/anticogging.json
+-rw-rw-rw-   0 root         (0) root         (0)     3601 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/brushless_drive.json
+-rw-rw-rw-   0 root         (0) root         (0)      748 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/buzzer_control.json
+-rw-rw-rw-   0 root         (0) root         (0)      766 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/esc_propeller_input_parser.json
+-rw-rw-rw-   0 root         (0) root         (0)      187 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/hobby_input.json
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/multi_turn_angle_control.json
+-rw-rw-rw-   0 root         (0) root         (0)      171 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/persistent_memory.json
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/power_monitor.json
+-rw-rw-rw-   0 root         (0) root         (0)     1959 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/propeller_motor_control.json
+-rw-rw-rw-   0 root         (0) root         (0)       88 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/serial_interface.json
+-rw-rw-rw-   0 root         (0) root         (0)      301 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/servo_input_parser.json
+-rw-rw-rw-   0 root         (0) root         (0)      169 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/step_direction_input.json
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/system_control.json
+-rw-rw-rw-   0 root         (0) root         (0)      591 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/temperature_estimator.json
+-rw-rw-rw-   0 root         (0) root         (0)      508 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_files/temperature_monitor_uc.json
+-rw-rw-rw-   0 root         (0) root         (0)     3966 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/clients/client_with_entries.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.453956 iqmotion-0.9.3/iqmotion/communication/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6077 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/circular_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/communicator.py
+-rwxrwxrwx   0 root         (0) root         (0)      961 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/crc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/packet_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      829 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/packet_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1523 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/packet_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     5491 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/serial_communicator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/serial_packet_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     9076 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/communication/serial_packet_states.py
+-rwxrwxrwx   0 root         (0) root         (0)     1449 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/custom_errors.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.454956 iqmotion-0.9.3/iqmotion/iq_devices/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.455956 iqmotion-0.9.3/iqmotion/iq_devices/common_commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/common_commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2254 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/common_commands/ramper.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/custom_iq_module.py
+-rw-rw-rw-   0 root         (0) root         (0)    18295 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/iq_module.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/iq_module_json_parser.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.455956 iqmotion-0.9.3/iqmotion/iq_devices/module_files/
+-rw-rw-rw-   0 root         (0) root         (0)      375 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/module_files/servo.json
+-rwxrwxrwx   0 root         (0) root         (0)      374 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/module_files/speed.json
+-rw-rw-rw-   0 root         (0) root         (0)      375 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/module_files/step_direction.json
+-rw-rw-rw-   0 root         (0) root         (0)      636 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/servo_module.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/speed_module.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/iq_devices/step_dir_module.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.456956 iqmotion-0.9.3/iqmotion/message_making/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/message_making/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/message_making/client_with_entries_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     4359 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/message_making/dictionary_message_maker.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/message_making/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      322 2020-06-29 17:44:53.000000 iqmotion-0.9.3/iqmotion/message_making/message_maker.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2020-06-29 17:45:04.448956 iqmotion-0.9.3/iqmotion.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4972 2020-06-29 17:45:04.000000 iqmotion-0.9.3/iqmotion.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2020-06-29 17:45:04.000000 iqmotion-0.9.3/iqmotion.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2020-06-29 17:45:04.000000 iqmotion-0.9.3/iqmotion.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2020-06-29 17:45:04.000000 iqmotion-0.9.3/iqmotion.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2020-06-29 17:45:04.000000 iqmotion-0.9.3/iqmotion.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      108 2020-06-29 17:45:04.456956 iqmotion-0.9.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2020-06-29 17:45:04.000000 iqmotion-0.9.3/setup.py
```

### Comparing `iqmotion-0.9.2/PKG-INFO` & `iqmotion-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqmotion
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python libraries to talk to IQ Motion Control devices
 Home-page: https://github.com/iq-motion-control/iq-module-communication-python
 Author: Raphael Van Hoffelen
 Author-email: raf@iq-control.com
 License: lgpl-3.0
 Download-URL: https://github.com/iq-motion-control/iq-module-communication-python/releases
 Description: # IQ Motion Python API
```

### Comparing `iqmotion-0.9.2/README.md` & `iqmotion-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/client_entries/client_entry.py` & `iqmotion-0.9.3/iqmotion/client_entries/client_entry.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/client_entries/dictionary_client_entry.py` & `iqmotion-0.9.3/iqmotion/client_entries/dictionary_client_entry.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/client_entries/process_client_entry.py` & `iqmotion-0.9.3/iqmotion/client_entries/process_client_entry.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client.py` & `iqmotion-0.9.3/iqmotion/clients/client.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/brushless_drive.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/brushless_drive.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/buzzer_control.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/buzzer_control.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/esc_propeller_input_parser.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/esc_propeller_input_parser.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/multi_turn_angle_control.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/multi_turn_angle_control.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/power_monitor.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/power_monitor.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/propeller_motor_control.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/propeller_motor_control.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/system_control.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/system_control.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_files/temperature_estimator.json` & `iqmotion-0.9.3/iqmotion/clients/client_files/temperature_estimator.json`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/clients/client_with_entries.py` & `iqmotion-0.9.3/iqmotion/clients/client_with_entries.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/circular_queue.py` & `iqmotion-0.9.3/iqmotion/communication/circular_queue.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/communicator.py` & `iqmotion-0.9.3/iqmotion/communication/communicator.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/crc.py` & `iqmotion-0.9.3/iqmotion/communication/crc.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/packet_parser.py` & `iqmotion-0.9.3/iqmotion/communication/packet_parser.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/packet_queue.py` & `iqmotion-0.9.3/iqmotion/communication/packet_queue.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/packet_state.py` & `iqmotion-0.9.3/iqmotion/communication/packet_state.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/serial_communicator.py` & `iqmotion-0.9.3/iqmotion/communication/serial_communicator.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/serial_packet_queue.py` & `iqmotion-0.9.3/iqmotion/communication/serial_packet_queue.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/communication/serial_packet_states.py` & `iqmotion-0.9.3/iqmotion/communication/serial_packet_states.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/custom_errors.py` & `iqmotion-0.9.3/iqmotion/custom_errors.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/common_commands/ramper.py` & `iqmotion-0.9.3/iqmotion/iq_devices/common_commands/ramper.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/custom_iq_module.py` & `iqmotion-0.9.3/iqmotion/iq_devices/custom_iq_module.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/iq_module.py` & `iqmotion-0.9.3/iqmotion/iq_devices/iq_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,17 +141,23 @@
 
         return True
 
     def _verify_value(self, set_value, returned_value, verify_range=0.01):
         if returned_value is None:
             return False
 
+        # makes sure the values are a list so that the for loop works
+        if not isinstance(set_value, list):
+            set_value = [set_value]
+            returned_value = [returned_value]
+
         # some values might loose precision when being saved so check if it's within a 0.01 range
-        if abs(set_value - returned_value) >= verify_range:
-            return False
+        for i, value in enumerate(set_value):
+            if abs(value - returned_value[i]) >= verify_range:
+                return False
 
         return True
 
     def get(
         self, client_name: str, client_entry_name: str, get_values=None, time_out=0.1
     ):
         """ Gets the value define by the client and client entry from the module.
```

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/iq_module_json_parser.py` & `iqmotion-0.9.3/iqmotion/iq_devices/iq_module_json_parser.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/servo_module.py` & `iqmotion-0.9.3/iqmotion/iq_devices/servo_module.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/speed_module.py` & `iqmotion-0.9.3/iqmotion/iq_devices/speed_module.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/iq_devices/step_dir_module.py` & `iqmotion-0.9.3/iqmotion/iq_devices/step_dir_module.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion/message_making/dictionary_message_maker.py` & `iqmotion-0.9.3/iqmotion/message_making/dictionary_message_maker.py`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/iqmotion.egg-info/PKG-INFO` & `iqmotion-0.9.3/iqmotion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqmotion
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python libraries to talk to IQ Motion Control devices
 Home-page: https://github.com/iq-motion-control/iq-module-communication-python
 Author: Raphael Van Hoffelen
 Author-email: raf@iq-control.com
 License: lgpl-3.0
 Download-URL: https://github.com/iq-motion-control/iq-module-communication-python/releases
 Description: # IQ Motion Python API
```

### Comparing `iqmotion-0.9.2/iqmotion.egg-info/SOURCES.txt` & `iqmotion-0.9.3/iqmotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqmotion-0.9.2/setup.py` & `iqmotion-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 
 setup(
     name="iqmotion",
     packages=find_packages(),
     include_package_data=True,
-    version="0.9.2",
+    version="0.9.3",
     license="lgpl-3.0",
     description="Python libraries to talk to IQ Motion Control devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Raphael Van Hoffelen",
     author_email="raf@iq-control.com",
     url="https://github.com/iq-motion-control/iq-module-communication-python",
```

