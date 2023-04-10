# Comparing `tmp/eco2ai-0.3.8.tar.gz` & `tmp/eco2ai-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eco2ai-0.3.8.tar", max compression
+gzip compressed data, was "eco2ai-0.3.9.tar", max compression
```

## Comparing `eco2ai-0.3.8.tar` & `eco2ai-0.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11405 2023-03-09 16:30:49.966410 eco2ai-0.3.8/LICENSE
--rw-r--r--   0        0        0     7972 2023-03-09 16:30:49.966691 eco2ai-0.3.8/README.md
--rw-r--r--   0        0        0       38 2023-03-09 16:30:49.969077 eco2ai-0.3.8/eco2ai/MLTracker.py
--rw-r--r--   0        0        0      345 2023-03-09 16:30:49.969239 eco2ai-0.3.8/eco2ai/__init__.py
--rw-r--r--   0        0        0   167304 2023-03-09 16:30:49.970662 eco2ai-0.3.8/eco2ai/data/carbon_index.csv
--rw-r--r--   0        0        0        0 2023-03-09 16:30:49.970821 eco2ai-0.3.8/eco2ai/data/config.txt
--rw-r--r--   0        0        0    93293 2023-03-09 16:30:49.971446 eco2ai-0.3.8/eco2ai/data/cpu_names.csv
--rw-r--r--   0        0        0    30281 2023-03-09 19:50:31.211828 eco2ai-0.3.8/eco2ai/emission_track.py
--rw-r--r--   0        0        0     6148 2023-03-09 16:30:49.971970 eco2ai-0.3.8/eco2ai/tools/.DS_Store
--rw-r--r--   0        0        0        0 2023-03-09 16:30:49.972035 eco2ai-0.3.8/eco2ai/tools/__init__.py
--rw-r--r--   0        0        0    20544 2023-03-09 16:30:49.972244 eco2ai-0.3.8/eco2ai/tools/tools_cpu.py
--rw-r--r--   0        0        0     8767 2023-03-09 16:30:49.972401 eco2ai-0.3.8/eco2ai/tools/tools_gpu.py
--rw-r--r--   0        0        0     2794 2023-03-09 16:30:49.972616 eco2ai-0.3.8/eco2ai/tools/tools_ram.py
--rw-r--r--   0        0        0    18039 2023-03-09 16:30:49.972807 eco2ai-0.3.8/eco2ai/utils.py
--rw-r--r--   0        0        0     1600 2023-03-09 16:33:33.300965 eco2ai-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     9289 2023-03-09 19:54:44.622666 eco2ai-0.3.8/setup.py
--rw-r--r--   0        0        0     9650 2023-03-09 19:54:44.623304 eco2ai-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11405 2023-03-09 16:30:49.966410 eco2ai-0.3.9/LICENSE
+-rw-r--r--   0        0        0     7972 2023-03-09 16:30:49.966691 eco2ai-0.3.9/README.md
+-rw-r--r--   0        0        0       38 2023-03-09 16:30:49.969077 eco2ai-0.3.9/eco2ai/MLTracker.py
+-rw-r--r--   0        0        0      345 2023-03-09 16:30:49.969239 eco2ai-0.3.9/eco2ai/__init__.py
+-rw-r--r--   0        0        0   167304 2023-03-09 16:30:49.970662 eco2ai-0.3.9/eco2ai/data/carbon_index.csv
+-rw-r--r--   0        0        0        0 2023-03-09 16:30:49.970821 eco2ai-0.3.9/eco2ai/data/config.txt
+-rw-r--r--   0        0        0    93293 2023-03-09 16:30:49.971446 eco2ai-0.3.9/eco2ai/data/cpu_names.csv
+-rw-r--r--   0        0        0    30281 2023-04-10 09:50:14.475511 eco2ai-0.3.9/eco2ai/emission_track.py
+-rw-r--r--   0        0        0     6148 2023-03-09 16:30:49.971970 eco2ai-0.3.9/eco2ai/tools/.DS_Store
+-rw-r--r--   0        0        0        0 2023-03-09 16:30:49.972035 eco2ai-0.3.9/eco2ai/tools/__init__.py
+-rw-r--r--   0        0        0    20544 2023-03-09 16:30:49.972244 eco2ai-0.3.9/eco2ai/tools/tools_cpu.py
+-rw-r--r--   0        0        0     8776 2023-04-10 09:50:12.786519 eco2ai-0.3.9/eco2ai/tools/tools_gpu.py
+-rw-r--r--   0        0        0     2794 2023-03-09 16:30:49.972616 eco2ai-0.3.9/eco2ai/tools/tools_ram.py
+-rw-r--r--   0        0        0    18039 2023-03-09 16:30:49.972807 eco2ai-0.3.9/eco2ai/utils.py
+-rw-r--r--   0        0        0     1600 2023-04-10 09:50:19.697665 eco2ai-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     9289 2023-04-10 09:53:50.792498 eco2ai-0.3.9/setup.py
+-rw-r--r--   0        0        0     9650 2023-04-10 09:53:50.793059 eco2ai-0.3.9/PKG-INFO
```

### Comparing `eco2ai-0.3.8/LICENSE` & `eco2ai-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/README.md` & `eco2ai-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/data/carbon_index.csv` & `eco2ai-0.3.9/eco2ai/data/carbon_index.csv`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/data/cpu_names.csv` & `eco2ai-0.3.9/eco2ai/data/cpu_names.csv`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/emission_track.py` & `eco2ai-0.3.9/eco2ai/emission_track.py`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/tools/.DS_Store` & `eco2ai-0.3.9/eco2ai/tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/tools/tools_cpu.py` & `eco2ai-0.3.9/eco2ai/tools/tools_cpu.py`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/tools/tools_gpu.py` & `eco2ai-0.3.9/eco2ai/tools/tools_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             deviceCount = pynvml.nvmlDeviceGetCount()
             gpus_name = []
             for i in range(deviceCount):
                 handle = pynvml.nvmlDeviceGetHandleByIndex(i)
                 pynvml.nvmlDeviceGetPowerUsage(handle)
                 gpus_name.append(pynvml.nvmlDeviceGetName(handle))
             pynvml.nvmlShutdown()
