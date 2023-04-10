# Comparing `tmp/EEGRAPH-0.1.8.tar.gz` & `tmp/EEGRAPH-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EEGRAPH-0.1.8.tar", last modified: Tue May  4 10:18:54 2021, max compression
+gzip compressed data, was "EEGRAPH-0.1.9.tar", last modified: Wed May  5 08:53:34 2021, max compression
```

## Comparing `EEGRAPH-0.1.8.tar` & `EEGRAPH-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.745338 EEGRAPH-0.1.8/
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.611225 EEGRAPH-0.1.8/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     1442 2021-05-04 10:11:51.000000 EEGRAPH-0.1.8/.ipynb_checkpoints/CHANGELOG-checkpoint.txt
--rw-rw-rw-   0        0        0     1114 2021-05-04 10:12:03.000000 EEGRAPH-0.1.8/.ipynb_checkpoints/setup-checkpoint.py
--rw-rw-rw-   0        0        0     1442 2021-05-04 10:11:51.000000 EEGRAPH-0.1.8/CHANGELOG.txt
--rw-rw-rw-   0        0        0     4394 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.618225 EEGRAPH-0.1.8/EEGRAPH.egg-info/
--rw-rw-rw-   0        0        0     7203 2021-05-04 10:18:54.000000 EEGRAPH-0.1.8/EEGRAPH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      690 2021-05-04 10:18:54.000000 EEGRAPH-0.1.8/EEGRAPH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-04 10:18:54.000000 EEGRAPH-0.1.8/EEGRAPH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2021-05-04 10:18:54.000000 EEGRAPH-0.1.8/EEGRAPH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2021-05-04 10:18:54.000000 EEGRAPH-0.1.8/EEGRAPH.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       30 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7203 2021-05-04 10:18:54.745338 EEGRAPH-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5743 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.627241 EEGRAPH-0.1.8/eegraph/
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.655224 EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0     1329 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/graph-checkpoint.py
--rw-rw-rw-   0        0        0     3110 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/importData-checkpoint.py
--rw-rw-rw-   0        0        0    15028 2021-05-04 09:35:57.000000 EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/strategy-checkpoint.py
--rw-rw-rw-   0        0        0    32573 2021-05-04 09:23:32.000000 EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/tools-checkpoint.py
--rw-rw-rw-   0        0        0       20 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/eegraph/__init__.py
--rw-rw-rw-   0        0        0     1329 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/eegraph/graph.py
--rw-rw-rw-   0        0        0     3110 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/eegraph/importData.py
--rw-rw-rw-   0        0        0     1047 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/eegraph/modelateData.py
--rw-rw-rw-   0        0        0    15028 2021-05-04 09:35:57.000000 EEGRAPH-0.1.8/eegraph/strategy.py
--rw-rw-rw-   0        0        0    32573 2021-05-04 09:23:32.000000 EEGRAPH-0.1.8/eegraph/tools.py
--rw-rw-rw-   0        0        0      134 2021-04-22 12:11:32.000000 EEGRAPH-0.1.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2021-05-04 10:18:54.745338 EEGRAPH-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1114 2021-05-04 10:12:03.000000 EEGRAPH-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.670225 EEGRAPH-0.1.8/tests/
-drwxrwxrwx   0        0        0        0 2021-05-04 10:18:54.717285 EEGRAPH-0.1.8/tests/.ipynb_checkpoints/
--rw-rw-rw-   0        0        0    17348 2021-04-23 08:47:54.000000 EEGRAPH-0.1.8/tests/.ipynb_checkpoints/tests-checkpoint.py
--rw-rw-rw-   0        0        0    17348 2021-04-23 08:47:54.000000 EEGRAPH-0.1.8/tests/tests.py
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.587346 EEGRAPH-0.1.9/
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.538346 EEGRAPH-0.1.9/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     1442 2021-05-04 10:11:51.000000 EEGRAPH-0.1.9/.ipynb_checkpoints/CHANGELOG-checkpoint.txt
+-rw-rw-rw-   0        0        0     1114 2021-05-05 08:30:22.000000 EEGRAPH-0.1.9/.ipynb_checkpoints/setup-checkpoint.py
+-rw-rw-rw-   0        0        0     1632 2021-05-05 08:30:38.000000 EEGRAPH-0.1.9/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     4394 2021-04-22 12:11:32.000000 EEGRAPH-0.1.9/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.561361 EEGRAPH-0.1.9/EEGRAPH.egg-info/
+-rw-rw-rw-   0        0        0     7203 2021-05-05 08:53:34.000000 EEGRAPH-0.1.9/EEGRAPH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2021-05-05 08:53:34.000000 EEGRAPH-0.1.9/EEGRAPH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-05 08:53:34.000000 EEGRAPH-0.1.9/EEGRAPH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2021-05-05 08:53:34.000000 EEGRAPH-0.1.9/EEGRAPH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2021-05-05 08:53:34.000000 EEGRAPH-0.1.9/EEGRAPH.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       30 2021-04-22 12:11:32.000000 EEGRAPH-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7203 2021-05-05 08:53:34.586350 EEGRAPH-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5743 2021-05-05 08:38:55.000000 EEGRAPH-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.570352 EEGRAPH-0.1.9/eegraph/
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.579347 EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0     1278 2021-05-05 08:26:02.000000 EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/graph-checkpoint.py
+-rw-rw-rw-   0        0        0     2287 2021-05-05 07:27:00.000000 EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/importData-checkpoint.py
+-rw-rw-rw-   0        0        0    15135 2021-05-05 08:13:53.000000 EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/strategy-checkpoint.py
+-rw-rw-rw-   0        0        0    33587 2021-05-05 08:25:01.000000 EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/tools-checkpoint.py
+-rw-rw-rw-   0        0        0       20 2021-04-22 12:11:32.000000 EEGRAPH-0.1.9/eegraph/__init__.py
+-rw-rw-rw-   0        0        0     1278 2021-05-05 08:26:02.000000 EEGRAPH-0.1.9/eegraph/graph.py
+-rw-rw-rw-   0        0        0     2287 2021-05-05 07:27:00.000000 EEGRAPH-0.1.9/eegraph/importData.py
+-rw-rw-rw-   0        0        0     1047 2021-04-22 12:11:32.000000 EEGRAPH-0.1.9/eegraph/modelateData.py
+-rw-rw-rw-   0        0        0    15135 2021-05-05 08:13:53.000000 EEGRAPH-0.1.9/eegraph/strategy.py
+-rw-rw-rw-   0        0        0    33587 2021-05-05 08:25:01.000000 EEGRAPH-0.1.9/eegraph/tools.py
+-rw-rw-rw-   0        0        0      134 2021-04-22 12:11:32.000000 EEGRAPH-0.1.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2021-05-05 08:53:34.587346 EEGRAPH-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2021-05-05 08:30:22.000000 EEGRAPH-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.581347 EEGRAPH-0.1.9/tests/
+drwxrwxrwx   0        0        0        0 2021-05-05 08:53:34.583346 EEGRAPH-0.1.9/tests/.ipynb_checkpoints/
+-rw-rw-rw-   0        0        0    17328 2021-05-05 08:43:48.000000 EEGRAPH-0.1.9/tests/.ipynb_checkpoints/tests-checkpoint.py
+-rw-rw-rw-   0        0        0    17328 2021-05-05 08:43:48.000000 EEGRAPH-0.1.9/tests/tests.py
```

### Comparing `EEGRAPH-0.1.8/.ipynb_checkpoints/CHANGELOG-checkpoint.txt` & `EEGRAPH-0.1.9/.ipynb_checkpoints/CHANGELOG-checkpoint.txt`

 * *Files identical despite different names*

### Comparing `EEGRAPH-0.1.8/.ipynb_checkpoints/setup-checkpoint.py` & `EEGRAPH-0.1.9/.ipynb_checkpoints/setup-checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='EEGRAPH',
-    version='0.1.8',
+    version='0.1.9',
     description='',
     url='https://github.com/ufvceiec/EEGRAPH',
     author='CEIEC',
     license= 'GPL-3.0',
     classifers=classifiers,
     keywords='',
     packages=find_packages(),
