# Comparing `tmp/gwbench-0.7.0.tar.gz` & `tmp/gwbench-0.7.1.tar.gz`

## Comparing `gwbench-0.7.0.tar` & `gwbench-0.7.1.tar`

### file list

```diff
@@ -1,75 +1,77 @@
--rw-r--r--   0        0        0     4943 2020-02-02 00:00:00.000000 gwbench-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 gwbench-0.7.0/a.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 gwbench-0.7.0/requirements_conda.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gwbench-0.7.0/requirements_pip.txt
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 gwbench-0.7.0/setup.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/__init__.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/compute_ant_pat_lpf_psd.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/generate_lambdified_functions.py
--rw-r--r--   0        0        0     9539 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/multi_network.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/num_gw_benchmarking.py
--rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/quick_start.ipynb
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/quick_start.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 gwbench-0.7.0/example_scripts/sym_gw_benchmarking.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/__init__.py
--rw-r--r--   0        0        0     8945 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/antenna_pattern_np.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/antenna_pattern_sp.py
--rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/basic_relations.py
--rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/detector.py
--rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/detector_response_derivatives.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/err_deriv_handling.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/fisher_analysis_tools.py
--rw-r--r--   0        0        0    22859 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/injections.py
--rw-r--r--   0        0        0    25552 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/network.py
--rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/psd.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/snr.py
--rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/utils.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/waveform.py
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_derivatives_num.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_derivatives_sym.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/__init__.py
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/a_plus.txt
--rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/a_sharp.txt
--rw-r--r--   0        0        0    87000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/advirgo_plus.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_10km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_10km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_20km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_20km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_30km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_30km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_40km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce1_40km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_10km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_10km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_20km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_20km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_30km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_30km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_40km_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/ce2_40km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_20km.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_20km_pm.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_40km.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_40km_lf.txt
--rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/et.txt
--rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/et_10km_xylophone.txt
--rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/kagra_plus.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/voyager_cb.txt
--rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/noise_curves/voyager_pm.txt
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/__init__.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/lal_bbh_np.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/lal_bns_np.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/tf2_np.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/tf2_sp.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/tf2_tidal_np.py
--rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 gwbench-0.7.0/gwbench/wf_models/tf2_tidal_sp.py
--rw-r--r--   0        0        0  2500050 2020-02-02 00:00:00.000000 gwbench-0.7.0/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gwbench-0.7.0/xtra_files/requirements_txts/requirements_conda_pre2021_09_21.txt
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 gwbench-0.7.0/xtra_files/requirements_txts/requirements_conda_pre2023_06_19.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gwbench-0.7.0/.gitignore
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 gwbench-0.7.0/AUTHORS.md
--rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 gwbench-0.7.0/LICENSE
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 gwbench-0.7.0/README.md
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 gwbench-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 gwbench-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 gwbench-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 gwbench-0.7.1/requirements_conda.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 gwbench-0.7.1/requirements_pip.txt
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 gwbench-0.7.1/setup.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/__init__.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/compute_ant_pat_lpf_psd.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/generate_lambdified_functions.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/multi_network.py
+-rw-r--r--   0        0        0     6674 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/num_gw_benchmarking.py
+-rw-r--r--   0        0        0     7251 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/quick_start.ipynb
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/quick_start.py
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 gwbench-0.7.1/example_scripts/sym_gw_benchmarking.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/__init__.py
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/antenna_pattern_np.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/antenna_pattern_sp.py
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/basic_relations.py
+-rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/detector.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/detector_response_derivatives.py
+-rw-r--r--   0        0        0     4306 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/err_deriv_handling.py
+-rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/fisher_analysis_tools.py
+-rw-r--r--   0        0        0    23012 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/injections.py
+-rw-r--r--   0        0        0    26350 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/network.py
+-rw-r--r--   0        0        0     8972 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/psd.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/snr.py
+-rw-r--r--   0        0        0     8548 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/utils.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/waveform.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_derivatives_ana.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_derivatives_num.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_derivatives_sym.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/__init__.py
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/a_plus.txt
+-rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/a_sharp.txt
+-rw-r--r--   0        0        0    87000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/advirgo_plus.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_10km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_10km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_20km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_20km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_30km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_30km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_40km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce1_40km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_10km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_10km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_20km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_20km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_30km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_30km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_40km_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/ce2_40km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_20km.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_20km_pm.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_40km.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_40km_lf.txt
+-rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/et.txt
+-rw-r--r--   0        0        0   150000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/et_10km_xylophone.txt
+-rw-r--r--   0        0        0    23000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/kagra_plus.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/voyager_cb.txt
+-rw-r--r--   0        0        0    50000 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/noise_curves/voyager_pm.txt
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/__init__.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/lal_bbh_np.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/lal_bns_np.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/tf2_np.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/tf2_sp.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/tf2_tidal_np.py
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 gwbench-0.7.1/gwbench/wf_models/tf2_tidal_sp.py
+-rw-r--r--   0        0        0  2500050 2020-02-02 00:00:00.000000 gwbench-0.7.1/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 gwbench-0.7.1/xtra_files/pypi/pyproject.toml
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gwbench-0.7.1/xtra_files/pypi/tutorial.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gwbench-0.7.1/xtra_files/requirements_txts/requirements_conda_pre2021_09_21.txt
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 gwbench-0.7.1/xtra_files/requirements_txts/requirements_conda_pre2023_06_19.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gwbench-0.7.1/.gitignore
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 gwbench-0.7.1/AUTHORS.md
+-rw-r--r--   0        0        0    15200 2020-02-02 00:00:00.000000 gwbench-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 gwbench-0.7.1/README.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 gwbench-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 gwbench-0.7.1/PKG-INFO
```

### Comparing `gwbench-0.7.0/CHANGELOG.md` & `gwbench-0.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## [0.7.1] - 2023-07-21
+
+### Added/Changed
+
+* switched to Ver 0.7.1
+* added the ability to choose analytical derivatives for DL, tc, phic (changes in wf_derivatives_num + where needed, added of wf_derivatives_ana)
+* improved example_scripts to reflect this possibility
+* fixed bug in injections.py
+* cleaned up some code
+
 ## [0.7.0] - 2023-06-19
 
 ### Added/Changed
 
 * switched to Ver 0.7.0
 * **noise curves**
   * added 4 most recent, official CE curves from https://dcc.cosmicexplorer.org/CE-T2000017/public
