# Comparing `tmp/edgepi-python-sdk-1.2.2.tar.gz` & `tmp/edgepi-python-sdk-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgepi-python-sdk-1.2.2.tar", last modified: Fri Jul  7 18:09:46 2023, max compression
+gzip compressed data, was "edgepi-python-sdk-1.2.5.tar", last modified: Fri Jul 21 00:20:06 2023, max compression
```

## Comparing `edgepi-python-sdk-1.2.2.tar` & `edgepi-python-sdk-1.2.5.tar`

### file list

```diff
@@ -1,208 +1,209 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.353278 edgepi-python-sdk-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-07 18:09:46.353278 edgepi-python-sdk-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 18:09:46.353278 edgepi-python-sdk-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.313277 edgepi-python-sdk-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.317277 edgepi-python-sdk-1.2.2/src/edgepi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.321277 edgepi-python-sdk-1.2.2/src/edgepi/adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_query_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/adc/edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.321277 edgepi-python-sdk-1.2.2/src/edgepi/calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/calibration/calibration_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/calibration/edgepi_calibration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.321277 edgepi-python-sdk-1.2.2/src/edgepi/dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/dac/dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/dac/dac_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/dac/edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.321277 edgepi-python-sdk-1.2.2/src/edgepi/digital_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/digital_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/digital_input/digital_input_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/digital_input/edgepi_digital_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.321277 edgepi-python-sdk-1.2.2/src/edgepi/digital_output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/digital_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/digital_output/digital_output_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/digital_output/edgepi_digital_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.325277 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/edgepi_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/edgepi_eeprom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/eeprom_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.325277 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.325277 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.325277 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.325277 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/proto_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/proto_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.329277 edgepi-python-sdk-1.2.2/src/edgepi/gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/gpio/edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/gpio/edgepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/gpio/edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/gpio/gpio_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/gpio/gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.329277 edgepi-python-sdk-1.2.2/src/edgepi/led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/led/edgepi_leds.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/led/led_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.329277 edgepi-python-sdk-1.2.2/src/edgepi/peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/peripherals/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/peripherals/i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/peripherals/pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/peripherals/spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.329277 edgepi-python-sdk-1.2.2/src/edgepi/pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/pwm/edgepi_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/pwm/pwm_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.333277 edgepi-python-sdk-1.2.2/src/edgepi/reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/reg_helper/reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.333277 edgepi-python-sdk-1.2.2/src/edgepi/relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/relay/edgepi_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.333277 edgepi-python-sdk-1.2.2/src/edgepi/tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/tc/edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.333277 edgepi-python-sdk-1.2.2/src/edgepi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/utilities/crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/edgepi/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.333277 edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-07 18:09:46.000000 edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-07 18:09:46.000000 edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:09:46.000000 edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 18:09:46.000000 edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 18:09:46.000000 edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.317277 edgepi-python-sdk-1.2.2/src/test_edgepi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_adc/test_adc.py
--rw-r--r--   0 runner    (1001) docker     (123)    55717 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_dac/test_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_in/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_in/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_out/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_out/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.337278 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_led/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_led/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_led/test_led.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.341277 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.341277 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.341277 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_relay/test_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.341277 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_tc/test_tc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.341277 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.341277 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
--rw-r--r--   0 runner    (1001) docker     (123)    45764 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.345278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_calibration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.345278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.345278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_din/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_din/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.345278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.345278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_eeprom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_eeprom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
--rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.349278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.349278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.349278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_pwm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_pwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.349278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_reg_helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.349278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_relay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_relay/test_relay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.353278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    39495 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:46.353278 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-07 18:09:27.000000 edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.207954 edgepi-python-sdk-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.207954 edgepi-python-sdk-1.2.5/src/edgepi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14779 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_query_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38761 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/adc/edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/calibration/calibration_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/calibration/edgepi_calibration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/dac/edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/digital_input_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_input/edgepi_digital_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/digital_output_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/digital_output/edgepi_digital_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/eeprom_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.211954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/proto_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/proto_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/led/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/led/edgepi_leds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/led/led_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/peripherals/spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/pwm/edgepi_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/pwm/pwm_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.215954 edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi/relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/relay/edgepi_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi/tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/utilities/crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/edgepi/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 00:20:06.000000 edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.207954 edgepi-python-sdk-1.2.5/src/test_edgepi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55717 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/test_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/test_gpio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.219954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/test_led.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/test_tc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24417 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45764 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9311 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19916 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.223954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/read_serialized.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14445 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_edgepi_eeprom_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15302 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/test_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24741 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39495 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 00:20:06.227954 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-21 00:19:48.000000 edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_utilities.py
```

### Comparing `edgepi-python-sdk-1.2.2/LICENSE` & `edgepi-python-sdk-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/PKG-INFO` & `edgepi-python-sdk-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.2.2
+Version: 1.2.5
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `edgepi-python-sdk-1.2.2/README.md` & `edgepi-python-sdk-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/setup.py` & `edgepi-python-sdk-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as file:
     long_description = file.read()
 
 setuptools.setup(
     name="edgepi-python-sdk",
-    version="1.2.2",
+    version="1.2.5",
     author="S.Park",
     author_email="spark@osensa.com",
     description="EdgePi Python SDK package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EdgePi-Cloud/edgepi-python-sdk",
     project_urls={
```

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_commands.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_conv_time.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_exceptions.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_exceptions.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_multiplexers.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_query_lang.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_query_lang.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_state.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_status.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/adc_voltage.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/adc_voltage.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/adc/edgepi_adc.py` & `edgepi-python-sdk-1.2.5/src/edgepi/adc/edgepi_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/calibration/calibration_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/calibration/calibration_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/calibration/edgepi_calibration.py` & `edgepi-python-sdk-1.2.5/src/edgepi/calibration/edgepi_calibration.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/dac/dac_commands.py` & `edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/dac/dac_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/dac/dac_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/dac/edgepi_dac.py` & `edgepi-python-sdk-1.2.5/src/edgepi/dac/edgepi_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/digital_input/edgepi_digital_input.py` & `edgepi-python-sdk-1.2.5/src/edgepi/digital_input/edgepi_digital_input.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/digital_output/edgepi_digital_output.py` & `edgepi-python-sdk-1.2.5/src/edgepi/digital_output/edgepi_digital_output.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/edgepi_eeprom.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/edgepi_eeprom_data.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/edgepi_eeprom_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,58 +2,50 @@
 from dataclasses import dataclass
 
 from edgepi.eeprom.protobuf_assets.generated_pb2 import (
     edgepi_module_pb2,
     dac_module_pb2,
     adc_module_pb2,
     rtd_module_pb2,
-    tc_module_pb2
+    tc_module_pb2,
+    keys_pb2
 )
 from edgepi.eeprom.protobuf_assets.eeprom_data_classes.eeprom_dac_module import DACModule
 from edgepi.eeprom.protobuf_assets.eeprom_data_classes.eeprom_adc_module import ADCModule
 from edgepi.eeprom.protobuf_assets.eeprom_data_classes.eeprom_rtd_module import RTDModule
 from edgepi.eeprom.protobuf_assets.eeprom_data_classes.eeprom_tc_module import TCModule