```

### Comparing `EEGRAPH-0.1.8/CHANGELOG.txt` & `EEGRAPH-0.1.9/CHANGELOG.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Change Log
 ==========
 
+0.1.9 (05/05/2021)
+------------------
+- Adding custom input percentage threshold for spectral entropy, power spectrum and shannon entropy.
+- Updating DTF to generate directed graphs. 
+
 0.1.8 (05/04/2021)
 ------------------
 - Updating Corrected cross-correlation default threshold.
 - Rescaling data for Corrected cross-correlation. 
 
 0.1.7 (04/22/2021)
 ------------------
```

### Comparing `EEGRAPH-0.1.8/CONTRIBUTING.md` & `EEGRAPH-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `EEGRAPH-0.1.8/EEGRAPH.egg-info/PKG-INFO` & `EEGRAPH-0.1.9/EEGRAPH.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EEGRAPH
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/ufvceiec/EEGRAPH
 Author: CEIEC
 License: GPL-3.0
 Description: <p align="center">
           <img src="https://github.com/ufvceiec/EEGRAPH/blob/develop-refactor/demo/eegraph-logo.png" alt="EEGraph Logo"/>
         </p>
@@ -82,22 +82,22 @@
         ## Usage
         Example usage of the library with Pearson Correlation. 
         ***
         ### Load data
         ```python
         import eegraph
         G = eegraph.Graph()
-        G.load_data(path = "espasmo1.edf", exclude = ['EEG TAntI1-TAntI', 'EEG TAntD1-TAntD', 'EEG EKG1-EKG2'])
+        G.load_data(path = 'espasmo1.edf', exclude = ['EEG TAntI1-TAntI', 'EEG TAntD1-TAntD', 'EEG EKG1-EKG2'])
         ```
         #### Electrode Montage
         An electrode montage file can be specified for channels names while loading EEG data. Visit [documentation](https://github.com/ufvceiec/EEGRAPH/wiki/Load-data-from-EEG) for more info.
         ```python
         import eegraph
         G = eegraph.Graph()
-        G.load_data(path = "espasmo1.edf", electrode_montage_path = 'electrodemontage.set.ced')
+        G.load_data(path = 'espasmo1.edf', electrode_montage_path = 'electrodemontage.set.ced')
         ```
         ***
         ### Modelate data
         ##### Without frequency bands
         ```python
         graphs, connectivity_matrix = G.modelate(window_size = 2, connectivity = 'pearson_correlation')
         ```
```

