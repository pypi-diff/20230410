# Comparing `tmp/pyBibX-2.9.0.tar.gz` & `tmp/pyBibX-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyBibX-2.9.0.tar", last modified: Sun Apr  9 14:52:46 2023, max compression
+gzip compressed data, was "dist\pyBibX-2.9.1.tar", last modified: Mon Apr 10 01:55:19 2023, max compression
```

## Comparing `pyBibX-2.9.0.tar` & `pyBibX-2.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 14:52:46.000000 pyBibX-2.9.0/
--rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.0/LICENSE
--rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9092 2023-04-09 14:52:46.000000 pyBibX-2.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     8655 2023-04-09 13:31:30.000000 pyBibX-2.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 14:52:45.000000 pyBibX-2.9.0/pyBibX/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.0/pyBibX/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:52:45.000000 pyBibX-2.9.0/pyBibX/base/
--rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.0/pyBibX/base/__init__.py
--rw-rw-rw-   0        0        0   261990 2023-04-09 13:26:45.000000 pyBibX-2.9.0/pyBibX/base/pbx.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:52:46.000000 pyBibX-2.9.0/pyBibX/base/stws/
--rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Arabic.txt
--rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bengali.txt
--rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bulgarian.txt
--rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Czech.txt
--rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-English.txt
--rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Finnish.txt
--rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-French.txt
--rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-German.txt
--rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hindi.txt
--rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hungarian.txt
--rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Italian.txt
--rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Marathi.txt
--rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Persian.txt
--rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Polish.txt
--rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Portuguese-br.txt
--rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Romanian.txt
--rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Russian.txt
--rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Spanish.txt
--rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Swedish.txt
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.0/pyBibX/base/stws/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 14:52:45.000000 pyBibX-2.9.0/pyBibX.egg-info/
--rw-rw-rw-   0        0        0     9092 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1047 2023-04-09 14:52:43.000000 pyBibX-2.9.0/pyBibX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 14:52:42.000000 pyBibX-2.9.0/pyBibX.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-09 14:52:46.000000 pyBibX-2.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1077 2023-04-08 01:55:27.000000 pyBibX-2.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:55:19.000000 pyBibX-2.9.1/
+-rw-rw-rw-   0        0        0      644 2022-03-01 19:24:07.000000 pyBibX-2.9.1/LICENSE
+-rw-rw-rw-   0        0        0       40 2022-05-19 14:46:22.000000 pyBibX-2.9.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9131 2023-04-10 01:55:19.000000 pyBibX-2.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8694 2023-04-10 01:54:14.000000 pyBibX-2.9.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 01:55:18.000000 pyBibX-2.9.1/pyBibX/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.1/pyBibX/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:55:18.000000 pyBibX-2.9.1/pyBibX/base/
+-rw-rw-rw-   0        0        0       27 2022-03-16 15:26:25.000000 pyBibX-2.9.1/pyBibX/base/__init__.py
+-rw-rw-rw-   0        0        0   263502 2023-04-10 01:50:45.000000 pyBibX-2.9.1/pyBibX/base/pbx.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:55:19.000000 pyBibX-2.9.1/pyBibX/base/stws/
+-rw-rw-rw-   0        0        0     1287 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Arabic.txt
+-rw-rw-rw-   0        0        0     1484 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bengali.txt
+-rw-rw-rw-   0        0        0     2408 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bulgarian.txt
+-rw-rw-rw-   0        0        0     1518 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Czech.txt
+-rw-rw-rw-   0        0        0     4212 2017-08-01 12:33:33.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-English.txt
+-rw-rw-rw-   0        0        0     6219 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Finnish.txt
+-rw-rw-rw-   0        0        0     3234 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-French.txt
+-rw-rw-rw-   0        0        0     4350 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-German.txt
+-rw-rw-rw-   0        0        0     2065 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hindi.txt
+-rw-rw-rw-   0        0        0     5552 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hungarian.txt
+-rw-rw-rw-   0        0        0     2379 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Italian.txt
+-rw-rw-rw-   0        0        0     1307 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Marathi.txt
+-rw-rw-rw-   0        0        0     3274 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Persian.txt
+-rw-rw-rw-   0        0        0      704 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Polish.txt
+-rw-rw-rw-   0        0        0     3772 2019-05-09 13:59:54.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Portuguese-br.txt
+-rw-rw-rw-   0        0        0     1926 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Romanian.txt
+-rw-rw-rw-   0        0        0     4963 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Russian.txt
+-rw-rw-rw-   0        0        0     2420 2017-08-01 12:33:16.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Spanish.txt
+-rw-rw-rw-   0        0        0     2757 2017-07-30 20:46:06.000000 pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Swedish.txt
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyBibX-2.9.1/pyBibX/base/stws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:55:18.000000 pyBibX-2.9.1/pyBibX.egg-info/
+-rw-rw-rw-   0        0        0     9131 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-10 01:55:17.000000 pyBibX-2.9.1/pyBibX.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-10 01:55:19.000000 pyBibX-2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0     1077 2023-04-10 01:51:00.000000 pyBibX-2.9.1/setup.py
```

### Comparing `pyBibX-2.9.0/LICENSE` & `pyBibX-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/PKG-INFO` & `pyBibX-2.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyBibX
 
 ## Introduction
 