-
-@dataclass
-class AwsKeys:
-    """Key Pair dataclass"""
-    private_key:str = None
-    certificate:str = None
+from edgepi.eeprom.protobuf_assets.eeprom_data_classes.eeprom_key_module import AwsKeys
 
 @dataclass
 class EepromDataClass:
     """EEPROM Dataclass"""
     # pylint: disable=too-many-instance-attributes
     dac_calib_params: DACModule = None
     adc1_calib_params: ADCModule = None
     adc2_calib_params: ADCModule = None
     rtd_calib_params: RTDModule = None
     tc_calib_params: TCModule = None
-    config_key: AwsKeys = None
-    data_key: AwsKeys = None
+    config_key: AwsKeys = AwsKeys(None, None)
+    data_key: AwsKeys = AwsKeys(None, None)
     serial:str = None
     model:str = None
     cm_part_number: str = None
     tb_part_number: str = None
     cm4_part_number: str = None
 
     def populate_eeprom_module(self, eeprom_pb:edgepi_module_pb2):
         """Serialize"""
         self.__populate_dac_module(eeprom_pb.dac_module)
         self.__populate_adc1_module(eeprom_pb.adc1_module)
         self.__populate_adc2_module(eeprom_pb.adc2_module)
         self.__populate_rtd_module(eeprom_pb.rtd_module)
         self.__populate_tc_module(eeprom_pb.tc_module)