### Comparing `EEGRAPH-0.1.8/EEGRAPH.egg-info/SOURCES.txt` & `EEGRAPH-0.1.9/EEGRAPH.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `EEGRAPH-0.1.8/PKG-INFO` & `EEGRAPH-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EEGRAPH
-Version: 0.1.8
+Version: 0.1.9
 Summary: UNKNOWN
 Home-page: https://github.com/ufvceiec/EEGRAPH
 Author: CEIEC
 License: GPL-3.0
 Description: <p align="center">
           <img src="https://github.com/ufvceiec/EEGRAPH/blob/develop-refactor/demo/eegraph-logo.png" alt="EEGraph Logo"/>
         </p>
@@ -82,22 +82,22 @@
         ## Usage
         Example usage of the library with Pearson Correlation. 
         ***
         ### Load data
         ```python
         import eegraph
         G = eegraph.Graph()
-        G.load_data(path = "espasmo1.edf", exclude = ['EEG TAntI1-TAntI', 'EEG TAntD1-TAntD', 'EEG EKG1-EKG2'])
+        G.load_data(path = 'espasmo1.edf', exclude = ['EEG TAntI1-TAntI', 'EEG TAntD1-TAntD', 'EEG EKG1-EKG2'])
         ```
         #### Electrode Montage
         An electrode montage file can be specified for channels names while loading EEG data. Visit [documentation](https://github.com/ufvceiec/EEGRAPH/wiki/Load-data-from-EEG) for more info.
         ```python
         import eegraph
         G = eegraph.Graph()
-        G.load_data(path = "espasmo1.edf", electrode_montage_path = 'electrodemontage.set.ced')
+        G.load_data(path = 'espasmo1.edf', electrode_montage_path = 'electrodemontage.set.ced')
         ```
         ***
         ### Modelate data
         ##### Without frequency bands
         ```python
         graphs, connectivity_matrix = G.modelate(window_size = 2, connectivity = 'pearson_correlation')
         ```
```

### Comparing `EEGRAPH-0.1.8/README.md` & `EEGRAPH-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,22 +75,22 @@
 ## Usage
 Example usage of the library with Pearson Correlation. 
 ***
 ### Load data
 ```python
 import eegraph
 G = eegraph.Graph()
-G.load_data(path = "espasmo1.edf", exclude = ['EEG TAntI1-TAntI', 'EEG TAntD1-TAntD', 'EEG EKG1-EKG2'])
+G.load_data(path = 'espasmo1.edf', exclude = ['EEG TAntI1-TAntI', 'EEG TAntD1-TAntD', 'EEG EKG1-EKG2'])
 ```
 #### Electrode Montage
 An electrode montage file can be specified for channels names while loading EEG data. Visit [documentation](https://github.com/ufvceiec/EEGRAPH/wiki/Load-data-from-EEG) for more info.
 ```python
 import eegraph
 G = eegraph.Graph()
-G.load_data(path = "espasmo1.edf", electrode_montage_path = 'electrodemontage.set.ced')
+G.load_data(path = 'espasmo1.edf', electrode_montage_path = 'electrodemontage.set.ced')
 ```
 ***
 ### Modelate data
 ##### Without frequency bands
 ```python
 graphs, connectivity_matrix = G.modelate(window_size = 2, connectivity = 'pearson_correlation')
 ```
```

### Comparing `EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/graph-checkpoint.py` & `EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/graph-checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,20 @@
         if(electrode_montage_path):
             self.ch_names=input_data.set_montage(electrode_montage_path)
         
         input_data.display_info(self.ch_names)
         
 
     def modelate(self, window_size, connectivity, bands = [None], threshold = None):
-        
         print('\033[1m' + 'Model Data.' + '\033[0m')
         print(search(connectivity_measures, connectivity))
         
         model_data = ModelData(self.data, self.ch_names, eval(search(connectivity_measures, connectivity)))  
         connectivity_matrix, G = model_data.connectivity_workflow(bands, window_size, threshold)
         
         return connectivity_matrix, G
         
 
     def visualize(self, graph, name):
-        print(str(graph))
-        fig = draw_graph(graph, False, False)
+        fig = draw_graph(graph)
         fig.update_layout(title='', plot_bgcolor='white' ) 
         fig.write_html(str(name) + '_plot.html', auto_open=True, default_height='100%', default_width='100%')
```

### Comparing `EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/strategy-checkpoint.py` & `EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/strategy-checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,28 +50,28 @@
         self.bands = input_bands(bands)
         data_intervals, steps, self.flag = calculate_time_intervals(data.raw_data, data.sample_rate, data.sample_duration, window_size, data.sample_length)
         self.connectivity_matrix = calculate_connectivity_single_channel_with_bands(data_intervals, data.sample_rate, self, self.bands)
         
         return self.connectivity_matrix
 
     def make_graph_workflow(self, data):
-        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels, self.bands)
+        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels, data.threshold, self.bands)
     
         return G
     
 class Connectivity_single_channel_No_Bands(Strategy):
     def calculate_connectivity_workflow(self, data, bands, window_size):
         dont_need_bands(bands)
         data_intervals, steps, self.flag = calculate_time_intervals(data.raw_data, data.sample_rate, data.sample_duration, window_size, data.sample_length)
         self.connectivity_matrix = calculate_connectivity_single_channel(data_intervals, data.sample_rate, self)
         
         return self.connectivity_matrix
 
     def make_graph_workflow(self, data):
-        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels)
+        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels, data.threshold)
     
         return G
     
 class Cross_correlation_rescaled(Strategy):
     def calculate_connectivity_workflow(self, data, bands, window_size):
         dont_need_bands(bands)
         scaled_data = re_scaling(data.raw_data)
