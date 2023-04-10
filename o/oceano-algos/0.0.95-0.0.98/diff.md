# Comparing `tmp/oceano_algos-0.0.95.tar.gz` & `tmp/oceano_algos-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceano_algos-0.0.95.tar", last modified: Mon Apr  3 19:56:42 2023, max compression
+gzip compressed data, was "oceano_algos-0.0.98.tar", last modified: Mon Apr 10 08:47:52 2023, max compression
```

## Comparing `oceano_algos-0.0.95.tar` & `oceano_algos-0.0.98.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-03 19:56:42.958701 oceano_algos-0.0.95/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      110 2023-01-17 20:50:26.000000 oceano_algos-0.0.95/MANIFEST.in
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-03 19:56:42.958701 oceano_algos-0.0.95/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      886 2023-01-22 15:00:56.000000 oceano_algos-0.0.95/README.md
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-03 19:56:42.954701 oceano_algos-0.0.95/oceano_algos/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       23 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/__init__.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2538 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/_nbdev.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      209 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/core.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     7402 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/hh_parser.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    10162 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/notificator.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    32653 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/parser.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     7049 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/postgres.py
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2478 2023-04-03 19:56:33.000000 oceano_algos-0.0.95/oceano_algos/preprocessor.py
-drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-03 19:56:42.958701 oceano_algos-0.0.95/oceano_algos.egg-info/
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-03 19:56:42.000000 oceano_algos-0.0.95/oceano_algos.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      422 2023-04-03 19:56:42.000000 oceano_algos-0.0.95/oceano_algos.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)        1 2023-04-03 19:56:42.000000 oceano_algos-0.0.95/oceano_algos.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      180 2023-04-03 19:56:42.000000 oceano_algos-0.0.95/oceano_algos.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       13 2023-04-03 19:56:42.000000 oceano_algos-0.0.95/oceano_algos.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      651 2023-04-03 19:54:01.000000 oceano_algos-0.0.95/settings.ini
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       38 2023-04-03 19:56:42.958701 oceano_algos-0.0.95/setup.cfg
--rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      647 2023-04-03 19:56:36.000000 oceano_algos-0.0.95/setup.py
+drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      110 2023-01-17 20:50:26.000000 oceano_algos-0.0.98/MANIFEST.in
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      886 2023-01-22 15:00:56.000000 oceano_algos-0.0.98/README.md
+drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/oceano_algos/
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       23 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/__init__.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2800 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/_nbdev.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      209 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/core.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    11617 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/hh_parser.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    10162 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/notificator.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)    32653 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/parser.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     7049 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/postgres.py
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)     2492 2023-04-10 08:47:46.000000 oceano_algos-0.0.98/oceano_algos/preprocessor.py
+drwxrwxr-x   0 gitlab-runner  (1000) gitlab-runner  (1001)        0 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/oceano_algos.egg-info/
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      119 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      422 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)        1 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      200 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       13 2023-04-10 08:47:52.000000 oceano_algos-0.0.98/oceano_algos.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      651 2023-04-10 08:44:41.000000 oceano_algos-0.0.98/settings.ini
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)       38 2023-04-10 08:47:52.150232 oceano_algos-0.0.98/setup.cfg
+-rw-rw-r--   0 gitlab-runner  (1000) gitlab-runner  (1001)      670 2023-04-10 08:47:47.000000 oceano_algos-0.0.98/setup.py
```

### Comparing `oceano_algos-0.0.95/README.md` & `oceano_algos-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.95/oceano_algos/_nbdev.py` & `oceano_algos-0.0.98/oceano_algos/_nbdev.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,18 +34,23 @@
          "сheck_if_exists": "02-parser.ipynb",
          "ShopstatMultipleItemScrapper": "02-parser.ipynb",
          "TelegramNotificator": "03-notificator.ipynb",
          "send": "03-notificator.ipynb",
          "TimewebNotificator": "03-notificator.ipynb",
          "check_expiration_date": "03-notificator.ipynb",
          "check_servers": "03-notificator.ipynb",
+         "TextPreprocessor": "04-hh_parser.ipynb",
+         "preprocess_string": "04-hh_parser.ipynb",
+         "preprocess_series": "04-hh_parser.ipynb",
          "HeadHunterScrapper": "04-hh_parser.ipynb",
          "get_urls_from_professional_role": "04-hh_parser.ipynb",
          "get_url_vs_responses": "04-hh_parser.ipynb",
          "get_url_vs_info": "04-hh_parser.ipynb",
