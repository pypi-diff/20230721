# Comparing `tmp/singlefactortest-1.0-py3-none-any.whl.zip` & `tmp/singlefactortest-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 11563 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    66976 b- defN 23-Jul-17 06:24 singlefactortest.py
--rw-rw-rw-  2.0 fat      741 b- defN 23-Jul-19 02:23 singlefactortest-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-19 02:23 singlefactortest-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-19 02:23 singlefactortest-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      402 b- defN 23-Jul-19 02:23 singlefactortest-1.0.dist-info/RECORD
-5 files, 68228 bytes uncompressed, 10811 bytes compressed:  84.2%
+Zip file size: 12075 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    68437 b- defN 23-Jul-20 09:46 singlefactortest.py
+-rw-rw-rw-  2.0 fat      756 b- defN 23-Jul-20 10:04 singlefactortest-1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 10:04 singlefactortest-1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-20 10:04 singlefactortest-1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      402 b- defN 23-Jul-20 10:04 singlefactortest-1.1.dist-info/RECORD
+5 files, 69704 bytes uncompressed, 11323 bytes compressed:  83.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: singlefactortest.py
 Comment: 
 
-Filename: singlefactortest-1.0.dist-info/METADATA
+Filename: singlefactortest-1.1.dist-info/METADATA
 Comment: 
 
-Filename: singlefactortest-1.0.dist-info/WHEEL
+Filename: singlefactortest-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: singlefactortest-1.0.dist-info/top_level.txt
+Filename: singlefactortest-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: singlefactortest-1.0.dist-info/RECORD
+Filename: singlefactortest-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## singlefactortest.py