@@ -90,15 +90,15 @@
         self.bands = input_bands(bands)
         data_intervals, steps, self.flag = calculate_time_intervals(data.raw_data, data.sample_rate, data.sample_duration, window_size, data.sample_length)
         self.connectivity_matrix = calculate_dtf(data_intervals, steps, data.num_channels, data.sample_rate, self.bands, self.flag)
         
         return self.connectivity_matrix
 
     def make_graph_workflow(self, data):
-        G = make_graph(self.connectivity_matrix, data.ch_names, data.threshold)
+        G = make_graph(self.connectivity_matrix, data.ch_names, data.threshold, True)
     
         return G    
         
         
 #Connectivity measures            
 class Cross_correlation_Estimator(Cross_correlation_rescaled):
     def __init__(self):
@@ -306,36 +306,36 @@
         phase_diff = (phase_diff  + np.pi) % (2 * np.pi) - np.pi
         pli = abs(np.mean(np.sign(phase_diff)))
         
         return pli
     
 class Power_spectrum_Estimator(Connectivity_single_channel_With_Bands):
     def __init__(self):
-        self.threshold = None
+        self.threshold = 0.25            #<----- 25%
         
     #https://www.kite.com/python/answers/how-to-plot-a-power-spectrum-in-python
     def single_channel_conn(self, data, sample_rate):
         fourier_transform = np.fft.rfft(data)
         abs_fourier_transform = np.abs(fourier_transform)
         power_spectrum = np.square(abs_fourier_transform)
         return power_spectrum.mean()    
     
 class Spectral_entropy_Estimator(Connectivity_single_channel_With_Bands):
     def __init__(self):
-        self.threshold = None
+        self.threshold = 0.25            #<----- 25%
         
     #https://raphaelvallat.com/antropy/build/html/generated/antropy.spectral_entropy.html#antropy.spectral_entropy
     def single_channel_conn(self, data, sample_rate):
         nperseg = len(data)
         se = ant.spectral_entropy(data, sample_rate, method='welch', nperseg = nperseg, normalize=True)
         return se
     
 class Shannon_entropy_Estimator(Connectivity_single_channel_No_Bands):
     def __init__(self):
-        self.threshold = None
+        self.threshold = 0.25            #<----- 25%
         
     #https://www.kite.com/python/answers/how-to-calculate-shannon-entropy-in-python
     def single_channel_conn(self, data, sample_rate):
         pd_series = pd.Series(data)
         counts = pd_series.value_counts()
         she = entropy(counts)
         return she
```

### Comparing `EEGRAPH-0.1.8/eegraph/.ipynb_checkpoints/tools-checkpoint.py` & `EEGRAPH-0.1.9/eegraph/.ipynb_checkpoints/tools-checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,29 @@
 from scipy import signal
 from itertools import combinations
 import networkx as nx
 import plotly.graph_objects as go
 import logging
 import warnings
 
+input_format = {'edf': 'mne.io.read_raw_edf(self.path, exclude= self.exclude)', 'gdf': 'mne.io.read_raw_gdf(self.path, exclude= self.exclude)', 'vhdr': 'mne.io.read_raw_brainvision(self.path, exclude= self.exclude)',
+               'cnt': 'mne.io.read_raw_cnt(self.path, exclude= self.exclude)', 'bdf': 'mne.io.read_raw_edf(self.path, exclude= self.exclude)', 'egi': 'mne.io.read_raw_egi(self.path, exclude= self.exclude)', 
+                'mff': 'mne.io.read_raw_egi(self.path, exclude= self.exclude)', 'nxe': 'mne.io.read_raw_eximia(self.path, exclude= self.exclude)'}
+
 connectivity_measures = {'cross_correlation': 'Cross_correlation_Estimator', 'pearson_correlation': 'Pearson_correlation_Estimator', 'squared_coherence': 'Squared_coherence_Estimator',
                          'imag_coherence': 'Imag_coherence_Estimator', 'corr_cross_correlation': 'Corr_cross_correlation_Estimator', 'wpli': 'Wpli_Estimator', 
                          'plv': 'Plv_Estimator', 'pli': 'Pli_No_Bands_Estimator', 'pli_bands': 'Pli_Bands_Estimator', 'dtf': 'Dtf_Estimator', 'power_spectrum': 'Power_spectrum_Estimator',
                          'spectral_entropy': 'Spectral_entropy_Estimator', 'shannon_entropy': 'Shannon_entropy_Estimator'}
 
+def search_input(values, searchFor):
+    for k in values:
+        if (searchFor == k):
+            return values[k]
+    raise NameError('File extension ' + "'" + searchFor + "'" + ' is not supported.')
+    
 def search(values, searchFor):
     for k in values:
         if (searchFor == k):
             return (values[k] + '()')
     raise NameError('Connectivity Measure ' + "'" + searchFor + "'" + ' does not exist.')
 
 def need_bands(bands):
@@ -412,15 +422,15 @@
         for z,item in enumerate([delta, theta, alpha, beta, gamma]):
             if bands[z]:
                 values.append(connectivity.single_channel_conn(item, sample_rate))
                 
     return values
 
 
