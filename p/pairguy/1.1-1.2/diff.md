# Comparing `tmp/pairguy-1.1.tar.gz` & `tmp/pairguy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pairguy-1.1.tar", last modified: Fri Jun 23 03:15:03 2023, max compression
+gzip compressed data, was "pairguy-1.2.tar", last modified: Fri Jul 21 01:42:43 2023, max compression
```

## Comparing `pairguy-1.1.tar` & `pairguy-1.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 03:15:03.516968 pairguy-1.1/
--rw-r--r--   0 cmw        (501) staff       (20)      351 2023-06-23 03:15:03.516704 pairguy-1.1/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 pairguy-1.1/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 03:15:03.515762 pairguy-1.1/pairguy/
--rw-r--r--   0 cmw        (501) staff       (20)    26735 2023-06-23 03:08:14.000000 pairguy-1.1/pairguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16885 2023-06-09 02:59:56.000000 pairguy-1.1/pairguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    65970 2023-06-16 03:57:57.000000 pairguy-1.1/pairguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    38515 2023-06-15 23:55:43.000000 pairguy-1.1/pairguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 pairguy-1.1/pairguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-06-23 03:15:03.516509 pairguy-1.1/pairguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      351 2023-06-23 03:15:03.000000 pairguy-1.1/pairguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-06-23 03:15:03.000000 pairguy-1.1/pairguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-06-23 03:15:03.000000 pairguy-1.1/pairguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-06-23 03:15:03.000000 pairguy-1.1/pairguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-06-23 03:15:03.000000 pairguy-1.1/pairguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-06-23 03:15:03.517017 pairguy-1.1/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      830 2023-06-23 03:12:07.000000 pairguy-1.1/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-21 01:42:43.430554 pairguy-1.2/
+-rw-r--r--   0 cmw        (501) staff       (20)      351 2023-07-21 01:42:43.430326 pairguy-1.2/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 pairguy-1.2/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-21 01:42:43.428817 pairguy-1.2/pairguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    26742 2023-07-20 23:24:02.000000 pairguy-1.2/pairguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    17010 2023-07-20 23:24:02.000000 pairguy-1.2/pairguy/pairguy_Aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    71232 2023-07-21 01:25:59.000000 pairguy-1.2/pairguy/pairguy_Components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    32787 2023-07-21 01:34:12.000000 pairguy-1.2/pairguy/pairguy_EquityCurves.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-07-21 01:42:43.430047 pairguy-1.2/pairguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      351 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      283 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-07-21 01:42:43.000000 pairguy-1.2/pairguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-07-21 01:42:43.430626 pairguy-1.2/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      830 2023-07-21 01:42:07.000000 pairguy-1.2/setup.py
```

### Comparing `pairguy-1.1/pairguy/__init__.py` & `pairguy-1.2/pairguy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import zlib
 import requests
 from bs4 import BeautifulSoup
 import pandas as pd
 import polars as pl
 import numpy as np
 
-from .equity_curves import *
-from .signals import *
-from .aggregate import *
+from .pairguy_EquityCurves import *
+from .pairguy_Aggregate import *
 
 
 def multi_process(function, parameters, number_of_core=8):
     pool = mp.Pool(processes=number_of_core)
     pool.map(function, parameters)
     pool.close()
 
@@ -251,18 +250,18 @@
         subchart_settings = {
             'histogram_period': [1, 3, 5, 10, 20],
             'subchart_1': ['volume', 'line']
         }
 
     if mode == 'equity_curves':
         result_df = pd.read_csv('backtest_result.csv', index_col=0)
-        app = equity_curves.Plot(all_para_combination, result_df, subchart_settings, number_of_curves)
+        app = pairguy_EquityCurves.Plot(all_para_combination, result_df, subchart_settings, number_of_curves)
 
     if mode == 'aggregate':
-        app = aggregate.Aggregate(risk_free_rate)
+        app = pairguy_Aggregate.Aggregate(risk_free_rate)
 
     return app
```

### Comparing `pairguy-1.1/pairguy/aggregate.py` & `pairguy-1.2/pairguy/pairguy_Aggregate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
+import pandas as pd
+import time
+import pairguy
+
 from dash import Dash, dcc, html, Input, Output, State, ALL
 import dash_daq as daq
-from .components import *
-import time
+from .pairguy_Components import *
+import dash_bootstrap_components as dbc
+import dash_dangerously_set_inner_html
+
+
 
 class Aggregate:
 
     chart_bg = '#1f2c56'
     valid_colour = 'DeepSkyBlue'
     df_equity_curves = pd.DataFrame()
     df_ready = False
@@ -239,15 +246,15 @@
 
                 df_csv['date'] = pd.to_datetime(df_csv['date'], format='%Y-%m-%d')
                 df_csv = df_csv.set_index('date')
 
                 # print(df_csv)
 
                 if (intraday or summary):