+        self.__populate_config_key_module(eeprom_pb.config_keys)
+        self.__populate_data_key_module(eeprom_pb.data_keys)
 
-        if self.config_key is not None:
-            eeprom_pb.config_keys.certificate = self.config_key.certificate
-            eeprom_pb.config_keys.private_key = self.config_key.private_key
-        if self.data_key is not None:
-            eeprom_pb.data_keys.certificate = self.data_key.certificate
-            eeprom_pb.data_keys.private_key = self.data_key.private_key
         if self.serial is not None:
             eeprom_pb.serial_number = self.serial
         if self.model is not None:
             eeprom_pb.model = self.model
         if self.cm_part_number is not None:
             eeprom_pb.cm_part_number = self.cm_part_number
         if self.tb_part_number is not None:
@@ -86,32 +78,44 @@
         self.rtd_calib_params.populate_rtd_module_pb(rtd_pb)
     def __populate_tc_module(self, tc_pb: tc_module_pb2):
         """Serialize TC"""
         if self.tc_calib_params is None:
             return
         self.tc_calib_params.populate_tc_module_pb(tc_pb)
 
+    def __populate_config_key_module(self, key_pb: keys_pb2):
+        """Serialize Config Keys"""
+        if self.config_key is None:
+            return
+        self.config_key.populate_keys_pb(key_pb)
+
+    def __populate_data_key_module(self, key_pb: keys_pb2):
+        """Serialize Data Keys"""
+        if self.data_key is None:
+            return
+        self.data_key.populate_keys_pb(key_pb)
+
     @staticmethod
     def extract_eeprom_data(eeprom_pb:edgepi_module_pb2):
         """De-serialize"""
         eeprom_data = EepromDataClass()
         eeprom_data.dac_calib_params = EepromDataClass.extract_dac_data(eeprom_pb.dac_module)
         eeprom_data.adc1_calib_params = EepromDataClass.extract_adc_data(eeprom_pb.adc1_module)
         eeprom_data.adc2_calib_params = EepromDataClass.extract_adc_data(eeprom_pb.adc2_module)
         eeprom_data.rtd_calib_params = EepromDataClass.extract_rtd_data(eeprom_pb.rtd_module)
         eeprom_data.tc_calib_params = EepromDataClass.extract_tc_data(eeprom_pb.tc_module)
 
+        if eeprom_pb.HasField("config_keys"):
+            eeprom_data.config_key = EepromDataClass.extract_config_key(eeprom_pb.config_keys)
+        if eeprom_pb.HasField("data_keys"):
+            eeprom_data.data_key = EepromDataClass.extract_data_key(eeprom_pb.data_keys)
         if eeprom_pb.HasField("serial_number"):
             eeprom_data.serial = eeprom_pb.serial_number
         if eeprom_pb.HasField("model"):
             eeprom_data.model = eeprom_pb.model
-        if eeprom_pb.HasField("config_keys"):
-            eeprom_data.config_key = eeprom_pb.config_keys
-        if eeprom_pb.HasField("data_keys"):
-            eeprom_data.data_key = eeprom_pb.data_keys
         if eeprom_pb.HasField("cm_part_number"):
             eeprom_data.cm_part_number = eeprom_pb.cm_part_number
         if eeprom_pb.HasField("tb_part_number"):
             eeprom_data.tb_part_number = eeprom_pb.tb_part_number
         if eeprom_pb.HasField("cm4_part_number"):
             eeprom_data.cm4_part_number = eeprom_pb.cm4_part_number
 
@@ -141,7 +145,17 @@
 
     @staticmethod
     def extract_tc_data(tc_pb: tc_module_pb2):
         """De-serialize TC"""
         if tc_pb is None:
             return
         return TCModule.extract_tc_calib_params(tc_pb)
