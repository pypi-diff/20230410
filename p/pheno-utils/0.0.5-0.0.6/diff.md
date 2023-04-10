# Comparing `tmp/pheno-utils-0.0.5.tar.gz` & `tmp/pheno-utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.0.5.tar", last modified: Thu Apr  6 20:38:38 2023, max compression
+gzip compressed data, was "pheno-utils-0.0.6.tar", last modified: Mon Apr 10 19:49:48 2023, max compression
```

## Comparing `pheno-utils-0.0.5.tar` & `pheno-utils-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-06 20:38:38.322388 pheno-utils-0.0.5/
--rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.5/LICENSE
--rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.5/MANIFEST.in
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-06 20:38:38.321987 pheno-utils-0.0.5/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.5/README.md
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-06 20:38:38.318053 pheno-utils-0.0.5/pheno_utils/
--rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/__init__.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-06 20:10:17.000000 pheno-utils-0.0.5/pheno_utils/_modidx.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/age_reference_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/basic_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/config.py
--rw-r--r--   0 alondmnt   (501) staff       (20)    11460 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/data_loader.py
--rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-06 20:09:00.000000 pheno-utils-0.0.5/pheno_utils/dates_plots.py
-drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-06 20:38:38.321334 pheno-utils-0.0.5/pheno_utils.egg-info/
--rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-06 20:38:38.000000 pheno-utils-0.0.5/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-06 20:38:38.000000 pheno-utils-0.0.5/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 20:38:38.000000 pheno-utils-0.0.5/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-06 20:38:38.000000 pheno-utils-0.0.5/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.5/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-06 20:38:38.000000 pheno-utils-0.0.5/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-06 20:38:38.000000 pheno-utils-0.0.5/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-06 20:15:47.000000 pheno-utils-0.0.5/settings.ini
--rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-06 20:38:38.322530 pheno-utils-0.0.5/setup.cfg
--rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.5/setup.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 19:49:48.599118 pheno-utils-0.0.6/
+-rw-r--r--   0 alondmnt   (501) staff       (20)    11357 2023-04-06 20:07:34.000000 pheno-utils-0.0.6/LICENSE
+-rw-r--r--   0 alondmnt   (501) staff       (20)      111 2023-04-06 20:07:42.000000 pheno-utils-0.0.6/MANIFEST.in
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 19:49:48.598790 pheno-utils-0.0.6/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      446 2023-04-06 20:07:47.000000 pheno-utils-0.0.6/README.md
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 19:49:48.595678 pheno-utils-0.0.6/pheno_utils/
+-rw-r--r--   0 alondmnt   (501) staff       (20)       22 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/__init__.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     8743 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/_modidx.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    16963 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2333 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/basic_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2517 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2740 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/config.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)    12339 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/data_loader.py
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2825 2023-04-10 19:46:34.000000 pheno-utils-0.0.6/pheno_utils/dates_plots.py
+drwxr-xr-x   0 alondmnt   (501) staff       (20)        0 2023-04-10 19:49:48.598373 pheno-utils-0.0.6/pheno_utils.egg-info/
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1479 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alondmnt   (501) staff       (20)      515 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       65 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)        1 2023-04-06 08:56:36.000000 pheno-utils-0.0.6/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 alondmnt   (501) staff       (20)       99 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)       12 2023-04-10 19:49:48.000000 pheno-utils-0.0.6/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 alondmnt   (501) staff       (20)     1040 2023-04-10 19:45:23.000000 pheno-utils-0.0.6/settings.ini
+-rw-r--r--   0 alondmnt   (501) staff       (20)       38 2023-04-10 19:49:48.599242 pheno-utils-0.0.6/setup.cfg
+-rw-r--r--   0 alondmnt   (501) staff       (20)     2560 2023-04-06 20:07:57.000000 pheno-utils-0.0.6/setup.py
```

### Comparing `pheno-utils-0.0.5/LICENSE` & `pheno-utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/PKG-INFO` & `pheno-utils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.5/pheno_utils/_modidx.py` & `pheno-utils-0.0.6/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/pheno_utils/age_reference_plots.py` & `pheno-utils-0.0.6/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/pheno_utils/basic_plots.py` & `pheno-utils-0.0.6/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.0.6/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/pheno_utils/config.py` & `pheno-utils-0.0.6/pheno_utils/config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/pheno_utils/data_loader.py` & `pheno-utils-0.0.6/pheno_utils/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     Args:
     
         dataset (str): The name of the dataset to load.
         cohort (str, optional): The name of the cohort within the dataset. Defaults to '10k'.
         base_path (str, optional): The base path where the data is stored. Defaults to '/home/ec2-user/studies'.
         age_sex_dataset (str, optional): The name of the dataset to use for computing age and sex. Defaults to 'Population_Characteristics'.