-                    df = plotguy.resample_summary_to_daily(para_combination=para_combination[i],folder=folders[i])
+                    df = pairguy.resample_summary_to_daily(para_combination=para_combination[i],folder=folders[i])
                 else:
                     df = df_csv
 
                 if 'date' in df.columns:
                     df = df.set_index('date')
 
                 df_current = pd.DataFrame()
```

### Comparing `pairguy-1.1/pairguy/components.py` & `pairguy-1.2/pairguy/pairguy_Components.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import pandas as pd
 import numpy as np
 import datetime
 import math
-import json
 import ast
 import os
 
 from dash import dcc, html    ## pip install dash
 import dash_bootstrap_components as dbc
 import plotly.express as px
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
-# import plotguy
 import pairguy
-import dash_dangerously_set_inner_html   # for all Plot Class
 
 
 class Components:
-    chart_bg = '#173A2B'
+    chart_bg = '#004225'
 
     sort_method_dropdown = html.Div()
 
     filter_dropdown = html.Div(id='filter_dropdown',
                                children=dbc.Select(id='filter_name',
                                                    placeholder="Select Filter",
                                                    options=[
@@ -660,58 +657,126 @@
 
             fig_line.add_trace(go.Scatter(mode='lines', hovertemplate=hovertemplate,
                                           x=df_daily['date'], y=df_daily['equity_value'],
                                           line=dict(color=line_colour, width=1.5), name=''), )
         return fig_line
 
 
-    def prepare_df_chart(self, df):     # Chart Data for Chart 2
-        initial_value = df.iloc[0].equity_value
+    def prepare_df_chart2(self, df):     # Chart Data for Chart 2
+        def apply_cal_equity(row, pnl_column):
+            realized_pnl = df.at[row.name, f'realized_pnl_{pnl_column}']
+            if not (np.isnan(realized_pnl) or (realized_pnl == '')):
+                apply_cal_equity.previous_equity = apply_cal_equity.previous_equity + float(
+                    df.at[row.name, f'realized_pnl_{pnl_column}'])
+                return apply_cal_equity.previous_equity
+            else:
+                if row.name == 0:
+                    return apply_cal_equity.previous_equity
+                else:
+                    return apply_cal_equity.previous_equity + df.at[row.name, f'unrealized_pnl_{pnl_column}']
 
-        df_chart = df.copy()
-        df_chart['date'] = pd.to_datetime(df_chart['date'], format='%Y-%m-%d')
-        df_chart['bah'] = df['close'] * (initial_value / df_chart.iloc[0].close)
-
-        _open = []
-        _stop_loss = []
-        _close_logic = []
-        _profit_target = []
-
-        for i in range(len(list(df['action']))):
-            element = list(df['action'])[i]
-            if element == 'open':
-                _open.append(df_chart.iloc[i].bah)
-                _stop_loss.append(None)
-                _close_logic.append(None)
-                _profit_target.append(None)
-            elif element == 'stop_loss':
-                _open.append(None)
-                _stop_loss.append(df_chart.iloc[i].bah)
-                _close_logic.append(None)
-                _profit_target.append(None)
-            elif element == 'close_logic':
-                _open.append(None)
-                _stop_loss.append(None)
-                _close_logic.append(df_chart.iloc[i].bah)
-                _profit_target.append(None)
-            elif element == 'profit_target':
-                _open.append(None)
-                _stop_loss.append(None)
-                _close_logic.append(None)
-                _profit_target.append(df_chart.iloc[i].bah)
+        def apply_cal_pos(row):
+            if row.name == 0:
+                apply_cal_pos.status = False
+            elif row.trade_logic_positive == True:
+                apply_cal_pos.status = True
+            elif ((df.at[row.name - 1, 'action_0'] == 'close_logic') or
+                  (df.at[row.name - 1, 'action_0'] == 'profit_target')) and apply_cal_pos.status:
+                apply_cal_pos.status = False
+
+            return apply_cal_pos.status
+
+        def apply_cal_neg(row):
+            if row.name == 0:
+                apply_cal_neg.status = False
+            elif row.trade_logic_negative == True:
+                apply_cal_neg.status = True
+            elif ((df.at[row.name - 1, 'action_0'] == 'close_logic') or
+                  (df.at[row.name - 1, 'action_0'] == 'profit_target')) and apply_cal_neg.status:
+                apply_cal_neg.status = False
+
+            return apply_cal_neg.status
+
+        def apply_cal_equity_pn(row, pn):
+            realized_pnl = df.at[row.name, f'realized_pnl']
+            if df.at[row.name, pn] == True:
+                if not (np.isnan(realized_pnl) or (realized_pnl == '')):
+                    apply_cal_equity_pn.previous_equity = apply_cal_equity_pn.previous_equity + float(
+                        df.at[row.name, f'realized_pnl'])
+                    return apply_cal_equity_pn.previous_equity
+                else:
+                    if row.name == 0:
+                        return apply_cal_equity_pn.previous_equity
+                    else:
+                        return apply_cal_equity_pn.previous_equity + df.at[row.name, f'unrealized_pnl']
             else:
-                _open.append(None)
-                _stop_loss.append(None)
-                _close_logic.append(None)
-                _profit_target.append(None)
-
-        df_chart['open'] = _open
-        df_chart['stop_loss'] = _stop_loss
-        df_chart['close_logic'] = _close_logic
-        df_chart['profit_target'] = _profit_target
+                return apply_cal_equity_pn.previous_equity
+
+        df = df.copy()
+        df = df.reset_index(drop=True)
+        initial_equity = df.at[0, 'equity_value'] / 2
+
+        df['pos'] = False
+        df['neg'] = False
+
+        df['pos'] = df.apply(apply_cal_pos, axis=1)
+        df['neg'] = df.apply(apply_cal_neg, axis=1)
+
+        apply_cal_equity.previous_equity = initial_equity
+        df['equity_0'] = df.apply(apply_cal_equity, args=(0,), axis=1)
+        apply_cal_equity.previous_equity = initial_equity
+        df['equity_1'] = df.apply(apply_cal_equity, args=(1,), axis=1)
+
+        apply_cal_equity_pn.previous_equity = initial_equity
+        df['equity_pos'] = df.apply(apply_cal_equity_pn, args=('pos',), axis=1)
+        apply_cal_equity_pn.previous_equity = initial_equity
+        df['equity_neg'] = df.apply(apply_cal_equity_pn, args=('neg',), axis=1)
+
+        return df
+
+
+        # df_chart['bah'] = df['close'] * (initial_value / df_chart.iloc[0].close)
+        #
+        # _open = []
+        # _stop_loss = []
+        # _close_logic = []
+        # _profit_target = []
+        #
+        # for i in range(len(list(df['action']))):
+        #     element = list(df['action'])[i]
+        #     if element == 'open':
+        #         _open.append(df_chart.iloc[i].bah)
+        #         _stop_loss.append(None)
+        #         _close_logic.append(None)
+        #         _profit_target.append(None)
+        #     elif element == 'stop_loss':
+        #         _open.append(None)
+        #         _stop_loss.append(df_chart.iloc[i].bah)
+        #         _close_logic.append(None)
+        #         _profit_target.append(None)
+        #     elif element == 'close_logic':
+        #         _open.append(None)
+        #         _stop_loss.append(None)
+        #         _close_logic.append(df_chart.iloc[i].bah)
+        #         _profit_target.append(None)
+        #     elif element == 'profit_target':
+        #         _open.append(None)
+        #         _stop_loss.append(None)
+        #         _close_logic.append(None)
+        #         _profit_target.append(df_chart.iloc[i].bah)
+        #     else:
+        #         _open.append(None)
+        #         _stop_loss.append(None)
+        #         _close_logic.append(None)
+        #         _profit_target.append(None)
+        #
+        # df_chart['open'] = _open
+        # df_chart['stop_loss'] = _stop_loss
+        # df_chart['close_logic'] = _close_logic
+        # df_chart['profit_target'] = _profit_target
 
         return df_chart
 
     def generate_chart_2_summary(self, para_combination, line_colour):
         df_daily = pairguy.resample_summary_to_daily(para_combination=para_combination)
 
         title = ''
@@ -764,28 +829,76 @@
 
 
 
 
         pass
 
 
-    def generate_chart_2_full(self, para_combination, line_colour, settings):
+    def generate_chart_2_full(self, para_combination, line_colour, aggregate_boolean, settings):
         file_format = para_combination['file_format']
 
         save_path = pairguy.generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
 
         df_csv = df_backtest.copy()
-        df_chart = self.prepare_df_chart(df_csv)
+        df_chart = self.prepare_df_chart2(df_csv)
+
+        title = ''
+        para_dict = para_combination['para_dict']
+        for key in para_dict:
+            title = title + f'{key}:{para_combination[key]} '
+
+        fig_line = px.line()
+        fig_line.update_layout(title={'text': title, 'font': {'size': 12}})
+        fig_line.update_layout(plot_bgcolor=self.chart_bg, paper_bgcolor=self.chart_bg, height=500,
+                               margin=dict(l=85, r=25, t=60, b=0),
+                               font={"color": "white", 'size': 10.5}, yaxis={'title': 'Equity'},
+                               xaxis={'title': ''}
+                               )
+        fig_line.update_xaxes(showline=True, zeroline=False, linecolor='white', gridcolor=self.chart_bg)
+        fig_line.update_yaxes(showline=True, zeroline=False, linecolor='white', gridcolor=self.chart_bg)
+
+        fig_line.add_trace(go.Scatter(mode='lines',
+                                      x=df_chart['date'], y=df_chart['equity_value'],
+                                      line=dict(color=line_colour, width=1.5), name='Overall Equity'), )
+
+        if aggregate_boolean:
+            fig_line.add_trace(go.Scatter(mode='lines',
+                                          x=df_chart['date'], y=df_chart['equity_0'],
+                                          line=dict(color='SpringGreen', width=1.5), name=para_combination['pairs'][0]), )
+            fig_line.add_trace(go.Scatter(mode='lines',
+                                          x=df_chart['date'], y=df_chart['equity_1'],
+                                          line=dict(color='Cyan', width=1.5), name=para_combination['pairs'][1]), )
+
+        else:
+            fig_line.add_trace(go.Scatter(mode='lines',
+                                          x=df_chart['date'], y=df_chart['equity_pos'],
+                                          line=dict(color='SpringGreen', width=1.5), name='Positive'), )
+
+            fig_line.add_trace(go.Scatter(mode='lines',
+                                          x=df_chart['date'], y=df_chart['equity_neg'],
+                                          line=dict(color='Cyan', width=1.5), name='Negative'), )
+
+        return df_csv, fig_line
+
+
+
+
+
+        # return df_csv, df_chart
+
+
 
         df_signal = df_chart.copy()
+
+
         df_signal = df_signal.dropna(subset=['action'])  # for csv
         df_signal = df_signal.loc[df_signal['action'] != '']  # for parquet
         df_signal = df_signal.reset_index()
         signal_open_date = []
         signal_open_close = []
         signal_close_date = []
         signal_close_close = []
```

### Comparing `pairguy-1.1/pairguy/equity_curves.py` & `pairguy-1.2/pairguy/pairguy_EquityCurves.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from dash import Dash, dcc, html, Input, Output, State, ALL
-from .components import *
+import dash_daq as daq
+from .pairguy_Components import *
+import datetime
+import pandas as pd
+import numpy as np
+
+from dash import dcc, html    ## pip install dash
+import dash_bootstrap_components as dbc
+import dash_dangerously_set_inner_html
 
 import os
 import itertools
 
 class Plot:
     # Settings
-    chart_bg = '#173A2B'
+    chart_bg = '#004225'
+    valid_colour = 'DeepSkyBlue'
 
     # State
     graph_df = pd.DataFrame()
     sort_method_current = ''
     filter_list = []
     add_button_count = 0
     chart1_button_clicks = 0
     chart2_button_clicks = 0
-    chart3_button_clicks = 0
-    chart3_back_button_clicks = 0
+    breakdown_toggle_status = True
     save_clicks = 0
     line_selected = -1
     button_list = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
     chart_type = 1
     relayoutData = []
     init = True
     save_path = ''
     initial_capital = 0
     return_in_capital = 0
     mdd = 0
     sharpe = 0
-
     start_date_datetime = 0
     end_date_datetime = 0
 
     para_combination = {}
     save_path = 'save_path'
     net_profit_to_mdd = 0
     net_profit = 0
@@ -51,25 +58,19 @@
     def __new__(self, all_para_combination, result_df, settings, number_of_curves):
         # start_date, end_date and para_dict is the same for all combination, ie use the 1st one
         start_date = all_para_combination[0]['start_date']
         end_date = all_para_combination[0]['end_date']
         para_dict = all_para_combination[0]['para_dict']
         intraday = all_para_combination[0]['intraday']
         summary_mode = all_para_combination[0]['summary_mode']
-        freq = all_para_combination[0]['freq']
-        # risk_free_rate = all_para_combination[0]['risk_free_rate']
         self.initial_capital = all_para_combination[0]['sec_profile']['initial_capital']
 
-        # For chart3 initial date range
-        self.start_date_datetime = datetime.datetime.strptime(start_date, '%Y-%m-%d')
-        self.end_date_datetime = self.start_date_datetime + datetime.timedelta(days=10)
-
-
-
         chart_bg = self.chart_bg
+        valid_colour = self.valid_colour
+
 
         components = Components(number_of_curves)
 
         start_date_year = datetime.datetime.strptime(start_date, '%Y-%m-%d').year
         end_date_year = datetime.datetime.strptime(end_date, '%Y-%m-%d').year
         self.year_list = list(range(start_date_year, end_date_year + 1))
 
@@ -175,64 +176,48 @@
                                       dbc.Row([
                                           dbc.Col(html.Div(id='chart1_button', children='',
                                                            style={'text-align': 'left', 'cursor': 'pointer',
                                                                   'font-size': '14px'}), width=4),
                                           dbc.Col(html.Div(html.Img()), width=4),
                                           dbc.Col(html.Div(id='chart2_button', children=''), width=4),
                                       ], style={'margin': '0px 5px'}),
+
+                                      html.Div(id='breakdown_toggle_div',
+                                               children=html.Div([
+
+                                                   html.Div(html.Img(),style={'height': '10px', }),
+
+                                                   html.Div('Equity Breakdown', style={'height': '10px', 'margin-left': '38px'}),
+
+                                                   html.Div(html.Img(), style={'height': '20px', }),
+
+                                                   html.Div(html.Div('Trade Logic', style={}),
+                                                            style={'margin-left': '39px', 'vertical-align': 'top',
+                                                                   'position': 'relative', 'top': '0.08em',
+                                                                   'display': 'inline-block'}),
+
+                                                   html.Div(daq.BooleanSwitch(on=True, color=valid_colour,
+                                                                           id='breakdown_toggle',  style={'height': '5px', }),
+                                                            style={'margin-left': '10px', 'display': 'inline-block'}),
+
+                                                   html.Div(html.Div('Underlying', style={}),
+                                                            style={'margin-left': '15px', 'vertical-align': 'top',
+                                                                   'position': 'relative', 'top': '0.08em',
+                                                                   'display': 'inline-block'}),
+                                               ]),
+                                               style={'display': 'none'}),
+
                                       html.Div(id='chart_area',
                                                children=dcc.Graph(id='line_chart', figure=empty_line_chart)),
 
                                       html.Div(style={'height': '10px', }),
 
                                      ],style={'padding':'5px','border-radius':'5px','background-color':chart_bg}),
 
 
-                        html.Div(id='chart3_area',
-                                 children=[html.Div(html.Img(), style={'height': '10px'}),
-
-                                           dbc.Row([
-                                               dbc.Col(html.Div(id='chart3_back_button', children='< Back',
-                                                                style={'text-align': 'left', 'cursor': 'pointer',
-                                                                       'font-size': '14px'}), width=4),
-                                               dbc.Col(html.Div(html.Img()), width=4)
-
-                                           ], style={'margin': '0px 5px'}),
-                                           html.Div(id='chart3',
-                                                    children=dcc.Graph(id='chart3_chart', figure=empty_line_chart)),
-
-                                           html.Div(style={'height': '10px', }),
-
-                                           ],
-                                 style={'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg, 'display': 'none'}),
-
-                        html.Div(id='chart3_dashboard',
-                            children=[html.Div(style={'height': '5px', }),
-                                  html.Div(children=dbc.Row([
-                                                dbc.Col(width=1),
-                                                dbc.Col(children=html.Div([
-                                                    html.Div(style={'height': '0.5px',}),
-                                                    dcc.DatePickerRange(
-                                                        id='chart3_date',
-                                                        style={'margin-left':'15px'},
-                                                        month_format='MMM Do, YY',
-                                                        end_date_placeholder_text='MMM Do, YY',
-                                                        start_date=datetime.date(self.start_date_datetime.year, self.start_date_datetime.month, self.start_date_datetime.day),
-                                                        end_date=datetime.date(self.end_date_datetime.year, self.end_date_datetime.month, self.end_date_datetime.day),)
-                                                ]),width=6),
-                                                dbc.Col(children=html.Div(id='chart3_button',
-                                                                          children=html.Div([html.Div(style={'height': '11px'}),'Show Intra Day Candlestick Chart']),
-                                                                          style={'margin': '0px', 'width': '300px', 'backgroundColor': 'blue', 'padding': '0px',
-                                                                                    'border-radius': '2.5px', 'text-align': 'center', 'cursor': 'pointer',
-                                                                                    'font-size': '18px', 'height':'48px'}
-                                                                    ), width=3),
-                                            ], style={'width':'650px'})
-                                           ,style={'padding': '15px 5px', 'border-radius': '5px', 'background-color': chart_bg})
-                                  ], style={'display': 'none'}),
-
                         html.Div(style={'height': '5px', }),
 
                         html.Div(id='hist_area', children=html.Div(),
                                  style={'display': 'none'}),
 
                     ]), style={'padding':'0'}, width=8),
                 ])