```

### Comparing `gwbench-0.7.0/example_scripts/README.md` & `gwbench-0.7.1/example_scripts/README.md`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/example_scripts/__init__.py` & `gwbench-0.7.1/example_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/example_scripts/compute_ant_pat_lpf_psd.py` & `gwbench-0.7.1/example_scripts/compute_ant_pat_lpf_psd.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/example_scripts/generate_lambdified_functions.py` & `gwbench-0.7.1/example_scripts/generate_lambdified_functions.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/example_scripts/multi_network.py` & `gwbench-0.7.1/example_scripts/multi_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,23 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 
-import argparse
-import os
-import sys
-
 import numpy as np
 from lal import GreenwichMeanSiderealTime
 
 import gwbench.basic_relations as brs
 import gwbench.injections as injections
 import gwbench.network as network
 
 np.set_printoptions(linewidth=200)
 
-
 ############################################################################
 ### User Choices
 ############################################################################
 
 # injection ID
 inj_id = 0
 
@@ -50,22 +45,30 @@
 # user defined waveform model
 if 1: user_waveform = None
 else:
     wf_model_name    = 'tf2_user'
     wf_other_var_dic = None
     user_waveform   = {'np': '../gwbench/wf_models/tf2_np.py', 'sp':'../gwbench/wf_models/tf2_sp.py'}
 
+# example detector location defined by user
+user_locs = {'user-loc':{'longitude': 3.2, 'latitude': 0.4, 'arm_azimuth':0.3, 'which_arm':'y', 'shape':'L'}}
+# example detector psd defined by the user
+user_psds = {'user-tec':{'psd_file':'../gwbench/noise_curves/ce2_40km_cb.txt', 'is_asd':True}}
+
 # user's choice: with respect to which parameters to take derivatives for the Fisher analysis
 if 'tidal' in wf_model_name or 'bns' in wf_model_name: deriv_symbs_string = 'Mc eta chi1z chi2z DL tc phic iota lam_t ra dec psi'
 else: deriv_symbs_string = 'Mc eta chi1z chi2z DL tc phic iota ra dec psi'
 
 # user's choice: convert derivatives to cos or log for specific variables
 conv_cos = ('dec','iota')
 conv_log = ('Mc','DL','lam_t')
 
+# user's choice: switch derivatives of DL, tc, and phic to be analytical
+ana_deriv_symbs_list = ('DL', 'tc', 'phic')
+
 # if symbolic derivatives, take from generate_lambdified_functions.py
 # if numeric  derivatives, user's decision
 use_rot = 0
 # 1 for True, 0 for False
 # calculate SNRs, error matrices, and errors only for the network
 only_net = 1
 
@@ -73,17 +76,17 @@
 sym_derivs = 0
 
 # number of cores to use to parallelize the calculation of unique detector response derivatives
 # = None for no parallelization, = 2,3,4,... to allocate N cores (even numbers preferred)
 num_cores = None
 
 # choose numdifftools parameters for numerical derivatives
-step = 1e-9
-method = 'central'
-order = 2
+step      = 1e-9
+method    = 'central'
+order     = 2
 d_order_n = 1
 
 # user's choice to generate injection parameters
 if 'tidal' in wf_model_name or 'bns' in wf_model_name:
     mmin      = 0.8
     mmax      = 3
     chi_lo    = -0.05
@@ -96,102 +99,65 @@
 
 cosmo_dict = {'zmin':0, 'zmax':0.2, 'sampler':'uniform_comoving_volume_inversion'}
 mass_dict  = {'dist':'uniform', 'mmin':mmin, 'mmax':mmax}
 # the default waveforms above are non-precessing, hence dim=1, set dim=3 for precessing waveforms like 'IMRPhenomPv2' or 'IMRPhenomPv2_NRTidalv2'
 spin_dict  = {'dim':1, 'geom':'cartesian', 'chi_lo':chi_lo, 'chi_hi':chi_hi}
 
 redshifted = 1
-num_injs  = 100
-seed  = 29378
-file_path = None
+num_injs   = 100
+seed       = 29378
+file_path  = None
 
 injections_data = injections.injections_CBC_params_redshift(cosmo_dict,mass_dict,spin_dict,redshifted,num_injs,seed,file_path)
 
 ############################################################################
-### Print the choices
-############################################################################
-
-#-----output run settings-----
-print('---run settings---')
-print('wf_model_name = ',wf_model_name)
-print('wf_other_var_dic = ',wf_other_var_dic)
-print('deriv_symbs_string = ',deriv_symbs_string)
-print()
-print('conv_cos = ',conv_cos)
-print('conv_log = ',conv_log)
-print()
-print('use_rot = ',use_rot)
-print('only_net = ',only_net)
-print()
-print('step = ',step)
-print('method = ',method)
-print('order = ',order)
-print('d_order_n = ',d_order_n)
-print()
-print('cosmo_dict = ',cosmo_dict)
-print('mass_dict = ',mass_dict)
-print('spin_dict = ',spin_dict)
-print('seed = ',seed)
-print('num_injs = ',num_injs)
-print('file_path',file_path)
-print('---run settings done---')
-print()
-
-############################################################################
 ### injection parameters
 ############################################################################
 
-inj_params                    = dict()
-
-inj_params['Mc']              = injections_data[0][inj_id]
-inj_params['eta']             = injections_data[1][inj_id]
-inj_params['chi1x']           = injections_data[2][inj_id]
-inj_params['chi1y']           = injections_data[3][inj_id]
-inj_params['chi1z']           = injections_data[4][inj_id]
-inj_params['chi2x']           = injections_data[5][inj_id]
-inj_params['chi2y']           = injections_data[6][inj_id]
-inj_params['chi2z']           = injections_data[7][inj_id]
-inj_params['DL']              = injections_data[8][inj_id]
-inj_params['tc']              = 0.
-inj_params['phic']            = 0.
-inj_params['iota']            = injections_data[9][inj_id]
+inj_params = {
+    'Mc'    : injections_data[0][inj_id],
+    'eta'   : injections_data[1][inj_id],
+    'chi1x' : injections_data[2][inj_id],
+    'chi1y' : injections_data[3][inj_id],
+    'chi1z' : injections_data[4][inj_id],
+    'chi2x' : injections_data[5][inj_id],
+    'chi2y' : injections_data[6][inj_id],
+    'chi2z' : injections_data[7][inj_id],
+    'DL'    : injections_data[8][inj_id],
+    'tc'    : 0.,
+    'phic'  : 0.,
+    'iota'  : injections_data[9][inj_id],
+    'ra'    : injections_data[10][inj_id],
+    'dec'   : injections_data[11][inj_id],
+    'psi'   : injections_data[12][inj_id],
+    'gmst0' : GreenwichMeanSiderealTime(1247227950.),
+    'z'     : injections_data[13][inj_id],
+    }
 
 if 'tidal' in wf_model_name or 'bns' in wf_model_name:
     inj_params['lam_t']       = 600.
     inj_params['delta_lam_t'] = 0.
 
-inj_params['ra']              = injections_data[10][inj_id]
-inj_params['dec']             = injections_data[11][inj_id]
-inj_params['psi']             = injections_data[12][inj_id]
-inj_params['gmst0']           = GreenwichMeanSiderealTime(1247227950.)
-inj_params['z']               = injections_data[13][inj_id]
-
 print('injections parameter: ', inj_params)
 print()
 
 ############################################################################
-### User choices
+### Network specification
 ############################################################################
 
-# example detector location defined by user
-user_locs = {'user-loc':{'longitude': 3.2, 'latitude': 0.4, 'arm_azimuth':0.3, 'which_arm':'y', 'shape':'L'}}
-
-# example detector psd defined by the user
-user_psds = {'user-tec':{'psd_file':'../gwbench/noise_curves/ce2_40km_cb.txt', 'is_asd':True}}
-
 network_specs = [ ['CE2-40-CBO_H','CE2-40-CBO_L','CE2-40-CBO_V']        ,
                   ['CE2-40-CBO_H','CE2-40-CBO_L','CE2-40-CBO_user-loc'] ,
                   ['CE2-40-CBO_H','CE2-40-CBO_V','user-tec_user-loc']   ]
 print('network specs: ', network_specs)
 print()
 
 f_lo = 1.
 f_hi = brs.f_isco_Msolar(brs.M_of_Mc_eta(inj_params['Mc'],inj_params['eta']))
-df = 2.**-4
-f = np.arange(f_lo,f_hi+df,df)
+df   = 2.**-4
+f    = np.arange(f_lo,f_hi+df,df)
 
 print('f_lo:', f_lo, '   f_hi:', f_hi, '   df:', df)
 print()
 
 ############################################################################
 ### Precalculate the unique components common among all networks
 ############################################################################
@@ -203,14 +169,15 @@
                                                        conv_cos=conv_cos, conv_log=conv_log, use_rot=use_rot, num_cores=num_cores,
                                                        user_waveform=user_waveform, user_locs=user_locs)
 else:
     unique_loc_net = network.unique_locs_det_responses(network_specs, f, inj_params, deriv_symbs_string,
                                                        wf_model_name, wf_other_var_dic=wf_other_var_dic,
                                                        conv_cos=conv_cos, conv_log=conv_log, use_rot=use_rot, num_cores=num_cores,
                                                        user_waveform=user_waveform, user_locs=user_locs,
+                                                       ana_deriv_symbs_list=ana_deriv_symbs_list,
                                                        step=step, method=method, order=order, n=d_order_n)
 
 # get the unique PSDs for the various detector technologies
 unique_tec_net = network.unique_tecs(network_specs, f, user_psds=user_psds)
 
 ############################################################################
 ### Perform the analysis for each network from the unique components
```

### Comparing `gwbench-0.7.0/example_scripts/num_gw_benchmarking.py` & `gwbench-0.7.1/example_scripts/num_gw_benchmarking.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,28 +11,23 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 
-import argparse
-import os
-import sys
-
 import numpy as np
 from lal import GreenwichMeanSiderealTime
 
 import gwbench.basic_relations as brs
 import gwbench.injections as injections
 import gwbench.network as network
 
 np.set_printoptions(linewidth=200)
 
-
 ############################################################################
 ### User Choices
 ############################################################################
 
 # injection ID
 inj_id = 0
 
@@ -50,33 +45,41 @@
 # user defined waveform model
 if 1: user_waveform = None
 else:
     wf_model_name    = 'tf2_user'
     wf_other_var_dic = None
     user_waveform   = {'np': '../gwbench/wf_models/tf2_np.py', 'sp':'../gwbench/wf_models/tf2_sp.py'}
 
+# example detector location defined by user
+user_locs = {'user-loc':{'longitude': 3.2, 'latitude': 0.4, 'arm_azimuth':0.3, 'which_arm':'y', 'shape':'L'}}
+# example detector psd defined by the user
+user_psds = {'user-tec':{'psd_file':'../gwbench/noise_curves/ce2_40km_cb.txt', 'is_asd':True}}
+
 # user's choice: with respect to which parameters to take derivatives for the Fisher analysis
 if 'tidal' in wf_model_name or 'bns' in wf_model_name: deriv_symbs_string = 'Mc eta chi1z chi2z DL tc phic iota lam_t ra dec psi'
 else: deriv_symbs_string = 'Mc eta chi1z chi2z DL tc phic iota ra dec psi'
 
 # user's choice: convert derivatives to cos or log for specific variables
 conv_cos = ('dec','iota')
 conv_log = ('Mc','DL','lam_t')
 
+# user's choice: switch derivatives of DL, tc, and phic to be analytical
+ana_deriv_symbs_list = ('DL', 'tc', 'phic')
+
 # if symbolic derivatives, take from generate_lambdified_functions.py
 # if numeric  derivatives, user's decision
 use_rot = 0
 # 1 for True, 0 for False
 # calculate SNRs, error matrices, and errors only for the network
 only_net = 1
 
 # choose numdifftools parameters for numerical derivatives
-step = 1e-9
-method = 'central'
-order = 2
+step      = 1e-9
+method    = 'central'
+order     = 2
 d_order_n = 1
 
 # user's choice to generate injection parameters
 if 'tidal' in wf_model_name or 'bns' in wf_model_name:
     mmin      = 0.8
     mmax      = 3
     chi_lo    = -0.05
