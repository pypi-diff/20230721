# Comparing `tmp/hypyp-0.4.0b8.tar.gz` & `tmp/hypyp-0.4.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypyp-0.4.0b8.tar", max compression
+gzip compressed data, was "hypyp-0.4.0b9.tar", max compression
```

## Comparing `hypyp-0.4.0b8.tar` & `hypyp-0.4.0b9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1524 2022-08-09 15:02:55.308284 hypyp-0.4.0b8/LICENSE
--rw-r--r--   0        0        0     3447 2022-08-09 15:02:55.308477 hypyp-0.4.0b8/README.md
--rw-r--r--   0        0        0      192 2022-08-09 15:02:55.518369 hypyp-0.4.0b8/hypyp/__init__.py
--rw-r--r--   0        0        0    35021 2023-01-31 23:04:31.734631 hypyp-0.4.0b8/hypyp/analyses.py
--rw-r--r--   0        0        0    13770 2022-08-09 15:02:55.518992 hypyp-0.4.0b8/hypyp/data/Basehead.obj
--rw-r--r--   0        0        0        1 2022-08-09 15:02:55.519393 hypyp-0.4.0b8/hypyp/ext/mpl3d/__init__.py
--rw-r--r--   0        0        0     4511 2022-08-09 15:02:55.519549 hypyp-0.4.0b8/hypyp/ext/mpl3d/camera.py
--rw-r--r--   0        0        0     7705 2022-08-09 15:02:55.519698 hypyp-0.4.0b8/hypyp/ext/mpl3d/glm.py
--rw-r--r--   0        0        0     3147 2022-08-09 15:02:55.519836 hypyp-0.4.0b8/hypyp/ext/mpl3d/lighting.py
--rw-r--r--   0        0        0     2990 2022-08-09 15:02:55.520074 hypyp-0.4.0b8/hypyp/ext/mpl3d/mesh.py
--rw-r--r--   0        0        0     9205 2022-08-09 15:02:55.520233 hypyp-0.4.0b8/hypyp/ext/mpl3d/trackball.py
--rw-r--r--   0        0        0     9887 2022-08-09 15:02:55.520401 hypyp-0.4.0b8/hypyp/fnirs_tools.py
--rw-r--r--   0        0        0        1 2022-08-09 15:02:55.520518 hypyp-0.4.0b8/hypyp/io.py
--rw-r--r--   0        0        0     9148 2022-08-09 15:02:55.520754 hypyp-0.4.0b8/hypyp/mvarica.py
--rw-r--r--   0        0        0    12588 2022-11-03 23:06:48.680785 hypyp-0.4.0b8/hypyp/prep.py
--rw-r--r--   0        0        0    21434 2022-11-03 23:16:20.313772 hypyp-0.4.0b8/hypyp/stats.py
--rw-r--r--   0        0        0    15193 2022-08-09 15:02:55.521405 hypyp-0.4.0b8/hypyp/utils.py
--rw-r--r--   0        0        0    69985 2023-01-31 23:04:31.735417 hypyp-0.4.0b8/hypyp/viz.py
--rw-r--r--   0        0        0     1735 2023-01-31 23:18:17.569658 hypyp-0.4.0b8/pyproject.toml
--rw-r--r--   0        0        0     4513 1970-01-01 00:00:00.000000 hypyp-0.4.0b8/setup.py
--rw-r--r--   0        0        0     4849 1970-01-01 00:00:00.000000 hypyp-0.4.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1524 2023-05-12 13:18:38.310986 hypyp-0.4.0b9/LICENSE
+-rw-r--r--   0        0        0     3524 2023-05-12 13:18:38.311148 hypyp-0.4.0b9/README.md
+-rw-r--r--   0        0        0      192 2023-05-12 13:18:38.586933 hypyp-0.4.0b9/hypyp/__init__.py
+-rw-r--r--   0        0        0    35571 2023-07-20 21:40:02.899871 hypyp-0.4.0b9/hypyp/analyses.py
+-rw-r--r--   0        0        0    13770 2023-05-12 13:18:38.588050 hypyp-0.4.0b9/hypyp/data/Basehead.obj
+-rw-r--r--   0        0        0        1 2023-05-12 13:18:38.588445 hypyp-0.4.0b9/hypyp/ext/mpl3d/__init__.py
+-rw-r--r--   0        0        0     4511 2023-05-12 13:18:38.588628 hypyp-0.4.0b9/hypyp/ext/mpl3d/camera.py
+-rw-r--r--   0        0        0     7705 2023-05-12 13:18:38.589183 hypyp-0.4.0b9/hypyp/ext/mpl3d/glm.py
+-rw-r--r--   0        0        0     3147 2023-05-12 13:18:38.589330 hypyp-0.4.0b9/hypyp/ext/mpl3d/lighting.py
+-rw-r--r--   0        0        0     2990 2023-05-12 13:18:38.589460 hypyp-0.4.0b9/hypyp/ext/mpl3d/mesh.py
+-rw-r--r--   0        0        0     9205 2023-05-12 13:18:38.589643 hypyp-0.4.0b9/hypyp/ext/mpl3d/trackball.py
+-rw-r--r--   0        0        0     9887 2023-05-12 13:18:38.589827 hypyp-0.4.0b9/hypyp/fnirs_tools.py
+-rw-r--r--   0        0        0        1 2023-05-12 13:18:38.589947 hypyp-0.4.0b9/hypyp/io.py
+-rw-r--r--   0        0        0     9148 2023-05-12 13:18:38.590193 hypyp-0.4.0b9/hypyp/mvarica.py
+-rw-r--r--   0        0        0    12650 2023-05-12 13:18:38.590381 hypyp-0.4.0b9/hypyp/prep.py
+-rw-r--r--   0        0        0    21562 2023-05-12 13:18:38.590649 hypyp-0.4.0b9/hypyp/stats.py
+-rw-r--r--   0        0        0    15121 2023-05-12 13:18:38.590859 hypyp-0.4.0b9/hypyp/utils.py
+-rw-r--r--   0        0        0    69698 2023-05-12 13:18:38.591292 hypyp-0.4.0b9/hypyp/viz.py
+-rw-r--r--   0        0        0     1779 2023-07-20 21:37:02.661190 hypyp-0.4.0b9/pyproject.toml
+-rw-r--r--   0        0        0     4926 1970-01-01 00:00:00.000000 hypyp-0.4.0b9/PKG-INFO
```

### Comparing `hypyp-0.4.0b8/LICENSE` & `hypyp-0.4.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/README.md` & `hypyp-0.4.0b9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # HyPyP 🐍〰️🐍
 
 The **Hy**perscanning **Py**thon **P**ipeline
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/hypyp.svg)](https://pypi.org/project/HyPyP/) <a href="https://travis-ci.org/ppsp-team/HyPyP"><img src="https://travis-ci.org/ppsp-team/HyPyP.svg?branch=master"></a> [![license](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Mattermost](https://img.shields.io/static/v1?label=chat&message=Mattermost&color=Blue)](https://mattermost.brainhack.org/brainhack/channels/hypyp)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/hypyp.svg)](https://pypi.org/project/HyPyP/) <a href="https://travis-ci.org/ppsp-team/HyPyP"><img src="https://travis-ci.org/ppsp-team/HyPyP.svg?branch=master"></a> <a href="https://hypyp.readthedocs.io"><img src="https://readthedocs.org/projects/hypyp/badge/?version=latest"></a> [![license](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Mattermost](https://img.shields.io/discord/1065810348944408616?color=blue)](https://discord.gg/zYzjeGj7D6)
 
 ⚠️ This software is in beta and thus should be considered with caution. While we have done our best to test all the functionalities, there is no guarantee that the pipeline is entirely bug-free. 
 
 📖 See our [paper](https://academic.oup.com/scan/advance-article/doi/10.1093/scan/nsaa141/5919711) for more explanation and our plan for upcoming functionalities (aka Roadmap).
 
 🤝 If you want to help you can submit bugs and suggestions of enhancements in our Github [Issues section](https://github.com/ppsp-team/HyPyP/issues).
 
@@ -54,8 +54,8 @@
 
 Step 4: ```poetry install```
 
 Step 5: ```poetry shell```
 
 You can now use ```jupyter notebook``` or ```ipython```!
 
-⚠️ If you need to install a new dependency (not recommended), you have to use `poetry add THE_NAME_OF_THE_LIBRARY` instead of your usual package manager.
+⚠️ If you need to install a new dependency (not recommended), you have to use `poetry add THE_NAME_OF_THE_LIBRARY` instead of your usual package manager.
```

#### html2text {}

```diff
@@ -1,44 +1,45 @@
 # HyPyP ðã°ï¸ð The **Hy**perscanning **Py**thon **P**ipeline [![PyPI
 version shields.io](https://img.shields.io/pypi/v/hypyp.svg)](https://pypi.org/
-project/HyPyP/) [https://travis-ci.org/ppsp-team/HyPyP.svg?branch=master] [!
-[license](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)]
-(https://opensource.org/licenses/BSD-3-Clause) [![Mattermost](https://
-img.shields.io/static/v1?label=chat&message=Mattermost&color=Blue)](https://
-mattermost.brainhack.org/brainhack/channels/hypyp) â ï¸ This software is in
-beta and thus should be considered with caution. While we have done our best to
-test all the functionalities, there is no guarantee that the pipeline is
-entirely bug-free. ð See our [paper](https://academic.oup.com/scan/advance-
-article/doi/10.1093/scan/nsaa141/5919711) for more explanation and our plan for
-upcoming functionalities (aka Roadmap). ð¤ If you want to help you can submit
-bugs and suggestions of enhancements in our Github [Issues section](https://
-github.com/ppsp-team/HyPyP/issues). ð¤ For the motivated contributors, you
-can even help directly in the developpment of HyPyP. You will need to install
-[Poetry](https://python-poetry.org/) (see section below). ## Contributors
-Original authors: Florence BRUN, AnaÃ«l AYROLLES, Phoebe CHEN, Amir DJALOVSKI,
-Yann BEAUXIS, Suzanne DIKKER, Guillaume DUMAS New contributors: Ghazaleh
-RANJBARAN, Quentin MOREAU, Caitriona DOUGLAS, Franck PORTEOUS, Jonas MAGO, Juan
-C. AVENDANO ## Installation ``` pip install HyPyP ``` ## Documentation HyPyP
-documentation of all the API functions is available online at
-[hypyp.readthedocs.io](https://hypyp.readthedocs.io/) For getting started with
-HyPyP, we have designed a little walkthrough: [getting_started.ipynb](https://
-github.com/ppsp-team/HyPyP/blob/master/tutorial/getting_started.ipynb) ## Core
-API ð  [io.py](https://github.com/ppsp-team/HyPyP/blob/master/hypyp/io.py)
-â Loaders (Florence, AnaÃ«l, Ghazaleh, Franck, Jonas, Guillaume) ð§°
-[utils.py](https://github.com/ppsp-team/HyPyP/blob/master/hypyp/utils.py) â
-Basic tools (Amir, Florence, Guilaume) âï¸ [prep.py](https://github.com/
-ppsp-team/HyPyP/blob/master/hypyp/prep.py) â Preprocessing (ICA & AutoReject)
-(AnaÃ«l, Florence, Guillaume) ð  [analyses.py](https://github.com/ppsp-team/
-HyPyP/blob/master/hypyp/analyses.py) â Power spectral density and wide choice
-of connectivity measures (Phoebe, Suzanne, Florence, Ghazaleh, Juan, Guillaume)
-ð [stats.py](https://github.com/ppsp-team/HyPyP/blob/master/hypyp/stats.py)
-â Statistics (permutations & cluster statistics) (Florence, Guillaume) ð§ 
-[viz.py](https://github.com/ppsp-team/HyPyP/blob/master/hypyp/viz.py) â
-Inter-brain visualization (AnaÃ«l, Amir, Florence, Guillaume) ð [Tutorials]
-(https://github.com/ppsp-team/HyPyP/tree/master/tutorial) - Examples &
-documentation (AnaÃ«l, Florence, Yann, Ghazaleh, Caitriona, Guillaume) ##
-Poetry installation (only for developpers and adventurous users) Step 1: ```pip
-install poetry``` Step 2: ```git clone git@github.com:ppsp-team/HyPyP.git```
-Step 3: ```cd HyPyP``` Step 4: ```poetry install``` Step 5: ```poetry shell```
-You can now use ```jupyter notebook``` or ```ipython```! â ï¸ If you need to
-install a new dependency (not recommended), you have to use `poetry add
+project/HyPyP/) [https://travis-ci.org/ppsp-team/HyPyP.svg?branch=master]
+[https://readthedocs.org/projects/hypyp/badge/?version=latest] [![license]
+(https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://
+opensource.org/licenses/BSD-3-Clause) [![Mattermost](https://img.shields.io/
+discord/1065810348944408616?color=blue)](https://discord.gg/zYzjeGj7D6) â ï¸
+This software is in beta and thus should be considered with caution. While we
+have done our best to test all the functionalities, there is no guarantee that
+the pipeline is entirely bug-free. ð See our [paper](https://
+academic.oup.com/scan/advance-article/doi/10.1093/scan/nsaa141/5919711) for
+more explanation and our plan for upcoming functionalities (aka Roadmap). ð¤
+If you want to help you can submit bugs and suggestions of enhancements in our
+Github [Issues section](https://github.com/ppsp-team/HyPyP/issues). ð¤ For
+the motivated contributors, you can even help directly in the developpment of
+HyPyP. You will need to install [Poetry](https://python-poetry.org/) (see
+section below). ## Contributors Original authors: Florence BRUN, AnaÃ«l
+AYROLLES, Phoebe CHEN, Amir DJALOVSKI, Yann BEAUXIS, Suzanne DIKKER, Guillaume
+DUMAS New contributors: Ghazaleh RANJBARAN, Quentin MOREAU, Caitriona DOUGLAS,
+Franck PORTEOUS, Jonas MAGO, Juan C. AVENDANO ## Installation ``` pip install
+HyPyP ``` ## Documentation HyPyP documentation of all the API functions is
+available online at [hypyp.readthedocs.io](https://hypyp.readthedocs.io/) For
+getting started with HyPyP, we have designed a little walkthrough:
+[getting_started.ipynb](https://github.com/ppsp-team/HyPyP/blob/master/
+tutorial/getting_started.ipynb) ## Core API ð  [io.py](https://github.com/
+ppsp-team/HyPyP/blob/master/hypyp/io.py) â Loaders (Florence, AnaÃ«l,
+Ghazaleh, Franck, Jonas, Guillaume) ð§° [utils.py](https://github.com/ppsp-
+team/HyPyP/blob/master/hypyp/utils.py) â Basic tools (Amir, Florence,
+Guilaume) âï¸ [prep.py](https://github.com/ppsp-team/HyPyP/blob/master/
+hypyp/prep.py) â Preprocessing (ICA & AutoReject) (AnaÃ«l, Florence,
+Guillaume) ð  [analyses.py](https://github.com/ppsp-team/HyPyP/blob/master/
+hypyp/analyses.py) â Power spectral density and wide choice of connectivity
+measures (Phoebe, Suzanne, Florence, Ghazaleh, Juan, Guillaume) ð [stats.py]
+(https://github.com/ppsp-team/HyPyP/blob/master/hypyp/stats.py) â Statistics
+(permutations & cluster statistics) (Florence, Guillaume) ð§  [viz.py](https:/
+/github.com/ppsp-team/HyPyP/blob/master/hypyp/viz.py) â Inter-brain
+visualization (AnaÃ«l, Amir, Florence, Guillaume) ð [Tutorials](https://
+github.com/ppsp-team/HyPyP/tree/master/tutorial) - Examples & documentation
+(AnaÃ«l, Florence, Yann, Ghazaleh, Caitriona, Guillaume) ## Poetry installation
+(only for developpers and adventurous users) Step 1: ```pip install poetry```
+Step 2: ```git clone git@github.com:ppsp-team/HyPyP.git``` Step 3: ```cd
+HyPyP``` Step 4: ```poetry install``` Step 5: ```poetry shell``` You can now
+use ```jupyter notebook``` or ```ipython```! â ï¸ If you need to install a
+new dependency (not recommended), you have to use `poetry add
 THE_NAME_OF_THE_LIBRARY` instead of your usual package manager.
```

### Comparing `hypyp-0.4.0b8/hypyp/analyses.py` & `hypyp-0.4.0b9/hypyp/analyses.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,27 +63,27 @@
             Option to collapse the time course or not, boolean.
             If False, PSD won't be averaged over epochs (the time
             course is maintained).
             If True, PSD values are averaged over epochs.
 
     Note:
         The function can be iterated on the group and/or on conditions
-      (for epochs in epochs['epochs_%s_%s_%s' % (subj, group, cond_name)]).
-     The PSD distribution on the group can be visualized to check normality
-      for statistics.
+        (for epochs in epochs['epochs_%s_%s_%s' % (subj, group, cond_name)]).
+        The PSD distribution on the group can be visualized to check normality
+        for statistics.
 
     Returns:
         freq_list, psd:
 
       - freq_list: list of frequencies in the actual frequency band of interest
         (frequency bin) used for PSD calculation.
       - psd: PSD value for each epoch, each channel, and each frequency,
-      ndarray (n_epochs, n_channels, n_frequencies).
-      Note that if time_resolved == True, PSD values are averaged
-      across epochs.
+        ndarray (n_epochs, n_channels, n_frequencies).
+        Note that if time_resolved == True, PSD values are averaged
+        across epochs.
     """
 
     # dropping EOG channels (incompatible with connectivity map model in stats)
     for ch in epochs.info['chs']:
         if ch['kind'] == 202:  # FIFFV_EOG_CH
             epochs.drop_channels([ch['ch_name']])
 
@@ -483,16 +483,17 @@
 
     elif mode.lower() == 'ccorr':
         angle = np.angle(complex_signal)
         mu_angle = circmean(angle, axis=3).reshape(n_epoch, n_freq, 2 * n_ch, 1)
         angle = np.sin(angle - mu_angle)
 
         formula = 'nilm,nimk->nilk'
-        con = np.einsum(formula, angle, angle.transpose(transpose_axes)) / \
-              np.sqrt(np.einsum('nil,nik->nilk', np.sum(angle ** 2, axis=3), np.sum(angle ** 2, axis=3)))
+        con = np.abs(np.einsum(formula, angle, angle.transpose(transpose_axes)) /
+                     np.sqrt(np.einsum('nil,nik->nilk', np.sum(angle ** 2, axis=3), 
+                                       np.sum(angle ** 2, axis=3))))
         
     elif mode.lower() == 'pli':
         c = np.real(complex_signal)
         s = np.imag(complex_signal)
         dphi = _multiply_conjugate_time(c, s, transpose_axes=transpose_axes)
         con = abs(np.mean(np.sign(np.imag(dphi)), axis=4))
         
@@ -648,61 +649,67 @@
         sampling_rate:
             sampling rate.
         freq_range:
             a list of two specifying the frequency range.
             e.g. [5,30] refers to every integer in the frequency bin from 5 Hz to 30 Hz.
     Returns:
         complex_signal:
-          shape is (2, n_epochs, n_channels, n_frequencies, n_times)
+          shape is (2, n_epochs, n_channels, n_tapers, n_frequencies, n_times)
     """
 
     complex_signal = np.array([mne.time_frequency.tfr_array_multitaper(data[participant], sfreq=sampling_rate,
                                                                        freqs=np.arange(
                                                                            freq_range[0], freq_range[1], 1),
                                                                        n_cycles=4, zero_mean=False, use_fft=True,
                                                                        decim=1,
                                                                        output='complex')
                                for participant in range(2)])
 
     return complex_signal
 
 
-def compute_freq_bands(data: np.ndarray, sampling_rate: int, freq_bands: dict, **filter_options) -> np.ndarray:
+def compute_freq_bands(data: np.ndarray, sampling_rate: int, freq_bands: dict, filter_signal: bool = True , **filter_options) -> np.ndarray:
     """
     Computes analytic signal per frequency band using FIR filtering
     and Hilbert transform.
 
     Arguments:
         data:
             shape is (2, n_epochs, n_channels, n_times)
             real-valued data to compute analytic signal from.
         sampling_rate:
             sampling rate.
+        filter_signal:
+            bool: whether to apply a filter on the signal,
+            default, true
         freq_bands:
             a dictionary specifying frequency band labels and corresponding frequency ranges
-            e.g. {'alpha':[8,12],'beta':[12,20]} indicates that computations are performed over two frequency bands: 8-12 Hz for the alpha band and 12-20 Hz for the beta band.
+            e.g. {'alpha':[8,12], 'beta':[12,20]} indicates that computations are performed over two frequency bands: 8-12 Hz for the alpha band and 12-20 Hz for the beta band.
         **filter_options:
             additional arguments for mne.filter.filter_data, such as filter_length, l_trans_bandwidth, h_trans_bandwidth
     Returns:
         complex_signal: array, shape is
             (2, n_epochs, n_channels, n_freq_bands, n_times)
     """
     assert data[0].shape[0] == data[1].shape[0], "Two data streams should have the same number of trials."
     data = np.array(data)
 
-    # filtering and hilbert transform
+    # filtering and Hilbert transform
     complex_signal = []
     for freq_band in freq_bands.values():
-        filtered = np.array([mne.filter.filter_data(data[participant],
+        if filter_signal:
+            filtered = np.array([mne.filter.filter_data(data[participant],
                                                     sampling_rate, l_freq=freq_band[0], h_freq=freq_band[1],
                                                     **filter_options,
                                                     verbose=False)
                              for participant in range(2)
                              # for each participant
                              ])
+        else:
+            filtered=np.array([data[participant] for participant in range(2)])
         hilb = signal.hilbert(filtered)
         complex_signal.append(hilb)
 
     complex_signal = np.moveaxis(np.array(complex_signal), [0], [3])
 
     return complex_signal
 
@@ -755,90 +762,88 @@
     s = np.imag(phase)
     dphi = _multiply_conjugate(c, s, transpose_axes=transpose_axes)
     con = abs(dphi) / n_samp
     con = np.nanmean(con, axis=1)
     return con
 
 
-def xwt(sig1: mne.Epochs, sig2: mne.Epochs, sfreq: Union[int, float],
-        freqs: Union[int, np.ndarray], analysis: str) -> np.ndarray:
+def xwt(sig1: mne.Epochs, sig2: mne.Epochs,
+        freqs: Union[int, np.ndarray], n_cycles=5.0, mode: str = "xwt") -> np.ndarray:
     """
-    Perfroms a cross wavelet transform on two signals.
+    Performs a cross wavelet transform on two signals.
 
     Arguments:
 
         sig1 : mne.Epochs
             Signal (eg. EEG data) of first participant.
 
         sig2 : mne.Epochs
             Signal (eg. EEG data) of second participant.
 
-        sfreq: int | float
-            Sampling frequency of the data in Hz.
-
         freqs: int | float
             Range of frequencies of interest in Hz.
 
-        analysis: str
-            Sets the type of analyses
+        mode: str
+            Sets the type of analyses.
 
     Note:
         This function relies on MNE's mne.time_frequency.morlet
         and mne.time_frequency.tfr.cwt functions.
-
+    
     Returns:
         data:
-            Wavelet results. The shape is (n_chans1, n_chans2, n_epochs, n_freqs, n_samples)
+            Wavelet results. The shape is (n_chans1, n_chans2, n_epochs, n_freqs, n_samples).
             Wavelet transform coherence calculated according to Maraun & Kurths (2004)
     """
+    
+    # Set parameters for the output
+    n_freqs = len(freqs)
+    sfreq = sig1.info['sfreq']
+    assert sig1.info['sfreq'] == sig2.info['sfreq'], "Sig1 et sig2 should have the same sfreq value."
 
+    n_epochs1, n_chans1, n_samples1 = sig1.get_data().shape
+    n_epochs2, n_chans2, n_samples2 = sig2.get_data().shape
 
-    # Set the mother wavelet
-    Ws = mne.time_frequency.tfr.morlet(sfreq, freqs, n_cycles=5.0, sigma=None,
-                                       zero_mean=True)
+    assert n_epochs1 == n_epochs2, "n_epochs1 and n_epochs2 should have the same number of epochs."
+    assert n_chans1 == n_chans2, "n_chans1 and n_chans2 should have the same number of channels."
+    assert n_samples1 == n_samples2, "n_samples1 and n_samples2 should have the same number of samples."
 
-    # Set parameters for the output
-    n_freqs = len(freqs)
-    n_epochs, n_chans1, n_samples = sig1.get_data().shape
-    n_epochs, n_chans2, n_samples = sig2.get_data().shape
+    cross_sigs = np.zeros((n_chans1, n_chans2, n_epochs1, n_freqs, n_samples1), dtype=complex) * np.nan
+    wcts = np.zeros((n_chans1, n_chans2, n_epochs1, n_freqs, n_samples1), dtype=complex) * np.nan
 
-    cross_sigs = np.zeros(
-        (n_chans1, n_chans2, n_freqs, n_samples),
-        dtype=complex) * np.nan
-    wcts = np.zeros(
-            (n_chans1, n_chans2, n_freqs, n_samples),
-            dtype=complex) * np.nan
+    # Set the mother wavelet
+    Ws = mne.time_frequency.tfr.morlet(sfreq, freqs, 
+                                       n_cycles=n_cycles, sigma=None, zero_mean=True)
 
-    # perform a continuous wavelet transform on all epochs of each signal
+    # Perform a continuous wavelet transform on all epochs of each signal
     for ind1, ch_label1 in enumerate(sig1.ch_names):
         for ind2, ch_label2 in enumerate(sig2.ch_names):
             # Extract the channel's data for both participants and apply cwt
             cur_sig1 = np.squeeze(sig1.get_data(mne.pick_channels(sig1.ch_names, [ch_label1])))
             out1 = mne.time_frequency.tfr.cwt(cur_sig1, Ws, use_fft=True,
                                               mode='same', decim=1)
             cur_sig2 = np.squeeze(sig2.get_data(mne.pick_channels(sig2.ch_names, [ch_label2])))
             out2 = mne.time_frequency.tfr.cwt(cur_sig2, Ws, use_fft=True,
                                               mode='same', decim=1)
-            # Average across epochs
-            tfr_cwt1 = out1.mean(0)
-            tfr_cwt2 = out2.mean(0)
+            
             # Compute cross-spectrum
-            wps1 = tfr_cwt1 * tfr_cwt1.conj()
-            wps2 = tfr_cwt2 * tfr_cwt2.conj()
-            cross_sig = (out1 * out2.conj()).mean(0)
-            cross_sigs[ind1, ind2, :, :] = cross_sig
+            wps1 = out1 * out1.conj()
+            wps2 = out2 * out2.conj()
+            cross_sig = out1 * out2.conj()
+            cross_sigs[ind1, ind2, :, :, :] = cross_sig
             coh = (cross_sig) / (np.sqrt(wps1*wps2))
             abs_coh = np.abs(coh)
             wct = (abs_coh - np.min(abs_coh)) / (np.max(abs_coh) - np.min(abs_coh))
-            wcts[ind1, ind2, :, :] = wct
-    if analysis == 'power':
-        data = np.abs((cross_sigs))
-    elif analysis == 'phase':
+            wcts[ind1, ind2, :, :, :] = wct
+
+    if mode == 'power':
+        data = np.abs(cross_sigs)
+    elif mode == 'phase':
         data = np.angle(cross_sigs)
-    elif analysis == 'xwt':
+    elif mode == 'xwt':
         data = cross_sigs
-    elif analysis == 'wtc':
-        data = wcts
+    elif mode == 'wtc':
+        data = wcts 
     else:
-        data = 'Please specify a valid analysis: power, phase, xwt, or wtc.'
+        data = 'Please specify a valid mode: power, phase, xwt, or wtc.'
         print(data)
-    return data
+    return data
```

### Comparing `hypyp-0.4.0b8/hypyp/data/Basehead.obj` & `hypyp-0.4.0b9/hypyp/data/Basehead.obj`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/ext/mpl3d/camera.py` & `hypyp-0.4.0b9/hypyp/ext/mpl3d/camera.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/ext/mpl3d/glm.py` & `hypyp-0.4.0b9/hypyp/ext/mpl3d/glm.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/ext/mpl3d/lighting.py` & `hypyp-0.4.0b9/hypyp/ext/mpl3d/lighting.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/ext/mpl3d/mesh.py` & `hypyp-0.4.0b9/hypyp/ext/mpl3d/mesh.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/ext/mpl3d/trackball.py` & `hypyp-0.4.0b9/hypyp/ext/mpl3d/trackball.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/fnirs_tools.py` & `hypyp-0.4.0b9/hypyp/fnirs_tools.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/mvarica.py` & `hypyp-0.4.0b9/hypyp/mvarica.py`

 * *Files identical despite different names*

### Comparing `hypyp-0.4.0b8/hypyp/prep.py` & `hypyp-0.4.0b9/hypyp/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 def filt(raw_S: list) -> list:
     """
     Filters list of raw data to remove slow drifts.
 
     Arguments:
         raw_S: list of Raw data (as an example: different occurences of
-          a condition for a participant). Raws are MNE objects.
+            a condition for a participant). Raws are MNE objects.
 
     Returns:
         raws: list of high-pass filtered raws.
     """
     # TODO: l_freq and h_freq as param
     raws = []
     for raw in raw_S:
@@ -43,22 +43,22 @@
     """
     Plots Independent Components for each participant (calculated from Epochs),
     let the user choose the relevant components for artifact rejection
     and apply ICA on Epochs.
 
     Arguments:
         icas: list of Independent Components for each participant (IC are MNE
-          objects).
+            objects).
         epochs: list of 2 Epochs objects (for each participant). Epochs_S1
-          and Epochs_S2 correspond to a condition and can result from the
-          concatenation of Epochs from different experimental realisations
-          of the condition.
-          Epochs are MNE objects: data are stored in an array of shape
-          (n_epochs, n_channels, n_times) and parameters information is
-          stored in a disctionnary.
+            and Epochs_S2 correspond to a condition and can result from the
+            concatenation of Epochs from different experimental realisations
+            of the condition.
+            Epochs are MNE objects: data are stored in an array of shape
+            (n_epochs, n_channels, n_times) and parameters information is
+            stored in a disctionnary.
 
     Returns:
         cleaned_epochs_ICA: list of 2 cleaned Epochs for each participant
           (the chosen IC have been removed from the signal).
     """
     # plotting Independant Components for each participant
     for ica in icas:
@@ -133,42 +133,42 @@
     on Epochs, for each participant.
 
     Pre requisite : install autoreject
     https://api.github.com/repos/autoreject/autoreject/zipball/master
 
     Arguments:
         epochs: list of 2 Epochs objects (for each participant).
-          Epochs_S1 and Epochs_S2 correspond to a condition and can result
-          from the concatenation of Epochs from different experimental
-          realisations of the condition (Epochs are MNE objects).
+            Epochs_S1 and Epochs_S2 correspond to a condition and can result
+            from the concatenation of Epochs from different experimental
+            realisations of the condition (Epochs are MNE objects).
         n_components: the number of principal components that are passed to the
-          ICA algorithm during fitting, int. For a first estimation,
-          n_components can be set to 15.
+            ICA algorithm during fitting, int. For a first estimation,
+            n_components can be set to 15.
         method: the ICA method used, str 'fastica', 'infomax' or 'picard'.
-          'Fastica' is the most frequently used. Use the fit_params argument to set
-           additional parameters. Specifically, if you want Extended Infomax, set
-           method=’infomax’ and fit_params=dict(extended=True) (this also works
-           for method=’picard’). 
+            'Fastica' is the most frequently used. Use the fit_params argument to set
+            additional parameters. Specifically, if you want Extended Infomax, set
+            method=’infomax’ and fit_params=dict(extended=True) (this also works
+            for method=’picard’). 
         fit_params: Additional parameters passed to the ICA estimator
-           as specified by method. None by default.
+            as specified by method. None by default.
         random_state: the parameter used to compute random distributions
-          for ICA calulation, int or None. It can be useful to fix
-          random_state value to have reproducible results. For 15
-          components, random_state can be set to 97, for 20 components to 0
-          for example.
+            for ICA calulation, int or None. It can be useful to fix
+            random_state value to have reproducible results. For 15
+            components, random_state can be set to 97, for 20 components to 0
+            for example.
 
     Note:
         If Autoreject and ICA take too much time, change the decim value
         (see MNE documentation).
         Please filter the Epochs between 2 and 30 Hz before ICA fit
         (mne.Epochs.filter(epoch, 2, 30, method='fir')).
 
     Returns:
         icas: list of Independant Components for each participant (IC are MNE
-          objects, see MNE documentation for more details).
+            objects, see MNE documentation for more details).
     """
     icas = []
     for epoch in epochs:
         # per subj
         # applying AR to find global rejection threshold
         reject = get_rejection_threshold(epoch, ch_types='eeg')
         # if very long, can change decim value
@@ -189,35 +189,35 @@
 
 
 def AR_local(cleaned_epochs_ICA: list, strategy:str = 'union', threshold:float = 50.0, verbose: bool = False) -> list:
     """
     Applies local Autoreject to repair or reject bad epochs.
 
     Arguments:
-        clean_epochs_ICA: list of Epochs after global Autoreject and ICA.
+        cleaned_epochs_ICA: list of Epochs after global Autoreject and ICA.
         strategy: more or less generous strategy to reject bad epochs: 'union'
-          or 'intersection'. 'union' rejects bad epochs from subject 1 and
-          subject 2 immediatly, whereas 'intersection' rejects shared bad epochs
-          between subjects, tries to repare remaining bad epochs per subject,
-          reject the non-reparable per subject and finally equalize epochs number
-          between subjects. Set to 'union' by default.
+            or 'intersection'. 'union' rejects bad epochs from subject 1 and
+            subject 2 immediatly, whereas 'intersection' rejects shared bad epochs
+            between subjects, tries to repare remaining bad epochs per subject,
+            reject the non-reparable per subject and finally equalize epochs number
+            between subjects. Set to 'union' by default.
         threshold: percentage of epochs removed that is accepted. Above
-          this threshold, data are considered as a too shortened sample
-          for further analyses. Set to 50.0 by default.
+            this threshold, data are considered as a too shortened sample
+            for further analyses. Set to 50.0 by default.
         verbose: option to plot data before and after AR, boolean, set to
-          False by default. # use verbose = false until next Autoreject update
+            False by default. # use verbose = false until next Autoreject update
 
     Note:
         To reject or repair epochs, parameters are more or less conservative,
         see http://autoreject.github.io/generated/autoreject.AutoReject.
 
     Returns:
         cleaned_epochs_AR: list of Epochs after local Autoreject.
         dic_AR: dictionnary with the percentage of epochs rejection
-          for each subject and for the intersection of the them.
+            for each subject and for the intersection of the them.
     """
     bad_epochs_AR = []
     AR = []
     dic_AR = {}
     dic_AR['strategy'] = strategy
     dic_AR['threshold'] = threshold
```

### Comparing `hypyp-0.4.0b8/hypyp/stats.py` & `hypyp-0.4.0b9/hypyp/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 def statsCond(data: np.ndarray, epochs: mne.Epochs, n_permutations: int, alpha: float) -> tuple:
     """
     Computes statistical t test on participant measure (e.g. PSD) for a condition.
 
     Arguments:
         data: array of participants measure (e.g. PSD) for
-          a condition (n_samples, n_tests, nfreq: n_tests the channels).
-          Values will be averaged on nfreq for statistics.
+            a condition (n_samples, n_tests, nfreq: n_tests the channels).
+            Values will be averaged on nfreq for statistics.
         epochs: Epochs object for a condition from a random participant, only
-          used to get parameters from the info (sampling frequencies for example).
+            used to get parameters from the info (sampling frequencies for example).
         n_permutations: the number of permutations, int. Should be at least 2*n
-          sample, can be set to 50000 for example.
+            sample, can be set to 50000 for example.
         alpha: the threshold for ttest, float, can be set to 0.05.
 
     Note:
         This ttest calculates if the observed mean significantly deviates
         from 0; it does not compare two periods, but one period with the null
         hypothesis. Randomized data are generated with random sign flips.
         The tail is set to 0 by default (= the alternative hypothesis is that
@@ -52,22 +52,22 @@
     Returns:
         T_obs, p_values, H0, adj_p, T_obs_plot:
         - T_obs: T-statistic observed for all variables, array of shape (n_tests).
 
         - p_values: p-values for all the tests, array of shape (n_tests).
 
         - H0: T-statistic obtained by permutations and t-max trick for multiple
-          comparisons, array of shape (n_permutations).
+            comparisons, array of shape (n_permutations).
 
         - adj_p: adjusted p values from FDR correction, array of shape
-          (n_tests, n_tests), with boolean assessment for p values
-          and p values corrected.
+            (n_tests, n_tests), with boolean assessment for p values
+            and p values corrected.
 
         - T_obs_plot: statistical values to plot, from sensors above alpha threshold,
-          array of shape (n_tests,).
+            array of shape (n_tests,).
     """
     # checking whether data have the same size
     assert(len(data.shape) == 3), "PSD does not have the appropriate shape!"
 
     # averaging across frequencies (compute stats only in ch space)
     power = np.mean(data, axis=2)
     T_obs, p_values, H0 = mne.stats.permutation_t_test(power, n_permutations,
@@ -102,27 +102,27 @@
 def con_matrix(epochs: mne.Epochs, freqs_mean: list, draw: bool = False) -> tuple:
     """
     Computes a priori channel connectivity across space and frequencies.
 
     Arguments:
         epochs: one participant Epochs object; contains channel information.
         freqs_mean: list of frequencies in frequency-band-of-interest used
-          by MNE for power or coherence spectral density calculation.
+            by MNE for power or coherence spectral density calculation.
         draw: option to plot the connectivity matrices, boolean.
 
     Returns:
         ch_con, ch_con_freq:
 
         - ch_con: connectivity matrix between channels along space based on
-          their position, scipy.sparse.csr_matrix of shape
-          (n_channels, n_channels).
+            their position, scipy.sparse.csr_matrix of shape
+            (n_channels, n_channels).
 
         - ch_con_freq: connectivity matrix between channels along space and
-          frequencies, scipy.sparse.csr_matrix of shape
-          (n_channels*len(freqs_mean), n_channels*len(freqs_mean)).
+            frequencies, scipy.sparse.csr_matrix of shape
+            (n_channels*len(freqs_mean), n_channels*len(freqs_mean)).
     """
 
     # creating channel-to-channel connectivity matrix in space
     ch_con, ch_names_con = find_ch_adjacency(epochs.info,
                                                 ch_type='eeg')
 
     ch_con_arr = ch_con.toarray()
@@ -162,37 +162,37 @@
     """
     Computes a priori connectivity across space and frequencies
     between pairs of channels for which connectivity indices have
     been calculated, to merge data (2 brains).
 
     Arguments:
         electrodes: electrode pairs for which connectivity indices have
-          been computed, list of tuples with channels indexes, see
-          indices_connectivity_interbrain function in toolbox (analyses).
+            been computed, list of tuples with channels indexes, see
+            indices_connectivity_interbrain function in toolbox (analyses).
         ch_con: connectivity matrix between channels along space based on their
-          position, scipy.sparse.csr_matrix of shape (n_channels, n_channels).
+            position, scipy.sparse.csr_matrix of shape (n_channels, n_channels).
         freqs_mean: list of frequencies in the frequency-band-of-interest used
-          by MNE for coherence spectral density calculation (connectivity indices).
+            by MNE for coherence spectral density calculation (connectivity indices).
         plot: option to plot the connectivity matrices, boolean.
 
     Note:
         It is assumed that there was no a priori connectivity
         between channels from the two participants.
 
     Returns:
         metaconn, metaconn_freq:
 
         - metaconn: a priori connectivity based on channel location, between
-          pairs of channels for which connectivity indices have been calculated,
-          to merge data, matrix of shape (len(electrodes), len(electrodes)).
+            pairs of channels for which connectivity indices have been calculated,
+            to merge data, matrix of shape (len(electrodes), len(electrodes)).
 
         - metaconn_freq: a priori connectivity between pairs of channels for which
-          connectivity indices have been calculated, across space and
-          frequencies, to merge data, matrix of shape
-          (len(electrodes)*len(freqs_mean), len(electrodes)*len(freqs_mean)).
+            connectivity indices have been calculated, across space and
+            frequencies, to merge data, matrix of shape
+            (len(electrodes)*len(freqs_mean), len(electrodes)*len(freqs_mean)).
     """
 
     n = np.max(electrodes, axis=0)[0]+1
     # n = 62
     metaconn = np.zeros((len(electrodes), len(electrodes)))
     for ne1, (e11, e12) in enumerate(electrodes):
         for ne2, (e21, e22) in enumerate(electrodes):
@@ -235,32 +235,32 @@
     """
     Computes a priori connectivity between pairs of sensors for which
     connectivity indices have been calculated, across space and frequencies
     (based on channel location).
 
     Arguments:
         electrodes: electrode pairs for which connectivity has been computed,
-          list of tuples with channel indices, see indices_connectivity
-          intrabrain function in toolbox (analyses).
+            list of tuples with channel indices, see indices_connectivity
+            intrabrain function in toolbox (analyses).
         ch_con: connectivity matrix between sensors along space based on their
-          position, scipy.sparse.csr_matrix of shape (n_channels, n_channels).
+            position, scipy.sparse.csr_matrix of shape (n_channels, n_channels).
         freqs_mean: list of frequencies in the frequency-band-of-interest used
-          by MNE for coherence spectral density calculation (connectivity indices).
+            by MNE for coherence spectral density calculation (connectivity indices).
 
     Returns:
         metaconn, metaconn_freq:
 
         - metaconn: a priori connectivity based on channel location, between
-          pairs of channels for which connectivity indices have been calculated,
-          matrix of shape (len(electrodes), len(electrodes)).
+            pairs of channels for which connectivity indices have been calculated,
+            matrix of shape (len(electrodes), len(electrodes)).
 
         - metaconn_freq: a priori connectivity between pairs of channels for which
-          connectivity indices have been calculated, across space and
-          frequencies, for merge data, matrix of shape
-          (len(electrodes)*len(freqs_mean), len(electrodes)*len(freqs_mean)).
+            connectivity indices have been calculated, across space and
+            frequencies, for merge data, matrix of shape
+            (len(electrodes)*len(freqs_mean), len(electrodes)*len(freqs_mean)).
     """
 
     metaconn = np.zeros((len(electrodes), len(electrodes)))
     for ne1, (e11, e12) in enumerate(electrodes):
         for ne2, (e21, e22) in enumerate(electrodes):
             # print(ne1,e11,e12,ne2,e21,e22)
             metaconn[ne1, ne2] = (((ch_con[e11, e21]) and (ch_con[e12, e22])) or
@@ -299,42 +299,42 @@
 def statscondCluster(data: list, freqs_mean: list, ch_con_freq: scipy.sparse.csr_matrix, tail: int, n_permutations: int, alpha: float) -> tuple:
     """
     Computes cluster-level statistical permutation test, corrected with
     channel connectivity across space and frequencies.
 
     Arguments:
         data: values from different conditions or different groups to compare,
-          list of arrays (3d for time-frequency power or connectivity values).
+            list of arrays (3d for time-frequency power or connectivity values).
         freqs_mean: frequencies in frequency-band-of-interest used by MNE
-          for PSD or CSD calculation, list.
+            for PSD or CSD calculation, list.
         ch_con_freq: connectivity or metaconnectivity matrix for PSD or CSD
-          values to assess a priori connectivity between channels across
-          space and frequencies based on their position, bsr_matrix.
+            values to assess a priori connectivity between channels across
+            space and frequencies based on their position, bsr_matrix.
         tail: direction of the ttest, can be set to 1, 0 or -1.
         n_permutations: number of permutations computed, can be set to 50000.
         alpha: threshold to consider clusters significant, can be set to 0.05
-          or less.
+            or less.
 
     Returns:
         F_obs, clusters, cluster_pv, H0, F_obs_plot:
 
         - F_obs: statistic (F by default) observed for all variables,
-          array of shape (n_tests,).
+            array of shape (n_tests,).
 
         - clusters: boolean array with same shape as the input data, 
-          True values indicating locations that are part of a cluster, array.
+            True values indicating locations that are part of a cluster, array.
 
         - cluster_p_values: p-value for each cluster, array.
 
         - H0: max cluster level stats observed under permutation, array of
-          shape (n_permutations,).
+            shape (n_permutations,).
 
         - F_obs_plot: statistical values above alpha threshold, to plot
-          significant sensors (see plot_significant_sensors function in the toolbox)
-          array of shape (n_tests,).
+            significant sensors (see plot_significant_sensors function in the toolbox)
+            array of shape (n_tests,).
     """
 
     # computing the cluster permutation t test
     F_obs, clusters, cluster_p_values, H0 = permutation_cluster_test(data,
                                                                      threshold=None,
                                                                      n_permutations=n_permutations,
                                                                      tail=tail, adjacency=ch_con_freq,
@@ -367,63 +367,63 @@
     """
     Computes cluster-level statistical permutation test, corrected with
     channel connectivity across space and frequencies to compare groups
     or conditions for simple or multiple comparisons.
 
     Arguments:
         data: values from different groups or conditions to compare,
-          list of arrays (3d for time-frequency power or connectivity values),
-          or np.array for f multiple-way ANOVA test. For this test and the 
-          paired ttest, samples must have the same dimension.
+            list of arrays (3d for time-frequency power or connectivity values),
+            or np.array for f multiple-way ANOVA test. For this test and the 
+            paired ttest, samples must have the same dimension.
         test: nature of the test used to compare groups or conditions.
-          Can be a t test for independant or paired samples
-          ('ind ttest' or 'rel ttest'), a one-way ANOVA test
-          ('f oneway'), or a multiple-way ANOVA test ('f multipleway), str.
+            Can be a t test for independant or paired samples
+            ('ind ttest' or 'rel ttest'), a one-way ANOVA test
+            ('f oneway'), or a multiple-way ANOVA test ('f multipleway), str.
         factor_level: for multiple-way ANOVA test, describe the number of level
-          for each factor, list (if compare 2 groups and 2 conditions,
-          factor_levels = [2, 2] and data should be an np.array with
-          group1-condition1, group1-condition2, group2-condition1,
-          group2-condition2).
-          Set to None otherwise.
+            for each factor, list (if compare 2 groups and 2 conditions,
+            factor_levels = [2, 2] and data should be an np.array with
+            group1-condition1, group1-condition2, group2-condition1,
+            group2-condition2).
+            Set to None otherwise.
         ch_con_freq: connectivity or metaconnectivity matrix for PSD or CSD
-          values to assess a priori connectivity between channels across
-          space and frequencies based on their position, bsr_matrix.
+            values to assess a priori connectivity between channels across
+            space and frequencies based on their position, bsr_matrix.
         tail: direction of the ttest, can be set to 1, 0 or -1. The tail must
-          be set to 0 for a one-way ANOVA test and to 1 for a mutiple-way
-          ANOVA test.
+            be set to 0 for a one-way ANOVA test and to 1 for a mutiple-way
+            ANOVA test.
         n_permutations: number of permutations computed, can be set to 50000.
         alpha: threshold to consider clusters significant, can be set to 0.05
-          that is the default value. An adjustment is done for a f one-way and
-          multiple-way tests to adapt 0.05 to the number of observations.
+            that is the default value. An adjustment is done for a f one-way and
+            multiple-way tests to adapt 0.05 to the number of observations.
 
     Notes:
         With t_power set to 1, each location is weighted by its statistical
         score in a cluster.
         For a f multipleway ANOVA test with connectivity values, the last
         dimensions have to be flattened in a vector, instead of the shape
         (n_sensors, n_sensors), you can use np.reshape.
 
     Returns:
         Stat_obs, clusters, cluster_pv, H0, Stat_obs_plot:
 
         - Stat_obs: statistic (T or F values according to the assignement
-          of 'test') observed for all variables,
-          array of shape (n_tests,).
+            of 'test') observed for all variables,
+            array of shape (n_tests,).
 
         - clusters: boolean array with same shape as the input data,
-          True values indicating locations that are part of a cluster, array.
+            True values indicating locations that are part of a cluster, array.
 
         - cluster_p_values: p-value for each cluster, array.
 
         - H0: max cluster level stats observed under permutation, array of
-          shape (n_permutations,).
+            shape (n_permutations,).
 
         - Stat_obs_plot: statistical values above alpha threshold,
-          to plot significant sensors (see plot_significant_sensors
-          function in the toolbox) array of shape (n_tests,).
+            to plot significant sensors (see plot_significant_sensors
+            function in the toolbox) array of shape (n_tests,).
     """
 
     # type of test
     if test == 'ind ttest':
         def stat_fun(*arg):
             return(scipy.stats.ttest_ind(arg[0], arg[1], equal_var=False)[0])
     elif test == 'rel ttest':
```

### Comparing `hypyp-0.4.0b8/hypyp/utils.py` & `hypyp-0.4.0b9/hypyp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 def create_epochs(raw_S1: mne.io.Raw, raw_S2: mne.io.Raw, duration: float) -> list:
     """
     Creates Epochs from Raws and vizualize Power Spectral Density (PSD)
     on average Epochs (option).
 
     Arguments:
         raw_S1: list of Raws for participant 1 (with the different
-          experimental realizations of a condition - for example
-          the baseline. The length can be 1).
+            experimental realizations of a condition - for example
+            the baseline. The length can be 1).
         raw_S2: list of Raws for participant 2.  
-          Raws are MNE objects: data are ndarray with shape
-          (n_channels, n_times) and information is a dictionnary
-          sampling parameters.
+            Raws are MNE objects: data are ndarray with shape
+            (n_channels, n_times) and information is a dictionnary
+            sampling parameters.
 
     Note:
         Plots topomaps of PSD values calculated with welch FFT
         for each epoch and each participant, averaged in each
         frequency band-of-interest.
         # TODO: option with verbose
 
@@ -94,30 +94,30 @@
 def merge(epoch_S1: mne.Epochs, epoch_S2: mne.Epochs) -> mne.Epochs:
     """
     Merges Epochs from 2 participants after interpolation of bad channels.
 
     Arguments:
         epoch_S1: Epochs object for participant 1.
         epoch_S2: Epochs object for participant 2.  
-          epoch_S1 and epoch_S2 correspond to a condition and can result
-          from the concatenation of epochs from different experimental
-          realizations of a condition.  
-          Epochs are MNE objects: data are stored in an array of shape
-          (n_epochs, n_channels, n_times) and parameters information
-          is stored in a disctionnary.
+            epoch_S1 and epoch_S2 correspond to a condition and can result
+            from the concatenation of epochs from different experimental
+            realizations of a condition.  
+            Epochs are MNE objects: data are stored in an array of shape
+            (n_epochs, n_channels, n_times) and parameters information
+            is stored in a disctionnary.
 
     Note:
         Bad channels labelling is removed.
         Note that average on reference can not be done anymore. Similarly,
         montage can not be set to the data and as a result topographies in MNE
         are not possible anymore. Use toolbox vizualisations instead.
 
     Returns:
         ep_hyper: Epochs object for the dyad (with merged data of the two
-          participants). The time alignement has been done at raw data creation.
+            participants). The time alignement has been done at raw data creation.
     """
     # checking bad ch for epochs, interpolating
     # and removing them from 'bads' if needed
     if len(epoch_S1.info['bads']) > 0:
         epoch_S1 = mne.Epochs.interpolate_bads(epoch_S1,
                                                reset_bads=True,
                                                mode='accurate',
@@ -195,34 +195,34 @@
 
 def split(raw_merge: mne.io.Raw) -> mne.io.Raw:
     """
     Splits merged Raw data into 2 participants Raw data.
 
     Arguments:
         raw_merge: Raw data for the dyad with data from participant 1
-          and data from participant 2 (channels name are defined with
-          the suffix S1 and S2 respectively).
+            and data from participant 2 (channels name are defined with
+            the suffix S1 and S2 respectively).
 
     Note:
         Participant's Raw data is set to the standard montage 1020
         available in MNE. An average is computed to avoid reference bias
         (see MNE documentation about set_eeg_reference).
 
     Returns:
         raw_1020_S1, raw_1020_S2: Raw data for each participant separately.
-          Raws are MNE objects.
+            Raws are MNE objects.
     """
     ch_S1 = []
     ch_S2 = []
     ch = []
     for name in raw_merge.info['ch_names']:
-        if name.endswith('S1'):
+        if name.endswith('S1') or name.endswith('_1'):
             ch_S1.append(name)
             ch.append(name.split('_')[0])
-        elif name.endswith('S2'):
+        elif name.endswith('S2') or name.endswith('_2'):
             ch_S2.append(name)
 
     # picking individual participant data
     data_S1 = raw_merge.get_data(picks=ch_S1)
     data_S2 = raw_merge.get_data(picks=ch_S2)
 
     # creating info for raws
@@ -234,88 +234,78 @@
     # setting info about channels and task
     raw_S1.info['bads'] = [
         ch.split('_')[0] for ch in ch_S1 if ch in raw_merge.info['bads']]
     raw_S2.info['bads'] = [
         ch.split('_')[0] for ch in ch_S2 if ch in raw_merge.info['bads']]
     for raws in (raw_S1, raw_S2):
         raws.info['description'] = raw_merge.info['description']
-        raws.info['events'] = raw_merge.info['events']
 
     # setting montage 94 electrodes (ignore somes to correspond to our data)
         for ch in raws.info['chs']:
-            if ch['ch_name'].startswith('MOh') or ch['ch_name'].startswith('MOb'):
+            if ch['ch_name'].startswith('MOh') or ch['ch_name'].startswith('MOb') or ('EOG' in ch['ch_name']):
                 # print('emg')
                 ch['kind'] = FIFF.FIFFV_EOG_CH
             else:
                 ch['kind'] = FIFF.FIFFV_EEG_CH
     montage = mne.channels.make_standard_montage('standard_1020')
-    raw_1020_S1 = raw_S1.copy().set_montage(montage)
-    raw_1020_S2 = raw_S2.copy().set_montage(montage)
-    # raw_1020_S1.plot_sensors()
+    raw_1020_S1 = raw_S1.copy().set_montage(montage, on_missing='ignore')
+    raw_1020_S2 = raw_S2.copy().set_montage(montage, on_missing='ignore')
 
     # set reference to electrodes average
     # (instate of initial ref to avoid ref biais)
     # and storing it in raw.info['projs']: applied when Epochs
-    raw_1020_S1, _ = mne.set_eeg_reference(
-        raw_1020_S1, 'average', projection=True)
-    raw_1020_S2, _ = mne.set_eeg_reference(
-        raw_1020_S2, 'average', projection=True)
-
-    # TODO: annotations, subj name, events
-    # task description different across subj
-
-    # raw_1020_S1.plot()
-    # raw_1020_S1.plot_psd()
+    raw_1020_S1, _ = mne.set_eeg_reference(raw_1020_S1, 'average', projection=True)
+    raw_1020_S2, _ = mne.set_eeg_reference(raw_1020_S2, 'average', projection=True)
 
     return raw_1020_S1, raw_1020_S2
 
 
 def concatenate_epochs(epoch_S1: mne.Epochs, epoch_S2: mne.Epochs) -> mne.Epochs:
     """
     Concatenates a list of Epochs in one Epochs object.
 
     Arguments:
         epoch_S1: list of Epochs for participant 1 (for example the
-          list samples different experimental realizations
-          of the baseline condition).
+            list samples different experimental realizations
+            of the baseline condition).
         epoch_S2: list of Epochs for participant 2.  
-          Epochs are MNE objects.
+            Epochs are MNE objects.
 
     Returns:
         epoch_S1_concat, epoch_S2_concat: list of concatenate Epochs
-          (for example one epoch with all the experimental realizations
-          of the baseline condition) for each participant.
+            (for example one epoch with all the experimental realizations
+            of the baseline condition) for each participant.
     """
     epoch_S1_concat = mne.concatenate_epochs(epoch_S1)
     epoch_S2_concat = mne.concatenate_epochs(epoch_S2)
 
     return epoch_S1_concat, epoch_S2_concat
 
 
 def normalizing(baseline: np.ndarray, task: np.ndarray, type: str) -> np.ndarray:
     """
     Computes Zscore or Logratio of a value between a 'task' condition and
     a baseline for example.
 
     Arguments:
         baseline: PSD or CSD values for the 'baseline',
-          ndarray, shape (n_epochs, n_channels, n_frequencies).
+            ndarray, shape (n_epochs, n_channels, n_frequencies).
         task: PSD or CSD values for the 'task' conditions,
-          ndarray, shape (n_epochs, n_channels, n_frequencies).
+            ndarray, shape (n_epochs, n_channels, n_frequencies).
         type: normalization choice, str 'Zscore' or 'Logratio'.
-        
+
     Note:
         If normalization's type is 'Logratio', only positive values
         can be used as input (if it is not the case, take the absolute
         value).
 
     Returns:
         Normed_task: PSD or CSD values for the condition 'task' normed by
-          values in a baseline and average across epochs, ndarray, shape
-          (n_channels, n_frequencies).
+            values in a baseline and average across epochs, ndarray, shape
+            (n_channels, n_frequencies).
     """
     m_baseline = np.mean(baseline, axis=0)
     m_task = np.mean(task, axis=0)
     std_baseline = np.std(baseline, axis=0)
     # normalizing power during task by baseline average power across events
     if type == 'Zscore':
         s = np.subtract(m_task, m_baseline)
@@ -328,23 +318,23 @@
 
 def generate_random_epoch(epoch: mne.Epochs, mu: float=0, sigma: float=2.0)-> mne.Epochs:
     """
     Generate epochs with random data. 
 
     Arguments:
         epoch: mne.Epochs
-          Epochs object to get epoch info structure
+            Epochs object to get epoch info structure
         mu: float
-          Mean of the normal distribution
+            Mean of the normal distribution
         sigma: float
-          Standart deviation of the normal distribution
+            Standart deviation of the normal distribution
 
     Returns:
         mne.Epochs
-          new epoch with random data with normal distribution
+            new epoch with random data with normal distribution
     """
 
     # Get epoch information 
     info = epoch.info #create_info(ch_names=ch_names, sfreq=sfreq, ch_types=ch_types)
 
     # Get epochs as a 3D NumPy array of shape (n_epochs, n_channels, n_times)
     # Get the arrays’ shape
@@ -360,29 +350,29 @@
 def generate_virtual_epoch(epoch: mne.Epochs, W: np.ndarray, frequency_mean: float=10, frequency_std: float=0.2,
                            noise_phase_level: float=0.005, noise_amplitude_level: float=0.1)-> mne.Epochs:
     """
     Generate epochs with simulated data using Kuramoto oscillators. 
 
     Arguments:
         epoch: mne.Epochs
-          Epochs object to get epoch info structure
+            Epochs object to get epoch info structure
         W: np.ndarray
-          Coupling matrix between the oscillators
+            Coupling matrix between the oscillators
         frequency_mean: float
-          Mean of the normal distribution for oscillators frequency
+            Mean of the normal distribution for oscillators frequency
         frequency_std: float
-          Standart deviation of the normal distribution for oscillators frequency
+            Standart deviation of the normal distribution for oscillators frequency
         noise_phase_level: float
-          Amount of noise at the phase level
+            Amount of noise at the phase level
         noise_amplitude_level: float
-          Amount of noise at the amplitude level
+            Amount of noise at the amplitude level
 
     Returns:
         mne.Epochs
-          new epoch with simulated data
+            new epoch with simulated data
     """
 
     n_epo, n_chan, n_samp = epochs.get_data().shape
     sfreq = epochs.info['sfreq']
 
     Nt = n_samp * n_epo
     tmax = n_samp / sfreq * n_epo  # s
```

### Comparing `hypyp-0.4.0b8/hypyp/viz.py` & `hypyp-0.4.0b9/hypyp/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 def transform(locs: np.ndarray,traX: float=0.15, traY: float=0, traZ: float=0.5, rotY: float=(np.pi)/2, rotZ: float=(np.pi)/2) -> np.ndarray:
     """
     Calculates new locations for the EEG locations.
 
     Arguments:
         locs: array of shape (n_sensors, 3)
-          3d coordinates of the sensors
+            3d coordinates of the sensors
         traX: float
-          X translation to apply to the sensors
+            X translation to apply to the sensors
         traY: float
-          Y translation to apply to the sensors
+            Y translation to apply to the sensors
         traZ: float
-          Z translation to apply to the sensors
+            Z translation to apply to the sensors
         rotY: float
-          Y rotation to apply to the sensors
+            Y rotation to apply to the sensors
         rotZ: float
-          Z rotation to apply to the sensors
+            Z rotation to apply to the sensors
 
     Returns:
         result: array (n_sensors, 3)
-          new 3d coordinates of the sensors
+            new 3d coordinates of the sensors
     """
     # Z rotation
     newX = locs[:, 0] * np.cos(rotZ) - locs[:, 1] * np.sin(rotZ)
     newY = locs[:, 0] * np.sin(rotZ) + locs[:, 1] * np.cos(rotZ)
     locs[:, 0] = newX
     locs[:, 0] = locs[:, 0] + traX
     locs[:, 1] = newY
@@ -76,19 +76,19 @@
 
 def plot_sensors_2d_inter(epo1: mne.Epochs, epo2: mne.Epochs, lab: bool = False):
     """
     Plots sensors in 2D with x representation for bad sensors.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         epo2: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         lab: option to plot channel names
-          True by default.
+            True by default.
 
     Returns:
         None: plot the sensors in 2D within the current axis.
     """
 
     # extract sensor info and transform loc to fit with headmodel
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
@@ -144,47 +144,42 @@
 
 def plot_links_2d_inter(epo1: mne.Epochs, epo2: mne.Epochs, C: np.ndarray, threshold: str='auto', steps: int=10):
     """
     Plots hyper-connectivity in 2D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         epo2: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         C: array, (len(loc1), len(loc2))
-          matrix with the values of hyper-connectivity
+            matrix with the values of hyper-connectivity
         threshold: float | str
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
-          Can also be "auto" to use a threshold automatically
-          calculated from your matrix as the maximum median 
-          by column + the maximum standard error by column.
-          Note that the automatic threshold is specific to a 
-          dyad and does not allow to compare different dyads.
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
+            Can also be "auto" to use a threshold automatically
+            calculated from your matrix as the maximum median 
+            by column + the maximum standard error by column.
+            Note that the automatic threshold is specific to a 
+            dyad and does not allow to compare different dyads.
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
-        weight: numpy.float
-          Connectivity weight to determine the thickness
-          of the link
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
 
     Returns:
         None: plot the links in 2D within the current axis.
     """
 
     # extract sensor infos and transform loc to fit with headmodel
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
     loc1 = transform(loc1, traX=-0.17, traY=0, traZ=0.08, rotY=(-np.pi/12), rotZ=(-np.pi/2))
 
     loc2 = copy(np.array([ch['loc'][:3] for ch in epo2.info['chs']]))
     loc2 = transform(loc2, traX=0.17, traY=0, traZ=0.08, rotY=(np.pi/12), rotZ=np.pi/2)
 
-
-
     ctr1 = np.nanmean(loc1, 0)
     ctr2 = np.nanmean(loc2, 0)
 
     # Calculate automatic threshold
     if threshold == 'auto':
       threshold = np.max(np.median(C, 0))+np.max(np.std(C, 0))
     else:
@@ -270,19 +265,19 @@
 def plot_sensors_3d_inter(ax: str, epo1: mne.Epochs, epo2: mne.Epochs, lab: bool = False):
     """
     Plots sensors in 3D with x representation for bad sensors.
 
     Arguments:
         ax: Matplotlib axis created with projection='3d'
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         lab: option to plot channel names
-          False by default.
+            False by default.
 
     Returns:
         None: plot the sensors in 3D within the current axis.
     """
 
     # extract sensor infos and transform loc to fit with headmodel 
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
@@ -337,38 +332,35 @@
 
 def plot_links_3d_inter(ax: str, epo1: mne.Epochs, epo2: mne.Epochs, C: np.ndarray, threshold: str='auto', steps: int=10):
     """
     Plots hyper-connectivity in 3D.
 
     Arguments:
         ax: Matplotlib axis created with projection='3d'
-        loc1: arrays of shape (n_sensors, 3)
-          3d coordinates of the sensors
-        loc2: arrays of shape (n_sensors, 3)
-          3d coordinates of the sensors
+        epo1: mne.Epochs
+            Epochs object to get channel information
+        epo2: mne.Epochs
+            Epochs object to get channel information
         C: array, (len(loc1), len(loc2))
-          matrix with the values of hyper-connectivity
+            matrix with the values of hyper-connectivity
         threshold: float | str
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
-          Can also be "auto" to use a threshold automatically
-          calculated from your matrix as the maximum median 
-          by column + the maximum standard error by column.
-          Note that the automatic threshold is specific to a 
-          dyad and does not allow to compare different dyads.
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
+            Can also be "auto" to use a threshold automatically
+            calculated from your matrix as the maximum median 
+            by column + the maximum standard error by column.
+            Note that the automatic threshold is specific to a 
+            dyad and does not allow to compare different dyads.
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
-        weight: numpy.float
-          Connectivity weight to determine the thickness
-          of the link
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
 
     Returns:
         None: plot the links in 3D within the current axis.
-          Plot hyper-connectivity in 3D.
+            Plot hyper-connectivity in 3D.
     """
     
     # extract sensor infos and transform loc to fit with headmodel 
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
     loc1 = transform(loc1, traX=-0.17, traY=0, traZ=0.08, rotY=(-np.pi/12), rotZ=(-np.pi/2))
   
 
@@ -490,15 +482,15 @@
     clusters corrected t test), computed between groups or conditions on power
     or connectivity values, across simple participants. For statistics with
     inter-brain connectivity values on participant pairs (merge data), use the
     plot_links_3d function.
 
     Arguments:
         T_obs_plot: statistical values to plot, from sensors above alpha threshold,
-          array of shape (n_tests,).
+            array of shape (n_tests,).
         epochs: one participant Epochs object to sample channel information in info.
 
     Returns:
         None: plot topomap with the T or F statistics for significant sensors.
     """
 
     # getting sensors position
@@ -670,32 +662,31 @@
 
 def viz_2D_topomap_inter (epo1: mne.Epochs, epo2: mne.Epochs, C: np.ndarray, threshold: float=0.95, steps: int=10, lab: bool = False):
     """
     Visualization of inter-brain connectivity in 2D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         C: array, (len(loc1), len(loc2))
-          matrix with the values of hyper-connectivity
+            matrix with the values of hyper-connectivity
         threshold: float
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
         lab: option to plot channel names
-          False by default.
-        
+            False by default.
 
     Returns:
         Plot head topomap with sensors and 
-              connectivity links in 2D.
+            connectivity links in 2D.
         ax: The new Axes object.
     """
 
     # defining head model and adding sensors
     fig = plt.figure()
     ax = fig.add_subplot(111, aspect = 1)
     ax.axis("off")
@@ -713,32 +704,31 @@
 
 def viz_2D_headmodel_inter (epo1: mne.Epochs, epo2: mne.Epochs, C: np.ndarray, threshold: float=0.95, steps: int=10, lab: bool = True):
     """
     Visualization of inter-brain connectivity in 2D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         C: array, (len(loc1), len(loc2))
-          matrix with the values of hyper-connectivity
+            matrix with the values of hyper-connectivity
         threshold: float
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
         lab: option to plot channel names
-          True by default.
-        
+            True by default.
 
     Returns:
         Plot headmodel with sensors and 
-              connectivity links in 2D.
+            connectivity links in 2D.
         ax: The new Axes object.
     """
 
     # Visualization of inter-brain connectivity in 2D
     # defining head model and adding sensors
     fig, ax = plt.subplots(1, 1)
     ax.axis("off")
@@ -762,32 +752,31 @@
 
 def viz_3D_inter (epo1: mne.Epochs, epo2: mne.Epochs, C: np.ndarray, threshold: float=0.95, steps: int=10, lab: bool = False):
     """
     Visualization of inter-brain connectivity in 3D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         C: array, (len(loc1), len(loc2))
-          matrix with the values of hyper-connectivity
+            matrix with the values of hyper-connectivity
         threshold: float
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
         lab: option to plot channel names
-          False by default.
-        
+            False by default.
 
     Returns:
         Plot headmodel with sensors and 
-              connectivity links in 3D.
+            connectivity links in 3D.
         ax: The new Axes object.
     """
 
     # defining head model and adding sensors
     vertices, faces = get_3d_heads_inter()
     fig = plt.figure()
     ax = fig.add_subplot(projection='3d')
@@ -806,27 +795,27 @@
 
 def transform_2d_intra(locs: np.ndarray,traX: float=0.15, traY: float=0, traZ:float=0, rotZ: float=(np.pi)/2) -> np.ndarray:
     """
     Calculates new locations for the EEG locations.
 
     Arguments:
         locs: array of shape (n_sensors, 3)
-          3d coordinates of the sensors
+            3d coordinates of the sensors
         traX: float
-          X translation to apply to the sensors
+            X translation to apply to the sensors
         traY: float
-          Y translation to apply to the sensors
+            Y translation to apply to the sensors
         traZ: float
-          Z translation to apply to the sensors
+            Z translation to apply to the sensors
         rotZ: float
-          Z rotation to apply to the sensors
+            Z rotation to apply to the sensors
 
     Returns:
         result: array (n_sensors, 3)
-          new coordinates of the sensors
+            new coordinates of the sensors
     """
     # translation
     locs[:, 0] = locs[:, 0] + traX
     locs[:, 1] = locs[:, 1] + traY
     locs[:, 2] = locs[:, 2] + traZ
 
     # Reduce the size of the eeg headsets
@@ -907,19 +896,19 @@
 
 def plot_sensors_2d_intra(epo1: mne.Epochs, epo2: mne.Epochs, lab: bool = False):
     """
     Plots sensors in 2D with x representation for bad sensors.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         epo2: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         lab: option to plot channel names
-          True by default.
+            True by default.
 
     Returns:
         None: plot the sensors in 2D within the current axis.
     """
 
     # extract sensor info and transform loc to fit with headmodel
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
@@ -978,35 +967,32 @@
                         C1: np.ndarray, C2: np.ndarray,
                         threshold: str='auto', steps: int=2):
     """
     Plots hyper-connectivity in 2D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         epo2: mne.Epochs
-          Epochs object to get channels information
+            Epochs object to get channels information
         C1: array, (len(loc1), len(loc1))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         C2: array, (len(loc2), len(loc2))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         threshold: float | str
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
-          Can also be "auto" to use a threshold automatically
-          calculated from your matrix as the maximum median 
-          by column + the maximum standard error by column.
-          Note that the automatic threshold is specific to a 
-          dyad and does not allow to compare different dyads.
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
+            Can also be "auto" to use a threshold automatically
+            calculated from your matrix as the maximum median 
+            by column + the maximum standard error by column.
+            Note that the automatic threshold is specific to a 
+            dyad and does not allow to compare different dyads.
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
-        weight: numpy.float
-          Connectivity weight to determine the thickness
-          of the link
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
 
     Returns:
         None: plot the links in 2D within the current axis.
     """
 
     # extract sensor infos and transform loc to fit with headmodel
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
@@ -1188,34 +1174,33 @@
                           threshold: float=0.95, steps: int=2,
                           lab: bool = False):
     """
     Visualization of inter-brain connectivity in 3D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         C1: array, (len(loc1), len(loc1))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         C2: array, (len(loc2), len(loc2))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         threshold: float
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
         lab: option to plot channel names
-          False by default.
-        
+            False by default.
 
     Returns:
         Plot head topomap with sensors and 
-              intra-brain connectivity links in 2D.
+            intra-brain connectivity links in 2D.
         ax: The new Axes object.
     """
 
     # defining head model and adding sensors
     fig = plt.figure()
     ax = fig.add_subplot(111, aspect = 1)
     ax.axis("off")
@@ -1265,19 +1250,19 @@
 def plot_sensors_3d_intra(ax: str, epo1: mne.Epochs, epo2: mne.Epochs, lab: bool = False):
     """
     Plots sensors in 3D with x representation for bad sensors.
 
     Arguments:
         ax: Matplotlib axis created with projection='3d'
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         lab: option to plot channel names
-          False by default.
+            False by default.
 
     Returns:
         None: plot the sensors in 3D within the current axis.
     """
 
     # extract sensor infos and transform loc to fit with headmodel 
     loc1 = copy(np.array([ch['loc'][:3] for ch in epo1.info['chs']]))
@@ -1335,36 +1320,33 @@
                         C1: np.ndarray, C2: np.ndarray, threshold: str='auto',
                         steps: int=10):
     """
     Plots hyper-connectivity in 3D.
 
     Arguments:
         ax: Matplotlib axis created with projection='3d'
-        loc1: arrays of shape (n_sensors, 3)
-          3d coordinates of the sensors
-        loc2: arrays of shape (n_sensors, 3)
-          3d coordinates of the sensors
+        epo1: arrays of shape (n_sensors, 3)
+            Epochs object to get channel information
+        epo2: arrays of shape (n_sensors, 3)
+            Epochs object to get channel information
         C1: array, (len(loc1), len(loc1))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         C2: array, (len(loc1), len(loc2))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         threshold: float | str
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
-          Can also be "auto" to use a threshold automatically
-          calculated from your matrix as the maximum median 
-          by column + the maximum standard error by column.
-          Note that the automatic threshold is specific to a 
-          dyad and does not allow to compare different dyads.
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
+            Can also be "auto" to use a threshold automatically
+            calculated from your matrix as the maximum median 
+            by column + the maximum standard error by column.
+            Note that the automatic threshold is specific to a 
+            dyad and does not allow to compare different dyads.
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
-        weight: numpy.float
-          Connectivity weight to determine the thickness
-          of the link
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
 
     Returns:
         None: plot the links in 3D within the current axis.
           Plot hyper-connectivity in 3D.
     """
         
     # extract sensor infos and transform loc to fit with headmodel 
@@ -1590,33 +1572,32 @@
                   threshold: float=0.95, steps: int=10,
                   lab: bool = False):
     """
     Visualization of intra-brain connectivity in 3D.
 
     Arguments:
         epo1: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         epo2: mne.Epochs
-          Epochs object to get channel information
+            Epochs object to get channel information
         C1: array, (len(loc1), len(loc1))
-          matrix with the values of intra-brain connectivity
+            matrix with the values of intra-brain connectivity
         C2: array, (len(loc2), len(loc2))
         threshold: float
-          threshold for the inter-brain links;
-          only those above the set value will be plotted
+            threshold for the inter-brain links;
+            only those above the set value will be plotted
         steps: int
-          number of steps for the Bezier curves
-          if <3 equivalent to ploting straight lines
+            number of steps for the Bezier curves
+            if <3 equivalent to ploting straight lines
         lab: option to plot channel names
-          False by default.
-        
+            False by default.
 
     Returns:
         Plot headmodel with sensors and 
-              connectivity links in 3D.
+            connectivity links in 3D.
         ax: The new Axes object.
     """
 
     # defining head model and adding sensors
     vertices, faces = get_3d_heads_intra()
     fig = plt.figure()
     ax = fig.add_subplot(projection='3d')
@@ -1641,15 +1622,15 @@
              time: int, analysis: str,
              figsize: tuple = (30, 8), tmin: int = 0,
              x_units: Union[int, float] = 100):
     """
     Plots the results of the Cross wavelet analysis.
 
     Arguments:
-         sig1 : mne.Epochs
+        sig1 : mne.Epochs
             Signal (eg. EEG data) of first participant.
 
         sig2 : mne.Epochs
             Signal (eg. EEG data) of second participant.
 
         freqs: int | float | np.ndarray
             Frequency range of interest in Hz.
@@ -1659,27 +1640,24 @@
 
         analysis: str
             Sets type of analysis.
 
         figsize: tuple
             Figure size (default is (30, 8)).
 
-        xmin: int
-            Minimum x-value (default is 0).
-
         x_units: int | float
             distance between xticks on x-axis (time) (default is 100)
 
     Note:
         This function is not meant to be called indepedently,
         but is meant to be called when using plot_xwt_crosspower
         or plot_xwt_phase_angle.
 
     Returns:
-    Figure of xwt results.
+        Figure: The figure with the xwt results.
     """
 
     dt = 1/sfreq
     xmax = time/dt
     xmin = tmin * dt
     tick_units = xmax/x_units
     unit_conv = time/x_units
```

### Comparing `hypyp-0.4.0b8/pyproject.toml` & `hypyp-0.4.0b9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypyp"
-version = "0.4.0-beta.8"
+version = "0.4.0-beta.9"
 description = "The Hyperscanning Python Pipeline."
 readme = "README.md"
 authors = [
     "Anaël AYROLLLES <anael.ayrollles@pasteur.fr>",
     "Florence BRUN <florence.brun@pasteur.fr>",
     "Phoebe CHEN <phoebe.chen1117@gmail.com>",
     "Amir DJALOVSKI <amir.djv@gmail.com>",
@@ -37,26 +37,27 @@
 mne = "^1.3"
 h5io = "^0.1.7"
 mistune = ">=2.0.4"
 future = ">=0.18.3"
 certifi = ">=2022.12.07"
 
 [tool.poetry.group.dev.dependencies]
-mkdocs = "^1.1"
-mkdocstrings = "^0.10.3"
-mkdocs-material = "^5.1.1"
+mkdocs = ">=1.3.0"
+mkdocs-material = ">=8.2.15"
 pylint = "^2.4.4"
 black = "^19.10b0"
 markdown-include = "^0.5.1"
 jupyterlab = "^2.1.4"
 widgetsnbextension = "^3.5.1"
 ipywidgets = "^7.5.1"
 livereload = "^2.6.3"
 ipykernel = "^6.19.4"
 pytest = ">=7.2.0"
+mkdocstrings = ">=0.20.0"
+mkdocstrings-python-legacy = "^0.2.3"
 
 [tool.dephell.main]
 from = {format = "poetry", path = "pyproject.toml"}
 to = {format = "setuppy", path = "setup.py"}
 
 [build-system]
 requires = ["poetry_core>=1.0"]
```

### Comparing `hypyp-0.4.0b8/PKG-INFO` & `hypyp-0.4.0b9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypyp
-Version: 0.4.0b8
+Version: 0.4.0b9
 Summary: The Hyperscanning Python Pipeline.
 Home-page: https://github.com/ppsp-team/HyPyP
 License: BSD-3-Clause
 Keywords: hyperscanning,neuroscience,pipeline,statistics,visualization
 Author: Anaël AYROLLLES
 Author-email: anael.ayrollles@pasteur.fr
 Requires-Python: >=3.8,<4.0
@@ -34,15 +34,15 @@
 Project-URL: Repository, https://github.com/ppsp-team/HyPyP
 Description-Content-Type: text/markdown
 
 # HyPyP 🐍〰️🐍
 
 The **Hy**perscanning **Py**thon **P**ipeline
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/hypyp.svg)](https://pypi.org/project/HyPyP/) <a href="https://travis-ci.org/ppsp-team/HyPyP"><img src="https://travis-ci.org/ppsp-team/HyPyP.svg?branch=master"></a> [![license](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Mattermost](https://img.shields.io/static/v1?label=chat&message=Mattermost&color=Blue)](https://mattermost.brainhack.org/brainhack/channels/hypyp)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/hypyp.svg)](https://pypi.org/project/HyPyP/) <a href="https://travis-ci.org/ppsp-team/HyPyP"><img src="https://travis-ci.org/ppsp-team/HyPyP.svg?branch=master"></a> <a href="https://hypyp.readthedocs.io"><img src="https://readthedocs.org/projects/hypyp/badge/?version=latest"></a> [![license](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Mattermost](https://img.shields.io/discord/1065810348944408616?color=blue)](https://discord.gg/zYzjeGj7D6)
 
 ⚠️ This software is in beta and thus should be considered with caution. While we have done our best to test all the functionalities, there is no guarantee that the pipeline is entirely bug-free. 
 
 📖 See our [paper](https://academic.oup.com/scan/advance-article/doi/10.1093/scan/nsaa141/5919711) for more explanation and our plan for upcoming functionalities (aka Roadmap).
 
 🤝 If you want to help you can submit bugs and suggestions of enhancements in our Github [Issues section](https://github.com/ppsp-team/HyPyP/issues).
 
@@ -91,7 +91,8 @@
 Step 4: ```poetry install```
 
 Step 5: ```poetry shell```
 
 You can now use ```jupyter notebook``` or ```ipython```!
 
 ⚠️ If you need to install a new dependency (not recommended), you have to use `poetry add THE_NAME_OF_THE_LIBRARY` instead of your usual package manager.
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hypyp Version: 0.4.0b8 Summary: The Hyperscanning
+Metadata-Version: 2.1 Name: hypyp Version: 0.4.0b9 Summary: The Hyperscanning
 Python Pipeline. Home-page: https://github.com/ppsp-team/HyPyP License: BSD-3-
 Clause Keywords: hyperscanning,neuroscience,pipeline,statistics,visualization
 Author: AnaÃ«l AYROLLLES Author-email: anael.ayrollles@pasteur.fr Requires-
 Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -15,20 +15,20 @@
 (>=1.18.3,<2.0.0) Requires-Dist: pandas (>=1.0.3,<2.0.0) Requires-Dist: scipy
 (>=1.4.1,<2.0.0) Requires-Dist: statsmodels (>=0.13.2,<0.14.0) Requires-Dist:
 tqdm (>=4.46.0,<5.0.0) Project-URL: Documentation, https://hypyp.readthedocs.io
 Project-URL: Repository, https://github.com/ppsp-team/HyPyP Description-
 Content-Type: text/markdown # HyPyP ðã°ï¸ð The **Hy**perscanning
 **Py**thon **P**ipeline [![PyPI version shields.io](https://img.shields.io/
 pypi/v/hypyp.svg)](https://pypi.org/project/HyPyP/) [https://travis-ci.org/
-ppsp-team/HyPyP.svg?branch=master] [![license](https://img.shields.io/badge/
-License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-
-Clause) [![Mattermost](https://img.shields.io/static/
-v1?label=chat&message=Mattermost&color=Blue)](https://mattermost.brainhack.org/
-brainhack/channels/hypyp) â ï¸ This software is in beta and thus should be
-considered with caution. While we have done our best to test all the
+ppsp-team/HyPyP.svg?branch=master] [https://readthedocs.org/projects/hypyp/
+badge/?version=latest] [![license](https://img.shields.io/badge/License-
+BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [!
+[Mattermost](https://img.shields.io/discord/1065810348944408616?color=blue)]
+(https://discord.gg/zYzjeGj7D6) â ï¸ This software is in beta and thus should
+be considered with caution. While we have done our best to test all the
 functionalities, there is no guarantee that the pipeline is entirely bug-free.
 ð See our [paper](https://academic.oup.com/scan/advance-article/doi/10.1093/
 scan/nsaa141/5919711) for more explanation and our plan for upcoming
 functionalities (aka Roadmap). ð¤ If you want to help you can submit bugs and
 suggestions of enhancements in our Github [Issues section](https://github.com/
 ppsp-team/HyPyP/issues). ð¤ For the motivated contributors, you can even help
 directly in the developpment of HyPyP. You will need to install [Poetry](https:
```