@@ -246,193 +231,131 @@
             Output('filter', 'children'),
             Output('filter_dropdown_div', 'children'),
             Output('filter_input_div', 'children'),
             Output('add_button', 'style'),
             Output('filter_input', 'value'),
             Output('chart1_button', 'children'),
             Output('chart2_button', 'children'),
-            Output('hist_area', 'children'),
-            Output('hist_area', 'style'),
             Output('main_chart_area', 'style'),
-            Output('chart3_dashboard', 'style'),
-            Output('chart3_area', 'style'),
-            Output('chart3_date', 'start_date'),
-            Output('chart3_date', 'end_date'),
-            Output('chart3_chart', 'figure'),
+            Output('breakdown_toggle_div', 'style'),
+            # Output('hist_area', 'children'),
+            # Output('hist_area', 'style'),
             Input('sort_method', 'value'),
             Input({'type': 'para-checklist', 'index': ALL}, 'value'),
             State('filter_dropdown_div', 'children'),
             State('filter_input_div', 'children'),
             State('line_chart', 'figure'),
             State('filter', 'children'),
             Input('add_button', 'n_clicks'),
             Input('chart1_button', 'n_clicks'),
             Input('chart2_button', 'n_clicks'),
-            Input('chart3_button', 'n_clicks'),
-            Input('chart3_back_button', 'n_clicks'),
             State('add_button', 'style'),
             State('filter_name', 'value'),
             State('filter_input', 'value'),