@@ -89,114 +92,77 @@
 
 cosmo_dict = {'zmin':0, 'zmax':0.2, 'sampler':'uniform_comoving_volume_inversion'}
 mass_dict  = {'dist':'uniform', 'mmin':mmin, 'mmax':mmax}
 # the default waveforms above are non-precessing, hence dim=1, set dim=3 for precessing waveforms like 'IMRPhenomPv2' or 'IMRPhenomPv2_NRTidalv2'
 spin_dict  = {'dim':1, 'geom':'cartesian', 'chi_lo':chi_lo, 'chi_hi':chi_hi}
 
 redshifted = 1
-num_injs  = 100
-seed  = 29378
-file_path = None
+num_injs   = 100
+seed       = 29378
+file_path  = None
 
 injections_data = injections.injections_CBC_params_redshift(cosmo_dict,mass_dict,spin_dict,redshifted,num_injs,seed,file_path)
 
 ############################################################################
-### Print the choices
-############################################################################
-
-#-----output run settings-----
-print('---run settings---')
-print('wf_model_name = ',wf_model_name)
-print('wf_other_var_dic = ',wf_other_var_dic)
-print('deriv_symbs_string = ',deriv_symbs_string)
-print()
-print('conv_cos = ',conv_cos)
-print('conv_log = ',conv_log)
-print()
-print('use_rot = ',use_rot)
-print('only_net = ',only_net)
-print()
-print('step = ',step)
-print('method = ',method)
-print('order = ',order)
-print('d_order_n = ',d_order_n)
-print()
-print('cosmo_dict = ',cosmo_dict)
-print('mass_dict = ',mass_dict)
-print('spin_dict = ',spin_dict)
-print('seed = ',seed)
-print('num_injs = ',num_injs)
-print('file_path',file_path)
-print('---run settings done---')
-print()
-
-############################################################################
 ### injection parameters
 ############################################################################
 
-inj_params                    = dict()
-
-inj_params['Mc']              = injections_data[0][inj_id]
-inj_params['eta']             = injections_data[1][inj_id]
-inj_params['chi1x']           = injections_data[2][inj_id]
-inj_params['chi1y']           = injections_data[3][inj_id]
-inj_params['chi1z']           = injections_data[4][inj_id]
-inj_params['chi2x']           = injections_data[5][inj_id]
-inj_params['chi2y']           = injections_data[6][inj_id]
-inj_params['chi2z']           = injections_data[7][inj_id]
-inj_params['DL']              = injections_data[8][inj_id]
-inj_params['tc']              = 0.
-inj_params['phic']            = 0.
-inj_params['iota']            = injections_data[9][inj_id]
+inj_params = {
+    'Mc'    : injections_data[0][inj_id],
+    'eta'   : injections_data[1][inj_id],
+    'chi1x' : injections_data[2][inj_id],
+    'chi1y' : injections_data[3][inj_id],
+    'chi1z' : injections_data[4][inj_id],
+    'chi2x' : injections_data[5][inj_id],
+    'chi2y' : injections_data[6][inj_id],
+    'chi2z' : injections_data[7][inj_id],
+    'DL'    : injections_data[8][inj_id],
+    'tc'    : 0.,
+    'phic'  : 0.,
+    'iota'  : injections_data[9][inj_id],
+    'ra'    : injections_data[10][inj_id],
+    'dec'   : injections_data[11][inj_id],
+    'psi'   : injections_data[12][inj_id],
+    'gmst0' : GreenwichMeanSiderealTime(1247227950.),
+    'z'     : injections_data[13][inj_id],
+    }
 
 if 'tidal' in wf_model_name or 'bns' in wf_model_name:
     inj_params['lam_t']       = 600.
     inj_params['delta_lam_t'] = 0.
 
-inj_params['ra']              = injections_data[10][inj_id]
-inj_params['dec']             = injections_data[11][inj_id]
-inj_params['psi']             = injections_data[12][inj_id]
-inj_params['gmst0']           = GreenwichMeanSiderealTime(1247227950.)
-inj_params['z']               = injections_data[13][inj_id]
-
 print('injections parameter: ', inj_params)
 print()
 
 ############################################################################
-### User choices
+### Network specification
 ############################################################################
 
-# example detector location defined by user
-user_locs = {'user-loc':{'longitude': 3.2, 'latitude': 0.4, 'arm_azimuth':0.3, 'which_arm':'y', 'shape':'L'}}
-
-# example detector psd defined by the user
-user_psds = {'user-tec':{'psd_file':'../gwbench/noise_curves/ce2_40km_cb.txt', 'is_asd':True}}
-
 network_spec = ['CE2-40-CBO_C','CE2-40-CBO_S','user-tec_user-loc']
 print('network spec: ', network_spec)
 print()
 
 f_lo = 1.
 f_hi = brs.f_isco_Msolar(brs.M_of_Mc_eta(inj_params['Mc'],inj_params['eta']))
-df = 2.**-4
-f = np.arange(f_lo,f_hi+df,df)
+df   = 2.**-4
+f    = np.arange(f_lo,f_hi+df,df)
 
 print('f_lo:', f_lo, '   f_hi:', f_hi, '   df:', df)
 print()
 
 ############################################################################
 ### Numeric GW Benchmarking
 ############################################################################
 
 # initialize Network and do general setup
 net = network.Network(network_spec, logger_name='CSU', logger_level='DEBUG')
 net.set_wf_vars(wf_model_name, wf_other_var_dic=wf_other_var_dic, user_waveform=user_waveform)
 net.set_net_vars(f=f, inj_params=inj_params, deriv_symbs_string=deriv_symbs_string,
                  conv_cos=conv_cos, conv_log=conv_log, use_rot=use_rot,
-                 user_locs=user_locs, user_psds=user_psds)
+                 user_locs=user_locs, user_psds=user_psds, ana_deriv_symbs_list=ana_deriv_symbs_list)
 net.setup_ant_pat_lpf_psds()
 
 # start the actual analysis
 #-----numeric derivatives-------------------------------------
 net.calc_det_responses_derivs_num(step,method,order,d_order_n)
 #-------------------------------------------------------------
 net.calc_snrs(only_net=only_net)
```

### Comparing `gwbench-0.7.0/example_scripts/quick_start.ipynb` & `gwbench-0.7.1/example_scripts/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/example_scripts/quick_start.py` & `gwbench-0.7.1/example_scripts/quick_start.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/example_scripts/sym_gw_benchmarking.py` & `gwbench-0.7.1/example_scripts/sym_gw_benchmarking.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,28 +11,23 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 
-import argparse
-import os
-import sys
-
 import numpy as np
 from lal import GreenwichMeanSiderealTime
 
 import gwbench.basic_relations as brs
 import gwbench.injections as injections
 import gwbench.network as network
 
 np.set_printoptions(linewidth=200)
 
-
 ############################################################################
 ### User Choices
 ############################################################################
 
 # injection ID
 inj_id = 0
 
@@ -46,14 +41,19 @@
 # user defined waveform model
 if 1: user_waveform = None
 else:
     wf_model_name    = 'tf2_user'
     wf_other_var_dic = None
     user_waveform   = {'np': '../gwbench/wf_models/tf2_np.py', 'sp':'../gwbench/wf_models/tf2_sp.py'}
 
+# example detector location defined by user
+user_locs = {'user-loc':{'longitude': 3.2, 'latitude': 0.4, 'arm_azimuth':0.3, 'which_arm':'y', 'shape':'L'}}
+# example detector psd defined by the user
+user_psds = {'user-tec':{'psd_file':'../gwbench/noise_curves/ce2_40km_cb.txt', 'is_asd':True}}
+
 # user's choice: with respect to which parameters to take derivatives for the Fisher analysis
 if 'tidal' in wf_model_name or 'bns' in wf_model_name: deriv_symbs_string = 'Mc eta chi1z chi2z DL tc phic iota lam_t ra dec psi'
 else: deriv_symbs_string = 'Mc eta chi1z chi2z DL tc phic iota ra dec psi'
 
 # user's choice: convert derivatives to cos or log for specific variables
 conv_cos = ('dec','iota')
 conv_log = ('Mc','DL','lam_t')
@@ -79,95 +79,63 @@
 
 cosmo_dict = {'zmin':0, 'zmax':0.2, 'sampler':'uniform_comoving_volume_inversion'}
 mass_dict  = {'dist':'uniform', 'mmin':mmin, 'mmax':mmax}
 # the default waveforms above are non-precessing, hence dim=1, set dim=3 for precessing waveforms like 'IMRPhenomPv2' or 'IMRPhenomPv2_NRTidalv2'
 spin_dict  = {'dim':1, 'geom':'cartesian', 'chi_lo':chi_lo, 'chi_hi':chi_hi}
 
 redshifted = 1
-num_injs  = 100
-seed  = 29378
-file_path = None
+num_injs   = 100
+seed       = 29378
+file_path  = None
 
 injections_data = injections.injections_CBC_params_redshift(cosmo_dict,mass_dict,spin_dict,redshifted,num_injs,seed,file_path)
 
 ############################################################################
-### Print the choices
-############################################################################
-
-#-----output run settings-----
-print('---run settings---')
-print('wf_model_name = ',wf_model_name)
-print('wf_other_var_dic = ',wf_other_var_dic)
-print('deriv_symbs_string = ',deriv_symbs_string)
-print()
-print('conv_cos = ',conv_cos)
-print('conv_log = ',conv_log)
-print()
-print('use_rot = ',use_rot)
-print('only_net = ',only_net)
-print()
-print('cosmo_dict = ',cosmo_dict)
-print('mass_dict = ',mass_dict)
-print('spin_dict = ',spin_dict)
-print('seed = ',seed)
-print('num_injs = ',num_injs)
-print('file_path',file_path)
-print('---run settings done---')
-print()
-
-############################################################################
 ### injection parameters
 ############################################################################
 
