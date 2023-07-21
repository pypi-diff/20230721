# Comparing `tmp/bcitoolbox-0.0.1.2.tar.gz` & `tmp/bcitoolbox-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcitoolbox-0.0.1.2.tar", last modified: Thu Jul 20 06:01:31 2023, max compression
+gzip compressed data, was "bcitoolbox-0.0.1.3.tar", last modified: Fri Jul 21 01:26:38 2023, max compression
```

## Comparing `bcitoolbox-0.0.1.2.tar` & `bcitoolbox-0.0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-20 06:01:31.649325 bcitoolbox-0.0.1.2/
--rw-r--r--   0 evans      (501) staff       (20)      534 2023-07-20 06:01:31.648873 bcitoolbox-0.0.1.2/PKG-INFO
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-20 06:01:31.645717 bcitoolbox-0.0.1.2/bcitoolbox/
--rw-r--r--   0 evans      (501) staff       (20)    13082 2023-07-20 05:31:26.000000 bcitoolbox-0.0.1.2/bcitoolbox/BCIbox.py
--rw-r--r--   0 evans      (501) staff       (20)      137 2023-07-20 05:29:09.000000 bcitoolbox-0.0.1.2/bcitoolbox/__init__.py
--rw-r--r--   0 evans      (501) staff       (20)    38260 2023-07-20 05:25:55.000000 bcitoolbox-0.0.1.2/bcitoolbox/guifunc.py
-drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-20 06:01:31.648441 bcitoolbox-0.0.1.2/bcitoolbox.egg-info/
--rw-r--r--   0 evans      (501) staff       (20)      534 2023-07-20 06:01:31.000000 bcitoolbox-0.0.1.2/bcitoolbox.egg-info/PKG-INFO
--rw-r--r--   0 evans      (501) staff       (20)      243 2023-07-20 06:01:31.000000 bcitoolbox-0.0.1.2/bcitoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-20 06:01:31.000000 bcitoolbox-0.0.1.2/bcitoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 evans      (501) staff       (20)       23 2023-07-20 06:01:31.000000 bcitoolbox-0.0.1.2/bcitoolbox.egg-info/requires.txt
--rw-r--r--   0 evans      (501) staff       (20)       11 2023-07-20 06:01:31.000000 bcitoolbox-0.0.1.2/bcitoolbox.egg-info/top_level.txt
--rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-20 06:01:31.649444 bcitoolbox-0.0.1.2/setup.cfg
--rw-r--r--   0 evans      (501) staff       (20)      880 2023-07-20 06:01:15.000000 bcitoolbox-0.0.1.2/setup.py
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-21 01:26:38.773249 bcitoolbox-0.0.1.3/
+-rw-r--r--   0 evans      (501) staff       (20)      534 2023-07-21 01:26:38.772792 bcitoolbox-0.0.1.3/PKG-INFO
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-21 01:26:38.766495 bcitoolbox-0.0.1.3/bcitoolbox/
+-rw-r--r--   0 evans      (501) staff       (20)    13082 2023-07-20 05:31:26.000000 bcitoolbox-0.0.1.3/bcitoolbox/BCIbox.py
+-rw-r--r--   0 evans      (501) staff       (20)      137 2023-07-20 05:29:09.000000 bcitoolbox-0.0.1.3/bcitoolbox/__init__.py
+-rw-r--r--   0 evans      (501) staff       (20)    38267 2023-07-21 01:24:31.000000 bcitoolbox-0.0.1.3/bcitoolbox/guifunc.py
+drwxr-xr-x   0 evans      (501) staff       (20)        0 2023-07-21 01:26:38.772244 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/
+-rw-r--r--   0 evans      (501) staff       (20)      534 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 evans      (501) staff       (20)      243 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 evans      (501) staff       (20)        1 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 evans      (501) staff       (20)       23 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/requires.txt
+-rw-r--r--   0 evans      (501) staff       (20)       11 2023-07-21 01:26:38.000000 bcitoolbox-0.0.1.3/bcitoolbox.egg-info/top_level.txt
+-rw-r--r--   0 evans      (501) staff       (20)       38 2023-07-21 01:26:38.773383 bcitoolbox-0.0.1.3/setup.cfg
+-rw-r--r--   0 evans      (501) staff       (20)      880 2023-07-21 01:25:03.000000 bcitoolbox-0.0.1.3/setup.py
```

### Comparing `bcitoolbox-0.0.1.2/PKG-INFO` & `bcitoolbox-0.0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcitoolbox
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A package for Bayesian causal inference model
 Author: evans.zhu
 Author-email: evanszhu2001@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bcitoolbox-0.0.1.2/bcitoolbox/BCIbox.py` & `bcitoolbox-0.0.1.3/bcitoolbox/BCIbox.py`

 * *Files identical despite different names*

### Comparing `bcitoolbox-0.0.1.2/bcitoolbox/guifunc.py` & `bcitoolbox-0.0.1.3/bcitoolbox/guifunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,28 +72,30 @@
     if file_paths:
         data_matrices = []
         for file_path in file_paths:
             print(file_path)
             df = np.loadtxt(file_path, delimiter=',')
             data_matrices.append(df)
             
+            
+        
 def open_file(text_entry):
     global data_matrices
     global file_paths
     file_paths = text_entry.get()
     file_paths = filedialog.askopenfilenames(title="Select CSV file", filetypes=[("CSV Files", "*.csv")])
     text_entry.delete(0, tk.END)
     text_entry.insert(tk.END, file_paths)
     if file_paths:
         data_matrices = []
         for file_path in file_paths:
             print(file_path)
             df = np.loadtxt(file_path, delimiter=',')
             data_matrices.append(df)