-def make_graph(matrix, ch_names, threshold):
+def make_graph(matrix, ch_names, threshold, directed = False):
     """Process to create the networkX graphs.
     Parameters
     ----------
     matrix : ndarray
         Matrix containing all the correlation matrix.
     ch_names : list
         Channel names in the EEG.
@@ -433,56 +443,62 @@
     
     G = {}
     num_nodes = len(nodes)
     
     #Loop over the number of graphs, creating the nx Graph, adding the nodes (which will be the same in all graphs) and adding an edge if the connectivity measure is above the threshold.
     #Also we add a weight to the edge, to draw the edge´s size according to this value. It is the connectivity coefficient to a power, to really difference big from smaller coefficients. 
     for k in range(num_graphs):
-        G[k] = nx.Graph()
+        if(directed):
+            G[k] = nx.DiGraph()
+        else:
+            G[k] = nx.Graph()
+            
         G[k].add_nodes_from(nodes)
         for i in range(num_nodes):
             for j in range(num_nodes):
                 if matrix[k][i,j] > threshold and i!=j:
                     #print("graph:",k,"Edge between:", i,j)
                     G[k].add_edge(nodes[i],nodes[j], thickness = pow(matrix[k][i,j], 3) * 6, weight = matrix[k][i,j])
     
     
     return G        
 
-def single_channel_graph(data, ch_names, channels, bands=None):     
+def single_channel_graph(data, ch_names, channels, percentage_threshold, bands=None):     
     num_graphs = int(len(data)/channels)
     print("Number of graphs created:", num_graphs)
     nodes = process_channel_names(ch_names)
+    percentile = 100 - (percentage_threshold*100)
     
     G = {}
     for i in range(num_graphs):
         G[i] = nx.Graph()
         G[i].add_nodes_from(nodes, values=5)
         elegible_nodes = []
         
-        #Calculate the 75th percentile of the channels
-        threshold = np.percentile(data[(i*channels):(((i+1)*channels)-1)], 75)
+        #Calculate the percentile of top channels channels for given percentage
+        threshold = np.percentile(data[(i*channels):(((i+1)*channels)-1)], percentile)
 
 
         for j in range(channels):
             if(data[(channels * i) + j]) >= threshold:
                 elegible_nodes.append(nodes[j])
         edges = combinations(elegible_nodes,2)        
         G[i].add_edges_from(edges, weight = 1, thickness=1)
         
         
     return G
         
         
-def draw_graph(G, directed, hover_nodes):
+def draw_graph(G):
     """Process to create the networkX graphs.
     Parameters
     ----------
     G : NetworkX graph
     """
+    directed = nx.is_directed(G)
     
     #Dictionary with all the possible electrode positions. 
     
     pos = {'Cz': (0,0), 'C2h': (1.2,0), 'C2': (2.5,0), 'C4h': (3.85,0), 'C4': (5,0),'C6h': (6.20,0), 'C6': (7.6,0), 'T8h': (8.9,0), 'T8': (10.1,0), 'T10h': (11.3,0), 'T10': (12.75,0), 
            'C1h': (-1.2,0), 'C1': (-2.5,0), 'C3h': (-3.85,0), 'C3': (-5,0), 'C5h': (-6.20,0),'C5': (-7.6,0), 'T7h': (-8.9,0), 'T7': (-10.1,0), 'T9h': (-11.3,0), 'T9': (-12.75,0),
            
            'CCPz': (0, -0.95), 'CCP2h': (1.15,-0.96), 'CCP2': (2.4,-0.97), 'CCP4h': (3.8,-0.98), 'CCP4': (4.98,-0.99), 'CCP6h': (6.10,-1), 'CCP6': (7.45,-1.05),'TTP8h': (8.7,-1.10),
```

### Comparing `EEGRAPH-0.1.8/eegraph/graph.py` & `EEGRAPH-0.1.9/eegraph/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,20 @@
         if(electrode_montage_path):
             self.ch_names=input_data.set_montage(electrode_montage_path)
         
         input_data.display_info(self.ch_names)
         
 
     def modelate(self, window_size, connectivity, bands = [None], threshold = None):
-        
         print('\033[1m' + 'Model Data.' + '\033[0m')
         print(search(connectivity_measures, connectivity))
         
         model_data = ModelData(self.data, self.ch_names, eval(search(connectivity_measures, connectivity)))  
         connectivity_matrix, G = model_data.connectivity_workflow(bands, window_size, threshold)
         
         return connectivity_matrix, G
         
 
     def visualize(self, graph, name):
-        print(str(graph))
-        fig = draw_graph(graph, False, False)
+        fig = draw_graph(graph)
         fig.update_layout(title='', plot_bgcolor='white' ) 
         fig.write_html(str(name) + '_plot.html', auto_open=True, default_height='100%', default_width='100%')
```

### Comparing `EEGRAPH-0.1.8/eegraph/modelateData.py` & `EEGRAPH-0.1.9/eegraph/modelateData.py`

 * *Files identical despite different names*

### Comparing `EEGRAPH-0.1.8/eegraph/strategy.py` & `EEGRAPH-0.1.9/eegraph/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,28 +50,28 @@
         self.bands = input_bands(bands)
         data_intervals, steps, self.flag = calculate_time_intervals(data.raw_data, data.sample_rate, data.sample_duration, window_size, data.sample_length)
         self.connectivity_matrix = calculate_connectivity_single_channel_with_bands(data_intervals, data.sample_rate, self, self.bands)
         
         return self.connectivity_matrix
 
     def make_graph_workflow(self, data):
-        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels, self.bands)
+        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels, data.threshold, self.bands)
     
         return G
     
 class Connectivity_single_channel_No_Bands(Strategy):
     def calculate_connectivity_workflow(self, data, bands, window_size):
         dont_need_bands(bands)
         data_intervals, steps, self.flag = calculate_time_intervals(data.raw_data, data.sample_rate, data.sample_duration, window_size, data.sample_length)
         self.connectivity_matrix = calculate_connectivity_single_channel(data_intervals, data.sample_rate, self)
         
         return self.connectivity_matrix
 
     def make_graph_workflow(self, data):
-        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels)
+        G = single_channel_graph(self.connectivity_matrix, data.ch_names, data.num_channels, data.threshold)
     
         return G
     
 class Cross_correlation_rescaled(Strategy):
     def calculate_connectivity_workflow(self, data, bands, window_size):
         dont_need_bands(bands)
         scaled_data = re_scaling(data.raw_data)
@@ -90,15 +90,15 @@
         self.bands = input_bands(bands)
         data_intervals, steps, self.flag = calculate_time_intervals(data.raw_data, data.sample_rate, data.sample_duration, window_size, data.sample_length)
         self.connectivity_matrix = calculate_dtf(data_intervals, steps, data.num_channels, data.sample_rate, self.bands, self.flag)
         
         return self.connectivity_matrix
 
     def make_graph_workflow(self, data):
-        G = make_graph(self.connectivity_matrix, data.ch_names, data.threshold)
+        G = make_graph(self.connectivity_matrix, data.ch_names, data.threshold, True)
     
         return G    
         
         
 #Connectivity measures            
 class Cross_correlation_Estimator(Cross_correlation_rescaled):
     def __init__(self):
@@ -306,36 +306,36 @@
         phase_diff = (phase_diff  + np.pi) % (2 * np.pi) - np.pi
         pli = abs(np.mean(np.sign(phase_diff)))
         
         return pli
     
 class Power_spectrum_Estimator(Connectivity_single_channel_With_Bands):
     def __init__(self):
-        self.threshold = None
+        self.threshold = 0.25            #<----- 25%
         
     #https://www.kite.com/python/answers/how-to-plot-a-power-spectrum-in-python
     def single_channel_conn(self, data, sample_rate):
         fourier_transform = np.fft.rfft(data)
         abs_fourier_transform = np.abs(fourier_transform)
         power_spectrum = np.square(abs_fourier_transform)
         return power_spectrum.mean()    
     
 class Spectral_entropy_Estimator(Connectivity_single_channel_With_Bands):
     def __init__(self):
-        self.threshold = None
+        self.threshold = 0.25            #<----- 25%
         
     #https://raphaelvallat.com/antropy/build/html/generated/antropy.spectral_entropy.html#antropy.spectral_entropy
     def single_channel_conn(self, data, sample_rate):
         nperseg = len(data)
         se = ant.spectral_entropy(data, sample_rate, method='welch', nperseg = nperseg, normalize=True)
         return se
     
 class Shannon_entropy_Estimator(Connectivity_single_channel_No_Bands):
     def __init__(self):
-        self.threshold = None
+        self.threshold = 0.25            #<----- 25%
         
     #https://www.kite.com/python/answers/how-to-calculate-shannon-entropy-in-python
     def single_channel_conn(self, data, sample_rate):
         pd_series = pd.Series(data)
         counts = pd_series.value_counts()
         she = entropy(counts)
         return she
```

### Comparing `EEGRAPH-0.1.8/eegraph/tools.py` & `EEGRAPH-0.1.9/eegraph/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,29 @@
 from scipy import signal
 from itertools import combinations
 import networkx as nx
 import plotly.graph_objects as go
 import logging
 import warnings
 
+input_format = {'edf': 'mne.io.read_raw_edf(self.path, exclude= self.exclude)', 'gdf': 'mne.io.read_raw_gdf(self.path, exclude= self.exclude)', 'vhdr': 'mne.io.read_raw_brainvision(self.path, exclude= self.exclude)',
+               'cnt': 'mne.io.read_raw_cnt(self.path, exclude= self.exclude)', 'bdf': 'mne.io.read_raw_edf(self.path, exclude= self.exclude)', 'egi': 'mne.io.read_raw_egi(self.path, exclude= self.exclude)', 
+                'mff': 'mne.io.read_raw_egi(self.path, exclude= self.exclude)', 'nxe': 'mne.io.read_raw_eximia(self.path, exclude= self.exclude)'}
+
 connectivity_measures = {'cross_correlation': 'Cross_correlation_Estimator', 'pearson_correlation': 'Pearson_correlation_Estimator', 'squared_coherence': 'Squared_coherence_Estimator',
                          'imag_coherence': 'Imag_coherence_Estimator', 'corr_cross_correlation': 'Corr_cross_correlation_Estimator', 'wpli': 'Wpli_Estimator', 
                          'plv': 'Plv_Estimator', 'pli': 'Pli_No_Bands_Estimator', 'pli_bands': 'Pli_Bands_Estimator', 'dtf': 'Dtf_Estimator', 'power_spectrum': 'Power_spectrum_Estimator',
                          'spectral_entropy': 'Spectral_entropy_Estimator', 'shannon_entropy': 'Shannon_entropy_Estimator'}
 
+def search_input(values, searchFor):
+    for k in values:
+        if (searchFor == k):
+            return values[k]
+    raise NameError('File extension ' + "'" + searchFor + "'" + ' is not supported.')
+    
 def search(values, searchFor):
     for k in values:
         if (searchFor == k):
             return (values[k] + '()')
     raise NameError('Connectivity Measure ' + "'" + searchFor + "'" + ' does not exist.')
 
 def need_bands(bands):
@@ -412,15 +422,15 @@
         for z,item in enumerate([delta, theta, alpha, beta, gamma]):
             if bands[z]:
                 values.append(connectivity.single_channel_conn(item, sample_rate))
                 
     return values
 
 
-def make_graph(matrix, ch_names, threshold):
+def make_graph(matrix, ch_names, threshold, directed = False):
     """Process to create the networkX graphs.
     Parameters
     ----------
     matrix : ndarray
         Matrix containing all the correlation matrix.
     ch_names : list
         Channel names in the EEG.