-inj_params                    = dict()
-
-inj_params['Mc']              = injections_data[0][inj_id]
-inj_params['eta']             = injections_data[1][inj_id]
-inj_params['chi1x']           = injections_data[2][inj_id]
-inj_params['chi1y']           = injections_data[3][inj_id]
-inj_params['chi1z']           = injections_data[4][inj_id]
-inj_params['chi2x']           = injections_data[5][inj_id]
-inj_params['chi2y']           = injections_data[6][inj_id]
-inj_params['chi2z']           = injections_data[7][inj_id]
-inj_params['DL']              = injections_data[8][inj_id]
-inj_params['tc']              = 0.
-inj_params['phic']            = 0.
-inj_params['iota']            = injections_data[9][inj_id]
+inj_params = {
+    'Mc'    : injections_data[0][inj_id],
+    'eta'   : injections_data[1][inj_id],
+    'chi1x' : injections_data[2][inj_id],
+    'chi1y' : injections_data[3][inj_id],
+    'chi1z' : injections_data[4][inj_id],
+    'chi2x' : injections_data[5][inj_id],
+    'chi2y' : injections_data[6][inj_id],
+    'chi2z' : injections_data[7][inj_id],
+    'DL'    : injections_data[8][inj_id],
+    'tc'    : 0.,
+    'phic'  : 0.,
+    'iota'  : injections_data[9][inj_id],
+    'ra'    : injections_data[10][inj_id],
+    'dec'   : injections_data[11][inj_id],
+    'psi'   : injections_data[12][inj_id],
+    'gmst0' : GreenwichMeanSiderealTime(1247227950.),
+    'z'     : injections_data[13][inj_id],
+    }
 
 if 'tidal' in wf_model_name or 'bns' in wf_model_name:
     inj_params['lam_t']       = 600.
     inj_params['delta_lam_t'] = 0.
 
-inj_params['ra']              = injections_data[10][inj_id]
-inj_params['dec']             = injections_data[11][inj_id]
-inj_params['psi']             = injections_data[12][inj_id]
-inj_params['gmst0']           = GreenwichMeanSiderealTime(1247227950.)
-inj_params['z']               = injections_data[13][inj_id]
-
 print('injections parameter: ', inj_params)
 print()
 
 ############################################################################
-### User choices
+### Network specification
 ############################################################################
 
-# example detector location defined by user
-user_locs = {'user-loc':{'longitude': 3.2, 'latitude': 0.4, 'arm_azimuth':0.3, 'which_arm':'y', 'shape':'L'}}
-
-# example detector psd defined by the user
-user_psds = {'user-tec':{'psd_file':'../gwbench/noise_curves/ce2_40km_cb.txt', 'is_asd':True}}
-
 network_spec = ['CE2-40-CBO_C','CE2-40-CBO_S','user-tec_user-loc']
 print('network spec: ', network_spec)
 print()
 
 f_lo = 1.
 f_hi = brs.f_isco_Msolar(brs.M_of_Mc_eta(inj_params['Mc'],inj_params['eta']))
-df = 2.**-4
-f = np.arange(f_lo,f_hi+df,df)
+df   = 2.**-4
+f    = np.arange(f_lo,f_hi+df,df)
 
 print('f_lo:', f_lo, '   f_hi:', f_hi, '   df:', df)
 print()
 
 ############################################################################
 ### Symbolic GW Benchmarking
 ############################################################################
```

### Comparing `gwbench-0.7.0/gwbench/__init__.py` & `gwbench-0.7.1/gwbench/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/antenna_pattern_np.py` & `gwbench-0.7.1/gwbench/antenna_pattern_np.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 import numpy as np
 
-from gwbench.basic_relations import Mc_of_m1_m2, Mc_of_M_eta, Mc_of_M_q
 from gwbench.utils import time_fac, REarth, AU, cLight, is_subset_lists, log_msg
 
 cos = np.cos
 sin = np.sin
 exp = np.exp
 PI = np.pi
```

### Comparing `gwbench-0.7.0/gwbench/antenna_pattern_sp.py` & `gwbench-0.7.1/gwbench/antenna_pattern_sp.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/basic_relations.py` & `gwbench-0.7.1/gwbench/basic_relations.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/detector.py` & `gwbench-0.7.1/gwbench/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,33 +101,30 @@
             is_asd   = user_psds[self.det_key]['is_asd']
         else:
             psd_file = user_psds[self.tec]['psd_file']
             is_asd   = user_psds[self.tec]['is_asd']
         self.psd, self.f = psd.psd(self.tec,self.f,F_lo,F_hi,psd_file,is_asd)
 
     def setup_ant_pat_lpf(self, inj_params, use_rot, user_locs=None):
-        if use_rot:
-            Mc = inj_params['Mc']
-            tc = inj_params['tc']
-        else:
-            Mc = None
-            tc = None
-        self.Fp, self.Fc, self.Flp = ant_pat_np.antenna_pattern_and_loc_phase_fac(
-            self.f, Mc, tc, inj_params['ra'], inj_params['dec'], inj_params['psi'], inj_params['gmst0'], self.loc, use_rot, user_locs=user_locs)
+        self.Fp, self.Fc, self.Flp = ant_pat_np.antenna_pattern_and_loc_phase_fac(self.f, inj_params.get('Mc'), inj_params.get('tc'),
+            inj_params['ra'], inj_params['dec'], inj_params['psi'], inj_params['gmst0'], self.loc, use_rot, user_locs=user_locs)
 
 
     ###
     #-----Detector responses-----
     def calc_det_responses(self, wf, inj_params):
         hfp, hfc = wf.eval_np_func(self.f,utils.get_sub_dict(inj_params,wf.wf_symbs_string))
         self.hf = self.Flp * (hfp * self.Fp + hfc * self.Fc)
 
-    def calc_det_responses_derivs_num(self, inj_params, deriv_variables, wf, deriv_symbs_string, conv_cos, conv_log, use_rot, step, method, order, n, user_locs):
+    def calc_det_responses_derivs_num(self, inj_params, deriv_variables, wf, deriv_symbs_string, conv_cos, conv_log, use_rot,
+                                      step, method, order, n, user_locs, ana_deriv_symbs_list):
         self.calc_det_responses(wf,inj_params)
-        self.del_hf = drd.calc_det_responses_derivs_num(self.loc,wf,deriv_symbs_string,self.f,inj_params,use_rot,'hf',step,method,order,n,user_locs)
+        self.del_hf = drd.calc_det_responses_derivs_num(self.loc, wf, deriv_symbs_string, self.f, inj_params, use_rot=use_rot, label='hf',
+                                                        step=step, method=method, order=order, n=n, user_locs=user_locs,
+                                                        ana_deriv_symbs_list=ana_deriv_symbs_list)
         self.del_hf, c_quants = edh.get_conv_del_eval_dic(self.del_hf, inj_params, conv_cos, conv_log, deriv_symbs_string)
         inj_params, deriv_variables = edh.get_conv_inj_params_deriv_variables(c_quants, inj_params, deriv_variables)
 
     def load_det_responses_derivs_sym(self, wf_model_name, deriv_symbs_string, return_bin=0, user_lambdified_functions_path=None):
         self.del_hf_expr = drd.load_det_responses_derivs_sym(self.loc, wf_model_name, deriv_symbs_string, return_bin, user_lambdified_functions_path)
 
     def calc_det_responses_derivs_sym(self, wf, inj_params, deriv_variables, conv_cos, conv_log, deriv_symbs_string):
```

### Comparing `gwbench-0.7.0/gwbench/detector_response_derivatives.py` & `gwbench-0.7.1/gwbench/detector_response_derivatives.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 import gwbench.antenna_pattern_sp as ant_pat_sp
 import gwbench.wf_derivatives_num as wfd_num
 import gwbench.wf_derivatives_sym as wfd_sym
 import gwbench.utils as utils
 
 lambdified_functions_path = os.path.join(os.getcwd(),'lambdified_functions')
 
-def calc_det_responses_derivs_num(loc, wf, deriv_symbs_string, f_arr, params_dic, use_rot=1, label='hf', step=1e-9, method='central', order=2, n=1, user_locs=None):
+def calc_det_responses_derivs_num(loc, wf, deriv_symbs_string, f_arr, params_dic, use_rot=1, label='hf',
+                                  step=1e-9, method='central', order=2, n=1, user_locs=None, ana_deriv_symbs_list=None):
 
     wf_symbs_list = wf.wf_symbs_string.split(' ')
     deriv_symbs_list = deriv_symbs_string.split(' ')
 
     if 'f' in wf_symbs_list: wf_symbs_list.remove('f')
     if 'f' in deriv_symbs_list: deriv_symbs_list.remove('f')
 
@@ -40,15 +41,17 @@
 
         def pc_func(f_arr,*wf_params_list):
             wf_list = []
             for i,el in enumerate(wf_symbs_list):
                 wf_list.append(wf_params_list[wf_symbs_list.index(el)])
             return wf.eval_np_func(f_arr, wf_list)
 