-            State('hist_area', 'children'),
-            State('hist_area', 'style'),
             State('main_chart_area', 'style'),
-            State('chart3_dashboard', 'style'),
-            State('chart3_area', 'style'),
-            State('chart3_date', 'start_date'),
-            State('chart3_date', 'end_date'),
-            State('chart3_chart', 'figure'),
+            State('breakdown_toggle_div', 'style'),
+            Input('breakdown_toggle', 'on'),
+            # State('hist_area', 'children'),
+            # State('hist_area', 'style'),
             [Input('button_' + str(i), 'n_clicks') for i in range(10)],
         )
-        def display_output(sort_method,para_checklist,filter_dropdown_div,filter_input_div,fig_line,\
-                           filter_div,add_button_clicks, \
-                           chart1_button_clicks,chart2_button_clicks, chart3_button_clicks, chart3_back_button_clicks, \
-                           _add_button_style,filter_name,filter_input_value,\
-                           hist_area,hist_style,main_chart_area_style,chart3_dashboard_style, chart3_area_style, \
-                           chart3_start_str, chart3_end_str, chart3_chart, *vals):
-
-            print(para_checklist)
+        def display_output(sort_method,para_checklist,filter_dropdown_div,filter_input_div,fig_line,
+                           filter_div,add_button_clicks,
+                           chart1_button_clicks,chart2_button_clicks,
+                           _add_button_style,filter_name,filter_input_value, main_chart_area_style,
+                           breakdown_toggle_div,  aggregate_boolean,
+                           *vals):
 
             chart1_button_text = ''
             chart2_button_text = ''
 
             chart1_button_click = False
 