-            return gpus_name[0].decode("UTF-8")
+            return gpus_name[0].encode().decode("UTF-8")
         except:
             return ""
     
     def gpu_num(self):
         """
             This class method returns number of visible GPU devices.
             Pynvml library is used.
```

### Comparing `eco2ai-0.3.8/eco2ai/tools/tools_ram.py` & `eco2ai-0.3.9/eco2ai/tools/tools_ram.py`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/eco2ai/utils.py` & `eco2ai-0.3.9/eco2ai/utils.py`

 * *Files identical despite different names*

### Comparing `eco2ai-0.3.8/pyproject.toml` & `eco2ai-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eco2ai"
-version = "0.3.8"
+version = "0.3.9"
 description = "emission tracking library"
 authors = ["AI Lab",
             "Vladimir Lazarev <lazarev@airi.net>",
             "Nikita Zakharenko <nnzakharenko@sberbank.ru>",
             "Semyon Budyonny  <sanbudenny@sberbank.ru>",
             "leonid zhukov <lezhukov@sberbank.ru>"]
```

### Comparing `eco2ai-0.3.8/setup.py` & `eco2ai-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  ':python_version >= "3.6"': ['pynvml', 'tzlocal'],
  ':python_version >= "3.7"': ['tornado', 'py-cpuinfo'],
  ':python_version >= "3.7" and python_version < "4"': ['requests'],
  ':python_version >= "3.8"': ['pandas>=1.4.0,<=1.4.3']}
 
 setup_kwargs = {
     'name': 'eco2ai',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'emission tracking library',
     'long_description': '<img src=https://github.com/sb-ai-lab/Eco2AI/blob/main/images/photo_2022-06-14_13-02-37.jpg />\n\n\n![PyPI Downloads](https://img.shields.io/pypi/dm/eco2ai?color=brightgreen&label=PyPI%20downloads&logo=pypi&logoColor=yellow)\n[![PyPI all Downloads](https://img.shields.io/badge/All%20PyPI%20downloads-look%20in%20Colab-brightgreen)](https://colab.research.google.com/drive/1UoSHPRUHbg5B1U2x8p_ACo21X9N6n1im?authuser=1)\n\n\n[![PyPI - Downloads](https://img.shields.io/badge/%20PyPI%20-link%20for%20download-brightgreen)](https://pypi.org/project/eco2ai/)\n![PyPI - Downloads](https://img.shields.io/pypi/v/eco2ai?color=bright-green&label=PyPI&logo=pypi&logoColor=yellow)\n[![DOI](https://img.shields.io/badge/DOI-eco2AI%20article-brightgreen)](https://link.springer.com/article/10.1134/S1064562422060230)\n[![telegram support](https://img.shields.io/twitter/url?label=eco2ai%20support&logo=telegram&style=social&url=https%3A%2F%2Ft.me%2F%2BjsaoAgioprQ4Zjk6)](https://t.me/eco2ai)\n\n# Eco2AI\n\n+ [About Eco2AI :clipboard:](#1)\n+ [Installation :wrench:](#2)\n+ [Use examples :computer:](#3)\n+ [Important note :blue_book:](#4)\n+ [Citing](#5)\n+ [Feedback :envelope:](#6) \n\n\n\n\n\n## About Eco2AI :clipboard: <a name="1"></a> \nThe Eco2AI is a python library for CO<sub>2</sub> emission tracking. It monitors energy consumption of CPU & GPU devices and estimates equivalent carbon emissions taking into account the regional emission coefficient. \nThe Eco2AI is applicable to all python scripts and all you need is to add the couple of strings to your code. All emissions data and information about your devices are recorded in a local file. \n\nEvery single run of Tracker() accompanies by a session description added to the log file, including the following elements:\n                              \n\n+ project_name\n+ experiment_description\n+ start_time\n+ duration(s)\n+ power_consumption(kWTh)\n+ CO<sub>2</sub>_emissions(kg)\n+ CPU_name\n+ GPU_name\n+ OS\n+ country\n\n##  Installation <a name="2"></a> \nTo install the eco2AI library, run the following command:\n\n```\npip install eco2ai\n```\n\n## Use examples <a name="3"></a> \n\nExample usage eco2AI [![Open In Collab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hn0DQiKHeyXwvOOR3UEXaGsD6DqVm6b7?authuser=1)\nYou can also find eco2AI tutorial on youtube [![utube](https://img.shields.io/youtube/views/-fegQpA2gPg?label=eco2AI&style=social)](https://www.youtube.com/watch?v=-fegQpA2gPg&ab_channel=AIRIInstitute)\n\nThe eco2AI interface is quite simple. Here is the simplest usage example:\n\n```python\n\nimport eco2ai\n\ntracker = eco2ai.Tracker(project_name="YourProjectName", experiment_description="training the <your model> model")\n\ntracker.start()\n\n<your gpu &(or) cpu calculations>\n\ntracker.stop()\n```\n\nThe eco2AI also supports decorators. As soon as the decorated function is executed, the information about the emissions will be written to the emission.csv file:\n\n```python\nfrom eco2ai import track\n\n@track\ndef train_func(model, dataset, optimizer, epochs):\n    ...\n\ntrain_func(your_model, your_dataset, your_optimizer, your_epochs)\n```\n\nFor your convenience, every time you instantiate the Tracker object with your custom parameters, these settings will be saved until the library is deleted. Each new tracker will be created with your custom settings (if you create a tracker with new parameters, they will be saved instead of the old ones). For example:\n\n```python\nimport eco2ai\n\ntracker = eco2ai.Tracker(\n    project_name="YourProjectName", \n    experiment_description="training <your model> model",\n    file_name="emission.csv"\n    )\n\ntracker.start()\n<your gpu &(or) cpu calculations>\ntracker.stop()\n\n...\n\n# now, we want to create a new tracker for new calculations\ntracker = eco2ai.Tracker()\n# now, it\'s equivalent to:\n# tracker = eco2ai.Tracker(\n#     project_name="YourProjectName", \n#     experiment_description="training the <your model> model",\n#     file_name="emission.csv"\n# )\ntracker.start()\n<your gpu &(or) cpu calculations>\ntracker.stop()\n\n```\n\nYou can also set parameters using the set_params() function, as in the example below:\n\n```python\nfrom eco2ai import set_params, Tracker\n\nset_params(\n    project_name="My_default_project_name",\n    experiment_description="We trained...",\n    file_name="my_emission_file.csv"\n)\n\ntracker = Tracker()\n# now, it\'s equivelent to:\n# tracker = Tracker(\n#     project_name="My_default_project_name",\n#     experiment_description="We trained...",\n#     file_name="my_emission_file.csv"\n# )\ntracker.start()\n<your code>\ntracker.stop()\n```\n\n\n\n<!-- There is [sber_emission_tracker_guide.ipynb](https://github.com/vladimir-laz/AIRIEmisisonTracker/blob/704ff88468f6ad403d69a63738888e1a3c41f59b/guide/sber_emission_tracker_guide.ipynb)  - useful jupyter notebook with more examples and notes. We highly recommend to check it out beforehand. -->\n## Important note <a name="4"></a> \n\nIf for some reasons it is not possible to define country, then emission coefficient is set to 436.529kg/MWh, which is global average.\n[Global Electricity Review](https://ember-climate.org/insights/research/global-electricity-review-2022/#supporting-material-downloads)\n\nFor proper calculation of gpu and cpu power consumption, you should create a "Tracker" before any gpu or CPU usage.\n\nCreate a new “Tracker” for every new calculation.\n\n# Usage of Eco2AI\n\nAn example of using the library is given in the [publication](https://arxiv.org/abs/2208.00406). It the paper we presented experiments of tracking equivalent CO<sub>2</sub> emissions using eco2AI while training [ruDALL-E](https://github.com/sberbank-ai/ru-dalle) models with with 1.3 billion ([Malevich](https://habr.com/ru/company/sberbank/blog/589673/), ruDALL-E XL 1.3B) and 12 billion parameters ([Kandinsky](https://github.com/sberbank-ai/ru-dalle), ruDALL-E XL 12B). These are [multimodal](https://arxiv.org/abs/2202.10435) pre-trained transformers that learn the conditional distribution of images with by some string of text capable of generating arbitrary images from a russian text prompt that describes the desired result.\nProperly accounted carbon emissions and power consumption Malevich and Kandinsky fine-tuning Malevich and Kandinsky on the [Emojis dataset](https://arxiv.org/abs/2112.02448) is given in the table below.\n   \n   | **Model** | **Train time** | **Power, kWh** | **CO<sub>2</sub>, kg** | **GPU** | **CPU** | **Batch Size** |\n   |:----------|:-------------:|:------:| :-----: |:-----:|:------:|:------:|\n   | **Malevich**| 4h 19m | 1.37 | **0.33** | A100 Graphics, 1 | AMD EPYC 7742 64-Core | 4 |\n   | **Kandinsky** | 9h 45m | 24.50 | **5.89** | A100 Graphics, 8 | AMD EPYC 7742 64-Core | 12 |\n\nAlso we presented results for training of Malevich with optimized variation of [GELU](https://arxiv.org/abs/1606.08415) activation function. Training of the Malevich with the [8-bit version of GELU](https://arxiv.org/abs/2110.02861) allows us to spent about 10\\% less energy and, consequently, produce less equivalent CO<sub>2</sub> emissions.\n\n# Citing Eco2AI\n[![DOI](https://img.shields.io/badge/DOI-eco2AI%20article-brightgreen)](https://link.springer.com/article/10.1134/S1064562422060230)\n\nThe Eco2AI is licensed under a [Apache licence 2.0](https://www.apache.org/licenses/LICENSE-2.0).\n\nPlease consider citing the following paper in any research manuscript using the Eco2AI library:\n\n```\n@inproceedings{budennyy2023eco2ai,\n  title={Eco2ai: carbon emissions tracking of machine learning models as the first step towards sustainable ai},\n  author={Budennyy, SA and Lazarev, VD and Zakharenko, NN and Korovin, AN and Plosskaya, OA and Dimitrov, DV and Akhripkin, VS and Pavlov, IV and Oseledets, IV and Barsola, IS and others},\n  booktitle={Doklady Mathematics},\n  pages={1--11},\n  year={2023},\n  organization={Springer}\n}\n```\n\n## In collaboration with\n[<img src="https://github.com/sb-ai-lab/Eco2AI/blob/main/images/AIRI%20-%20Full%20logo%20(2).png" width="200"/>](https://airi.net/)\n',
     'author': 'AI Lab',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sb-ai-lab/Eco2AI',
```

### Comparing `eco2ai-0.3.8/PKG-INFO` & `eco2ai-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eco2ai
-Version: 0.3.8
+Version: 0.3.9
 Summary: emission tracking library
 Home-page: https://github.com/sb-ai-lab/Eco2AI
 Author: AI Lab
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