-        return wfd_num.part_deriv_hf_func(pc_func, wf_symbs_list, deriv_symbs_list, f_arr, params_dic, pl_cr=1, compl=1, label=label, step=step, method=method, order=order, n=n)
+        return wfd_num.part_deriv_hf_func(pc_func, wf_symbs_list, deriv_symbs_list, f_arr, params_dic,
+                                          pl_cr=1, compl=1, label=label, ana_deriv_symbs_list=ana_deriv_symbs_list,
+                                          step=step, method=method, order=order, n=n)
 
     else:
         ap_symbs_list = ant_pat_np.ap_symbs_string.split(' ')
         if 'f' in ap_symbs_list: ap_symbs_list.remove('f')
 
         dr_symbs_list = utils.reduce_symbols_strings(wf.wf_symbs_string, ant_pat_np.ap_symbs_string).split(' ')
         dr_params_list = list(utils.get_sub_dict(params_dic,dr_symbs_list).values())
@@ -63,15 +66,17 @@
                 ap_list.append(dr_params_list[dr_symbs_list.index(el)])
 
             hfp, hfc = wf.eval_np_func(f_arr, wf_list)
             Fp, Fc, Flp = ant_pat_np.antenna_pattern_and_loc_phase_fac(f_arr, *ap_list, loc, use_rot, user_locs=user_locs)
 
             return Flp * (hfp * Fp + hfc * Fc)
 
-        return wfd_num.part_deriv_hf_func(dr_func, dr_symbs_list, deriv_symbs_list, f_arr, params_dic, pl_cr=0, compl=1, label=label, step=step, method=method, order=order, n=n)
+        return wfd_num.part_deriv_hf_func(dr_func, dr_symbs_list, deriv_symbs_list, f_arr, params_dic,
+                                          pl_cr=0, compl=1, label=label, ana_deriv_symbs_list=ana_deriv_symbs_list,
+                                          step=step, method=method, order=order, n=n)
 
 
 
 def generate_det_responses_derivs_sym(wf, deriv_symbs_string, locs=None, use_rot=1, user_lambdified_functions_path=None, user_locs=None):
 
     hfpc = wf.get_sp_expr()
```

### Comparing `gwbench-0.7.0/gwbench/err_deriv_handling.py` & `gwbench-0.7.1/gwbench/err_deriv_handling.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,95 +15,79 @@
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 
 
 import numpy as np
 from scipy.integrate import simps
 from scipy.optimize import toms748
 
-PI = np.pi
-
 #-----derivative and error manipulations-----
 def convert_to_cos_derivative(deriv, param_key, param_val):
-    c_deriv = (-1./np.sin(param_val)) * deriv
+    c_deriv     = (-1./np.sin(param_val)) * deriv
     c_param_key = 'cos_'+param_key
     c_param_val = np.cos(param_val)
     return c_deriv, c_param_key, c_param_val
 
 def convert_to_log_derivative(deriv, param_key, param_val):
-    c_deriv = param_val * deriv
+    c_deriv     = param_val * deriv
     c_param_key = 'log_'+param_key
     c_param_val = np.log(param_val)
     return c_deriv, c_param_key, c_param_val
 
 def dim_err_to_rel_err(err, param_val, param_key=None, param_kind=None):
-    if param_key in ('M','Mc','Dl','DL','tc') or param_kind == 'dim':
-        return np.abs(err/param_val)
-    else:
-        return err
+    if param_key in ('M','Mc','Dl','DL','tc') or param_kind == 'dim': return np.abs(err/param_val)
+    else:                                                             return err
 
 def one_sigma_to_percent_error(percent, sigma):
     sigma_orders = [0, 1, 2, 3, 4, 5, 6]
     sigma_percents = [0., 68.2689492137, 95.4499736104, 99.7300203937, 99.9936657516, 99.9999426697, 99.9999998027]
     for i,sigma_order in enumerate(sigma_orders):
         if percent < sigma_percents[i]: break
 
     def func(error,percent,sigma,sigma_order):
         x = np.linspace(0,error,sigma_order*100)
         return percent/100/2 - simps(np.exp(-x**2/2/sigma**2)/np.sqrt(2*np.pi)/sigma,x)
 
-    if sigma_order == 1:
-        return toms748(func,1e-2*sigma,sigma_order*sigma,args=(percent,sigma,sigma_order))
-    else:
-        return toms748(func,(sigma_order-1)*sigma,sigma_order*sigma,args=(percent,sigma,sigma_order))
+    if sigma_order == 1: return toms748(func,1e-2*sigma,sigma_order*sigma,args=(percent,sigma,sigma_order))
+    else:                return toms748(func,(sigma_order-1)*sigma,sigma_order*sigma,args=(percent,sigma,sigma_order))
 
 #-----Convert the evaluated derivatives according to conv_cos, conv_log-----
 def get_conv_inj_params_deriv_variables(c_quants, inj_params, deriv_variables):
-    if c_quants == {}:
-        return inj_params, deriv_variables
-
+    if c_quants == {}: return inj_params, deriv_variables
     else:
         for o_key in c_quants:
             c_key = c_quants[o_key][0]
             c_val = c_quants[o_key][1]
 
-            if c_key not in deriv_variables:
-                deriv_variables[deriv_variables.index(o_key)] = c_key
+            if c_key not in deriv_variables: deriv_variables[deriv_variables.index(o_key)] = c_key
             inj_params[c_key] = c_val
 
         return inj_params, deriv_variables
 
 def get_conv_del_eval_dic(del_eval_dic, params_dic, conv_cos, conv_log, deriv_symbs_string):
-    if conv_cos is None and conv_log is None:
-        return del_eval_dic, {}
+    if conv_cos is None and conv_log is None: return del_eval_dic, {}
     else:
         conv_dic = {}
         c_quants = {}
 
         for deriv in del_eval_dic:
             key = '_'.join(deriv.split('_')[1:-1])
             c_key = None
 
-            if conv_cos is not None and key in conv_cos:
-                c_deriv, c_key, c_val = convert_to_cos_derivative(del_eval_dic[deriv],key,params_dic[key])
-            elif conv_log is not None and key in conv_log:
-                c_deriv, c_key, c_val = convert_to_log_derivative(del_eval_dic[deriv],key,params_dic[key])
-            else:
-                conv_dic[deriv] = del_eval_dic[deriv]
+            if   conv_cos is not None and key in conv_cos: c_deriv, c_key, c_val = convert_to_cos_derivative(del_eval_dic[deriv],key,params_dic[key])
+            elif conv_log is not None and key in conv_log: c_deriv, c_key, c_val = convert_to_log_derivative(del_eval_dic[deriv],key,params_dic[key])
+            else:                                          conv_dic[deriv]       = del_eval_dic[deriv]
 
             if c_key is not None:
-                c_quants[key] = (c_key, c_val)
-
-                prefix,suffix = deriv.split(key)
-                n_key = prefix + c_key + suffix
+                c_quants[key]   = (c_key, c_val)
+                prefix,suffix   = deriv.split(key)
+                n_key           = prefix + c_key + suffix
                 conv_dic[n_key] = c_deriv
 
         return conv_dic, c_quants
 
 #-----sky area calculations-----
 def sky_area_90(ra_err, dec_err, cov_ra_dec, dec_val, is_cos_dec):
     # sources ... arXiv:1403.6915 (2.31), arXiv:gr-qc/0310125v3 (43)
     if is_cos_dec: trig_fac = np.abs( 1/np.tan(dec_val) )
     else:          trig_fac = np.abs(   np.cos(dec_val) )
-    if (ra_err*dec_err)**2 > cov_ra_dec**2:
-        return trig_fac * np.sqrt( (ra_err * dec_err)**2 - cov_ra_dec**2 ) * 2*PI * (180./PI)**2 * np.log(10)
-    else:
-        return None
+    if (ra_err*dec_err)**2 > cov_ra_dec**2: return trig_fac * np.sqrt( (ra_err * dec_err)**2 - cov_ra_dec**2 ) * 2*np.pi * (180./np.pi)**2 * np.log(10)
+    else:                                   return None
```

### Comparing `gwbench-0.7.0/gwbench/fisher_analysis_tools.py` & `gwbench-0.7.1/gwbench/fisher_analysis_tools.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/injections.py` & `gwbench-0.7.1/gwbench/injections.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         peak_frac  = mass_dict['peak_frac']     # peak_frac  = 0.1
         peak_mean  = mass_dict['peak_mean']     # peak_mu    = 33.07
         peak_sigma = mass_dict['peak_sigma']    # peak_sigma = 5.69
         delta_m    = mass_dict['delta_m']       # delta_m    = 4.82
         q_beta     = mass_dict['q_beta']        # q_beta     = 1.26
         m1_m2      = 1
 
-        m1_vec     = power_peak(mmin, mmax, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, nm1s=5001)
+        m1_vec     = power_peak(mmin, mmax, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, num_injs, nm1s=5001, rng=rngs[0])
 
         q_vec      = rngs[1].power(q_beta + 1, num_injs)
         m2_vec     = q_vec * m1_vec
         m2_mask    = m2_vec < mmin
 
         while m2_mask.sum():
             q_vec[m2_mask] = rngs[1].power(q_beta + 1, m2_mask.sum())