+        skip_dfs (list, optional): A list of tables (or substrings that match to tables) to skip when loading the data. Defaults to [].
         unique_index (bool, optional): Whether to ensure the index of the data is unique. Defaults to False.
         valid_dates (bool, optional): Whether to ensure that all timestamps in the data are valid dates. Defaults to False.
         valid_stage (bool, optional): Whether to ensure that all research stages in the data are valid. Defaults to False.
         errors (str, optional): Whether to raise an error or issue a warning if missing data is encountered.
             Possible values are 'raise' and 'warn'. Defaults to 'raise'.
 
     Attributes:
@@ -37,49 +38,52 @@
         dict (pd.DataFrame): The data dictionary for the dataset, containing information about each field.
         dfs (dict): A dictionary of dataframes, one for each table in the dataset.
         fields (list): A list of all fields in the dataset.
         dataset (str): The name of the dataset being used.
         cohort (str): The name of the cohort being used.
         base_path (str): The base path where the data is stored.
         age_sex_dataset (str): The name of the dataset being used to compute age and sex.
+        skip_dfs (list): A list of tables to skip when loading the data.
         unique_index (bool): Whether to ensure the index of the data is unique.
         valid_dates (bool): Whether to ensure that all timestamps in the data are valid dates.
         valid_stage (bool): Whether to ensure that all research stages in the data are valid.
         errors (str): Whether to raise an error or issue a warning if missing data is encountered.
     """
 
     def __init__(
         self,
         dataset: str,
         cohort: str = '10k',
         base_path: str = DATASETS_PATH,
         age_sex_dataset: str = POPULATION_DATASET,
+        skip_dfs: List[str] = [],
         unique_index: bool = False,
         valid_dates: bool = False,
         valid_stage: bool = False,
         errors: str = 'raise'
     ) -> None:
         self.dataset = dataset
         self.cohort = cohort
         self.base_path = base_path
         self.age_sex_dataset = age_sex_dataset
+        self.skip_dfs = skip_dfs
         self.unique_index = unique_index
         self.valid_dates = valid_dates
         self.valid_stage = valid_stage
         self.errors = errors
 
         self.__load_dictionary__()
         self.__load_dataframes__()
         if self.age_sex_dataset is not None:
             self.__load_age_sex__()
 
     def load_sample_data(
         self,
         field_name: str,
-        participant_id: Union[str, List[str]],
+        participant_id: Union[int, List[int]],
         research_stage: Union[None, str, List[str]] = None,
         array_index: Union[None, int, List[int]] = None,
         load_func: callable = pd.read_parquet,
         concat: bool = True
     ) -> Union[pd.DataFrame, None]:
         """
         Load time series or bulk data for sample(s).
@@ -119,14 +123,16 @@
             if len(sample) == 0:
                 return None
 
         data = []
         for p in sample.unique():
             try:
                 data.append(load_func(p))
+                if isinstance(data[-1], pd.DataFrame):
+                    data[-1].sort_index(inplace=True)
             except Exception as e:
                 if self.errors == 'raise':
                     raise e
                 elif self.errors == 'warn':
                     warnings.warn(f'Error loading {p}: {e}')
         if concat:
             data = pd.concat(data, axis=0)