+
+    @staticmethod
+    def extract_config_key(key_pb: keys_pb2):
+        """De-serialize Config Keys"""
+        return AwsKeys.extract_keys(key_pb)
+
+    @staticmethod
+    def extract_data_key(key_pb: keys_pb2):
+        """De-serialize Data Keys"""
+        return AwsKeys.extract_keys(key_pb)
```

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/eeprom_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/eeprom_constants.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,74 @@
 '''Address map of eeprom'''
 
 from enum import Enum
 
 # page write cycle time requirements https://www.onsemi.com/pdf/datasheet/cat24c256-d.pdf
 PAGE_WRITE_CYCLE_TIME=0.01
-DEFAULT_EEPROM_BIN_B64 = b"CmAKCg0AAIA/FQAAAAASCg0AAIA/FQAAAAAaCg0AAIA/FQAAAAAiCg0AAIA/FQAAAAAqCg0A\
-                       AIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/FQAAAAASkAEKCg0AAIA/FQAA\
-                       AAASCg0AAIA/FQAAAAAaCg0AAIA/FQAAAAAiCg0AAIA/FQAAAAAqCg0AAIA/FQAAAAAyCg0AAIA/\
-                       FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/FQAAAABKCg0AAIA/FQAAAABSCg0AAIA/FQAAAABaCg0A\
-                       AIA/FQAAAABiCg0AAIA/FQAAAAAakAEKCg0AAIA/FQAAAAASCg0AAIA/FQAAAAAaCg0AAIA/FQAA\
-                       AAAiCg0AAIA/FQAAAAAqCg0AAIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/\
-                       FQAAAABKCg0AAIA/FQAAAABSCg0AAIA/FQAAAABaCg0AAIA/FQAAAABiCg0AAIA/FQAAAAAiEQoK\
-                       DQAAgD8VAAAAABUAAPpEKmAKCg0AAIA/FQAAAAASCg0AAIA/FQAAAAAaCg0AAIA/FQAAAAAiCg0A\
-                       AIA/FQAAAAAqCg0AAIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/FQAAAAAy\
-                       NAoWVGhpcyBpcyBDb25maWcgUHJpdmF0ZRIaVGhpcyBpcyBDb25maWcgQ2VydGlmaWNhdGU6MAoU\
-                       VGhpcyBpcyBEYXRhIFByaXZhdGUSGFRoaXMgaXMgRGF0YSBDZXJ0aWZpY2F0ZUIVVGhpcyBpcyBT\
-                       ZXJpYWwgTnVtYmVyShxUaGlzIGlzIGNtIGJvYXJkIHBhcnQgbnVtYmVyUhZUaGlzIGlzIHRiIHBh\
-                       cnQgbnVtYmVyWhdUaGlzIGlzIGNtNCBwYXJ0IG51bWJlcmIUVGhpcyBpcyBNb2RlbCBOdW1iZXI="
+DEFAULT_EEPROM_BIN_B64 = b'CmAKCg0AAIA/FQAAAAASCg0AAIA/FQAAAAAaCg0AAIA/FQAAAAAiCg0AAIA/FQAAAAAqCg0A\
+AIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/FQAAAAASkAEKCg0AAIA/FQAAAAASCg0AAIA/FQAAAAAaCg0\
+AAIA/FQAAAAAiCg0AAIA/FQAAAAAqCg0AAIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/FQAAAABKCg0AAI\
+A/FQAAAABSCg0AAIA/FQAAAABaCg0AAIA/FQAAAABiCg0AAIA/FQAAAAAakAEKCg0AAIA/FQAAAAASCg0AAIA/FQAAAAAaCg0AA\
+IA/FQAAAAAiCg0AAIA/FQAAAAAqCg0AAIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg0AAIA/FQAAAABKCg0AAIA/\
+FQAAAABSCg0AAIA/FQAAAABaCg0AAIA/FQAAAABiCg0AAIA/FQAAAAAiEQoKDQAAgD8VAAAAABUAAPpEKmAKCg0AAIA/FQAAAAA\
+SCg0AAIA/FQAAAAAaCg0AAIA/FQAAAAAiCg0AAIA/FQAAAAAqCg0AAIA/FQAAAAAyCg0AAIA/FQAAAAA6Cg0AAIA/FQAAAABCCg\
+0AAIA/FQAAAAA='
+
+"""
+Defaul EEPROM Dataclass
+dac_calib_params
+    dac_ch1
+        gain = 1
+        offset = 0
+    ~
+    dac_ch8
+        gain = 1
+        offset = 0
+adc1_calib_params
+    adc_ch_1
+        gain = 1
+        offset = 0
+    ~
+    adc_ch_8
+        gain = 1
+        offset = 0
+    diff1
+        gain = 1
+        offset = 0
+    ~
+    diff4
+adc2_calib_params
+    same as adc1_calib_params
+rtd_calib_params
+    rtd
+        gain = 1
+        offset = 0
+    rtd_resistor = 2000
+tc_calib_params
+    tc_B
+        gain = 1
+        offset = 0
+    ~
+    tc_T
+        gain = 1
+        offset = 0
+config_key
+    private_key = None
+    certificate = None
+data_key
+    private_key = None
+    certificate = None
+serial = None
+model = None
+cm_part_number = None
+tb_part_number = None
+cm4_part_number = None
+"""
+
+
 
 class EEPROMInfo(Enum):
     """
     EEPROM device address for I2C addressing
     """
     DEV_ADDR = 0x50
     PAGE_SIZE = 64
```

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/keys_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nkeys.proto\"3\n\x07\x41wsKeys\x12\x13\n\x0bprivate_key\x18\x01 \x01(\t\x12\x13\n\x0b\x63\x65rtificate\x18\x02 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\nkeys.proto\"]\n\x07\x41wsKeys\x12\x18\n\x0bprivate_key\x18\x01 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x63\x65rtificate\x18\x02 \x01(\tH\x01\x88\x01\x01\x42\x0e\n\x0c_private_keyB\x0e\n\x0c_certificateb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'keys_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _AWSKEYS._serialized_start=14
-  _AWSKEYS._serialized_end=65
+  _AWSKEYS._serialized_end=107
 # @@protoc_insertion_point(module_scope)