@@ -244,30 +244,30 @@
         m1_alpha   = mass_dict['m1_alpha']
         peak_frac  = mass_dict['peak_frac']
         peak_mean  = mass_dict['peak_mean']
         peak_sigma = mass_dict['peak_sigma']
         delta_m    = mass_dict['delta_m']
         m1_m2      = 1
 
-        m1_vec     = power_peak(mmin, mmax, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, nm1s=5001)
+        m1_vec     = power_peak(mmin, mmax, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, num_injs, nm1s=5001, rng=rngs[0])
         m2_vec     = rngs[1].uniform(mmin, m1_vec)
 
     elif mass_dict['dist'] == 'nsbh_power_peak_uniform':
         m1_min     = mass_dict['m1_min']
         m1_max     = mass_dict['m1_max']
         m1_alpha   = mass_dict['m1_alpha']
         peak_frac  = mass_dict['peak_frac']
         peak_mean  = mass_dict['peak_mean']
         peak_sigma = mass_dict['peak_sigma']
         delta_m    = mass_dict['delta_m']
         m2_min     = mass_dict['m2_min']
         m2_max     = mass_dict['m2_max']
         m1_m2      = 1
 
-        m1_vec     = power_peak(m1_min, m1_max, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, nm1s=5001)
+        m1_vec     = power_peak(m1_min, m1_max, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, num_injs, nm1s=5001, rng=rngs[0])
         m2_vec     = rngs[1].uniform(low=m2_min, high=m2_max, size=num_injs)
 
     elif mass_dict['dist'] == 'power_uniform':
         mmin  = mass_dict['mmin']
         mmax  = mass_dict['mmax']
         alpha = mass_dict['alpha'] + 1
         m1_m2 = 1
@@ -326,31 +326,32 @@
     ids    = np.nonzero(np.logical_and(m_arr >= mmin, m_arr < mmin + delta_m))[0]
     m_arr -= mmin
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         res[ids] = 1 / (1 + np.exp(delta_m/m_arr[ids] + delta_m/(m_arr[ids] - delta_m)))
     return res
 
-def power_peak(mmin, mmax, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, nm1s=5001):
+def power_peak(mmin, mmax, m1_alpha, peak_frac, peak_mean, peak_sigma, delta_m, num_injs, nm1s=5001, rng=None, seed=None):
+    if rng is None: rng = np.random.default_rng(seed)
     m1s            = np.linspace(mmin, mmax, nm1s)
     power_part     = (1 - peak_frac) * power(m1s, -m1_alpha) / simps(power(m1s, -m1_alpha), m1s)
     gauss_part     = peak_frac * gaussian(m1s, peak_mean, peak_sigma) / simps(gaussian(m1s, peak_mean, peak_sigma), m1s)
     m1_dist        = (power_part + gauss_part) * smoothing(m1s, mmin, delta_m)
     window_cdf     = np.array([simps(m1_dist[:i], m1s[:i]) for i in range(1, len(m1s)+1)]) / simps(m1_dist, m1s)
     inv_window_cdf = interp1d(window_cdf, m1s)
-    return inv_window_cdf(rngs[0].random(num_injs))
+    return inv_window_cdf(rng.random(num_injs))
 
 #-----general helpers-----
-def truncated_gaussian(mean, sigma, minv, maxv, num_injs, seed, rng=None):
-    if rng is None: rng = np.random.default_rng(seeed)
+def truncated_gaussian(mean, sigma, minv, maxv, num_injs, rng=None, seed=None):
+    if rng is None: rng = np.random.default_rng(seed)
     sample_vec = np.zeros(num_injs)
     ids        = np.arange(num_injs)
     while ids.size > 0:
         sample_vec[ids] = rng.normal(loc=mean, scale=sigma, size=ids.size)
-        ids             = np.nonzero(np.logical_not(np.logical_and(sample_vec > minv, sample_vecN < maxv)))[0]
+        ids             = np.nonzero(np.logical_not(np.logical_and(sample_vec > minv, sample_vec < maxv)))[0]
     return sample_vec
 
 
 ###
 #-----redshift and lum distance samplers-----
 def redshift_lum_distance_sampler(cosmo_dict,num_injs,seed):
     zmin = cosmo_dict['zmin']
```

### Comparing `gwbench-0.7.0/gwbench/network.py` & `gwbench-0.7.1/gwbench/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         # frequency array
         self.f = None
         # dictionary of injection parameters
         self.inj_params = None
         # derivative variables - symbs_string and list
         self.deriv_symbs_string = None
         self.deriv_variables = None
+        # derivative variables for which analytical derivatives should be used
+        self.ana_deriv_symbs_list = None
         # waveform
         self.wf = None
 
         #-----analysis settings-----
         # list of inj_params to convert to cos, ln versions
         self.conv_cos = None
         self.conv_log = None
@@ -153,25 +155,27 @@
         for det_key in self.det_keys:
             self.detectors.append(dc.Detector(det_key))
 
     def set_wf_vars(self, wf_model_name, wf_other_var_dic=None, user_waveform=None, cosmo=None):
         self.wf = wfc.Waveform(wf_model_name, wf_other_var_dic=wf_other_var_dic, user_waveform=user_waveform, cosmo=cosmo, logger=self.logger)
 
     def set_net_vars(self, f=None, inj_params=None, deriv_symbs_string=None, conv_cos=None, conv_log=None,
-                     use_rot=None, user_locs=None, user_psds=None, user_lambdified_functions_path=None):
+                     use_rot=None, user_locs=None, user_psds=None, user_lambdified_functions_path=None, ana_deriv_symbs_list=None):
         if f is not None:
             self.f = copy(f)
             if self.detectors is not None:
                 for det in self.detectors:
                     det.set_f(self.f)
         if inj_params is not None:
             self.inj_params = deepcopy(inj_params)
         if deriv_symbs_string is not None:
             self.deriv_symbs_string = copy(deriv_symbs_string)
             self.deriv_variables = deriv_symbs_string.split(' ')
+        if ana_deriv_symbs_list is not None:
+            self.ana_deriv_symbs_list = copy(ana_deriv_symbs_list)
         if conv_cos is not None:
             self.conv_cos = copy(conv_cos)
         if conv_log is not None:
             self.conv_log = copy(conv_log)
         if use_rot is not None:
             self.use_rot = copy(use_rot)
         if user_locs is not None:
@@ -258,16 +262,17 @@
         self.hfp, self.hfc = self.wf.eval_np_func(self.f,utils.get_sub_dict(self.inj_params,self.wf.wf_symbs_string))
         self.logger.info('Polarizations calculated.')
 
     def calc_wf_polarizations_derivs_num(self, step=1e-9, method='central', order=2, n=1):
         self.logger.info('Calculate numeric derivatives of polarizations.')
         self.calc_wf_polarizations()
         wf_deriv_symbs_string = utils.remove_symbols(self.deriv_symbs_string,self.wf.wf_symbs_string)
-        self.del_hfpc = drd.calc_det_responses_derivs_num(None, self.wf, wf_deriv_symbs_string, self.f, self.inj_params, self.use_rot, 'hf',
-                                                          step, method, order, n, self.user_locs)
+        self.del_hfpc = drd.calc_det_responses_derivs_num(None, self.wf, wf_deriv_symbs_string, self.f, self.inj_params, use_rot=self.use_rot, label='hf',
+                                               step=step, method=method, order=order, n=n, user_locs=self.user_locs,
+                                               ana_deriv_symbs_list=self.ana_deriv_symbs_list)
         self.del_hfpc, c_quants = edh.get_conv_del_eval_dic(self.del_hfpc, self.inj_params, self.conv_cos, self.conv_log, self.deriv_symbs_string)
         self.inj_params, self.deriv_variables = edh.get_conv_inj_params_deriv_variables(c_quants, self.inj_params, self.deriv_variables)
         self.logger.info('Numeric derivatives of polarizations calculated.')
 
     def load_wf_polarizations_derivs_sym(self, return_bin=0):
         wf_deriv_symbs_string = utils.remove_symbols(self.deriv_symbs_string,self.wf.wf_symbs_string)
         self.del_hfpc_expr = drd.load_det_responses_derivs_sym('pl_cr', self.wf.wf_model_name, wf_deriv_symbs_string, return_bin, self.user_lambdified_functions_path)
@@ -292,15 +297,15 @@
             det.calc_det_responses(self.wf,self.inj_params)
         self.logger.info('Detector responses calculated.')
 
     def calc_det_responses_derivs_num(self, step=1e-9, method='central', order=2, n=1):
         self.logger.info('Calculate numeric derivatives of detector responses.')
         for det in self.detectors:
             self.logger.info(f'   {det.det_key}')
-            det.calc_det_responses_derivs_num(self.inj_params, self.deriv_variables, self.wf, self.deriv_symbs_string, self.conv_cos, self.conv_log, self.use_rot, step, method, order, n, self.user_locs)
+            det.calc_det_responses_derivs_num(self.inj_params, self.deriv_variables, self.wf, self.deriv_symbs_string, self.conv_cos, self.conv_log, self.use_rot, step, method, order, n, self.user_locs, self.ana_deriv_symbs_list)
         self.logger.info('Numeric derivatives of detector responses calculated.')
 
     def load_det_responses_derivs_sym(self, return_bin=0):
         for det in self.detectors:
             det.load_det_responses_derivs_sym(self.wf.wf_model_name, self.deriv_symbs_string, return_bin, self.user_lambdified_functions_path)
         self.logger.info('Lambdified detector responses loaded.')
 
