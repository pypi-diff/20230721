# Comparing `tmp/Thermobar-1.0.7.tar.gz` & `tmp/Thermobar-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Thermobar-1.0.7.tar", last modified: Fri Dec 16 19:05:04 2022, max compression
+gzip compressed data, was "Thermobar-1.0.9.tar", last modified: Wed Dec 28 04:37:54 2022, max compression
```

## Comparing `Thermobar-1.0.7.tar` & `Thermobar-1.0.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:05:04.207567 Thermobar-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2022-12-16 19:05:04.207567 Thermobar-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2022-12-16 19:04:52.000000 Thermobar-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-16 19:05:04.207567 Thermobar-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2022-12-16 19:04:54.000000 Thermobar-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:05:04.195567 Thermobar-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:05:04.207567 Thermobar-1.0.7/src/Thermobar/
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Brugman_2019_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    53409 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Brugman_2019_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   183916 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Jorgenson2022_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  1633192 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Jorgenson2022_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      690 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/ML_scaler_Petrelli2020_Cpx_Only.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Masotta_2013_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    66746 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Masotta_2013_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Mutch_Cali_Amp.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    46260 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Mutch_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/NeavePutirka_2017_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    91834 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/NeavePutirka_2017_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    17235 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Nimis_1999.py
--rw-r--r--   0 runner    (1001) docker     (123)    75764 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Petrelli20_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   669647 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Petrelli20_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    17505 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Putirka16_Cali_Amp.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   110244 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Putirka16_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   111756 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Putirka2008_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   990303 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Putirka2008_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Ridolfi_Cali_Amp.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    49946 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Ridolfi_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    50147 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Wang21_Cali_Cpx.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   441503 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Wang21_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    34438 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Waters_Lange2015_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    14489 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Zhang17_Cali_Amp.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    99829 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/Zhang17_Cali_input.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    67247 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/amphibole.py
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/calibration_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)   141770 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/clinopyroxene_thermobarometry.py
--rw-r--r--   0 runner    (1001) docker     (123)   199469 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/density_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    64888 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/feldspar.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/garnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    26616 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/garnet_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    31721 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/garnet_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12490 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/geotherm.py
--rw-r--r--   0 runner    (1001) docker     (123)    39474 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/liquid_barometers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21932 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/liquid_thermometers.py
--rw-r--r--   0 runner    (1001) docker     (123)    57581 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/mineral_equilibrium.py
--rw-r--r--   0 runner    (1001) docker     (123)    26490 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/noise_averaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    28517 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/olivine_liquid_olivine_spinel_thermometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    34136 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/orthopyroxene_thermobarometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24119 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/pyroxenes_garnet.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/scaler_MinClass.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/spinel.py
--rw-r--r--   0 runner    (1001) docker     (123)   615624 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/svc_model_linear_MinClass.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    37404 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/two_pyroxene.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2022-12-16 19:04:54.000000 Thermobar-1.0.7/src/Thermobar/viscosity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-16 19:05:04.207567 Thermobar-1.0.7/src/Thermobar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2022-12-16 19:05:04.000000 Thermobar-1.0.7/src/Thermobar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2022-12-16 19:05:04.000000 Thermobar-1.0.7/src/Thermobar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-16 19:05:04.000000 Thermobar-1.0.7/src/Thermobar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-16 19:05:04.000000 Thermobar-1.0.7/src/Thermobar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-16 19:05:04.000000 Thermobar-1.0.7/src/Thermobar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 04:37:54.937394 Thermobar-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2022-12-28 04:37:54.937394 Thermobar-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2022-12-28 04:37:43.000000 Thermobar-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-28 04:37:54.937394 Thermobar-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2022-12-28 04:37:45.000000 Thermobar-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 04:37:54.917394 Thermobar-1.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 04:37:54.933394 Thermobar-1.0.9/src/Thermobar/
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Brugman_2019_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    53409 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Brugman_2019_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   183916 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Jorgenson2022_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  1633192 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Jorgenson2022_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/ML_scaler_Petrelli2020_Cpx_Only.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Masotta_2013_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    66746 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Masotta_2013_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Mutch_Cali_Amp.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    46260 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Mutch_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/NeavePutirka_2017_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    91834 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/NeavePutirka_2017_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    17235 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Nimis_1999.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75764 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Petrelli20_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   669647 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Petrelli20_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    17505 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Putirka16_Cali_Amp.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   110244 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Putirka16_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   111756 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Putirka2008_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   990303 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Putirka2008_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Ridolfi_Cali_Amp.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    49946 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Ridolfi_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    50147 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Wang21_Cali_Cpx.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   441503 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Wang21_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    34438 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Waters_Lange2015_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Zhang17_Cali_Amp.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    99829 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/Zhang17_Cali_input.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67247 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/amphibole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/calibration_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)   141770 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/clinopyroxene_thermobarometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199469 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/density_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64888 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/feldspar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/garnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26616 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/garnet_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31721 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/garnet_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12490 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/geotherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39702 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/liquid_barometers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21932 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/liquid_thermometers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57581 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/mineral_equilibrium.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26490 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/noise_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28517 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/olivine_liquid_olivine_spinel_thermometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34136 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/orthopyroxene_thermobarometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24119 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/pyroxenes_garnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/scaler_MinClass.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/spinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)   615624 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/svc_model_linear_MinClass.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    37404 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/two_pyroxene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2022-12-28 04:37:45.000000 Thermobar-1.0.9/src/Thermobar/viscosity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 04:37:54.933394 Thermobar-1.0.9/src/Thermobar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2022-12-28 04:37:54.000000 Thermobar-1.0.9/src/Thermobar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2022-12-28 04:37:54.000000 Thermobar-1.0.9/src/Thermobar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 04:37:54.000000 Thermobar-1.0.9/src/Thermobar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2022-12-28 04:37:54.000000 Thermobar-1.0.9/src/Thermobar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-28 04:37:54.000000 Thermobar-1.0.9/src/Thermobar.egg-info/top_level.txt
```

### Comparing `Thermobar-1.0.7/PKG-INFO` & `Thermobar-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thermobar
-Version: 1.0.7
+Version: 1.0.9
 Summary: Thermobar
 Home-page: https://github.com/PennyWieser/Thermobar
 Author: Penny, Maurizio, Jordan, Eric, Sinan
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/Thermobar)](https://pypi.org/project/Thermobar/)
         [![Build Status](https://github.com/PennyWieser/Thermobar/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/Thermobar/actions/workflows/main.yml)
```

### Comparing `Thermobar-1.0.7/README.md` & `Thermobar-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/setup.py` & `Thermobar-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Brugman_2019_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/Brugman_2019_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Brugman_2019_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Brugman_2019_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Jorgenson2022_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/Jorgenson2022_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Jorgenson2022_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Jorgenson2022_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/ML_scaler_Petrelli2020_Cpx_Only.pkl` & `Thermobar-1.0.9/src/Thermobar/ML_scaler_Petrelli2020_Cpx_Only.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Masotta_2013_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/Masotta_2013_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Masotta_2013_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Masotta_2013_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Mutch_Cali_Amp.pkl` & `Thermobar-1.0.9/src/Thermobar/Mutch_Cali_Amp.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Mutch_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Mutch_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/NeavePutirka_2017_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/NeavePutirka_2017_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/NeavePutirka_2017_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/NeavePutirka_2017_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Nimis_1999.py` & `Thermobar-1.0.9/src/Thermobar/Nimis_1999.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Petrelli20_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/Petrelli20_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Petrelli20_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Petrelli20_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Putirka16_Cali_Amp.pkl` & `Thermobar-1.0.9/src/Thermobar/Putirka16_Cali_Amp.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Putirka16_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Putirka16_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Putirka2008_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/Putirka2008_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Putirka2008_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Putirka2008_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Ridolfi_Cali_Amp.pkl` & `Thermobar-1.0.9/src/Thermobar/Ridolfi_Cali_Amp.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Ridolfi_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Ridolfi_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Wang21_Cali_Cpx.pkl` & `Thermobar-1.0.9/src/Thermobar/Wang21_Cali_Cpx.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Wang21_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Wang21_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Waters_Lange2015_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Waters_Lange2015_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Zhang17_Cali_Amp.pkl` & `Thermobar-1.0.9/src/Thermobar/Zhang17_Cali_Amp.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/Zhang17_Cali_input.pkl` & `Thermobar-1.0.9/src/Thermobar/Zhang17_Cali_input.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/__init__.py` & `Thermobar-1.0.9/src/Thermobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/amphibole.py` & `Thermobar-1.0.9/src/Thermobar/amphibole.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/calibration_plots.py` & `Thermobar-1.0.9/src/Thermobar/calibration_plots.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/clinopyroxene_thermobarometry.py` & `Thermobar-1.0.9/src/Thermobar/clinopyroxene_thermobarometry.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/core.py` & `Thermobar-1.0.9/src/Thermobar/core.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/density_profiles.py` & `Thermobar-1.0.9/src/Thermobar/density_profiles.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/feldspar.py` & `Thermobar-1.0.9/src/Thermobar/feldspar.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/garnet.py` & `Thermobar-1.0.9/src/Thermobar/garnet.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/garnet_class.py` & `Thermobar-1.0.9/src/Thermobar/garnet_class.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/garnet_plot.py` & `Thermobar-1.0.9/src/Thermobar/garnet_plot.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/geotherm.py` & `Thermobar-1.0.9/src/Thermobar/geotherm.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/import_export.py` & `Thermobar-1.0.9/src/Thermobar/import_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,23 +376,29 @@
     if suffix is not None:
         if any(my_input.columns.str.contains("FeO")) and (all(my_input.columns.str.contains("FeOt")==False)):
             raise ValueError("No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
             " thermobar only recognises columns with FeOt for all phases except liquid"
             " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
 
     if any(my_input.columns.str.contains("FeO_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
-        raise ValueError("No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
-        " thermobar only recognises columns with FeOt for all phases except liquid"
-        " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
 
-    if any(my_input.columns.str.contains("Fe2O3_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
-        raise ValueError("No FeOt column found. You've got a column heading with Fe2O3. To avoid errors based on common EPMA outputs"
+        if any(my_input.columns.str.contains("FeO_Liq")) and any(my_input.columns.str.contains("Fe2O3_Liq")):
+            my_input_c['FeOt_Liq']=my_input_c['FeO_Liq']+my_input_c['Fe2O3_Liq']*0.89998
+
+
+        else:
+            raise ValueError("No FeOt found. You've got a column heading with FeO. To avoid errors based on common EPMA outputs"
         " thermobar only recognises columns with FeOt for all phases except liquid"
         " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
 
+    # if any(my_input.columns.str.contains("Fe2O3_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
+    #     raise ValueError("No FeOt column found. You've got a column heading with Fe2O3. To avoid errors based on common EPMA outputs"
+    #     " thermobar only recognises columns with FeOt for all phases except liquid"
+    #     " where you can also enter a Fe3Fet_Liq heading used for equilibrium tests")
+
     if any(my_input.columns.str.contains("FeOT_")) and (all(my_input.columns.str.contains("FeOt_")==False)):
         raise ValueError("No FeOt column found. You've got a column heading with FeOT. Change to a lower case t")
 
 
 
  #   myLabels=my_input.Sample_ID
 
@@ -770,15 +776,15 @@
 
    Returns
     -------
     DataFrame formatted so that it can be inputted into VESIcal.
 
     '''
     df = liq_comps.copy()
-    if unit is Kelvin:
+    if unit=='Kelvin':
         df['Temp'] = T1 - 273.15
     else:
         df['Temp'] = T1
     if Fe3Fet_Liq is None:
         Fe3Fet_Liq=df['Fe3Fet_Liq']
     FeOt=df['FeOt_Liq']
     df.drop(['Fe3Fet_Liq', 'FeOt_Liq'], inplace=True, axis=1)
```

### Comparing `Thermobar-1.0.7/src/Thermobar/liquid_thermometers.py` & `Thermobar-1.0.9/src/Thermobar/liquid_thermometers.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/mineral_equilibrium.py` & `Thermobar-1.0.9/src/Thermobar/mineral_equilibrium.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/noise_averaging.py` & `Thermobar-1.0.9/src/Thermobar/noise_averaging.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/olivine_liquid_olivine_spinel_thermometry.py` & `Thermobar-1.0.9/src/Thermobar/olivine_liquid_olivine_spinel_thermometry.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/orthopyroxene_thermobarometry.py` & `Thermobar-1.0.9/src/Thermobar/orthopyroxene_thermobarometry.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/plotting.py` & `Thermobar-1.0.9/src/Thermobar/plotting.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/pyroxenes_garnet.py` & `Thermobar-1.0.9/src/Thermobar/pyroxenes_garnet.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/scaler_MinClass.pkl` & `Thermobar-1.0.9/src/Thermobar/scaler_MinClass.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/spinel.py` & `Thermobar-1.0.9/src/Thermobar/spinel.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/svc_model_linear_MinClass.pkl` & `Thermobar-1.0.9/src/Thermobar/svc_model_linear_MinClass.pkl`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/two_pyroxene.py` & `Thermobar-1.0.9/src/Thermobar/two_pyroxene.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar/viscosity.py` & `Thermobar-1.0.9/src/Thermobar/viscosity.py`

 * *Files identical despite different names*

### Comparing `Thermobar-1.0.7/src/Thermobar.egg-info/PKG-INFO` & `Thermobar-1.0.9/src/Thermobar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Thermobar
-Version: 1.0.7
+Version: 1.0.9
 Summary: Thermobar
 Home-page: https://github.com/PennyWieser/Thermobar
 Author: Penny, Maurizio, Jordan, Eric, Sinan
 Author-email: penny.wieser@gmail.com
 License: UNKNOWN
 Description: [![PyPI](https://badgen.net/pypi/v/Thermobar)](https://pypi.org/project/Thermobar/)
         [![Build Status](https://github.com/PennyWieser/Thermobar/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/PennyWieser/Thermobar/actions/workflows/main.yml)
```

### Comparing `Thermobar-1.0.7/src/Thermobar.egg-info/SOURCES.txt` & `Thermobar-1.0.9/src/Thermobar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