-            
+    
 def open_document():
     file_path = filedialog.askopenfilename()
     if file_path:  
         print(file_path)
 
 def done_setting():
     global count
@@ -279,15 +281,15 @@
 
 def plot_func(ifsave):
     # 用户选择的图片序号
     selected_image = tk.IntVar()
     if ifsave==2:
         target_folder = filedialog.askdirectory()
     else:
-        num_plot = tk.simpledialog.askinteger("Plot", "Please enter the number of bits of data you want to plot (e.g. 1 for the first one)", minvalue=0, maxvalue=10000)
+        num_plot = tk.simpledialog.askinteger("Plot", "Please enter the position number of data you want to plot (e.g. 1 for the first one)", minvalue=0, maxvalue=10000)
 
     for ndata in range (len(data_matrices)):
         plt.figure()
         [error,modelprop,dataprop,d] = simulateVV(parameters_list[ndata], 10000, data_matrices[ndata], 1, strategy = strategy_list[ndata], fitType = 'mll')
         a = dataprop.shape
         condi = int((a[1] + 1) ** 0.5)
         plt.subplots_adjust(hspace=0.5, wspace=0.5)  
@@ -538,15 +540,15 @@
         file_name = os.path.splitext(file_name)[0]
         file_list.append(file_name)
 
     result_list = list(zip(file_list, parameters_list, error_list, strategy_list))
     file_path = filedialog.asksaveasfilename(defaultextension=".txt",
                                              filetypes=[("Text Files", "*.txt"), ("All Files", "*.*")])
     if file_path:
-        header = "file_name\tParameters\terror\tstrategy\n" 
+        header = "File Name\tParameters\tError\tStrategy\n" 
         with open(file_path, "w") as txtfile:
             txtfile.write(header)
             for rdata in result_list:
                 arr_str = np.array2string(rdata[1], separator=',', precision=6, suppress_small=True)
                 txtfile.write(f"{rdata[0]}\t{arr_str}\t{rdata[2]}\t{rdata[3]}\n")
 
 def plot_Simuall():
@@ -983,29 +985,29 @@
     
         # Plot
         placeholder = tk.Frame(simu_frame, height=30)
         placeholder.pack()
         plot_Simuall_but = tk.Button(simu_frame, text="Simulate", command=plot_Simuall)
         plot_Simuall_but.pack()
         pcommon_label = tk.Label(simu_frame, text="Pcommon", fg="black")
-        pcommon_label.place(relx=0.19, rely=0.13, anchor="w")
+        pcommon_label.place(relx=0.3, rely=0.12, anchor="w")
     
         sigmaU_label = tk.Label(simu_frame, text="sigmaU", fg="blue")
-        sigmaU_label.place(relx=0.2, rely=0.28, anchor="w")
+        sigmaU_label.place(relx=0.3, rely=0.27, anchor="w")
     
         sigmaD_label = tk.Label(simu_frame, text="sigmaD", fg="red")
-        sigmaD_label.place(relx=0.2, rely=0.45, anchor="w")
+        sigmaD_label.place(relx=0.3, rely=0.43, anchor="w")
     
         sigmaZ_label = tk.Label(simu_frame, text="sigmaZ", fg="black")
-        sigmaZ_label.place(relx=0.2, rely=0.61, anchor="w")
+        sigmaZ_label.place(relx=0.3, rely=0.57, anchor="w")
     
         mup_label = tk.Label(simu_frame, text="Z_center", fg="black")
-        mup_label.place(relx=0.19, rely=0.76, anchor="w")
+        mup_label.place(relx=0.3, rely=0.72, anchor="w")
         Num_label = tk.Label(simu_frame, text="Number of stimuli", fg="black")
-        Num_label.place(relx=0.2, rely=0.83, anchor="center")
+        Num_label.place(relx=0.3, rely=0.78, anchor="center")
                 
     var_a_simu = tk.BooleanVar(value=True)
     var_b_simu = tk.BooleanVar()
     var_c_simu = tk.BooleanVar()
 
     check_button_a_simu = tk.Checkbutton(simu_frame, text="Averaging", variable=var_a_simu, command=function_a_simu)
     check_button_b_simu = tk.Checkbutton(simu_frame, text="Selecting", variable=var_b_simu, command=function_b_simu)
@@ -1041,9 +1043,7 @@
     startSim_button.place(relx=0.5, rely=0.45, anchor="center")
 
     startSimall_button = tk.Button(welcome_frame, text="Simulate for Numerosity Task", command=lambda: simu_page(2))
     startSimall_button.place(relx=0.5, rely=0.5, anchor="center")
 
     # 
     tk.Label(welcome_frame).pack()
-    
-
```

### Comparing `bcitoolbox-0.0.1.2/bcitoolbox.egg-info/PKG-INFO` & `bcitoolbox-0.0.1.3/bcitoolbox.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcitoolbox
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A package for Bayesian causal inference model
 Author: evans.zhu
 Author-email: evanszhu2001@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `bcitoolbox-0.0.1.2/setup.py` & `bcitoolbox-0.0.1.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bcitoolbox',  # Replace with your desired package name
-    version='0.0.1.2',         # Replace with your desired version number
+    version='0.0.1.3',         # Replace with your desired version number
     author='evans.zhu',
     author_email='evanszhu2001@gmail.com',
     description='A package for Bayesian causal inference model',
     long_description='A zero-programming toolbox.',
     long_description_content_type='text/markdown',
     packages=['bcitoolbox'],
     install_requires=['numpy', 'matplotlib', 'scipy'],  # Add any dependencies required by your function
```