@@ -507,15 +512,15 @@
     tec_net.logger.info('PSDs for unique detector technologies calculated.')
     return tec_net
 
 
 def unique_locs_det_responses(network_specs, f, inj_params, deriv_symbs_string, wf_model_name,
                               wf_other_var_dic=None, conv_cos=None, conv_log=None, use_rot=1,
                               user_waveform=None, user_locs=None, user_lambdified_functions_path=None,
-                              cosmo=None, logger_level='WARNING', num_cores=None,
+                              ana_deriv_symbs_list=None, cosmo=None, logger_level='WARNING', num_cores=None,
                               step=None, method=None, order=None, n=None):
     # initialize empty network
     loc_net = Network(logger_name='unique_locs_det_responses', logger_level=logger_level)
     # get the detector keys
     loc_net.det_keys = []
 
     # find unique locations
@@ -549,27 +554,28 @@
     loc_net.logger.info('Evaluate lambdified detector responses for unique locations.')
     if num_cores is None:
         if step is None:
             for det in loc_net.detectors:
                 det.del_hf, c_quants = eval_loc_sym(det.loc,det.del_hf_expr,deriv_symbs_string,f,inj_params,conv_cos,conv_log,logger=loc_net.logger)
         else:
             for det in loc_net.detectors:
-                det.del_hf, c_quants = eval_loc_num(det.loc,loc_net.wf,deriv_symbs_string,f,inj_params,conv_cos,conv_log,use_rot,step,method,order,n,user_locs,logger=loc_net.logger)
-
+                det.del_hf, c_quants = eval_loc_num(det.loc,loc_net.wf,deriv_symbs_string,f,inj_params,conv_cos,conv_log,use_rot,
+                                                    step,method,order,n,user_locs,ana_deriv_symbs_list,logger=loc_net.logger)
         loc_net.inj_params, loc_net.deriv_variables = edh.get_conv_inj_params_deriv_variables(c_quants, loc_net.inj_params, loc_net.deriv_variables)
 
     else:
         from multiprocessing import Pool
         pool = Pool(num_cores)
         if step is None:
             arg_tuple_list = [(det.loc,det.del_hf_expr,deriv_symbs_string,f,inj_params,conv_cos,conv_log,loc_net.logger) for det in loc_net.detectors]
             result = pool.starmap_async(eval_loc_sym, arg_tuple_list)
             result.wait()
         else:
-            arg_tuple_list = [(det.loc,loc_net.wf,deriv_symbs_string,f,inj_params,conv_cos,conv_log,use_rot,step,method,order,n,user_locs,loc_net.logger) for det in loc_net.detectors]
+            arg_tuple_list = [(det.loc,loc_net.wf,deriv_symbs_string,f,inj_params,conv_cos,conv_log,use_rot,
+                               step,method,order,n,user_locs,ana_deriv_symbs_list,loc_net.logger) for det in loc_net.detectors]
             result = pool.starmap_async(eval_loc_num, arg_tuple_list)
             result.wait()
 
         for det, (del_hf,c_quants) in zip(loc_net.detectors, result.get()):
             det.del_hf = del_hf
 
         loc_net.inj_params, loc_net.deriv_variables = edh.get_conv_inj_params_deriv_variables(c_quants, loc_net.inj_params, loc_net.deriv_variables)
@@ -587,12 +593,15 @@
     del_hf = {}
     del_hf_expr = dill.loads(del_hf_expr)
     for deriv in del_hf_expr:
         if deriv in ('variables','deriv_variables'): continue
         del_hf[deriv] = del_hf_expr[deriv](f,**utils.get_sub_dict(inj_params,del_hf_expr['variables']))
     return edh.get_conv_del_eval_dic(del_hf,inj_params,conv_cos,conv_log, deriv_symbs_string)
 
-def eval_loc_num(loc, wf, deriv_symbs_string, f, inj_params, conv_cos, conv_log, use_rot, step, method, order, n, user_locs, logger=None):
+def eval_loc_num(loc, wf, deriv_symbs_string, f, inj_params, conv_cos, conv_log, use_rot,
+                 step, method, order, n, user_locs, ana_deriv_symbs_list, logger=None):
     if logger is None: glob_logger.info(f'   {loc}')
     else:              logger.info(f'   {loc}')
-    del_hf = drd.calc_det_responses_derivs_num(loc,wf,deriv_symbs_string,f,inj_params,use_rot,'hf',step,method,order,n,user_locs)
+    del_hf = drd.calc_det_responses_derivs_num(loc, wf, deriv_symbs_string, f, inj_params, use_rot=use_rot, label='hf',
+                                               step=step, method=method, order=order, n=n, user_locs=user_locs,
+                                               ana_deriv_symbs_list=ana_deriv_symbs_list)
     return edh.get_conv_del_eval_dic(del_hf,inj_params,conv_cos,conv_log, deriv_symbs_string)
```

### Comparing `gwbench-0.7.0/gwbench/psd.py` & `gwbench-0.7.1/gwbench/psd.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/snr.py` & `gwbench-0.7.1/gwbench/snr.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/utils.py` & `gwbench-0.7.1/gwbench/utils.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/waveform.py` & `gwbench-0.7.1/gwbench/waveform.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_derivatives_num.py` & `gwbench-0.7.1/gwbench/wf_derivatives_num.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,68 +17,49 @@
 
 '''This module contains two methods that calculate numerical derivatives.
 '''
 
 import numdifftools as nd
 
 import gwbench.utils as utils
+from gwbench.wf_derivatives_ana import ana_derivs
 
-def part_deriv_hf_func(hf, symbols_list, deriv_symbs_list, f, params_dic, pl_cr=0, compl=1, label='hf', step=1e-9, method='central', order=2, n=1):
+def part_deriv_hf_func(hf, symbols_list, deriv_symbs_list, f, params_dic,
+                       pl_cr=0, compl=1, label='hf', ana_deriv_symbs_list=None,
+                       step=1e-9, method='central', order=2, n=1):
+
+    if 'f' in symbols_list: symbols_list.remove('f')
+    if ana_deriv_symbs_list is None: ana_deriv_symbs_list = []
+    params_list       = [ params_dic[param] for param in symbols_list ]
+    _deriv_symbs_list = [ el for el in deriv_symbs_list if el not in ana_deriv_symbs_list ]
+    deriv_params_list = [ params_dic[param] for param in _deriv_symbs_list ]
+
+    if pl_cr: del_hf_dic_ana = { f'del_{name}_{label + pc}' : ana_derivs(name, _hf,                 f, params_dic)
+                                 for name in ana_deriv_symbs_list for pc,_hf in zip(('p', 'c'), hf(f, *params_list)) }
+    else:     del_hf_dic_ana = { f'del_{name}_{label}'      : ana_derivs(name, hf(f, *params_list), f, params_dic)
+                                 for name in ana_deriv_symbs_list }
 
-    if 'f' in symbols_list:
-        symbols_list.remove('f')
-
-    params_list = []
-    for param in symbols_list:
-        params_list.append(params_dic[param])
-
-    deriv_params_list = []
-    for param in deriv_symbs_list:
-        deriv_params_list.append(params_dic[param])
+    if not _deriv_symbs_list: return del_hf_dic_ana
 
     def hf_of_deriv_params(f, *deriv_params_list):
-        tmp_list = []
-        for i,el in enumerate(symbols_list):
-            if el in deriv_symbs_list:
-                tmp_list.append(deriv_params_list[deriv_symbs_list.index(el)])
-            else:
-                tmp_list.append(params_list[i])
-
-        return hf(f,*tmp_list)
+        return hf(f, *[deriv_params_list[_deriv_symbs_list.index(el)] if el in _deriv_symbs_list else params_list[i] for i,el in enumerate(symbols_list)])
 
     del_hf = part_deriv(hf_of_deriv_params, f, deriv_params_list, pl_cr, compl, step, method, order, n)
-    if pl_cr:
-        del_hf_dic = {}
-
-        if len(deriv_symbs_list) == 1:
-            key_string = 'del_'+deriv_symbs_list[0]+'_'+label+'p'
-            del_hf_dic[key_string] = del_hf[0]
-
-            key_string = 'del_'+deriv_symbs_list[0]+'_'+label+'c'
-            del_hf_dic[key_string] = del_hf[1]
-
-        else:
-            for i,name in enumerate(deriv_symbs_list):
-                key_string = 'del_'+name+'_'+label+'p'
-                del_hf_dic[key_string] = del_hf[0][:,i]
-
-                key_string = 'del_'+name+'_'+label+'c'
-                del_hf_dic[key_string] = del_hf[1][:,i]
 
+    if pl_cr:
+        if len(_deriv_symbs_list) == 1: del_hf = (del_hf[0][:,None], del_hf[1][:,None])
+        del_hf_dic = { f'del_{name}_{label + pc}' : _del_hf[:,i] for i,name in enumerate(_deriv_symbs_list) for pc, _del_hf in zip(('p', 'c'), del_hf) }
     else:
-        del_hf_dic = {}
+        if len(_deriv_symbs_list) == 1: del_hf = del_hf[:,None]
+        del_hf_dic = { f'del_{name}_{label}'      :  del_hf[:,i] for i,name in enumerate(_deriv_symbs_list) }
 
