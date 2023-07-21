# Comparing `tmp/cfr-2023.6.30.tar.gz` & `tmp/cfr-2023.7.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-2023.6.30.tar", last modified: Fri Jun 30 11:57:53 2023, max compression
+gzip compressed data, was "cfr-2023.7.21.tar", last modified: Fri Jul 21 21:06:39 2023, max compression
```

## Comparing `cfr-2023.6.30.tar` & `cfr-2023.7.21.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.936493 cfr-2023.6.30/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.6.30/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-06-30 11:57:53.936313 cfr-2023.6.30/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1421 2023-06-28 18:00:43.000000 cfr-2023.6.30/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.925572 cfr-2023.6.30/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.6.30/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.932745 cfr-2023.6.30/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.6.30/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-2023.6.30/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.935807 cfr-2023.6.30/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.6.30/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.6.30/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.6.30/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.6.30/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    67397 2023-06-30 11:55:02.000000 cfr-2023.6.30/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-2023.6.30/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    57520 2023-06-29 20:52:53.000000 cfr-2023.6.30/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.6.30/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-06-26 04:41:16.000000 cfr-2023.6.30/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26818 2023-06-26 23:02:19.000000 cfr-2023.6.30/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    58412 2023-06-30 11:55:02.000000 cfr-2023.6.30/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-30 11:57:53.935003 cfr-2023.6.30/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.6.30/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-30 11:57:53.000000 cfr-2023.6.30/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-30 11:57:53.936564 cfr-2023.6.30/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-06-30 11:57:28.000000 cfr-2023.6.30/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.942666 cfr-2023.7.21/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-2023.7.21/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-07-21 21:06:39.942480 cfr-2023.7.21/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1421 2023-06-28 18:00:43.000000 cfr-2023.7.21/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.933181 cfr-2023.7.21/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5134 2023-06-22 22:28:33.000000 cfr-2023.7.21/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.938993 cfr-2023.7.21/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-2023.7.21/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-2023.7.21/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.942141 cfr-2023.7.21/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-2023.7.21/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-2023.7.21/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-2023.7.21/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-2023.7.21/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    67751 2023-07-10 01:52:31.000000 cfr-2023.7.21/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-2023.7.21/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    57520 2023-06-29 20:52:53.000000 cfr-2023.7.21/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     4551 2023-06-26 04:44:01.000000 cfr-2023.7.21/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-07-21 20:46:49.000000 cfr-2023.7.21/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    25261 2023-07-10 00:33:58.000000 cfr-2023.7.21/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    60578 2023-07-21 20:57:56.000000 cfr-2023.7.21/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-21 21:06:39.941239 cfr-2023.7.21/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1988 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-2023.7.21/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      201 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-07-21 21:06:39.000000 cfr-2023.7.21/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-07-21 21:06:39.942724 cfr-2023.7.21/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1404 2023-07-21 18:01:48.000000 cfr-2023.7.21/setup.py
```

### Comparing `cfr-2023.6.30/LICENSE` & `cfr-2023.7.21/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/PKG-INFO` & `cfr-2023.7.21/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2023.6.30
+Version: 2023.7.21
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2023.6.30/README.md` & `cfr-2023.7.21/README.md`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/bin/cfr` & `cfr-2023.7.21/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/__init__.py` & `cfr-2023.7.21/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/climate.py` & `cfr-2023.7.21/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/da/enkf.py` & `cfr-2023.7.21/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/gcm.py` & `cfr-2023.7.21/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/ml.py` & `cfr-2023.7.21/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/proxy.py` & `cfr-2023.7.21/cfr/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -606,16 +606,16 @@
             ax['map'].scatter(
                 self.lon, self.lat, marker=visual.STYLE.markers_dict[self.ptype],
                 s=ms, c=kwargs['color'], edgecolor=edge_clr, transform=transform,
             )
 
         return fig, ax
 
-    def dashboard(self, figsize=[10, 8], ms=200, stock_img=True, edge_clr='w',
-        wspace=0.1, hspace=0.3, spec_method='wwz', pseudo_clr=None, **kwargs):
+    def dashboard(self, figsize=[10, 8], ms=200, stock_img=True, edge_clr='w', self_lb='real', pseudo_lb='pseudo',
+        wspace=0.1, hspace=0.3, spec_method='wwz', spec_settings=None, pseudo_clr=None, **kwargs):
         ''' Plot a dashboard of the proxy/pseudoproxy.
         '''
         if not hasattr(self, 'pseudo'):
             raise ValueError('Need to get the pseudoproxy data.')
 
         if 'color' not in kwargs and 'c' not in kwargs:
             kwargs['color'] = visual.STYLE.colors_dict[self.ptype]
@@ -625,26 +625,26 @@
         gs = gridspec.GridSpec(2, 3)
         gs.update(wspace=wspace, hspace=hspace)
         ax = {}
 
         # plot proxy/pseudoproxy timeseries
         ax['ts'] = plt.subplot(gs[0, :2])
 
-        _kwargs = {'label': 'real', 'zorder': 3, 'alpha': 0.7}
+        _kwargs = {'label': self_lb, 'zorder': 3, 'alpha': 0.7}
         _kwargs.update(kwargs)
         ax['ts'].plot(self.time, self.value, **_kwargs)
 
         time_lb = visual.make_lb(self.time_name, self.time_unit)
         value_lb = visual.make_lb(self.value_name, self.value_unit)
 
         ax['ts'].set_ylabel(value_lb)
         ax['ts'].set_xlabel(time_lb)
         ax['ts'].plot(
             self.pseudo.time, self.pseudo.value,
-            color=pseudo_clr, label='pseudo')
+            color=pseudo_clr, label=pseudo_lb)
         ax['ts'].legend(loc='upper left', ncol=2)
         title = f'{self.pid} ({self.ptype})'
         if self.seasonality is not None:
             title += f'\nSeasonality: {self.seasonality}'
         ax['ts'].set_title(title)
 
         # plot probability density
@@ -688,19 +688,19 @@
         )
         ax['map'].set_title(f'lat: {self.lat:.2f}, lon: {self.lon:.2f}')
 
         # plot PSD
         ax['psd'] = plt.subplot(gs[1, :2])
         ts, psd = {}, {}
         ts['real'] = pyleo.Series(time=self.time, value=self.value)
-        psd['real'] = ts['real'].spectral(method=spec_method)
+        psd['real'] = ts['real'].spectral(method=spec_method, settings=spec_settings)
         psd['real'].plot(ax=ax['psd'], **_kwargs)
 
         ts['pseudo'] = pyleo.Series(time=self.pseudo.time, value=self.pseudo.value)
-        psd['pseudo'] = ts['pseudo'].slice([self.time.min(), self.time.max()]).spectral(method=spec_method)
+        psd['pseudo'] = ts['pseudo'].slice([self.time.min(), self.time.max()]).spectral(method=spec_method, settings=spec_settings)
         psd['pseudo'].plot(ax=ax['psd'], color=pseudo_clr, label='pseudo')
 
         ax['psd'].legend_ = None
         ax['psd'].text(
             x=0.95, y=0.97, s=f'Timespan: {int(self.time.min())}-{int(self.time.max())}',
             horizontalalignment='right',
             verticalalignment='top',
@@ -1313,15 +1313,22 @@
 
 
     def plotly(self, **kwargs):
         '''Plot the database on an interactive map utilizing Plotly
         '''
 
         df = self.to_df()
-        fig = visual.plotly_proxies(df)
+        fig = visual.plotly_proxies(df,**kwargs)
+        return fig
+    
+    def plotly_count(self,**kwargs):
+        ''' Plot the database number-counting on an interactive map utilizing Plotly
+        '''
+        df = self.to_df()
+        fig = visual.plotly_proxies_count(df,**kwargs)
         return fig
 
 
 
     def make_composite(self, obs=None, obs_nc_path=None, vn='tas', lat_name=None, lon_name=None, bin_width=10, n_bootstraps=1000, qs=(0.025, 0.975), stat_func=np.nanmean, anom_period=[1951, 1980]):
         ''' Make composites of the records in the proxy database.'''
         if obs is None and obs_nc_path is not None:
```