-            if chart3_button_clicks:
-                if chart3_button_clicks > self.chart3_button_clicks:
-                    self.chart3_button_clicks = chart3_button_clicks
-
-                    if (chart3_start_str and chart3_end_str):
-                        chart3_start = datetime.datetime.strptime(chart3_start_str, '%Y-%m-%d')
-                        chart3_end = datetime.datetime.strptime(chart3_end_str, '%Y-%m-%d')
-                        detla = chart3_end - chart3_start
-
-                        if (detla.days > 60) or (detla.days < 1):
-                            print('CandleStick Chart Limit: 1 to 60 Days')
-                        else:
-                            para_combination = self.para_combination
-                            hist_style = {'display': 'none'}
-                            file_format = para_combination['file_format']
-                            chart3_chart = components.generate_chart_3(para_combination, chart3_start, chart3_end, freq, file_format)
-
-                            main_chart_area_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg, 'display': 'none'}
-                            chart3_area_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg,}
-
-
-                    return fig_line, filter_div, filter_dropdown_div, filter_input_div, _add_button_style, \
-                           None, chart1_button_text, chart2_button_text, hist_area, hist_style, \
-                           main_chart_area_style, chart3_dashboard_style, chart3_area_style, \
-                           chart3_start_str, chart3_end_str, chart3_chart
-
-            if chart3_back_button_clicks:
-                if chart3_back_button_clicks > self.chart3_back_button_clicks:
-                    self.chart3_back_button_clicks = chart3_back_button_clicks
-                    chart1_button_text = '< Back'
-                    hist_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg}
-                    main_chart_area_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg,}
-                    chart3_area_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg,
-                                         'display': 'none'}
-
-
-                    return fig_line, filter_div, filter_dropdown_div, filter_input_div, _add_button_style, \
-                           None, chart1_button_text, chart2_button_text, hist_area, hist_style, \
-                           main_chart_area_style, chart3_dashboard_style, chart3_area_style, \
-                           chart3_start_str, chart3_end_str, chart3_chart
-
-
             if chart1_button_clicks:
                 if chart1_button_clicks > self.chart1_button_clicks:
                     chart1_button_click = True
                     self.chart1_button_clicks = chart1_button_clicks
                     self. chart_type = 1
                     hist_style = {'display': 'none'}