@@ -199,28 +205,29 @@
         Add sex and compute age from birth date.
         """
         age_path = os.path.join(
             self.base_path,
             self.age_sex_dataset,
             self.cohort,
             'events.parquet')
-        age_df = pd.read_parquet(age_path)
         align_df = self.dfs[list(self.dfs)[0]]
 
         # TODO: check if research stage is "continuous"
         if ('research_stage' in align_df.columns) or ('research_stage' in align_df.index.names):
+            age_df = pd.read_parquet(age_path)
             self.dfs['age_sex'] = align_df.join(
                 age_df[['age_at_research_stage', 'sex']].droplevel('array_index'))\
                 .rename(columns={'age_at_research_stage': 'age'})
             self.fields += ['age', 'sex']
             return
 
         date_cols = np.array(['collection_timestamp', 'collection_date', 'sequencing_date'])
         date = date_cols[np.isin(date_cols, align_df.columns)][0]  # prefer first match
 
+        age_df = pd.read_parquet(age_path.replace('events', 'population'))
         age_df['birth_date'] = pd.to_datetime(
             age_df['year_of_birth'].astype(str) + '-' + age_df['month_of_birth'].astype(str))
 
         self.dfs['age_sex'] = align_df[[date]].join(age_df[['sex', 'birth_date']])\
             .assign(age=lambda x: ((x[date].dt.date - x['birth_date'].dt.date).dt.days / 365.25).round(1))\
             .drop(columns=['birth_date'])
         self.fields += ['age', 'sex']
@@ -228,14 +235,17 @@
     def __load_dataframes__(self) -> None:
         """
         Load all tables in the dataset dictionary.
         """
         self.dfs = {}
         self.fields = set()
         for relative_location in self.dict['relative_location'].dropna().unique():
+            if any([pattern in relative_location for pattern in self.skip_dfs]):
+                print(f'Skipping {relative_location}')
+                continue
             self.dfs[relative_location.split('.')[0]] = self.__load_one_dataframe__(relative_location)
             self.fields |= set(self.dfs[relative_location.split('.')[0]].columns.tolist())
         self.fields = list(self.fields)
 
     def __load_one_dataframe__(self, relative_location: str) -> pd.DataFrame:
         """
         Load one dataframe.
@@ -247,15 +257,23 @@
             pd.DataFrame: the loaded dataframe
         """
         df_path = os.path.join(
             self.base_path,
             self.dataset,
             self.cohort,
             relative_location)
-        data =  pd.read_parquet(df_path)
+        try:
+            data =  pd.read_parquet(df_path)
+        except Exception as err:
+            if self.errors == 'raise':
+                raise err
+            if self.errors == 'warn':
+                warnings.warn(f'Error loading {df_path}:\n{err}')
+            return pd.DataFrame()
+
         # set the order of columns according to the dictionary
         dict_columns = self.dict.index.intersection(data.columns)
         other_columns = data.columns.difference(self.dict.index)
         assert (len(dict_columns) + len(other_columns)) == len(data.columns), "something isn't right"
         data = data[dict_columns.tolist() + other_columns.tolist()]
 
         before = len(data)
```

### Comparing `pheno-utils-0.0.5/pheno_utils/dates_plots.py` & `pheno-utils-0.0.6/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.0.6/pheno_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/hrossman/pheno-utils
 Author: hrossman
 Author-email: hagairossman@gmail.com
 License: Apache Software License 2.0
 Description: pheno-utils
         ================
```

### Comparing `pheno-utils-0.0.5/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.0.6/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.0.5/settings.ini` & `pheno-utils-0.0.6/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = pheno-utils
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = pheno_utils
```

### Comparing `pheno-utils-0.0.5/setup.py` & `pheno-utils-0.0.6/setup.py`

 * *Files identical despite different names*