@@ -433,56 +443,62 @@
     
     G = {}
     num_nodes = len(nodes)
     
     #Loop over the number of graphs, creating the nx Graph, adding the nodes (which will be the same in all graphs) and adding an edge if the connectivity measure is above the threshold.
     #Also we add a weight to the edge, to draw the edge´s size according to this value. It is the connectivity coefficient to a power, to really difference big from smaller coefficients. 
     for k in range(num_graphs):
-        G[k] = nx.Graph()
+        if(directed):
+            G[k] = nx.DiGraph()
+        else:
+            G[k] = nx.Graph()
+            
         G[k].add_nodes_from(nodes)
         for i in range(num_nodes):
             for j in range(num_nodes):
                 if matrix[k][i,j] > threshold and i!=j:
                     #print("graph:",k,"Edge between:", i,j)
                     G[k].add_edge(nodes[i],nodes[j], thickness = pow(matrix[k][i,j], 3) * 6, weight = matrix[k][i,j])
     
     
     return G        
 
-def single_channel_graph(data, ch_names, channels, bands=None):     
+def single_channel_graph(data, ch_names, channels, percentage_threshold, bands=None):     
     num_graphs = int(len(data)/channels)
     print("Number of graphs created:", num_graphs)
     nodes = process_channel_names(ch_names)