-                    chart3_dashboard_style = {'display': 'none'}
+                    breakdown_toggle_div = {'display': 'none'}
+                    self.breakdown_toggle_status = aggregate_boolean
 
-            if chart2_button_clicks:
-                if chart2_button_clicks > self.chart2_button_clicks:
-                    self.chart2_button_clicks = chart2_button_clicks
-                    if self.chart_type == 2:
-                        chart1_button_text = '< Back'
-                        return fig_line, filter_div, filter_dropdown_div, filter_input_div, _add_button_style, \
-                               None, chart1_button_text, chart2_button_text, hist_area, hist_style, \
-                               main_chart_area_style, chart3_dashboard_style, chart3_area_style, \
-                               chart3_start_str, chart3_end_str, chart3_chart
-                    else:
-                        if self.line_selected > -1:
-                            para_combination = self.para_combination
-                            line_colour = self.graph_df.iloc[self.line_selected].line_colour
+                print(aggregate_boolean, self.breakdown_toggle_status)
 
-                            if (intraday or summary_mode):
-                                df, fig_line = components.generate_chart_2_summary(para_combination, line_colour)
+            if chart2_button_clicks or (not (aggregate_boolean == self.breakdown_toggle_status)):
+                if (chart2_button_clicks > self.chart2_button_clicks) or (not (aggregate_boolean == self.breakdown_toggle_status)):
+                    self.chart2_button_clicks = chart2_button_clicks
+                    self.breakdown_toggle_status = aggregate_boolean
+                    if self.line_selected > -1:
+                        para_combination = self.para_combination
+                        line_colour = self.graph_df.iloc[self.line_selected].line_colour
+
+                        df, fig_line = components.generate_chart_2_full(para_combination, line_colour, aggregate_boolean, settings)
+
+                        # if (intraday or summary_mode):
+                        #     df, fig_line = components.generate_chart_2_summary(para_combination, line_colour)
+                        #
+                        # else:
+                        #     df, fig_line = components.generate_chart_2_full(para_combination, line_colour, settings)
 