```

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/rtd_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py` & `edgepi-python-sdk-1.2.5/src/edgepi/eeprom/protobuf_assets/generated_pb2/tc_module_pb2.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/gpio/edgepi_gpio.py` & `edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/gpio/edgepi_gpio_chip.py` & `edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_chip.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/gpio/edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.5/src/edgepi/gpio/edgepi_gpio_expander.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/gpio/gpio_configs.py` & `edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_configs.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/gpio/gpio_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/gpio/gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/led/edgepi_leds.py` & `edgepi-python-sdk-1.2.5/src/edgepi/led/edgepi_leds.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/peripherals/gpio.py` & `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/peripherals/i2c.py` & `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/peripherals/pwm.py` & `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/peripherals/spi.py` & `edgepi-python-sdk-1.2.5/src/edgepi/peripherals/spi.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/pwm/edgepi_pwm.py` & `edgepi-python-sdk-1.2.5/src/edgepi/pwm/edgepi_pwm.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         if self.__pwm_devs[pwm_num] is None:
             self.__init_pwm_dev(pwm_num)
             return
 
         self.log.debug("init_pwm: PWM device is already open")
 
     def set_config(self, pwm_num: PWMPins,
-                   frequency: int = None,
+                   frequency: float = None,
                    duty_cycle: int = None,
                    polarity: Polarity = None
                    ):
         """
         Setting PWM configuration
         Args:
             pwm_num (PWMPins): PWM number enum
```

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/pwm/pwm_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/pwm/pwm_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/reg_helper/reg_helper.py` & `edgepi-python-sdk-1.2.5/src/edgepi/reg_helper/reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/relay/edgepi_relay.py` & `edgepi-python-sdk-1.2.5/src/edgepi/relay/edgepi_relay.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/tc/edgepi_tc.py` & `edgepi-python-sdk-1.2.5/src/edgepi/tc/edgepi_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_commands.py` & `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_constants.py` & `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_conv_time.py` & `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/tc/tc_faults.py` & `edgepi-python-sdk-1.2.5/src/edgepi/tc/tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/utilities/crc_8_atm.py` & `edgepi-python-sdk-1.2.5/src/edgepi/utilities/crc_8_atm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi/utilities/utilities.py` & `edgepi-python-sdk-1.2.5/src/edgepi/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/PKG-INFO` & `edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgepi-python-sdk
-Version: 1.2.2
+Version: 1.2.5
 Summary: EdgePi Python SDK package
 Home-page: https://github.com/EdgePi-Cloud/edgepi-python-sdk
 Author: S.Park
 Author-email: spark@osensa.com
 Project-URL: Bug Tracker, https://github.com/EdgePi-Cloud/edgepi-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `edgepi-python-sdk-1.2.2/src/edgepi_python_sdk.egg-info/SOURCES.txt` & `edgepi-python-sdk-1.2.5/src/edgepi_python_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/edgepi/eeprom/edgepi_eeprom.py
 src/edgepi/eeprom/edgepi_eeprom_data.py
 src/edgepi/eeprom/eeprom_constants.py
 src/edgepi/eeprom/protobuf_assets/__init__.py
 src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/__init__.py
 src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_adc_module.py
 src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_dac_module.py