```diff
@@ -1,22 +1,17 @@
 def backtest(df_factor,df_close):
     import pandas as pd 
     import numpy as np
     import statsmodels.api as sm
     import matplotlib.pyplot as plt
-    import math
     import scipy.stats as st
     import seaborn as sns
     from scipy.stats import pearsonr
-    import matplotlib.dates as mdate
-    from matplotlib.pyplot import rcParams 
     import matplotlib.ticker as ticker
     import warnings
-    from pandas import read_parquet
-    import sys
     import baostock as bs
     warnings.filterwarnings("ignore")
     plt.rcParams['font.sans-serif'] = ['SimHei']  # 用来正常显示中文标签
     plt.rcParams['axes.unicode_minus'] = False  # 用来正常显示负号
     
     def process_bar(percent, start_str='', end_str='', total_length=0):
         bar = ''.join(["\033[31m%s\033[0m"%'   '] * int(percent * total_length)) + ''
@@ -146,17 +141,17 @@
         def factor_scater(self,x,y,z):
             sns.set(palette="muted", color_codes=True)
             sns.set(font='SimHei', font_scale=0.8)
             if x==0 and y==0:
                 for i in range(0,len(self.portfolio)):
                     fig, ax = plt.subplots(figsize=(20,15))
                     if z=='1':
-                        ax.plot(self.factor.index, self.factor[self.portfolio[i]], 'o', label=portfolio[i]+"的因子值散点图")
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.factor[self.portfolio[i]], 'o', label=portfolio[i]+"的因子值散点图")
                     elif z=='2':
-                        ax.plot(self.factor.index, self.factor[self.portfolio[i]], label=portfolio[i]+"的因子值折线图")
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.factor[self.portfolio[i]], label=portfolio[i]+"的因子值折线图")
                     ax.legend(loc='best')
                     ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("时间",fontsize=16)
                     plt.ylabel("因子值",fontsize=16)
                     self.set_picture()
                     if z=='1':
                         plt.title(Chinese_name[i]+'的散点图',fontdict={'size': 20})
@@ -168,34 +163,34 @@
                 sub_portfolio=[]
                 for i in range(0,x):
                     s=input('请输入第'+str(i+1)+'个标的的名称: ')
                     sub_portfolio.append(s)
                 for i in range(0,len(sub_portfolio)):
                     fig, ax = plt.subplots(figsize=(20,15))
                     if z=='1':
-                        ax.plot(self.factor.index, self.factor[sub_portfolio[i]], 'o', label=portfolio[i]+"的因子值散点图")
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.factor[sub_portfolio[i]], 'o', label=portfolio[i]+"的因子值散点图")
                     elif z=='2':
-                        ax.plot(self.factor.index, self.factor[sub_portfolio[i]], label=portfolio[i]+"的因子值折线图")
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.factor[sub_portfolio[i]], label=portfolio[i]+"的因子值折线图")
                     ax.legend(loc='best')
                     ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("时间",fontsize=16)
                     plt.ylabel("因子值",fontsize=16)
                     self.set_picture()
                     if z=='1':
                         plt.title(sub_portfolio[i]+'的散点图',fontdict={'size': 20})
                     elif z=='2':
                         plt.title(sub_portfolio[i]+'的折线图',fontdict={'size': 20})
                     plt.show()
             else:
                  for i in range(x-1,y):
                     fig, ax = plt.subplots(figsize=(20,15))
                     if z=='1':
-                        ax.plot(self.factor.index, self.factor[self.portfolio[i]], 'o', label=portfolio[i]+"的因子值散点图")
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.factor[self.portfolio[i]], 'o', label=portfolio[i]+"的因子值散点图")
                     elif z=='2':
-                        ax.plot(self.factor.index, self.factor[self.portfolio[i]], label=portfolio[i]+"的因子值折线图")
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.factor[self.portfolio[i]], label=portfolio[i]+"的因子值折线图")
                     ax.legend(loc='best')
                     ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("时间",fontsize=16)
                     plt.ylabel("因子值",fontsize=16)
                     self.set_picture()
                     if z=='1':
                         plt.title(Chinese_name[i]+'的散点图',fontdict={'size': 20})
@@ -231,15 +226,15 @@
                 else:
                     t_absolute_value.append(result.tvalues[1])
                 t_value.append(result.tvalues[1])
                 return_value.append(result.params[1])
             for i in range(0,len(t_absolute_value)):
                 if t_absolute_value[i]>2:
                     sum_t+=1
-            print('t的绝对值超过2占比为',end=' ')
+            print('t的绝对值超过2占比为: ',end=' ')
             print(sum_t/len(t_absolute_value))
             print('t的绝对值均值为：',end=' ')
             print(np.mean(t_absolute_value))
             print('t的均值为：',end=' ')
             print(np.mean(t_value))
             print('t均值/t标准差为：',end=' ')
             print(np.mean(t_value)/np.std(t_value))
@@ -478,32 +473,31 @@
                 months.append([])
                 for j in range(0,12):
                     months[i].append(0)
             if x==0 and y==0:
                 fig, ax = plt.subplots(figsize=(20,15))
                 for i in range(0,groups):
                     if kind==1:
-                        ax.plot(self.factor.index, self.group_total_return[i], label="第"+str(i+1)+'分位的累计收益率')
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_total_return[i], label="第"+str(i+1)+'分位的累计收益率')
                     elif kind==2:
-                        ax.plot(self.factor.index, self.group_compound_return[i], label="第"+str(i+1)+'分位的复利累计收益率')
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return[i], label="第"+str(i+1)+'分位的复利累计收益率')
                 ax.legend(loc='best')
                 ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                 plt.xlabel("时间",fontsize=16)
                 plt.ylabel("收益情况",fontsize=16)
                 self.set_picture()
                 if kind==1:
                     plt.title('分位的累计收益率',fontdict={'size': 20})
                 elif kind==2:
                     plt.title('分位的复利累计收益率',fontdict={'size': 20})
                 plt.show()
                 for i in range(0,groups):
                     fig, ax = plt.subplots(figsize=(20,15))
                     sns.distplot(self.daily_rate[i],bins=40,kde=True)
                     ax.legend(loc='best')
-                    ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("收益率",fontsize=16)
                     plt.ylabel("频数",fontsize=16)
                     self.set_picture()
                     plt.title("第"+str(i+1)+'分位的收益率分布',fontdict={'size': 20})
                     plt.show()
                 ylist=[self.factor.index[0].year]
                 current_year=self.factor.index[0].year
@@ -553,17 +547,17 @@
                 sub_portfolio=[]
                 for i in range(0,x):
                     s=int(input('请输入第'+str(i+1)+'个分位的数字: '))
                     sub_portfolio.append(s)
                 fig, ax = plt.subplots(figsize=(20,15))    
                 for i in range(0,len(sub_portfolio)):
                     if kind==1:
-                        ax.plot(self.factor.index, self.group_total_return[sub_portfolio[i]-1], label="第"+str(sub_portfolio[i])+'分位的累计收益率')
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_total_return[sub_portfolio[i]-1], label="第"+str(sub_portfolio[i])+'分位的累计收益率')
                     elif kind==2:
-                        ax.plot(self.factor.index, self.group_compound_return[sub_portfolio[i]-1], label="第"+str(sub_portfolio[i])+'分位的复利累计收益率')
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return[sub_portfolio[i]-1], label="第"+str(sub_portfolio[i])+'分位的复利累计收益率')
                 ax.legend(loc='best')
                 ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                 plt.xlabel("时间",fontsize=16)
                 plt.ylabel("收益情况",fontsize=16)
                 self.set_picture()
                 if kind==1:
                     plt.title('分位的累计收益率',fontdict={'size': 20})
@@ -617,17 +611,17 @@
                     elif kind==2:
                         ax.set_title(str(time_gap)+'天收益周期的第'+str(sub_portfolio[i])+'分位的复利月度收益图',fontdict={'size': 24})
                     plt.show()
             else:
                 fig, ax = plt.subplots(figsize=(20,15))
                 for i in range(x-1,y):
                     if kind==1:
-                        ax.plot(self.factor.index, self.group_total_return[i], label="第"+str(i+1)+'分位的累计收益率')
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_total_return[i], label="第"+str(i+1)+'分位的累计收益率')
                     elif kind==2:
-                        ax.plot(self.factor.index, self.group_compound_return[i], label="第"+str(i+1)+'分位的复利累计收益率')
+                        ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), self.group_compound_return[i], label="第"+str(i+1)+'分位的复利累计收益率')
                 ax.legend(loc='best')
                 plt.xlabel("时间",fontsize=16)
                 plt.ylabel("收益情况",fontsize=16)
                 self.set_picture()
                 if kind==1:
                     plt.title('分位的累计收益率',fontdict={'size': 20})
                 elif kind==2:
@@ -700,26 +694,25 @@
             for i in range(0,len(final_rate)):
                 basic*=(1+final_rate[i])
                 rate.append(basic)
             self.strategy_information(final_rate, rate)
             sns.set(palette="muted", color_codes=True)
             sns.set(font='SimHei', font_scale=0.8)
             fig, ax = plt.subplots(figsize=(20,15))
-            ax.plot(self.factor.index, rate, label='复利累计收益情况')
+            ax.plot(self.factor.index.strftime('%Y-%m-%d %H:%M:%S'), rate, label='复利累计收益情况')
             ax.legend(loc='best')
             ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
             plt.xlabel("时间",fontsize=16)
             plt.ylabel("收益情况",fontsize=16)
             self.set_picture()
             plt.title("因子值处于"+str(left)+'和'+str(right)+'之间的复利累计收益率',fontdict={'size': 20})
             plt.show()
             fig, ax = plt.subplots(figsize=(20,15))
             sns.distplot(final_rate,bins=40,kde=True)
             ax.legend(loc='best')
-            ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
             plt.xlabel("收益率",fontsize=16)
             plt.ylabel("频数",fontsize=16)
             self.set_picture()
             plt.title("因子值处于"+str(left)+'和'+str(right)+'之间的收益率分布',fontdict={'size': 20})
             plt.show()
             self.return_rate=return_rate
     
@@ -794,15 +787,15 @@
             print(df)
             if left==0 and right==0:
                 for i in range(0,groups):
                     df=pd.DataFrame(index=self.factor.index[time_gap:])
                     df['第'+str(i+1)+'分位每个时间单位的换手率']=change_rate_everyday[i]
                     print(df)
                     fig, ax = plt.subplots(figsize=(20,15))
-                    ax.plot(self.factor.index[time_gap:], change_rate_everyday[i], label="第"+str(i+1)+'分位的每个时间单位的换手率')
+                    ax.plot(self.factor.index[time_gap:].strftime('%Y-%m-%d %H:%M:%S'), change_rate_everyday[i], label="第"+str(i+1)+'分位的每个时间单位的换手率')
                     ax.legend(loc='best')
                     ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("时间",fontsize=16)
                     plt.ylabel("换手率",fontsize=16)
                     self.set_picture()
                     plt.title("第"+str(i+1)+'分位的每个时间单位的换手率',fontdict={'size': 20})
                     plt.show()
@@ -813,29 +806,29 @@
                     s=int(input('请输入第'+str(i+1)+'个分位的数字: '))
                     sub_portfolio.append(s)
                 for i in range(0,len(sub_portfolio)):
                     df=pd.DataFrame(index=self.factor.index[time_gap:])
                     df['第'+str(i)+'分位每个时间单位的换手率']=change_rate_everyday[sub_portfolio[i]-1]
                     print(df)
                     fig, ax = plt.subplots(figsize=(20,15))
-                    ax.plot(self.factor.index[time_gap:], change_rate_everyday[sub_portfolio[i]-1], label="第"+str(sub_portfolio[i])+'分位的每个时间单位的换手率')
+                    ax.plot(self.factor.index[time_gap:].strftime('%Y-%m-%d %H:%M:%S'), change_rate_everyday[sub_portfolio[i]-1], label="第"+str(sub_portfolio[i])+'分位的每个时间单位的换手率')
                     ax.legend(loc='best')
                     ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("时间",fontsize=16)
                     plt.ylabel("换手率",fontsize=16)
                     self.set_picture()
                     plt.title("第"+str(sub_portfolio[i])+'分位的每个时间单位的换手率',fontdict={'size': 20})
                     plt.show()
             else:
                  for i in range(left-1,right):
                     df=pd.DataFrame(index=self.factor.index[time_gap:])
                     df['第'+str(i+1)+'分位每个时间单位的换手率']=change_rate_everyday[i]
                     print(df)
                     fig, ax = plt.subplots(figsize=(20,15))
-                    ax.plot(self.factor.index[time_gap:], change_rate_everyday[i], label="第"+str(i+1)+'分位的每个时间单位的换手率')
+                    ax.plot(self.factor.index[time_gap:].strftime('%Y-%m-%d %H:%M:%S'), change_rate_everyday[i], label="第"+str(i+1)+'分位的每个时间单位的换手率')
                     ax.legend(loc='best')
                     ax.xaxis.set_major_locator(ticker.MultipleLocator(base=len(self.factor)/6))
                     plt.xlabel("时间",fontsize=16)
                     plt.ylabel("换手率",fontsize=16)
                     self.set_picture()
                     plt.title("第"+str(i+1)+'分位的每个时间单位的换手率',fontdict={'size': 20})
                     plt.show()
@@ -892,14 +885,20 @@
                     average_return.append(self.return_rate[portfolio[i]][left-1:right].mean())
             else:
                 for i in range(0,len(self.portfolio)):
                     average_factor.append(self.factor[portfolio[i]][left+kind-2])
                     average_return.append(self.return_rate[portfolio[i]][left+kind-2])
             x = average_factor
             y = average_return
+            new_df=pd.DataFrame()
+            new_df['x']=x
+            new_df['y']=y
+            new_df.dropna(inplace=True)
+            x = new_df['x']
+            y = new_df['y']
             X = sm.add_constant(x)
             result = (sm.OLS(y,X)).fit()
             print(result.summary())
             fig, ax = plt.subplots(figsize=(20,15))
             ax.plot(x, y, 'o', label="data")
             ax.plot(x, result.fittedvalues, 'r')
             ax.legend(loc='best')
@@ -1005,158 +1004,183 @@
             if kind==1:
                 ax.set_title(str(time_gap)+'天收益周期的第'+str(left+1)+'分位减去第'+str(right+1)+'分位的非复利月度收益图',fontdict={'size': 24})
             elif kind==2:
                 ax.set_title(str(time_gap)+'天收益周期的第'+str(left+1)+'分位减去第'+str(right+1)+'分位的复利月度收益图',fontdict={'size': 24})
             plt.show()
         
     
-
-    
-    from datetime import datetime
-    time_gap=int(input('请输入收益率的时间间隔: '))
+    time_gap_choice=input('''
+请选择收益率的得到方式，输入1或者2：
+1.间隔X根K线
+例如：您目前的时间间隔为5分钟，那么统一以下一个交易日同时刻作为基准的话，请在稍后输入48；
+2.统一以X天后的时刻Y(仅限分钟级别的测试)
+例如：您想以次个交易日(1个交易日后）的收盘价作为清算，那么请在稍后首先输入1，再输入15:00
+''')
     factor=df_factor
     close=df_close
     ##确保index为时间序列
     factor.index=pd.to_datetime(factor.index)
     close.index=pd.to_datetime(close.index)
-    
-    neutralize=input('''
-    请问您是否需要进行因子的中性化处理:
-    0:不需要
-    或者请输入代码：综合指数，例如：sh.000001 上证指数，sz.399106 深证综指 等；
-    规模指数，例如：sh.000016 上证50，sh.000300 沪深300，sh.000905 中证500，sz.399001 深证成指等；
-    一级行业指数，例如：sh.000037 上证医药，sz.399433 国证交运 等；
-    二级行业指数，例如：sh.000952 300地产，sz.399951 300银行 等；
-    策略指数，例如：sh.000050 50等权，sh.000982 500等权 等；
-    成长指数，例如：sz.399376 小盘成长 等；
-    价值指数，例如：sh.000029 180价值 等；
-    主题指数，例如：sh.000015 红利指数，sh.000063 上证周期 等；
-    ''')
+    original_factor=factor.copy() 
+    if time_gap_choice=='1':
+        time_gap=int(input('请输入收益率的时间间隔: '))
+        ##得到收益率
+        return_rate=(close/close.shift(time_gap)-1).shift(-time_gap)
+        return_rate.replace(np.inf, np.nan,inplace=True)
+        factor.replace(np.inf,np.nan,inplace=True)
         
-    
-    if neutralize!='0':
-        while(1):
-            if neutralize=='0':
-                break
+        factor=factor[:-time_gap]
+        return_rate=return_rate[:-time_gap]
+        neutralize=input('''
+请问您是否需要进行因子的中性化处理(目前只有日级别的才可以进行中性化处理！！！其他的请选择0！):
+0:不需要
+或者请输入代码：综合指数，例如：sh.000001 上证指数，sz.399106 深证综指 等；
+规模指数，例如：sh.000016 上证50，sh.000300 沪深300，sh.000905 中证500，sz.399001 深证成指等；
+一级行业指数，例如：sh.000037 上证医药，sz.399433 国证交运 等；
+二级行业指数，例如：sh.000952 300地产，sz.399951 300银行 等；
+策略指数，例如：sh.000050 50等权，sh.000982 500等权 等；
+成长指数，例如：sz.399376 小盘成长 等；
+价值指数，例如：sh.000029 180价值 等；
+主题指数，例如：sh.000015 红利指数，sh.000063 上证周期 等；
+''')
+            
+        
+        if neutralize!='0':
+            while(1):
+                if neutralize=='0':
+                    break
+                try:
+                    lg = bs.login()  
+                    start_date=str(factor.index[0])[:10]
+                    end_date=str(factor.index[len(factor)-1])[:10]
+                    rs = bs.query_history_k_data_plus(neutralize,
+                        "date,close",
+                        start_date=start_date, end_date=end_date, frequency="d")
+                    data_list = []
+                    while (rs.error_code == '0') & rs.next():
+                        data_list.append(rs.get_row_data())
+                    result = pd.DataFrame(data_list, columns=rs.fields)
+                    result.set_index('date',inplace=True)
+                    result.index=pd.to_datetime(result.index)
+                    result=result.astype(float)
+                    result=(result/result.shift(time_gap)-1).shift(-time_gap)
+                    result.replace(np.inf, np.nan,inplace=True)
+                    result=result[:-time_gap]
+                    result.rename(columns={'close':'return_rate'},inplace=True)
+                    print('您获取的指数收益率为：')
+                    print(result)
+                    bs.logout()  
+                    break
+                except:
+                    neutralize=input('''
+输入有误！请重新输入！
+请问您是否需要进行因子的中性化处理(目前只有日级别的才可以进行中性化处理！！！其他的请选择0！):
+0:不需要
+或者请输入代码：综合指数，例如：sh.000001 上证指数，sz.399106 深证综指 等；
+规模指数，例如：sh.000016 上证50，sh.000300 沪深300，sh.000905 中证500，sz.399001 深证成指等；
+一级行业指数，例如：sh.000037 上证医药，sz.399433 国证交运 等；
+二级行业指数，例如：sh.000952 300地产，sz.399951 300银行 等；
+策略指数，例如：sh.000050 50等权，sh.000982 500等权 等；
+成长指数，例如：sz.399376 小盘成长 等；
+价值指数，例如：sh.000029 180价值 等；
+主题指数，例如：sh.000015 红利指数，sh.000063 上证周期 等；
+''')
+        
+    elif time_gap_choice=='2':
+        all_trade_days=list(set(list(factor.index.date.astype(str))))
+        all_trade_days.sort()
+        next_trade_day=int(input('请输入一个数字X，X表示为X个交易日后： '))
+        next_trade_time=input('请输入时刻，格式为15:00:00(英文的:): ')
+        return_rate=pd.DataFrame()
+        for i in range(len(factor)):
             try:
-                lg = bs.login()  
-                start_date=str(factor.index[0])[:10]
-                end_date=str(factor.index[len(factor)-1])[:10]
-                rs = bs.query_history_k_data_plus(neutralize,
-                    "date,close",
-                    start_date=start_date, end_date=end_date, frequency="d")
-                data_list = []
-                while (rs.error_code == '0') & rs.next():
-                    data_list.append(rs.get_row_data())
-                result = pd.DataFrame(data_list, columns=rs.fields)
-                result.set_index('date',inplace=True)
-                result.index=pd.to_datetime(result.index)
-                result=result.astype(float)
-                result=(result/result.shift(time_gap)-1).shift(-time_gap)
-                result.replace(np.inf, np.nan,inplace=True)
-                result=result[:-time_gap]
-                result.rename(columns={'close':'return_rate'},inplace=True)
-                print('您获取的指数收益率为：')
-                print(result)
-                bs.logout()  
-                break
+                new_time=all_trade_days[all_trade_days.index(factor.index.values[i].astype(str)[:10])+next_trade_day]+" "+next_trade_time
+                new_time=pd.to_datetime(new_time)
+                new_dataframe=pd.DataFrame(close.loc[new_time]/close.iloc[i]-1).T
+                if i==0:
+                    for j in range(len(factor)):
+                        if close.index.values[j]==new_time:
+                            time_gap=j-i
+                            break 
+                new_dataframe.index=[factor.index.values[i]]
+                return_rate=pd.concat([return_rate,new_dataframe])
             except:
-                neutralize=input('''
-    输入有误！请重新输入！
-    请问您是否需要进行因子的中性化处理:
-    0:不需要
-    或者请输入代码：综合指数，例如：sh.000001 上证指数，sz.399106 深证综指 等；
-    规模指数，例如：sh.000016 上证50，sh.000300 沪深300，sh.000905 中证500，sz.399001 深证成指等；
-    一级行业指数，例如：sh.000037 上证医药，sz.399433 国证交运 等；
-    二级行业指数，例如：sh.000952 300地产，sz.399951 300银行 等；
-    策略指数，例如：sh.000050 50等权，sh.000982 500等权 等；
-    成长指数，例如：sz.399376 小盘成长 等；
-    价值指数，例如：sh.000029 180价值 等；
-    主题指数，例如：sh.000015 红利指数，sh.000063 上证周期 等；
-    ''')
-        
-    
-    
-    ##得到收益率
-    return_rate=(close/close.shift(time_gap)-1).shift(-time_gap)
-    return_rate.replace(np.inf, np.nan,inplace=True)
-    factor.replace(np.inf,np.nan,inplace=True)
+                break
+            
     
     ##存一下名称（目前仍然是代号，可以替换成中文名称，但是要确保代号的顺序和中文名称的顺序一致）
     ##存一下原来的因子值，不要被筛掉了
     portfolio=list(factor.columns)
     Chinese_name=portfolio
-    original_factor=factor
-    factor=factor[:-time_gap]
-    return_rate=return_rate[:-time_gap]
-    if neutralize!='0':
-        return_rate=return_rate.sub(result['return_rate'],axis=0)
+    factor=factor.iloc[:len(return_rate)]     
     print('目前的因子值为： ')
     print(factor)
-    print('目前的中性化后收益率为： ')
+    print('目前的收益率为： ')
     print(return_rate)
+            
+        
     
     ##现在开始进入class
     answer=factor_analysis(factor,return_rate,portfolio)
     while(1):
         print('''
     
     
     请选择你要进行的操作:''',end=' ')
         x=input('''
-    0.退出操作
-    1.进行OLS的相关操作：可得到OLS相关系数以及拟合曲线图（比较丑，为单个标的的时间序列）
-    2.进行散点图的制作：X轴为因子值，Y轴为收益率（该图比1得到的图好看，为单个标的的时间序列）
-    3.得到不同标的的该因子的相关数据：包括分位数划分、最大值、均值、最小值、标准差、数量
-    4.进行图的制作，X轴为时间，Y轴为因子值，用以观测因子值随时间的变化趋势
-    5.进行t统计量的相关检验 
-    6.进行IC值的统计
-    7.进行IC图的制作：IC值随时间的变化关系以及一段时间内的IC均值曲线
-    8.进行分组回测：得到分组后的各组收益率的相关情况以及分位数情况
-    9.进行分组回测：得到分组后的各组收益率的走势图以及频率分布直方图（需要首先完成8）
-    10.根据因子值制定策略：指定因子值区间，只购买处于区间内的标的
-    11.换手率分析：用于分析因子的稳定性
-    12.更换收益周期
-    13.因子值的分布频率直方图（若时间周期为多天，因子值为该标的的平均值或者该周期内的第X天的值）
-    14.因子值横截面回归
-    15.任意两个分位之间的月度收益率作差（请确保完成8）
-    
-    
-    ''')
+0.退出操作
+1.进行OLS的相关操作：可得到OLS相关系数以及拟合曲线图（比较丑，为单个标的的时间序列）
+2.进行散点图的制作：X轴为因子值，Y轴为收益率（该图比1得到的图好看，为单个标的的时间序列）
+3.得到不同标的的该因子的相关数据：包括分位数划分、最大值、均值、最小值、标准差、数量
+4.进行图的制作，X轴为时间，Y轴为因子值，用以观测因子值随时间的变化趋势
+5.进行t统计量的相关检验 
+6.进行IC值的统计
+7.进行IC图的制作：IC值随时间的变化关系以及一段时间内的IC均值曲线
+8.进行分组回测：得到分组后的各组收益率的相关情况以及分位数情况
+9.进行分组回测：得到分组后的各组收益率的走势图以及频率分布直方图（需要首先完成8）
+10.根据因子值制定策略：指定因子值区间，只购买处于区间内的标的
+11.换手率分析：用于分析因子的稳定性
+12.更换收益周期
+13.因子值的分布频率直方图（若时间周期为多天，因子值为该标的的平均值或者该周期内的第X天的值）
+14.因子值横截面回归
+15.任意两个分位之间的月度收益率作差（请确保完成8）
+
+
+''')
         
         if x=='0':
             break
     
         if x=='1':
             print('''
-    请输入两个数字x、y：
-    确保x<y,
-    表明你要对列数处于x~y的标的进行时间序列的回归
-    在输入x和y的时候请确保换行
-    如果想使用全部的标的，请把x和y都输入为0
-    如果想使用标的名称而不是标的所处的列数：
-    请x输入为0，y输入为1，
-    并传入你想要进行时间序列回归标的的代码名称
-    ''')
+请输入两个数字x、y：
+确保x<y,
+表明你要对列数处于x~y的标的进行时间序列的回归
+在输入x和y的时候请确保换行
+如果想使用全部的标的，请把x和y都输入为0
+如果想使用标的名称而不是标的所处的列数：
+请x输入为0，y输入为1，
+并传入你想要进行时间序列回归标的的代码名称
+''')
             x=int(input())
             y=int(input())
             print()
             answer.OLS_data_time(x, y)
         
         elif x=='2':
             print('''
-    请输入两个数字x、y：
-    确保x<y,
-    表明你要对列数处于x~y的标的进行制作散点图
-    在输入x和y的时候请确保换行
-    如果想使用全部的标的，请把x和y都输入为0
-    如果想使用标的名称而不是标的所处的列数：
-    请x输入为0，y输入为1，
-    并传入你想要进行图制作的代码名称
-    ''')
+请输入两个数字x、y：
+确保x<y,
+表明你要对列数处于x~y的标的进行制作散点图
+在输入x和y的时候请确保换行
+如果想使用全部的标的，请把x和y都输入为0
+如果想使用标的名称而不是标的所处的列数：
+请x输入为0，y输入为1，
+并传入你想要进行图制作的代码名称
+''')
             x=int(input())
             y=int(input())
             print()
             answer.factor_return(x,y)
         
         
         elif x=='3':
@@ -1165,79 +1189,79 @@
             for i in range(0,a):
                 s=float(input('请输入第'+str(i+1)+'个分位数，确保输入的数字在0-1之间: '))
                 percent.append(s)
             answer.describe(percent)
         
         elif x=='4':
             print('''
-    请输入两个数字x、y：
-    确保x<y,
-    表明你要对列数处于x~y的标的进行图的制作
-    在输入x和y的时候请确保换行
-    如果想使用全部的标的，请把x和y都输入为0
-    如果想使用标的名称而不是标的所处的列数：
-    请x输入为0，y输入为1，
-    并传入你想要进行图制作的代码名称
-    ''')
+请输入两个数字x、y：
+确保x<y,
+表明你要对列数处于x~y的标的进行图的制作
+在输入x和y的时候请确保换行
+如果想使用全部的标的，请把x和y都输入为0
+如果想使用标的名称而不是标的所处的列数：
+请x输入为0，y输入为1，
+并传入你想要进行图制作的代码名称
+''')
             x=int(input())
             y=int(input())
             print()
             z=input('''请问你想制作下列哪种类型的图：
-    1.散点图
-    2.折线图
-    
-    ''')
+1.散点图
+2.折线图
+
+''')
             answer.factor_scater(x, y,z)
     
     
         elif x=='5':
             answer.t_analysis()
     
     
         elif x=='6':
             IC_per=float(input('''请输入一个位于0~1之间的数字X
-    该数字用以表示你想得到的|IC|>X的占比
-    
-    '''))
+该数字用以表示你想得到的|IC|>X的占比
+
+'''))
             answer.IC_value(IC_per)
     
     
         elif x=='7':
             gap=int(input('''请输入你想要得到多长时间单位的均值移动曲线：
-    时间单位是因子值的index
-    
-    '''))
+时间单位是因子值的index
+
+'''))
             IC_type=int(input('''请输入你想要得到哪种类型的IC图：
-    1.Normal IC
-    2.Rank IC
-    '''))
+1.Normal IC
+2.Rank IC
+'''))
             answer.IC_picture(gap,IC_type)
     
     
         elif x=='8':
             groups=int(input('请输入你想要将这些标的分为几组，输入的组数请不要超过标的的总数: '))
             answer.group_test(groups)
     
     
         elif x=='9':
             print('请确保在进行9之前已经进行选项8的操作，分组数量为选项8的分组数量')
             kind=int(input('''请输入你想要得到哪种收益率的走势图：
-    1.累计收益率
-    2.复利收益率
-    '''))
+1.累计收益率
+2.复利收益率
+'''))
             print('''
-    请输入两个数字x、y：
-    确保x<y,
-    表明你要对处于x~y的分位进行图的制作
-    在输入x和y的时候请确保换行
-    如果想使用全部分位，请把x和y都输入为0
-    如果想使用特定分位：
-    请x输入为0，y输入为1，
-    并传入你想要进行图制作的分位数字
-    ''')
+请输入两个数字x、y：
+确保x<y,
+表明你要对处于x~y的分位进行图的制作
+在输入x和y的时候请确保换行
+如果想使用全部分位，请把x和y都输入为0
+如果想使用特定分位：
+请x输入为0，y输入为1，
+并传入你想要进行图制作的分位数字
+''')
             x=int(input())
             y=int(input())
             print()
             answer.group_picture(kind,x,y)
     
     
         elif x=='10':
@@ -1245,94 +1269,90 @@
             right=float(input('请输入因子值区间的右边界: '))
             answer.strategy(left,right)
     
     
         elif x=='11':
             groups=int(input('请输入你想要将这些标的分为几组，输入的组数请不要超过标的的总数: '))
             print('''
-    请输入两个数字x、y：
-    确保x<y,
-    表明你要对处于x~y的分位进行换手率图的制作以及每日详细的换手率
-    在输入x和y的时候请确保换行
-    如果想使用全部分位，请把x和y都输入为0
-    如果想使用特定分位：
-    请x输入为0，y输入为1，
-    并传入你想要进行图制作的分位数字
-    ''')
+请输入两个数字x、y：
+确保x<y,
+表明你要对处于x~y的分位进行换手率图的制作以及每日详细的换手率
+在输入x和y的时候请确保换行
+如果想使用全部分位，请把x和y都输入为0
+如果想使用特定分位：
+请x输入为0，y输入为1，
+并传入你想要进行图制作的分位数字
+''')
             left=int(input())
             right=int(input())
             print()
             answer.change_hands(groups,left,right)
     
     
         elif x=='12':
             time_gap=int(input('请输入收益率的时间间隔: '))
-            factor=df_factor
-            close=df_close
+            factor=original_factor
             return_rate=pd.DataFrame(index=factor.index,columns=factor.columns)
             portfolio=list(factor.columns)
             return_rate=close.diff(periods=time_gap)
             return_rate=return_rate.shift(-time_gap)
             return_rate=return_rate/close
             factor=factor[:-time_gap]
             return_rate=return_rate[:-time_gap]
             print(factor)
             print(return_rate)
             answer=factor_analysis(factor,return_rate,portfolio)
     
     
         elif x=='13':
-            from datetime import datetime
             print('请输入因子值的时间范围，确保输入的起始时间<终止时间')
             choice=int(input('''请输入时间的格式
-    1.第X天到第Y天
-    2.从2020-01-01到2020-01-31
-    '''))
+1.第X天到第Y天
+2.从2020-01-01到2020-01-31
+'''))
             if choice==1:
                 left=int(input('请输入起始时间：'))
                 right=int(input('请输入终止时间： '))
             else:
                 left=(input('请输入起始时间：'))
                 right=(input('请输入终止时间：'))
-                left = datetime.strptime(left, "%Y-%m-%d")
-                right = datetime.strptime(right, "%Y-%m-%d")
+                left = pd.to_datetime(left)
+                right = pd.to_datetime(right)
             kind=int(input('''请输入你想要以哪一种因子值作为最终因子值
-    0.这一段时间内的平均值
-    X.这一段时间的第X天的值，请注意：1<=X<=（终止时间-起始时间+1）且X为正整数
-    '''))
+0.这一段时间内的平均值
+X.这一段时间的第X天的值，请注意：1<=X<=（终止时间-起始时间+1）且X为正整数
+'''))
             answer.factor_bins(left,right,kind,choice)
         
         
         elif x=='14':
-            from datetime import datetime
             print('请输入因子值的时间范围，确保输入的起始时间<终止时间')
             choice=int(input('''请输入时间的格式
-    1.第X天到第Y天
-    2.从2020-01-01到2020-01-31
-    '''))
+1.第X天到第Y天
+2.从2020-01-01到2020-01-31
+'''))
             if choice==1:
                 left=int(input('请输入起始时间：'))
                 right=int(input('请输入终止时间： '))
             else:
                 left=(input('请输入起始时间：'))
                 right=(input('请输入终止时间：'))
-                left = datetime.strptime(left, "%Y-%m-%d")
-                right = datetime.strptime(right, "%Y-%m-%d")
-            kind=int(input('''请输入你想要以哪一种因子值作为最终因子值
-    0.这一段时间内的平均值
-    X.这一段时间的第X天的值，请注意：1<=X<=（终止时间-起始时间+1）且X为正整数
-    '''))
+                left = pd.to_datetime(left)
+                right = pd.to_datetime(right)
+            kind=int(input('''请输入你想要以哪一种因子值和收益率作为最终因子值以及收益率
+0.这一段时间内的平均值
+X.这一段时间的第X天的值，请注意：1<=X<=（终止时间-起始时间+1）且X为正整数
+'''))
             answer.panel_ols(left,right,kind,choice)
         
         
         elif x=='15':
             print('请输入你想得到的第X分位-第Y分位的月度收益图')
             left=int(input('请输入第X分位：'))
             right=int(input('请输入第Y分位：'))
             kind=int(input('''请输入你想要得到哪种收益率的走势图：
-    1.累计收益率
-    2.复利收益率
-    '''))
+1.累计收益率
+2.复利收益率
+'''))
             answer.difference_month(left,right,kind)
     
-if __name__=='__namin__':
-    backtest('turn','close')
+
```

## Comparing `singlefactortest-1.0.dist-info/METADATA` & `singlefactortest-1.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: singlefactortest
-Version: 1.0
-Summary: 单因子的测试（日级别）
+Version: 1.1
+Summary: 单因子的测试（日级别and分钟级别）
 Home-page: https://github.com/Masteryeda
 Author: IDEA_Wenzhi
 Author-email: 1259429314@qq.com
 Maintainer: IDEA_Wenzhi
 Maintainer-email: 1259429314@qq.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
```