-A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Bibliometric Results and Text Data
+A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also, Powered with Advanced AI Technologies for Analyzing Bibliometric, Scientometric Outcomes, and Textual Data
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
@@ -44,20 +44,20 @@
 - e) Visualize topics heatmap
 - f) Find the most representative documents from each topic
 - g) Find the most representative topics according to a word
 - h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
 - i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
 - j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
-- l) **Ask chatGPT to Analyze Results** available for: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (see Example 08). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- l) **Ask chatGPT** to analyze the following results: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (consult **Example 08**). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 
 Correction and Manipulation Capabilities:
 - a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
 - b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
-- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
+- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (consult **Examples 04 and 05**)
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyBibX
 ```
@@ -67,15 +67,15 @@
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
-- Example 08: Ask chatGPT Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
+- Example 08: **Ask chatGPT** Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
 - b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
```

### Comparing `pyBibX-2.9.0/README.md` & `pyBibX-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyBibX
 
 ## Introduction
 
-A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Bibliometric Results and Text Data
+A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also, Powered with Advanced AI Technologies for Analyzing Bibliometric, Scientometric Outcomes, and Textual Data
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
@@ -33,20 +33,20 @@
 - e) Visualize topics heatmap
 - f) Find the most representative documents from each topic
 - g) Find the most representative topics according to a word
 - h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
 - i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
 - j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
-- l) **Ask chatGPT to Analyze Results** available for: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (see Example 08). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- l) **Ask chatGPT** to analyze the following results: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (consult **Example 08**). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 
 Correction and Manipulation Capabilities:
 - a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
 - b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
-- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
+- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (consult **Examples 04 and 05**)
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyBibX
 ```
@@ -56,15 +56,15 @@
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
-- Example 08: Ask chatGPT Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
+- Example 08: **Ask chatGPT** Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
 - b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
```

### Comparing `pyBibX-2.9.0/pyBibX/base/pbx.py` & `pyBibX-2.9.1/pyBibX/base/pbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -4040,23 +4040,23 @@
         else:
             summary    = 'No abstracts were found in the selected set of documents'
         return summary
 
 ############################################################################
 
     # Function: Ask chatGPT about Authors Productivity by Year