-        if len(deriv_symbs_list) == 1:
-            key_string = 'del_'+deriv_symbs_list[0]+'_'+label
-            del_hf_dic[key_string] = del_hf
-
-        else:
-            for i,name in enumerate(deriv_symbs_list):
-                key_string = 'del_'+name+'_'+label
-                del_hf_dic[key_string] = del_hf[:,i]
+    if ana_deriv_symbs_list:
+        del_hf_dic  = { **del_hf_dic, **del_hf_dic_ana }
+        sorted_keys = [ key for name in deriv_symbs_list for key in del_hf_dic if name == key[4:].split(f'_{label}')[0] ]
+        del_hf_dic  = { key : del_hf_dic[key] for key in sorted_keys}
 
     return del_hf_dic
 
 
 def part_deriv(func, f, params_list, pl_cr=0, compl=None, step=1e-9, method='central', order=2, n=1):
     if pl_cr:
         if compl:
```

### Comparing `gwbench-0.7.0/gwbench/wf_derivatives_sym.py` & `gwbench-0.7.1/gwbench/wf_derivatives_sym.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/__init__.py` & `gwbench-0.7.1/gwbench/noise_curves/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/a_plus.txt` & `gwbench-0.7.1/gwbench/noise_curves/a_plus.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/a_sharp.txt` & `gwbench-0.7.1/gwbench/noise_curves/a_sharp.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/advirgo_plus.txt` & `gwbench-0.7.1/gwbench/noise_curves/advirgo_plus.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_10km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_10km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_10km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_10km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_20km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_20km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_20km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_20km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_30km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_30km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_30km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_30km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_40km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_40km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce1_40km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce1_40km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_10km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_10km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_10km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_10km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_20km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_20km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_20km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_20km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_30km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_30km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_30km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_30km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_40km_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_40km_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/ce2_40km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/ce2_40km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_20km.txt` & `gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_20km.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_20km_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_20km_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_40km.txt` & `gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_40km.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/cosmic_explorer_40km_lf.txt` & `gwbench-0.7.1/gwbench/noise_curves/cosmic_explorer_40km_lf.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/et.txt` & `gwbench-0.7.1/gwbench/noise_curves/et.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/et_10km_xylophone.txt` & `gwbench-0.7.1/gwbench/noise_curves/et_10km_xylophone.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/kagra_plus.txt` & `gwbench-0.7.1/gwbench/noise_curves/kagra_plus.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/voyager_cb.txt` & `gwbench-0.7.1/gwbench/noise_curves/voyager_cb.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/noise_curves/voyager_pm.txt` & `gwbench-0.7.1/gwbench/noise_curves/voyager_pm.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/__init__.py` & `gwbench-0.7.1/gwbench/wf_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/lal_bbh_np.py` & `gwbench-0.7.1/gwbench/wf_models/lal_bbh_np.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/lal_bns_np.py` & `gwbench-0.7.1/gwbench/wf_models/lal_bns_np.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/tf2_np.py` & `gwbench-0.7.1/gwbench/wf_models/tf2_np.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/tf2_sp.py` & `gwbench-0.7.1/gwbench/wf_models/tf2_sp.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/tf2_tidal_np.py` & `gwbench-0.7.1/gwbench/wf_models/tf2_tidal_np.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/gwbench/wf_models/tf2_tidal_sp.py` & `gwbench-0.7.1/gwbench/wf_models/tf2_tidal_sp.py`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt` & `gwbench-0.7.1/xtra_files/merger_rates/bns_n_dot_bns_md_merger_rate.txt`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/LICENSE` & `gwbench-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwbench-0.7.0/README.md` & `gwbench-0.7.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-# **BEWARE - Please Update to Version 0.7.0 or higher**
-#### The sky area calculation was fixed in Version 0.65 and the matrix inversion was improved in 0.7.0 (refer to respective CHANGELOG.md entries)
-
 # gwbench
-
 ## Acknowledgment
-
 We request that any academic report, publication, or other academic
 disclosure of results derived from the use of this software acknowledge
 the use of the software by an appropriate acknowledgment or citation.
 
 The gwbench software can be cited from [arXiv:2010.15202](https://arxiv.org/abs/2010.15202), with INSPIRE BibTeX entry:
 ```
 @article{Borhanian:2020ypi,
@@ -18,25 +13,28 @@
     archivePrefix = "arXiv",
     primaryClass = "gr-qc",
     month = "10",
     year = "2020"
 }
 ```
 
-## Installation from source
+## Installation via pip
+```
+pip install gwbench
+```
 
-### Clone the `gwbench` repository and enter it
+## Installation from source
+### Clone the gwbench repository and enter it
 Clone this repository and follow the next steps.
 ```
 git clone https://gitlab.com/sborhanian/gwbench.git
 cd gwbench
 ```
 
-### Using `conda`
-
+### Using conda
 #### Source Oasis Conda - *do this first; only on LIGO clusters needed*
 ```
 source /cvmfs/oasis.opensciencegrid.org/ligo/sw/conda/etc/profile.d/conda.sh  
 which conda
 ```
 
 The last line should print `/cvmfs/oasis.opensciencegrid.org/ligo/sw/conda/condabin/conda` or similar.
@@ -44,23 +42,23 @@
 #### Setup conda virtual environment
 ```
 conda create -y --name gwbench python=3.7  
 conda activate gwbench  
 conda install -y -c conda-forge --file requirements_conda.txt  
 ```
 
-### Using `python -m venv` and `pip`
+### Using `python -m venv` and pip
 Replace `~/gwbench` with the appropriate path of choice in the following instructions:
 ```
 python3 -m venv ~/gwbench
 source ~/gwbench/bin/activate
 pip install -r requirements_pip.txt
 ```
 
-### Using `pip` or `conda`
+### Using pip or conda
 Install while the virtual environment is active:
 ```
 pip install .
 ```
 
 ### Uninstall
 ```
```

### Comparing `gwbench-0.7.0/pyproject.toml` & `gwbench-0.7.1/xtra_files/pypi/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gwbench"
-version = "0.7.0"
+version = "0.7.1"
 authors = [
   { name="Ssohrab Borhanian", email="sborhanian@gmail.com" },
 ]
 dependencies = [
     "astropy",
     "dill",
     "lalsuite",
@@ -21,15 +21,14 @@
     "tqdm",
 ]
 description = "A Python package for gravitational-wave benchmarking, particularly with Fisher information matrices."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://gitlab.com/sborhanian/gwbench"
 "Bug Tracker" = "https://gitlab.com/sborhanian/gwbench/-/issues"
-
```

### Comparing `gwbench-0.7.0/PKG-INFO` & `gwbench-0.7.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gwbench
-Version: 0.7.0
+Version: 0.7.1
 Summary: A Python package for gravitational-wave benchmarking, particularly with Fisher information matrices.
 Project-URL: Homepage, https://gitlab.com/sborhanian/gwbench
 Project-URL: Bug Tracker, https://gitlab.com/sborhanian/gwbench/-/issues
 Author-email: Ssohrab Borhanian <sborhanian@gmail.com>
 License-File: AUTHORS.md
 License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: astropy
 Requires-Dist: dill
 Requires-Dist: lalsuite
 Requires-Dist: mpmath
@@ -19,21 +19,16 @@
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: sympy
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-# **BEWARE - Please Update to Version 0.7.0 or higher**
-#### The sky area calculation was fixed in Version 0.65 and the matrix inversion was improved in 0.7.0 (refer to respective CHANGELOG.md entries)
-
 # gwbench
-
 ## Acknowledgment
-
 We request that any academic report, publication, or other academic
 disclosure of results derived from the use of this software acknowledge
 the use of the software by an appropriate acknowledgment or citation.
 
 The gwbench software can be cited from [arXiv:2010.15202](https://arxiv.org/abs/2010.15202), with INSPIRE BibTeX entry:
 ```
 @article{Borhanian:2020ypi,
@@ -43,25 +38,28 @@
     archivePrefix = "arXiv",
     primaryClass = "gr-qc",
     month = "10",
     year = "2020"
 }
 ```
 
-## Installation from source
+## Installation via pip
+```
+pip install gwbench
+```
 
-### Clone the `gwbench` repository and enter it
+## Installation from source
+### Clone the gwbench repository and enter it
 Clone this repository and follow the next steps.
 ```
 git clone https://gitlab.com/sborhanian/gwbench.git
 cd gwbench
 ```
 
-### Using `conda`
-
+### Using conda
 #### Source Oasis Conda - *do this first; only on LIGO clusters needed*
 ```
 source /cvmfs/oasis.opensciencegrid.org/ligo/sw/conda/etc/profile.d/conda.sh  
 which conda
 ```
 
 The last line should print `/cvmfs/oasis.opensciencegrid.org/ligo/sw/conda/condabin/conda` or similar.
@@ -69,23 +67,23 @@
 #### Setup conda virtual environment
 ```
 conda create -y --name gwbench python=3.7  
 conda activate gwbench  
 conda install -y -c conda-forge --file requirements_conda.txt  
 ```
 
-### Using `python -m venv` and `pip`
+### Using `python -m venv` and pip
 Replace `~/gwbench` with the appropriate path of choice in the following instructions:
 ```
 python3 -m venv ~/gwbench
 source ~/gwbench/bin/activate
 pip install -r requirements_pip.txt
 ```
 
-### Using `pip` or `conda`
+### Using pip or conda
 Install while the virtual environment is active:
 ```
 pip install .
 ```
 
 ### Uninstall
 ```
```