+src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_key_module.py
 src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_rtd_module.py
 src/edgepi/eeprom/protobuf_assets/eeprom_data_classes/eeprom_tc_module.py
 src/edgepi/eeprom/protobuf_assets/generated_pb2/__init__.py
 src/edgepi/eeprom/protobuf_assets/generated_pb2/adc_module_pb2.py
 src/edgepi/eeprom/protobuf_assets/generated_pb2/calibration_parameters_pb2.py
 src/edgepi/eeprom/protobuf_assets/generated_pb2/dac_module_pb2.py
 src/edgepi/eeprom/protobuf_assets/generated_pb2/edgepi_module_pb2.py
```

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_adc/test_adc.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_adc/test_adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_dac/test_dac.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_dac/test_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_in/test_digital_in.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_digital_out/test_digital_out.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_eeprom/test_eeprom.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     # Write the original data back
     eeprom.write_edgepi_data(original_data)
 
 @pytest.mark.parametrize("bin_hash, error",
                         [
                          (None, pytest.raises(PermissionDenied)),
                          ("This is Dummy", pytest.raises(PermissionDenied)),
-                         ("48d088f7536e5c59938724b174184611", does_not_raise())
+                         ("6b68b8e2dd2a6bec300ef91572270723", does_not_raise())
                         ])
 def test_reset_edgepi_memory(bin_hash, error, eeprom):
     original_data = eeprom.read_edgepi_data()
     with error:
         eeprom.reset_edgepi_memory(bin_hash, base64.b64decode(DEFAULT_EEPROM_BIN_B64))
         written_data = eeprom.read_edgepi_data()
         default_data = eeprom.eeprom_pb.ParseFromString(base64.b64decode(DEFAULT_EEPROM_BIN_B64))
```

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_gpio/test_gpio.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_gpio/test_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_led/test_led.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_led/test_led.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_peripherals/test_i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_pwm/test_edgepi_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_relay/test_relay.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_relay/test_relay.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/integration_tests/test_tc/test_tc.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/integration_tests/test_tc/test_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_multiplexers.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_state.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_state.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_status.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_status.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_adc_voltage.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_adc/test_edgepi_adc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_edgepi_calibration.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_calibration/test_protobuf_mapping.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_dac_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dac/test_edgepi_dac.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_din/test_edgepi_din.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_dout/test_edgepi_dout.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_eeprom/test_access_eeprom.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         else:
             assert eeprom.data_list == []
 
 @pytest.mark.parametrize("bin_hash, error",
                         [
                          (None, pytest.raises(PermissionDenied)),
                          ("This is Dummy", pytest.raises(PermissionDenied)),
-                         ("48d088f7536e5c59938724b174184611", does_not_raise())
+                         ("6b68b8e2dd2a6bec300ef91572270723", does_not_raise())
                         ])
 def test_reset_edgepi_memory(mocker, bin_hash, error, eeprom):
     mocker.patch(
         "edgepi.eeprom.edgepi_eeprom.EdgePiEEPROM._EdgePiEEPROM__write_edgepi_reserved_memory")
     with error:
         eeprom.reset_edgepi_memory(bin_hash, base64.b64decode(DEFAULT_EEPROM_BIN_B64))
```

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgepi_gpio_expander.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_edgpepi_gpio_chip.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_config.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_gpio/test_gpio_constants.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_gpio.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_i2c.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_peripherals/test_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_pwm/test_edgepi_pwm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_reg_helper/test_reg_helper.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_relay/test_relay.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_relay/test_relay.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_edgepi_tc.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_commands.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_conv_time.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_tc/test_tc_faults.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_crc_8_atm.py`

 * *Files identical despite different names*

### Comparing `edgepi-python-sdk-1.2.2/src/test_edgepi/unit_tests/test_utilities/test_utilities.py` & `edgepi-python-sdk-1.2.5/src/test_edgepi/unit_tests/test_utilities/test_utilities.py`

 * *Files identical despite different names*