-                            else:
-                                df, fig_line = components.generate_chart_2_full(para_combination, line_colour, settings)
+                        self.chart_type = 2
+                        chart1_button_text = '< Back'
 
-                            self.chart_type = 2
-                            chart1_button_text = '< Back'
 
 
-                            # For Chart 3 date range
-                            if intraday:
-                                chart3_dashboard_style = {}
-
-                                df_chart3 = df.loc[df['action'].isnull() == False].copy()
-                                self.start_date_datetime = df_chart3.iloc[0].date - datetime.timedelta(days=1)
-                                self.end_date_datetime = self.start_date_datetime + datetime.timedelta(days=10)
-
-                                chart3_start_str = datetime.date(self.start_date_datetime.year, self.start_date_datetime.month,
-                                              self.start_date_datetime.day)
-                                chart3_end_str = datetime.date(self.end_date_datetime.year, self.end_date_datetime.month,
-                                              self.end_date_datetime.day)
-
-
-                            # Histograms
-                            period = settings['histogram_period']
-                            # First column of the 5 charts
-                            title_list = [dbc.Col(width=1)]
-                            pct_list = [dbc.Col(html.Div('pct_change', style={'font-size': '12px', 'margin-top': '55px',
-                                                                              'margin-left': '45px',
-                                                                              'transform': 'rotate(-90deg)'}), width=1)]
-                            rise_list = [dbc.Col(html.Div('max_rise', style={'font-size': '12px', 'margin-top': '55px',
-                                                                              'margin-left': '45px',
-                                                                              'transform': 'rotate(-90deg)'}), width=1)]
-                            fall_list = [dbc.Col(html.Div('max_fall', style={'font-size': '12px', 'margin-top': '55px',
-                                                                              'margin-left': '45px',
-                                                                              'transform': 'rotate(-90deg)'}), width=1)]
-
-
-                            for p in period:
-                                title_list.append(dbc.Col(f'{p} Days',style={'font-size': '12px', 'text-align': 'center'},width=2))
-                                fig_pct, fig_rise, fig_fall = components.generate_histogram(df, p, 'backtest')
-                                pct_list.append( dbc.Col(dcc.Graph(figure=fig_pct,config={'displayModeBar': False})
-                                                         ,style={'padding':'0'},width=2))
-                                rise_list.append(dbc.Col(dcc.Graph(figure=fig_rise,config={'displayModeBar': False})
-                                                         ,style={'padding': '0'}, width=2))
-                                fall_list.append(dbc.Col(dcc.Graph(figure=fig_fall,config={'displayModeBar': False})
-                                                         ,style={'padding': '0'}, width=2))
-
-
-                            title_list = html.Div(dbc.Row(title_list))
-                            pct_list = html.Div(dbc.Row(pct_list))
-                            rise_list = html.Div(dbc.Row(rise_list))
-                            fall_list = html.Div(dbc.Row(fall_list))
-
-                            hist_area = [html.Div(style={'height': '5px', }),
-                                         title_list, pct_list, rise_list, fall_list,
-                                         html.Div(style={'height': '5px', })]
-
-                            hist_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg}
-
-                            return fig_line, filter_div, filter_dropdown_div, filter_input_div, _add_button_style,\
-                                   None, chart1_button_text, chart2_button_text, hist_area, hist_style, \
-                                   main_chart_area_style, chart3_dashboard_style, chart3_area_style, \
-                                   chart3_start_str, chart3_end_str, chart3_chart
+                        #
+                        # # Histograms
+                        # period = settings['histogram_period']
+                        # # First column of the 5 charts
+                        # title_list = [dbc.Col(width=1)]
+                        # pct_list = [dbc.Col(html.Div('pct_change', style={'font-size': '12px', 'margin-top': '55px',
+                        #                                                   'margin-left': '45px',
+                        #                                                   'transform': 'rotate(-90deg)'}), width=1)]
+                        # rise_list = [dbc.Col(html.Div('max_rise', style={'font-size': '12px', 'margin-top': '55px',
+                        #                                                   'margin-left': '45px',
+                        #                                                   'transform': 'rotate(-90deg)'}), width=1)]
+                        # fall_list = [dbc.Col(html.Div('max_fall', style={'font-size': '12px', 'margin-top': '55px',
+                        #                                                   'margin-left': '45px',
+                        #                                                   'transform': 'rotate(-90deg)'}), width=1)]
+                        #
+                        #
+                        # for p in period:
+                        #     title_list.append(dbc.Col(f'{p} Days',style={'font-size': '12px', 'text-align': 'center'},width=2))
+                        #     fig_pct, fig_rise, fig_fall = components.generate_histogram(df, p, 'backtest')
+                        #     pct_list.append( dbc.Col(dcc.Graph(figure=fig_pct,config={'displayModeBar': False})
+                        #                              ,style={'padding':'0'},width=2))
+                        #     rise_list.append(dbc.Col(dcc.Graph(figure=fig_rise,config={'displayModeBar': False})
+                        #                              ,style={'padding': '0'}, width=2))
+                        #     fall_list.append(dbc.Col(dcc.Graph(figure=fig_fall,config={'displayModeBar': False})
+                        #                              ,style={'padding': '0'}, width=2))
+                        #
+                        #
+                        # title_list = html.Div(dbc.Row(title_list))
+                        # pct_list = html.Div(dbc.Row(pct_list))
+                        # rise_list = html.Div(dbc.Row(rise_list))
+                        # fall_list = html.Div(dbc.Row(fall_list))
+                        #
+                        # hist_area = [html.Div(style={'height': '5px', }),
+                        #              title_list, pct_list, rise_list, fall_list,
+                        #              html.Div(style={'height': '5px', })]
+                        #
+                        # hist_style = {'padding': '5px', 'border-radius': '5px', 'background-color': chart_bg}
+
+                        breakdown_toggle_div = {'margin-left': '10px', 'display': 'inline-block'}
+
+                        return fig_line, filter_div, filter_dropdown_div, filter_input_div, _add_button_style,\
+                               None, chart1_button_text, chart2_button_text, main_chart_area_style, \
+                               breakdown_toggle_div
+                        #       hist_area, hist_style, \
+                               # main_chart_area_style, # chart3_dashboard_style,  chart3_area_style, \
+                               # chart3_start_str, chart3_end_str, chart3_chart
 
 
-                        else:
-                            pass    # No Line Selected
+                    else:
+                        pass    # No Line Selected
 
 
             ## Initialize After Refresh
             if not self.init:
                 if not add_button_clicks:
                     if not chart1_button_click:
                         self.sort_method_current = sort_method