-    def ask_chatgpt_ap(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to authors productivity by year'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_ap(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to authors productivity by year', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus = ''
         for author, row in self.ask_gpt_ap.iterrows():
             years        = [(year, row[year]) for year in row.index if row[year] > 0]
             paper_counts = ', '.join([f'({year}: {count} paper{"s" if count > 1 else ""})' for year, count in years])
             corpus       = corpus +  f'{author} {paper_counts}\n'
@@ -4064,232 +4064,232 @@
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
     
     # Function: Ask chatGPT about Bar Plots 
-    def ask_chatgpt_bp(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_bp(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_bp.to_string(index = False)    
         openai.api_key = api_key
         prompt         = query + ' regarding ' + self.ask_gpt_bp_t + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
     
     # Function: Ask chatGPT about Citation Analysis 
-    def ask_chatgpt_citation(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_citation(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_nad.to_string(index = False)    
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Collaboration Analysis
-    def ask_chatgpt_colab(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following network information, knowing that Node 1 is connected with Node 2'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_colab(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following network information, knowing that Node 1 is connected with Node 2', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_adj.to_string(index = False)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about EDA Report 
-    def ask_chatgpt_eda(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_eda(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_rt.to_string(index = False)    
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
     
     # Function: Ask chatGPT about Evolution Plot
-    def ask_chatgpt_ep(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to words apperance by year'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_ep(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information, related to words apperance by year', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_ep
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Citation Analysis 
-    def ask_chatgpt_hist(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the most influential references, also discover if there is relevant network connections'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_hist(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the most influential references, also discover if there is relevant network connections', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus = []
         for i in range(0, self.ask_gpt_hist.shape[0]):
             corpus.append('Paper ' + self.ask_gpt_hist.iloc[i,0] + ' Cites Paper ' + self.ask_gpt_hist.iloc[i,1])
         corpus         = ', '.join(corpus)    
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Map Analysis 
-    def ask_chatgpt_map(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_map(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_map.to_string(index = False)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about N-Grms 
-    def ask_chatgpt_ngrams(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the n-grams and their frequency'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_ngrams(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information relating the n-grams and their frequency', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_ng.to_string(index = False)  
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)  
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Sankey Diagram
-    def ask_chatgpt_sankey(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information from a network called Sankey'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_sankey(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information from a network called Sankey', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_sk.to_string(index = False)   
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Similarity Analysis 
-    def ask_chatgpt_sim(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_sim(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = self.ask_gpt_sim.to_string(index = False)
         openai.api_key = api_key
         prompt         = query + ':\n\n' + f'{corpus}\n'
         prompt         = prompt[:char_limit]
         analyze        = query_chatgpt(prompt)
         print('Number of Characters: ' + str(len(prompt)))
         return analyze
 
     # Function: Ask chatGPT about Wordcloud 
-    def ask_chatgpt_wordcloud(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information'):
-        def query_chatgpt(prompt, model = 'text-davinci-003', n = 1):
+    def ask_chatgpt_wordcloud(self, char_limit = 4097, api_key = 'your_api_key_here', query = 'give me insights about the following information', model = 'text-davinci-003', max_tokens = 2000, n = 1, temperature = 0.8):
+        def query_chatgpt(prompt, model = model, max_tokens = max_tokens, n = n, temperature = temperature):
             response = openai.Completion.create(
                                                 engine      = model,
                                                 prompt      = prompt,
-                                                max_tokens  = 2000,
+                                                max_tokens  = max_tokens,
                                                 n           = n,
                                                 stop        = None,
-                                                temperature = 0.8
+                                                temperature = temperature
                                                 )
             return response.choices[0].text.strip()
         corpus         = pd.DataFrame.from_dict(self.ask_gpt_wd, orient = 'index', columns = ['Frequency'])    
         corpus         = corpus.reset_index().rename(columns = {'index': 'Word'})
         corpus         = corpus.to_string(index = False)
         lines          = corpus.split('\n')
         corpus         = '\n'.join(' '.join(line.split()) for line in lines)
```

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Arabic.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Arabic.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bengali.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bengali.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Bulgarian.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Bulgarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Czech.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Czech.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-English.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-English.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Finnish.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Finnish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-French.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-French.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-German.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-German.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hindi.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hindi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Hungarian.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Hungarian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Italian.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Italian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Marathi.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Marathi.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Persian.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Persian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Polish.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Polish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Portuguese-br.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Portuguese-br.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Romanian.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Romanian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Russian.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Russian.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Spanish.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Spanish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX/base/stws/Stopwords-Swedish.txt` & `pyBibX-2.9.1/pyBibX/base/stws/Stopwords-Swedish.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/pyBibX.egg-info/PKG-INFO` & `pyBibX-2.9.1/pyBibX.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyBibX
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Bibliometric and Scientometric Library Powered with Artificial Intelligence Tools
 Home-page: https://github.com/Valdecy/pyBibX
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyBibX
 
 ## Introduction
 
-A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also Powered with Artificial Intelligence Tools to Analyze Bibliometric Results and Text Data
+A Bibliometric and Scientometric python library that uses the raw files generated by **Scopus** (.bib files), **WOS (Web of Science)** (.bib files), and **PubMed** (.txt files) scientific databases. Also, Powered with Advanced AI Technologies for Analyzing Bibliometric, Scientometric Outcomes, and Textual Data
 
 General Capabilities:
 - a) Works with **Scopus** (.bib files), **WOS** (.bib files) and **PubMed** (.txt files) databases 
 - b) Identification and Removal of duplicates
 - c) Identification of documents per type
 - d) Generates an **EDA (Exploratory Data Analysis)** Report: Publications Timespan, Total Number of Countries, Total Number of Institutions, Total Number of Sources, Total Number of References, Total Number of Languages (and also the number of docs for each language), Total Number of Documents, Average Documents per Author, Average Documents per Institution, Average Documents per Source, Average Documents per Year, Total Number of Authors, Total Number of Authors Keywords, Total Number of Authors Keywords Plus, Total Single-Authored Documents, Total Multi-Authored Documents, Average Collaboration Index, Max H-Index, Total Number of Citations, Average Citations per Author, Average Citations per Institution, Average Citations per Document, Average Citations per Source
 - e) Creates an **ID (Identification)** for each Document, Authors, Sources, Institutions, Countries, Authors' Keywords, Keywords Plus. The IDs can be used in graphs/plots to obtain a cleaner visualization
@@ -44,20 +44,20 @@
 - e) Visualize topics heatmap
 - f) Find the most representative documents from each topic
 - g) Find the most representative topics according to a word
 - h) Creates **Embeddings** from Abstracts, Titles, Authors Keywords or Keywords Plus
 - i) **Abstractive Text Summarization** using **PEGASUS** on a set of selected documents or all documents
 - j) **Abstractive Text Summarization** using **chatGPT** on a set of selected documents or all documents. Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 - k) **Extractive Text Summarization** using **BERT** on a set of selected documents or all documents
-- l) **Ask chatGPT to Analyze Results** available for: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (see Example 08). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
+- l) **Ask chatGPT** to analyze the following results: EDA Report, WordCloud, N-Grams, Evolution Plot, Sankey Diagram, Authors Productivity Plot, Bar Plots, Citation Analysis, Collaboration Analysis, Similarity Analysis, and World Map Collaboration Analysis (consult **Example 08**). Requires the user to have an **API key** (https://platform.openai.com/account/api-keys)
 
 Correction and Manipulation Capabilities:
 - a) Filter the .bib or .txt file by Year, Sources, Bradford Law Cores, Countries, Languages and/or Abstracts (Documents with Abstracts)
 - b) Merge Authors, Institutions, Countries, Languages and/or Sources that have multiple entries 
-- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (see Examples 04 and 05)
+- c) Merge different or the same database files one at a time. The preference for information preservation is given to the old database, so the order of merging matters (consult **Examples 04 and 05**)
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyBibX
 ```
@@ -67,15 +67,15 @@
 - Example 01: Scopus                ([ Colab Demo ](https://colab.research.google.com/drive/1yHiMMZIKa-RrarXbPB9ca0gLN9YvvtPU?usp=sharing))
 - Example 02: WOS                   ([ Colab Demo ](https://colab.research.google.com/drive/13HLjC4myTvYcjLk2XBTZKbWJ2aqZUST1?usp=sharing))
 - Example 03: PubMed                ([ Colab Demo ](https://colab.research.google.com/drive/13CU-KvZMnazga1BmQf2J8wYM9mhHL2e1?usp=sharing))
 - Example 04: Scopus + WOS          ([ Colab Demo ](https://colab.research.google.com/drive/1DqEk0_IakJPfIZDVcnTWBE_nxyhW9p-W?usp=sharing))
 - Example 05: WOS + Scopus          ([ Colab Demo ](https://colab.research.google.com/drive/12k_IOcSDwumbEtPqqSMbCIE6ZypgKAJn?usp=sharing))
 - Example 06: Scopus + WOS + Pubmed ([ Colab Demo ](https://colab.research.google.com/drive/1Ko6AibkXtB_Kwg3Eu0fhzNMVEIXPkbez?usp=sharing))
 - Example 07: Your Own              ([ Colab Demo ](https://colab.research.google.com/drive/19EYjgal9V1kemmzpHnyp6MSlk9S-kGHT?usp=sharing))
-- Example 08: Ask chatGPT Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
+- Example 08: **Ask chatGPT** Analysis  ([ Colab Demo ](https://colab.research.google.com/drive/1LMrR49F54MuX-stlrQbrrjX_dEU3kZ8Y?usp=sharing))
 
 # Acknowledgement 
 This section indicates the libraries that inspired pyBibX
 
 * BERT (https://smrzr.io/)
 - a) Github: https://github.com/dmmiller612/bert-extractive-summarizer
 - b) Paper: DEREK, M. (2019). Leveraging BERT for Extractive Text Summarization on Lectures. arXiv. doi: https://doi.org/10.48550/arXiv.1906.04165
```

### Comparing `pyBibX-2.9.0/pyBibX.egg-info/SOURCES.txt` & `pyBibX-2.9.1/pyBibX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyBibX-2.9.0/setup.py` & `pyBibX-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyBibX',
-    version='2.9.0',
+    version='2.9.1',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyBibX',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
```