### Comparing `cfr-2023.6.30/cfr/psm.py` & `cfr-2023.7.21/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/reconjob.py` & `cfr-2023.7.21/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/reconres.py` & `cfr-2023.7.21/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/ts.py` & `cfr-2023.7.21/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-2023.6.30/cfr/utils.py` & `cfr-2023.7.21/cfr/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,62 +40,14 @@
         bin_width*(np.min(ts)//bin_width),
         bin_width*(np.max(ts)//bin_width+2),
         step=bin_width,
     )
 
     return bin_vector
     
-
-def smooth_ts(ts, ys, bin_vector=None, bin_width=10):
-    if bin_vector is None:
-        bin_vector = make_bin_vector(ts, bin_width=bin_width)
-
-    ts_bin = (bin_vector[1:] + bin_vector[:-1])/2
-    n_bin = np.size(ts_bin)
-    ys_bin = np.zeros(n_bin)
-
-    for i in range(n_bin):
-        t_start = bin_vector[i]
-        t_end = bin_vector[i+1]
-        t_range = (ts >= t_start) & (ts < t_end)
-        if np.sum(t_range*1) == 1:
-            ys_bin[i] = ys[t_range]
-        else:
-            ys_bin[i] = np.average(ys[t_range], axis=0)
-
-    return ts_bin, ys_bin, bin_vector
-
-def bin_ts(ts, ys, bin_vector=None, bin_width=10, resolution=1, smoothed=False):
-    if not smoothed:
-        ts_smooth, ys_smooth, bin_vector = smooth_ts(ts, ys, bin_vector=bin_vector, bin_width=bin_width)
-    else:
-        ts_smooth, ys_smooth = ts, ys
-
-    bin_vector_finer = np.arange(np.min(bin_vector), np.max(bin_vector)+1, step=resolution)
-    bin_value = np.zeros(bin_vector_finer.size)
-
-    n_bin = np.size(ts_smooth)
-    for i in range(n_bin):
-        t_start = bin_vector[i]
-        t_end = bin_vector[i+1]
-        t_range = (bin_vector_finer >= t_start) & (bin_vector_finer <= t_end)
-        bin_value[t_range] = ys_smooth[i]
-
-    return bin_vector_finer, bin_value
-
-def bootstrap(samples, n_bootstraps=1000, stat_func=np.nanmean):
-
-    n_samples = np.shape(samples)[0]
-    stats = np.zeros(n_bootstraps)
-    for i in range(n_bootstraps):
-        rand_ind = np.random.randint(n_samples, size=n_samples)
-        stats[i] = stat_func(samples[rand_ind])
-
-    return stats
-
 def smooth_ts(ts, ys, bin_vector=None, bin_width=10):
     if bin_vector is None:
         bin_vector = np.arange(
             bin_width*(np.min(ts)//bin_width),
             bin_width*(np.max(ts)//bin_width+2),
             step=bin_width)
```

### Comparing `cfr-2023.6.30/cfr/visual.py` & `cfr-2023.7.21/cfr/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     label_legend = ax.legend(handles=[line],loc=loc,handlelength=0,handleheight=0,handletextpad=0,borderaxespad=0,borderpad=borderpad,frameon=False,**kwargs)
     label_legend.remove()
     ax.add_artist(label_legend)
     line.remove()
 
 def plot_field_map(field_var, lat, lon, levels=50, add_cyclic_point=True,
                    title=None, title_size=20, title_weight='normal', figsize=[10, 8],
-                   plot_proxydb=False, proxydb=None, proxydb_lgd_kws=None,
+                   plot_proxydb=False, proxydb=None, plot_proxydb_lgd=False, proxydb_lgd_kws=None,
                    proxy_marker=None, proxy_color=None,
                    site_lats=None, site_lons=None, site_marker='o',
                    site_markersize=50, site_color=sns.xkcd_rgb['amber'],
                    projection='Robinson', transform=ccrs.PlateCarree(),
                    proj_args=None, latlon_range=None, central_longitude=180,
                    lon_ticks=[60, 120, 180, 240, 300], lat_ticks=[-90, -45, 0, 45, 90],
                    land_color=sns.xkcd_rgb['light grey'], ocean_color=sns.xkcd_rgb['light grey'],
@@ -481,18 +481,19 @@
             s_plots.append(
                 ax.scatter(
                     site_lons[ptype], site_lats[ptype], marker=marker,
                     c=color, edgecolor='k', s=site_markersize, transform=ccrs.PlateCarree()
                 )
             )
 
-        ax.legend(
-            s_plots, ptype_labels,
-            **proxydb_lgd_kws,
-        )
+        if plot_proxydb_lgd:
+            ax.legend(
+                s_plots, ptype_labels,
+                **proxydb_lgd_kws,
+            )
         
 
     return fig, ax
 
 def plot_proxies(df, year=np.arange(2001), lon_col='lon', lat_col='lat', type_col='type', time_col='time',
                  title=None, title_weight='normal', markers_dict=None, colors_dict=None,
                  plot_timespan=None,  plot_xticks=[850, 1000, 1200, 1400, 1600, 1800, 2000],
@@ -613,22 +614,58 @@
             setlabel(ax['map'], '(a)', prop=enumerate_prop, bbox_to_anchor=enumerate_anchor_map)
             setlabel(ax['count'], '(b)', prop=enumerate_prop, bbox_to_anchor=enumerate_anchor_count)
 
     if not return_gs:
         return fig, ax
     else:
         return fig, ax, gs
+    
+def count_time(df,lgd_ncol=None, type_col="ptype", year=np.arange(2001),time_col='time'):
+    df_count = {}
+    type_set = df[type_col].unique()
+    if lgd_ncol is None:
+        lgd_ncol = len(type_set) // 20 + 1
+
+    for ptype in type_set[::-1]:
+        df_count[ptype] = pd.DataFrame(index=year)
+
+    for index, row in df.iterrows():
+        ptype = row[type_col]
+        time = np.array(row[time_col]).astype(np.int32)
+        time = time[~np.isnan(time)]
+        time = time[time < np.max(year) + 1]
+        time = np.sort(np.unique(time))
+        ts = pd.Series(index=time, data=1, name=row['pid'])
+        df_count[ptype] = pd.concat([df_count[ptype], ts], axis=1)
+
+    proxy_count_all = []
+    color_discrete_sequence=[]
+    for ptype in list(df_count.keys()):
+        ptype_df_sum = df_count[ptype].sum(axis=1)
+        ptype_df = pd.DataFrame(columns=["ptype", 'time','num'])
+        ptype_df.loc[:,'time'] = ptype_df_sum.index
+        ptype_df.loc[:,'num'] = ptype_df_sum
+        ptype_df['ptype'] = ptype
+        proxy_count_all.append(ptype_df)
+        color_discrete_sequence.append(STYLE.colors_dict[ptype]) # get color
+
+    proxy_count_all = pd.concat(proxy_count_all)
+    
+    return proxy_count_all,color_discrete_sequence
 
 def plotly_proxies(df):
+    """ 
+    Visualize proxies.
+    Args:
+        df (pandas.DataFrame): proxy database in `pandas.DataFrame`.
+    """
     import plotly.graph_objects as go
-    # from .visual import STYLE
-
-    # df = self.to_df()
     fig = go.Figure()
     ptype_ls = df['ptype'].unique() 
+
     for ptype in ptype_ls:  # draw every ptype
         dfu = df.loc[df['ptype'] == ptype]
         fig.add_trace(
         go.Scattergeo(
             lon=dfu.lon,
             lat=dfu.lat,
             text=ptype,
@@ -638,29 +675,57 @@
             marker_size=10,
             hovertext=dfu['pid'],
             name=f'{ptype} (n={len(dfu)})',
             hoverinfo='lon+lat',
             hovertemplate= \
             "<br>pid: %{hovertext}</br>ptype: %{data.text}<br>lon: %{lon}</br>lat: %{lat}<extra></extra>",
         ))
+
     fig.update_geos(projection_type="natural earth",
                 center_lon=180,
                 lonaxis_range=[0, 360],
                 lataxis_range=[-90, 90],
                 showocean=True,
                 showland=True,
                 oceancolor="#70A0C1",
                 landcolor="#CBCBBA")
+
     fig.update_layout(
         margin=dict(l=35, r=35, t=35, b=35),
         legend_x=1,
         width=1000,
-        height=450,
+        height=450
     )
+
     fig.layout.dragmode = False
+        
+    return fig
+
+def plotly_proxies_count(pdb_df, xaxis_range=[1, 2000]):
+    import plotly.express as px
+    pdb_count, colors = count_time(pdb_df)
+
+    fig = px.area(pdb_count,
+                  x="time",
+                  y="num",
+                  color="ptype",
+                  color_discrete_sequence=colors)
+
+    fig.update_layout(xaxis_range=xaxis_range,
+                      margin=dict(l=45, r=35, t=35, b=45),
+                      width=900,
+                      height=450,
+                      font={
+                          'family': 'Arial',
+                          'size': 15,
+                      },
+                      legend_title="Proxy Type",
+                      xaxis_title="Year (AD)",
+                      yaxis_title="Number of Proxies")
+
     return fig
 
 
 def plot_proxy_age_map(df, lon_col='lon', lat_col='lat', type_col='type', time_col='time',
                        title=None, title_weight='normal', font_scale=1.5,
                        figsize=[12, 10], projection=ccrs.Robinson, central_longitude=0, markersize=150,
                        plot_cbar=True, marker_color=None, transform=ccrs.PlateCarree(), p=STYLE,
```

### Comparing `cfr-2023.6.30/cfr.egg-info/PKG-INFO` & `cfr-2023.7.21/cfr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 2023.6.30
+Version: 2023.7.21
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-2023.6.30/setup.py` & `cfr-2023.7.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='2023.6.30',
+    version='2023.7.21',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
```