@@ -442,14 +365,16 @@
                         self.chart3_button_clicks = 0
                         self.chart3_back_button_clicks = 0
                         self.save_clicks = 0
                         self.chart_type = 1
                         self.line_selected = -1
                         hist_area = []
                         hist_style = {'display': 'none'}
+                        breakdown_toggle_div = {'display': 'none'}
+                        self.breakdown_toggle_status = aggregate_boolean
                         self.init = True
                         filter_dropdown_div = filter_dropdown
                         filter_input_div = filter_input
 
 
             ## Add Button Pressed
             if add_button_clicks:
@@ -523,18 +448,14 @@
                         if key == 'pairs':   # replace code by pairs
                             pairs = list(itertools.combinations(para_checklist[i], 2))
                             pairs = [tuple(sorted(pair)) for pair in pairs]  # sort the order of each pair
                             elements = pairs
                         else:
                             elements = para_checklist[i]
 
-
-                        print(key, len(elements) ,elements)
-
-
                         for element in elements: # -1 because code / para_dict index
 
                             if key == 'pairs':
                                 element = str(element)
 
                             if element == 'True':element = True
                             elif element == 'False':element = False
@@ -551,32 +472,29 @@
 
                     df_checked = current_df.loc[pd.DataFrame(and_list, columns=['check'])['check']].reset_index(
                         drop=True).copy()
                 else:
 
                     df_checked = current_df.copy()
 
-                print('df checked', len(df_checked))
-
                 # Sort
                 graph_df = components.sort_method_df(sort_method, df_checked, number_of_curves)
                 self.graph_df = graph_df
 
                 fig_line = components.generate_chart_1(graph_df, all_para_combination, intraday, summary_mode)
 
                 # Disable Chart 2
                 chart2_button_text = 'Strategy Analysis >'
                 self.chart_type = 1
                 hist_style = {'display': 'none'}
 
 
             return fig_line, filter_div, filter_dropdown_div,filter_input_div,_add_button_style, \
-                   None, chart1_button_text, chart2_button_text, hist_area, hist_style, \
-                   main_chart_area_style, chart3_dashboard_style, chart3_area_style, \
-                   chart3_start_str, chart3_end_str, chart3_chart
+                   None, chart1_button_text, chart2_button_text, main_chart_area_style, \
+                   breakdown_toggle_div
 
 
 
         # Click on Chart 1 line
         @app.callback(
             Output(component_id='performance_matrix', component_property='children'),
             Output('chart2_button', 'style'),
```

### Comparing `pairguy-1.1/setup.py` & `pairguy-1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pairguy",
-    version="1.1",
+    version="1.2",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
-    description="Plotguy",
+    description="Pairguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas==1.5.3',  
         'numpy>=1.24.1',  
         'hkfdb>=2.2', 
         'pyarrow',
```