+    percentile = 100 - (percentage_threshold*100)
     
     G = {}
     for i in range(num_graphs):
         G[i] = nx.Graph()
         G[i].add_nodes_from(nodes, values=5)
         elegible_nodes = []
         
-        #Calculate the 75th percentile of the channels
-        threshold = np.percentile(data[(i*channels):(((i+1)*channels)-1)], 75)
+        #Calculate the percentile of top channels channels for given percentage
+        threshold = np.percentile(data[(i*channels):(((i+1)*channels)-1)], percentile)
 
 
         for j in range(channels):
             if(data[(channels * i) + j]) >= threshold:
                 elegible_nodes.append(nodes[j])
         edges = combinations(elegible_nodes,2)        
         G[i].add_edges_from(edges, weight = 1, thickness=1)
         
         
     return G
         
         
-def draw_graph(G, directed, hover_nodes):
+def draw_graph(G):
     """Process to create the networkX graphs.
     Parameters
     ----------
     G : NetworkX graph
     """
+    directed = nx.is_directed(G)
     
     #Dictionary with all the possible electrode positions. 
     
     pos = {'Cz': (0,0), 'C2h': (1.2,0), 'C2': (2.5,0), 'C4h': (3.85,0), 'C4': (5,0),'C6h': (6.20,0), 'C6': (7.6,0), 'T8h': (8.9,0), 'T8': (10.1,0), 'T10h': (11.3,0), 'T10': (12.75,0), 
            'C1h': (-1.2,0), 'C1': (-2.5,0), 'C3h': (-3.85,0), 'C3': (-5,0), 'C5h': (-6.20,0),'C5': (-7.6,0), 'T7h': (-8.9,0), 'T7': (-10.1,0), 'T9h': (-11.3,0), 'T9': (-12.75,0),
            
            'CCPz': (0, -0.95), 'CCP2h': (1.15,-0.96), 'CCP2': (2.4,-0.97), 'CCP4h': (3.8,-0.98), 'CCP4': (4.98,-0.99), 'CCP6h': (6.10,-1), 'CCP6': (7.45,-1.05),'TTP8h': (8.7,-1.10),
```

### Comparing `EEGRAPH-0.1.8/setup.py` & `EEGRAPH-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
             
     this_directory = path.abspath(path.dirname(__file__))
     with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
 
 setup(
     name='EEGRAPH',
-    version='0.1.8',
+    version='0.1.9',
     description='',
     url='https://github.com/ufvceiec/EEGRAPH',
     author='CEIEC',
     license= 'GPL-3.0',
     classifers=classifiers,
     keywords='',
     packages=find_packages(),
```

### Comparing `EEGRAPH-0.1.8/tests/.ipynb_checkpoints/tests-checkpoint.py` & `EEGRAPH-0.1.9/tests/.ipynb_checkpoints/tests-checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,38 +274,38 @@
         channels = 16
         data = [([0.54337644]), ([-0.85042714]), ([-0.63641063]), ([0.02879978]), ([0.97642451]), ([0.47373244]), ([-0.13785667]), ([-0.19336038]), ([0.55023686]), ([-0.05053916]), ([0.34913885]), 
                 ([-0.10666878]), ([0.94642219]), ([0.20702023]), ([-0.16919901]), ([-0.17072353])]
         
         ch_names = ['Fp1', 'Fp2', 'AF7', 'AF3', 'AF4', 'AF8', 'F7', 'F5', 'F3', 'F1', 'Fz', 'F2', 'F4', 'F6', 'F8', 'FT9']
         expected_edges = 6 #All edges between top 25% nodes. 16 channels -> 4 nodes with connections. All 4 nodes interconnected -> 6 edges in total. 
         
-        result = single_channel_graph(data, ch_names, channels)
+        result = single_channel_graph(data, ch_names, channels, 0.25)
         self.assertEqual(len(result[0].nodes()), channels)
         self.assertEqual(len(result[0].edges()), expected_edges)
     
     def test_draw_graph(self):
         G1 = nx.Graph()
         nodes_list = ['Fp1', 'Fp2', 'AF7', 'AF3', 'AF4', 'AF8', 'F7', 'F5', 'F3', 'F1', 'Fz', 'F2', 'F4', 'F6', 'F8', 'FT9']
         edges_list = [('Fp1', 'Fp2'), ('Fp1', 'AF3'), ('Fp1', 'F7'), ('AF7', 'AF3'), ('AF8', 'F7')]
         G1.add_nodes_from(nodes_list)
         for pair in edges_list:
             G1.add_edge(pair[0], pair[1], weight=1, thickness=1)
     
-        self.assertTrue(draw_graph(G1, False, False))
+        self.assertTrue(draw_graph(G1))
         
     def test_draw_graph_unkown_node(self):
         G1 = nx.Graph()
         nodes_list = ['Fp1', 'Fp2', 'AF7', 'AF3', 'AF4', 'AF8', 'XX', 'F5', 'F3', 'F1', 'Fz', 'F2', 'F4', 'F6', 'F8', 'FT9']
         edges_list = [('Fp1', 'Fp2'), ('Fp1', 'AF3'), ('Fp1', 'F7'), ('AF7', 'AF3'), ('AF8', 'F7')]
         G1.add_nodes_from(nodes_list)
         for pair in edges_list:
             G1.add_edge(pair[0], pair[1], weight=1, thickness=1)
     
         with self.assertWarns(Warning):
-            draw_graph(G1, True, True)
+            draw_graph(G1)
     
 
 class TestImportData(unittest.TestCase):
     
     def test_load_data(self):
         path = '.chb02_16.edf'                               #Public EEG dataset. https://physionet.org/content/chbmit/1.0.0/
         channels = 23
```

### Comparing `EEGRAPH-0.1.8/tests/tests.py` & `EEGRAPH-0.1.9/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,38 +274,38 @@
         channels = 16
         data = [([0.54337644]), ([-0.85042714]), ([-0.63641063]), ([0.02879978]), ([0.97642451]), ([0.47373244]), ([-0.13785667]), ([-0.19336038]), ([0.55023686]), ([-0.05053916]), ([0.34913885]), 
                 ([-0.10666878]), ([0.94642219]), ([0.20702023]), ([-0.16919901]), ([-0.17072353])]
         
         ch_names = ['Fp1', 'Fp2', 'AF7', 'AF3', 'AF4', 'AF8', 'F7', 'F5', 'F3', 'F1', 'Fz', 'F2', 'F4', 'F6', 'F8', 'FT9']
         expected_edges = 6 #All edges between top 25% nodes. 16 channels -> 4 nodes with connections. All 4 nodes interconnected -> 6 edges in total. 
         
-        result = single_channel_graph(data, ch_names, channels)
+        result = single_channel_graph(data, ch_names, channels, 0.25)
         self.assertEqual(len(result[0].nodes()), channels)
         self.assertEqual(len(result[0].edges()), expected_edges)
     
     def test_draw_graph(self):
         G1 = nx.Graph()
         nodes_list = ['Fp1', 'Fp2', 'AF7', 'AF3', 'AF4', 'AF8', 'F7', 'F5', 'F3', 'F1', 'Fz', 'F2', 'F4', 'F6', 'F8', 'FT9']
         edges_list = [('Fp1', 'Fp2'), ('Fp1', 'AF3'), ('Fp1', 'F7'), ('AF7', 'AF3'), ('AF8', 'F7')]
         G1.add_nodes_from(nodes_list)
         for pair in edges_list:
             G1.add_edge(pair[0], pair[1], weight=1, thickness=1)
     
-        self.assertTrue(draw_graph(G1, False, False))
+        self.assertTrue(draw_graph(G1))
         
     def test_draw_graph_unkown_node(self):
         G1 = nx.Graph()
         nodes_list = ['Fp1', 'Fp2', 'AF7', 'AF3', 'AF4', 'AF8', 'XX', 'F5', 'F3', 'F1', 'Fz', 'F2', 'F4', 'F6', 'F8', 'FT9']
         edges_list = [('Fp1', 'Fp2'), ('Fp1', 'AF3'), ('Fp1', 'F7'), ('AF7', 'AF3'), ('AF8', 'F7')]
         G1.add_nodes_from(nodes_list)
         for pair in edges_list:
             G1.add_edge(pair[0], pair[1], weight=1, thickness=1)
     
         with self.assertWarns(Warning):
-            draw_graph(G1, True, True)
+            draw_graph(G1)
     
 
 class TestImportData(unittest.TestCase):
     
     def test_load_data(self):
         path = '.chb02_16.edf'                               #Public EEG dataset. https://physionet.org/content/chbmit/1.0.0/
         channels = 23
```

