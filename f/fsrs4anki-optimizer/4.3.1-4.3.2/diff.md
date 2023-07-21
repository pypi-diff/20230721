# Comparing `tmp/fsrs4anki_optimizer-4.3.1.tar.gz` & `tmp/fsrs4anki_optimizer-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.3.1.tar", last modified: Fri Jul 21 08:36:27 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.3.2.tar", last modified: Fri Jul 21 12:34:53 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.3.1.tar` & `fsrs4anki_optimizer-4.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:36:27.556448 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51134 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 08:36:27.000000 fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:36:27.560448 fsrs4anki_optimizer-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 08:36:12.000000 fsrs4anki_optimizer-4.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51382 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/setup.py
```

### Comparing `fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-4.3.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -501,15 +501,15 @@
             delta_t = group['delta_t']
             recall = (group['y']['mean'] * group['y']['count'] + average_recall * 1) / (group['y']['count'] + 1)
             count = group['y']['count']
             total_count = sum(count)
             if total_count < 100:
                 tqdm.write(f'Not enough data for first rating {first_rating}. Expected at least 100, got {total_count}.')
                 continue
-            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (15 if total_count < 1000 else 365)))
+            params, _ = curve_fit(power_forgetting_curve, delta_t, recall, sigma=1/np.sqrt(count), bounds=((0.1), (30 if total_count < 1000 else 365)))
             stability = params[0]
             rating_stability[int(first_rating)] = stability
             rating_count[int(first_rating)] = total_count
             predict_recall = power_forgetting_curve(delta_t, *params)
             rmse = mean_squared_error(recall, predict_recall, sample_weight=count, squared=False)
 
             if verbose:
@@ -545,24 +545,26 @@
         params, covs = curve_fit(S0_rating_curve, list(rating_stability.keys()), list(rating_stability.values()), sigma=1/np.sqrt(list(rating_count.values())), method='dogbox', bounds=((-15, 0.03, -5), (15, 7, 30)))
         if verbose:
             tqdm.write(f'Weighted fit parameters: {params}')
             predict_stability = S0_rating_curve(np.array(list(rating_stability.keys())), *params)
             tqdm.write(f"Fit stability: {predict_stability}")
             tqdm.write(f'RMSE: {mean_squared_error(list(rating_stability.values()), predict_stability, sample_weight=list(rating_count.values()), squared=False):.4f}')
             plt.plot(list(rating_stability.keys()), list(rating_stability.values()), label='Exact')
-            plt.plot(list(rating_stability.keys()), predict_stability, label='Weighted fit')
+            plt.plot(np.linspace(1, 4), S0_rating_curve(np.linspace(1, 4), *params), label='Weighted fit')
+            scatter_size = np.array([x/sum(rating_count.values()) for x in rating_count.values()]) * 1000
+            plt.scatter(list(rating_stability.keys()), list(rating_stability.values()), scatter_size, label='Exact', alpha=0.5)
             plt.legend(loc='upper right', fancybox=True, shadow=False)
             plt.grid(True)
             plt.xlabel('First rating')
             plt.ylabel('Stability')
             plt.title('Stability for first rating')
             plt.show()
 
         for rating in (1, 2, 3, 4):
-            again_extrap = max(min(S0_rating_curve(1, *params), 15), 0.1)
+            again_extrap = max(min(S0_rating_curve(1, *params), 30), 0.1)
             # if there isn't enough data to calculate the value for "Again" exactly
             if 1 not in rating_stability:
                 # then check if there exists an exact value for "Hard"
                 if 2 in rating_stability:
                     # if it exists, then check whether the extrapolation breaks monotonicity
                     # Again > Hard is possible, but we should allow it only for exact values, otherwise we should assume monotonicity
                     if again_extrap > rating_stability[2]:
@@ -571,15 +573,15 @@
                     else:
                         # if it doesn't break monotonicity, then use the extrapolated value
                         rating_stability[1] = again_extrap
                 # if an exact value for "Hard" doesn't exist, then just use the extrapolation, there's nothing else we can do
                 else:
                     rating_stability[1] = again_extrap
             elif rating not in rating_stability:
-                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 15), 0.1)
+                rating_stability[rating] = max(min(S0_rating_curve(rating, *params), 30), 0.1)
 
         rating_stability = {k: round(v, 2) for k, v in sorted(rating_stability.items(), key=lambda item: item[0])}
         for rating, stability in rating_stability.items():
             self.init_w[rating-1] = stability
         tqdm.write(f"Pretrain finished!")
 
     def train(self, lr: float = 4e-2, n_epoch: int = 5, n_splits: int = 5, batch_size: int = 512, verbose: bool = True):
```