+         "SimilarityFinder": "04-hh_parser.ipynb",
+         "get_url_vs_similarity": "04-hh_parser.ipynb",
          "Preprocessor": "05-preprocessor.ipynb",
          "preprocess_description": "05-preprocessor.ipynb"}
 
 modules = ["core.py",
            "postgres.py",
            "parser.py",
            "notificator.py",
```

### Comparing `oceano_algos-0.0.95/oceano_algos/hh_parser.py` & `oceano_algos-0.0.98/oceano_algos/hh_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,116 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/04-hh_parser.ipynb (unless otherwise specified).
 
-__all__ = ['HeadHunterScrapper', 'get_urls_from_professional_role', 'get_url_vs_responses', 'get_url_vs_info']
+__all__ = ['TextPreprocessor', 'preprocess_string', 'preprocess_series', 'HeadHunterScrapper',
+           'get_urls_from_professional_role', 'get_url_vs_responses', 'get_url_vs_info', 'SimilarityFinder',
+           'get_url_vs_similarity']
 
 # Cell
 
 import pandas as pd
 from random import choice, uniform
 import requests
 import numpy as np
 import fastcore.basics as fcb
 from .core import logger
 from .postgres import PostgresConnector
-import time
 from tqdm import tqdm
 import re
-from .preprocessor import Preprocessor
+from sklearn.feature_extraction.text import TfidfVectorizer
+from sklearn.decomposition import TruncatedSVD
+from sklearn.metrics.pairwise import cosine_similarity
+import time
+from pymystem3 import Mystem
+
+# Cell
+
+class TextPreprocessor:
+    def __init__(self):
+
+        # get mystem object:
+        self.mystem = Mystem()
+
+# Cell
+
+@fcb.patch_to(TextPreprocessor)
+
+def preprocess_string(self, string):
+
+    """
+    FUNC TO PREPROCESS STRING
+
+    Return: string
+
+    """
+
+    # lower text:
+    string = string.lower()
+
+    # replace ",", ".", ":", ";", "-", ", ', `  with gaps:
+    string = re.sub(r'[,.:;\'\-"`]', ' ', string)
+
+    # replace "c++" and "c#" in order not to be dropped:
+    string = re.sub(r'(c\+\+|с\+\+)', 'cplusplus ', string)
+    string = re.sub(r'(c#|с#)', 'csharp ', string)
+
+    # remove all punctuation:
+    string = re.sub(r'[^\w\s]', '', string)
+
+    # remove digits if surrounded by spaces:
+    string = re.sub(r'(?<=\s)\d+(?=\s+)', '', string)
+
+
+    # lemmatize:
+    mystem = self.mystem
+    tokens = mystem.lemmatize(string)
+    tokens = [token for token in tokens if token != " " and token != "\n"]
+    string = " ".join(tokens)
+
+    # remove duplicated gaps:
+    string = ' '.join(string.split())
+
+    return string
+
+# Cell
+
+@fcb.patch_to(TextPreprocessor)
+
+def preprocess_series(self, series):
+
+    """
+    FUNC TO PREPROCESS Series
+
+    Return: pd.Series
+
+    """
+
+    return series.apply(lambda x: self.preprocess_string(x))
 
 # Cell
 
 class HeadHunterScrapper:
     def __init__(self, base_url='https://api.hh.ru/vacancies'):
 
-        # self.proxies_list = proxies_list
         self.base_url = base_url
 
 # Cell
 
 @fcb.patch_to(HeadHunterScrapper)
 
 def get_urls_from_professional_role(self, professional_role, per_page=100, pages=20, sleep=(1,3)):
 
+
+    """
+    FUNC TO GET professional_role's vacancies URLS, RESPONSES
+
+    Return: pd.DataFrame (columns: professional_role, url, responses, id)
+    """
+
+
+
     logger.info(f'SUCCESS: started scrapping vacancies URLs for professional_role = {professional_role}')
 
     # get API's base url:
     base_url = self.base_url
 
     # get vacancies' urls of entered professional_role:
     urls = []
@@ -77,15 +154,21 @@
 
 # Cell
 
 @fcb.patch_to(HeadHunterScrapper)
 
 def get_url_vs_responses(self, professional_roles, per_page=100, pages=20, sleep=(1,3), postgres_creds=None, save_to_postgres=False):
 
-    logger.info(f'SUCCESS: started scrapping vacancies URLs for professional_roles = {professional_roles}')
+
+    """
+    FUNC TO GET professional_roles's vacancies URLS, RESPONSES
+
+    Return: pd.DataFrame (columns: url, responses)
+    """
+
 
     dfs = []
     for professional_role in tqdm(professional_roles):
 
         # try up to 5 times:
         for attempt in range(5):
             try:
@@ -112,15 +195,21 @@
 
 # Cell
 
 @fcb.patch_to(HeadHunterScrapper)
 
 def get_url_vs_info(self, urls, sleep=(1,3), postgres_creds=None, save_to_postgres=False):
 
-    logger.info(f'SUCCESS: started scrapping vacancies info')
+
+    """
+    FUNC TO GET vacancy's INFO
+
+    Return: pd.DataFrame
+    """
+
 
     dfs = []
     for url in tqdm(urls):
 
         # try up to 5 times:
         for attempt in range(5):
             try:
@@ -151,15 +240,15 @@
 
     logger.info(f'SUCCESS: finished scrapping vacancies info')
 
     # preproccess data:
     logger.info(f'SUCCESS: started preprocessing data')
     vacancy_info_df = pd.concat(dfs)
 
-    # edit description:
+    # remove HTML tags from description:
     vacancy_info_df.description = vacancy_info_df.description.apply(lambda x: re.sub(re.compile('<.*?>'), '', x))
 
     # edit key_skills:
     vacancy_info_df.key_skills = vacancy_info_df.key_skills.apply(lambda x: ', '.join([d['name'] for d in x]))
 
     # edit experience:
     vacancy_info_df.experience = vacancy_info_df.experience.apply(lambda x: x['name'])
@@ -178,19 +267,92 @@
     # choose columns:
     vacancy_info_df = vacancy_info_df[['id', 'url', 'name', 'key_skills', 'experience', 'description', 'schedule', 'salary_from', 'salary_to', 'salary_currency']]
 
     # filter currency RUR, NaN:
     vacancy_info_df = vacancy_info_df[vacancy_info_df.salary_currency.isin([None, 'RUR'])]
 
     # preprocess description:
-    vacancy_info_df = Preprocessor().run(vacancy_info_df)
+    tp = TextPreprocessor()
+    vacancy_info_df['description'] = tp.preprocess_series(vacancy_info_df['description'])
 
     logger.info(f'SUCCESS: finished preprocessing data')
 
     if save_to_postgres:
         logger.info(f'SUCCESS: started saving to Postgres')
         pc = PostgresConnector(**postgres_creds)
         pc.save(df=vacancy_info_df, table_name='url_vs_info', schema='main_schema', if_table_exists='append') # append new rows
         pc.execute('DELETE FROM main_schema.url_vs_info WHERE inserted_into_db_msk != (SELECT max(inserted_into_db_msk) FROM main_schema.url_vs_info);') # drop old data
         logger.info(f'SUCCESS: finished saving to Postgres')
 
+    return vacancy_info_df
+
+# Cell
+
+class SimilarityFinder:
+    def __init__(self, cv, postgres_creds, min_df=0.002, n_components=300, ngram_range=(1,1)):
+
+        # get cv:
+        self.cv = cv
+
+        # get postgres_creds:
+        self.postgres_creds = postgres_creds
+
+        # get ngram_range:
+        self.ngram_range = ngram_range
+
+        # get min_df:
+        self.min_df = min_df
+
+        # get n_components:
+        self.n_components = n_components
+
+# Cell
+
+@fcb.patch_to(SimilarityFinder)
+
+def get_url_vs_similarity(self):
+
+    # preprocess cv:
+    cv = TextPreprocessor().preprocess_string(self.cv)
+
+    # get russian stop words:
+    pc = PostgresConnector(**self.postgres_creds)
+    self.russian_stop_words = pc.download('SELECT * from main_schema.stop_words')['word'].to_list()
+    logger.info(f"SUCCESS: extracted {len(self.russian_stop_words)} russian stop words")
+
+    # get vacancy_info_df:
+    t1 = time.time()
+    vacancy_info_df = pc.download('SELECT * FROM main_schema.vacancies')
+    t2 = time.time()
+    logger.info(f"SUCCESS: finished downloading vacancy_info_df. Time: {t2-t1:.1f} s")
+
+    # TfidfVectorizer:
+    t1 = time.time()
+    vectorizer = TfidfVectorizer(min_df=self.min_df, stop_words=self.russian_stop_words, ngram_range=self.ngram_range)
+    vacancy_tfidf = vectorizer.fit_transform(vacancy_info_df['description'])
+    cv_tfidf = vectorizer.transform([cv])
+    t2 = time.time()
+    logger.info(f"SUCCESS: finished TfidfVectorizer. {len(vectorizer.get_feature_names())} words. Time: {t2-t1:.1f} s")
+
+    # LSA:
+    t1 = time.time()
+    lsa = TruncatedSVD(n_components=self.n_components, random_state=1)
+    vacancy_lsa = lsa.fit_transform(vacancy_tfidf)
+    cv_lsa = lsa.transform(cv_tfidf)
+    t2 = time.time()
+    logger.info(f"SUCCESS: finished LSA. Time: {t2-t1:.1f} s")
+
+    # calculate cosine similarity between the cv and each vacancy description:
+    similarity_scores = cosine_similarity(vacancy_lsa, cv_lsa)
+    logger.info(f"SUCCESS: finished calculating cosine similarity")
+
+
+    # Add the similarity_scores column:
+    vacancy_info_df['similarity'] = similarity_scores.flatten()
+    vacancy_info_df['similarity'] = vacancy_info_df['similarity'].apply(lambda x: 0 if x<0 else x)
+
+    # add column url:
+    col = vacancy_info_df['id'].apply(lambda x: f'https://hh.ru/vacancy/{x}')
+    vacancy_info_df.insert(0, 'url', col)
+    vacancy_info_df = vacancy_info_df.drop(['id'], axis=1) # delete column id
+
     return vacancy_info_df
```

### Comparing `oceano_algos-0.0.95/oceano_algos/notificator.py` & `oceano_algos-0.0.98/oceano_algos/notificator.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.95/oceano_algos/parser.py` & `oceano_algos-0.0.98/oceano_algos/parser.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.95/oceano_algos/postgres.py` & `oceano_algos-0.0.98/oceano_algos/postgres.py`

 * *Files identical despite different names*

### Comparing `oceano_algos-0.0.95/oceano_algos/preprocessor.py` & `oceano_algos-0.0.98/oceano_algos/preprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     RETURN: pd.DataFrame
 
     """
 
     # lower text:
     vacancy_df['description'] = vacancy_df['description'].str.lower()
 
-    # replace ",", ".", ":", ";", "-" with gaps:
-    vacancy_df['description'] = vacancy_df['description'].apply(lambda x: re.sub(r'[,.:;-]', ' ', x))
+    # replace ",", ".", ":", ";", "-", ", ', `  with gaps:
+    vacancy_df['description'] = vacancy_df['description'].apply(lambda x: re.sub(r'[,.:;\'-"`]', ' ', x))
 
     # replace "c++" and "c#" in order not to be dropped:
     vacancy_df['description'] = vacancy_df['description'].apply(lambda x: re.sub(r'(c\+\+|с\+\+)', 'cplusplus ', x))
     vacancy_df['description'] = vacancy_df['description'].apply(lambda x: re.sub(r'(c#|с#)', 'csharp ', x))
 
     # remove all punctuation:
     vacancy_df['description'] = vacancy_df['description'].apply(lambda x: re.sub(r'[^\w\s]', '', x))
```

### Comparing `oceano_algos-0.0.95/settings.ini` & `oceano_algos-0.0.98/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 description = A description of your project
 long_description = Long description text
 keywords = some keywords for pypi search
 author = mrtweety123
 author_email = mrtweety123@proton.me
 copyright = some copyright information
 branch = main
-version = 0.0.95
+version = 0.0.98
 min_python = 3.6
 audience = Developers
 language = English
 custom_sidebar = False
 license = some license
 status = 2
 nbs_path = nbs
```

### Comparing `oceano_algos-0.0.95/setup.py` & `oceano_algos-0.0.98/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 config.read('settings.ini')
 cfg = config['DEFAULT']
 
 setup(
     name = cfg['lib_name'],
     version=cfg['version'],
     packages=find_packages(),
-    install_requires = ['pandas', 'fastcore', 'sqlalchemy==1.4.46', 'sshtunnel==0.4.0', 'loguru', 'psycopg2-binary', 'oceano-algos', 'selenium', 'beautifulsoup4', 'numpy', 'tqdm', 'psutil', 'boltons', 'pytelegrambotapi==4.10.0', 'pymystem3==0.2.0'], # <-- DO NOT EDIT, THIS LINE IS AUTOGENERATED
+    install_requires = ['pandas', 'fastcore', 'sqlalchemy==1.4.46', 'sshtunnel==0.4.0', 'loguru', 'psycopg2-binary', 'oceano-algos', 'selenium', 'beautifulsoup4', 'numpy', 'tqdm', 'psutil', 'boltons', 'pytelegrambotapi==4.10.0', 'pymystem3==0.2.0', 'scikit-learn==1.0.2'], # <-- DO NOT EDIT, THIS LINE IS AUTOGENERATED
     long_description=cfg['long_description'],
     description=cfg['description']
 )
```

