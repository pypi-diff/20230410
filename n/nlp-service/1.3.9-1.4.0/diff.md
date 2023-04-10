# Comparing `tmp/nlp_service-1.3.9.tar.gz` & `tmp/nlp_service-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.3.9.tar", max compression
+gzip compressed data, was "nlp_service-1.4.0.tar", max compression
```

## Comparing `nlp_service-1.3.9.tar` & `nlp_service-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-03-19 12:24:32.645525 nlp_service-1.3.9/LICENSE
--rw-r--r--   0        0        0     8218 2023-03-19 12:24:32.645525 nlp_service-1.3.9/README.md
--rw-r--r--   0        0        0      226 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/py.typed
--rw-r--r--   0        0        0    14827 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-03-19 12:24:32.645525 nlp_service-1.3.9/nlp_service/typing.py
--rw-r--r--   0        0        0     1364 2023-03-19 12:25:05.749716 nlp_service-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     9857 1970-01-01 00:00:00.000000 nlp_service-1.3.9/setup.py
--rw-r--r--   0        0        0     9743 1970-01-01 00:00:00.000000 nlp_service-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-10 13:54:39.508267 nlp_service-1.4.0/LICENSE
+-rw-r--r--   0        0        0     8218 2023-04-10 13:54:39.508267 nlp_service-1.4.0/README.md
+-rw-r--r--   0        0        0      226 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/py.typed
+-rw-r--r--   0        0        0    15633 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-04-10 13:54:39.508267 nlp_service-1.4.0/nlp_service/typing.py
+-rw-r--r--   0        0        0     1509 2023-04-10 13:55:12.393848 nlp_service-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9982 1970-01-01 00:00:00.000000 nlp_service-1.4.0/PKG-INFO
```

### Comparing `nlp_service-1.3.9/LICENSE` & `nlp_service-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.3.9/README.md` & `nlp_service-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nlp_service-1.3.9/nlp_service/client.py` & `nlp_service-1.4.0/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.3.9/nlp_service/infersent.py` & `nlp_service-1.4.0/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.3.9/nlp_service/server.py` & `nlp_service-1.4.0/nlp_service/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 from thinc.types import Floats1d as SpacyVector
 
 from nlp_service.similarity import SimilarityFactory as SimilarityFactory
 from nlp_service.typing import ArrayLike, NumpyMatrix, NumpyVector
 
 log = logging.getLogger(__name__)
 
-# import tensorflow_hub as hub
-
 # https://spacy.io/usage/processing-pipelines#built-in
 spacy_components = (
     "tagger",
     "parser",
     "ner",
     "entity_linker",
     "entity_ruler",
@@ -174,30 +172,60 @@
         def vector(self, text: str) -> SpacyVector:
             embeddings = t.cast(
                 NumpyVector, self.model.encode([text], convert_to_numpy=True)
             )
 
             return embeddings[0]
 
-    embedding_map[
-        nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS
-    ] = SentenceTransformersModel
+    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS] = (
+        SentenceTransformersModel
+    )
+
+except ModuleNotFoundError:
+    log.info("'sentence-transformers' not installed.")
+
+
+try:
+    import tensorflow_hub as hub
+
+    class TensorflowHubModel(ModelBase):
+        def __init__(self, model: EmbeddingModel):
+            self.model: t.Any = hub.load(model.model_name)
+
+        def vector(self, text: str) -> SpacyVector:
+            embeddings: t.Sequence[t.Any] = self.model([text])
+
+            return embeddings[0].numpy()
+
+    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_TENSORFLOW_HUB] = (
+        TensorflowHubModel
+    )
 
 except ModuleNotFoundError:
-    log.info("'sentence_transformers' not installed.")
+    log.info("'tensorflow-hub' not installed.")
+
+
+try:
+    import openai
 
+    openai.api_key_path = "./openai_api_key.txt"
 
-# class TensorflowHubModel(ModelBase):
-#     def __init__(self, model: EmbeddingModel):
-#         self.model = hub.load(model.model_name)
+    class OpenaiModel(ModelBase):
+        def __init__(self, model: EmbeddingModel):
+            self.model_name: str = model.model_name
+
+        def vector(self, text: str) -> SpacyVector:
+            res: t.Any = openai.Embedding.create(input=[text], model=self.model_name)
 
-#     def vector(self, text: str):
-#         embeddings = self.model([text])  # type: ignore
+            return t.cast(SpacyVector, np.array(res["data"][0]["embedding"]))
 
-#         return embeddings[0].numpy()
+    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_OPENAI] = OpenaiModel
+
+except ModuleNotFoundError:
+    log.info("'openai' not installed.")
 
 
 @SpacyLanguage.factory("embeddings_factory")
 class EmbeddingsFactory:
     def __init__(self, nlp, name, models):
         self.models: list[ModelBase] = []
 
@@ -233,15 +261,15 @@
 SpacyKey = tuple[str, str, tuple[EmbeddingModel, ...]]
 SpacyCache = t.Tuple[SpacyLanguage, dict[str, Doc]]
 spacy_cache: dict[SpacyKey, SpacyCache] = {}
 model_cache: dict[EmbeddingModel, ModelBase] = {}
 
 
 def _load_spacy_model(name: t.Optional[str]) -> SpacyLanguage:
-    if name is None:
+    if not name:
         return spacy.blank("en")
 
     try:
         return spacy.load(name)
     except OSError:
         spacy_download(name)
         return spacy.load(name)
```

### Comparing `nlp_service-1.3.9/nlp_service/similarity.py` & `nlp_service-1.4.0/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.3.9/pyproject.toml` & `nlp_service-1.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.3.9"
+version = "1.4.0"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
 
 [tool.poetry.scripts]
 nlp-service = "nlp_service.server:app"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.12"
+python = ">=3.10, <3.12"
 numpy = "^1.23.5"
 scipy = "^1.9.3"
 spacy = "^3.5.1"
-arg-services = "^1.2.3"
+arg-services = "^1.3.0"
 nltk = "^3.8.1"
 nptyping = "^2.5.0"
-mashumaro = "^3.5"
+mashumaro = "^3.6"
 typer = "^0.7.0"
-gensim = { version = "^4.3.0", optional = true }
+gensim = { version = "^4.3.1", optional = true }
 python-Levenshtein = { version = "^0.20.9", optional = true }
 sentence-transformers = { version = "^2.2.2", optional = true }
 torch = { version = ">=1.13.1, <3.0", optional = true }
-transformers = { version = "^4.26.1", optional = true }
-# tensorflow = { version = "^2.11.0", optional = true }
-# tensorflow-hub = { version = "^0.12.0", optional = true }
+transformers = { version = "^4.27.4", optional = true }
+tensorflow = { version = "^2.12.0", optional = true }
+tensorflow-hub = { version = "^0.13.0", optional = true }
+openai = { version = "^0.27.2", optional = true }
 
 [tool.poetry.extras]
 wmd = ["gensim"]
 levenshtein = ["python-Levenshtein"]
 sentence-transformers = ["sentence-transformers", "torch"]
 transformers = ["transformers", "torch"]
+tensorflow = ["tensorflow", "tensorflow-hub"]
+openai = ["openai"]
 all = [
     "gensim",
     "python-Levenshtein",
     "sentence-transformers",
     "transformers",
     "torch",
+    "tensorflow",
+    "openai",
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nlp_service-1.3.9/setup.py` & `nlp_service-1.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,201 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nlp-service
+Version: 1.4.0
+Summary: Microservice for NLP tasks using gRPC
+Home-page: http://recap.uni-trier.de
+License: MIT
+Author: Mirko Lenz
+Author-email: info@mirko-lenz.de
+Requires-Python: >=3.10,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: levenshtein
+Provides-Extra: openai
+Provides-Extra: sentence-transformers
+Provides-Extra: tensorflow
+Provides-Extra: transformers
+Provides-Extra: wmd
+Requires-Dist: arg-services (>=1.3.0,<2.0.0)
+Requires-Dist: gensim (>=4.3.1,<5.0.0) ; extra == "wmd" or extra == "all"
+Requires-Dist: mashumaro (>=3.6,<4.0)
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
+Requires-Dist: nptyping (>=2.5.0,<3.0.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: openai (>=0.27.2,<0.28.0) ; extra == "openai" or extra == "all"
+Requires-Dist: python-Levenshtein (>=0.20.9,<0.21.0) ; extra == "levenshtein" or extra == "all"
+Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "sentence-transformers" or extra == "all"
+Requires-Dist: spacy (>=3.5.1,<4.0.0)
+Requires-Dist: tensorflow (>=2.12.0,<3.0.0) ; extra == "tensorflow" or extra == "all"
+Requires-Dist: tensorflow-hub (>=0.13.0,<0.14.0) ; extra == "tensorflow"
+Requires-Dist: torch (>=1.13.1,<3.0) ; extra == "sentence-transformers" or extra == "transformers" or extra == "all"
+Requires-Dist: transformers (>=4.27.4,<5.0.0) ; extra == "transformers" or extra == "all"
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Project-URL: Repository, https://github.com/recap-utr/nlp-service
+Description-Content-Type: text/markdown
+
+# NLP Microservice
+
+The goal of this project is to provide a [gRPC](https://grpc.io) server for resource-heavy NLP tasks&mdash;for instance, computing vectors/embeddings for words or sentences.
+By using [protobuf](https://developers.google.com/protocol-buffers) internally, our NLP server provides native and strongly typed interfaces for many programming languages.
+There are multiple advantages that arise from outsourcing such computations to such a server:
+
+- If multiple apps rely on NLP, the underlying models (which are usually quite large) only need to be loaded once into the main memory.
+- All programming languages supported by gRPC get easy access to state-of-the-art NLP architectures (e.g., transformers).
+- The logic is consolidated at a central place, drastically decreasing the maintenance effort required.
+
+In addition to the server, we also provide a client containing convenience functions.
+This makes it easier for python applications to interact with the gRPC server.
+We will discuss the client at the end of this README.
+
+## Installation and Setup
+
+We are using [poetry](https://python-poetry.org) to manage the dependencies.
+For easier setup, we also provide a `Dockerfile` and a `docker-compose` specification.
+
+### Docker-Compose (recommended)
+
+You first need to pull this repository.
+Then execute the following in the project directory:
+
+```sh
+docker-compose build cpu
+# OR, if you need extras:
+docker-compose build --build-arg EXTRAS="levenshtein transformers" cpu
+# Start the CPU-only container
+docker-compose up cpu
+```
+
+In case you have a **CUDA-enabled GPU**, you can replace `cpu` with `cuda` in the above commands and make full use of your card for advanced models like BERT.
+
+### Poetry (advanced)
+
+```sh
+# The server dependencies are optional, thus they have to be installed explicitly.
+poetry install --extras server
+# To get startet, we recommend to use the default spacy model.
+# In case you are dealing with English texts, you can run.
+poetry run python -m spacy download core_en_web_lg
+# To run the server, you need to specify the address it should listen on.
+# In this example, it should liston on port 5678 on localhost.
+poetry run python -m nlp_service "127.0.0.1:50100"
+```
+
+## General Usage
+
+Once the server is running, you are free to call any of the functions defined in the underlying [protobuf file](https://github.com/recap-utr/arg-services/blob/main/arg_services/nlp/v1/nlp.proto).
+The corresponding documentation is located at the [Buf Schema Registry](https://buf.build/recap/arg-services/docs/main:arg_services.nlp.v1).
+_Please note:_ The examples here use the Python programming language, but are also directly applicable to any other language supported by gRPC.
+
+```python
+import grpc
+from arg_services.nlp.v1 import nlp_pb2, nlp_pb2_grpc
+
+# First of all, we are creating a channel (i.e., establish a connection to our server)
+channel = grpc.insecure_channel("127.0.0.1:5678")
+
+# The channel can now be used to create the actual client (allowing us to call all available functions)
+client = nlp_pb2_grpc.NlpServiceStub(channel)
+
+# Now the time has come to prepare our actual function call.
+# We will start by creating a very simple NlpConfig with the default spacy model.
+# FOr details about the parameters, please have a look at the next section.
+config = nlp_pb2.NlpConfig(
+  language="en",
+  spacy_model="en_core_web_lg",
+)
+
+# Next, we will build a request to query vectors from our server.
+request = nlp_pb2.VectorsRequest(
+  # The first parameter is a list of strings that shall be embedded by our server.
+  texts=["What a great tutorial!", "I will definitely recommend this to my friends."],
+  # Now we need to specify which embeddings have to be computed. In this example, we create one vector for each text
+  embedding_levels=[nlp_pb2.EmbeddingLevel.EMBEDDING_LEVEL_DOCUMENT],
+  # The only thing missing now is the spacy configuration we created in the previous step.
+  config=config
+)
+
+# Having created the request, we can now send it to the server and retrieve the corresponding response.
+response = client.Vectors(request)
+
+# Due to technical constraints, we cannot directly transfer numpy arrays, thus we convert our response.
+vectors = [np.array(entry.document.vector) for entry in response.vectors]
+```
+
+<!-- TODO: Prefer Vectors instead of Similarities for Python to increase performacne. -->
+
+## Advanced Usage
+
+A central piece for all available function is the `NlpConfig` message, allowing you to create even complex embedding models easily.
+In addition to [its documentation](https://buf.build/recap/arg-services/docs/main:arg_services.nlp.v1), we will in the following present some examples to demonstrate the possibilities you have.
+
+```python
+from arg_services.nlp.v1 import nlp_pb2
+
+# In the example above, we already introduced a quite basic config:
+config = nlp_pb2.NlpConfig(
+  # You have to provide a language for every config: https://spacy.io/usage/models#languages
+  language="en",
+  # Also, you need to specify the model that spacy should load: https://spacy.io/models/en
+  spacy_model="en_core_web_lg",
+)
+
+# A central feature of our library is the possibility to combine multiple embedding models, potentially capturing more contextual information.
+config = nlp_pb2.NlpConfig(
+  language="en",
+  # This parameter expects a list of models. If you pass more than one, the respective vectors are **concatenated** to each other
+  # (e.g., two 300-dimensional embeddings will result in a 600-dimensional one).
+  # This approach is based on https://arxiv.org/abs/1803.01400
+  embedding_models=[
+    nlp_pb2.EmbeddingModel(
+      # First select the type of model you would like to use (e.g., SBERT/Sentence Transformers).
+      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS,
+      # Then select the actual model.
+      # Any of those specified on the website (https://www.sbert.net/docs/pretrained_models.html) are allowed.
+      model_name="all-mpnet-base-v2"
+    ),
+    nlp_pb2.EmbeddingModel(
+      # It is also possible to use a standard spacy model
+      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY,
+      model_name="en_core_web_lg",
+      # Since we have selected a word embedding (i.e., it cannot directly encode sentences), the token vectors need to be aggregated somehow.
+      # The default strategy is to use the arithmetic mean, but you are free to use other strategies (e.g., the geometric mean).
+      pooling_type=nlp_pb2.Pooling.POOLING_GMEAN
+    ),
+    nlp_pb2.EmbeddingModel(
+      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY,
+      model_name="en_core_web_lg",
+      # Alternatively, it is also possible to use the generalized mean / power mean.
+      # In this example, the selected pmean corresponds to the geometic mean (thus this embedding is identical to the previous one).
+      # This approach is based on https://arxiv.org/abs/1803.01400
+      pmean=0
+    )
+  ]
+  # This setting is now optional and only needed if you need spacy features (e.g., POS tagging) besides embeddings.
+  # spacy_model="en_core_web_lg",
+)
+
+# If computing the similarity between strings, you get one additional parameter.
+config = nlp_pb2.NlpConfig(
+  language="en",
+  # To keep the example simple, we will now only use a single spacy model instead of the more powerful embedding models.
+  # However, it is of course possible to use them here as well.
+  spacy_model="en_core_web_lg",
+  # If not specified, we will always use the cosine similarity when comparing two strings.
+  # As indicated in a recent paper (https://arxiv.org/abs/1904.13264), you may achieve better results with alternative approaches like DynaMax Jaccard.
+  # Please note that this particular method ignores your selected pooling method due to the fact that even plain word embeddings are not pooled at all.
+  similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_DYNAMAX_JACCARD
+)
+
+# It is also possible to determine a similarity score without the use of embeddings.
+config = nlp_pb2.NlpConfig(
+  language="en",
+  spacy_model="en_core_web_lg",
+  # Traditional metric (Jaccard similarity and Levenshtein edit distance) are also available
+  similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_EDIT
+)
+```
 
-packages = \
-['nlp_service']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['arg-services>=1.2.3,<2.0.0',
- 'mashumaro>=3.5,<4.0',
- 'nltk>=3.8.1,<4.0.0',
- 'nptyping>=2.5.0,<3.0.0',
- 'numpy>=1.23.5,<2.0.0',
- 'scipy>=1.9.3,<2.0.0',
- 'spacy>=3.5.1,<4.0.0',
- 'typer>=0.7.0,<0.8.0']
-
-extras_require = \
-{'all': ['gensim>=4.3.0,<5.0.0',
-         'python-Levenshtein>=0.20.9,<0.21.0',
-         'sentence-transformers>=2.2.2,<3.0.0',
-         'torch>=1.13.1,<3.0',
-         'transformers>=4.26.1,<5.0.0'],
- 'levenshtein': ['python-Levenshtein>=0.20.9,<0.21.0'],
- 'sentence-transformers': ['sentence-transformers>=2.2.2,<3.0.0',
-                           'torch>=1.13.1,<3.0'],
- 'transformers': ['torch>=1.13.1,<3.0', 'transformers>=4.26.1,<5.0.0'],
- 'wmd': ['gensim>=4.3.0,<5.0.0']}
-
-entry_points = \
-{'console_scripts': ['nlp-service = nlp_service.server:app']}
-
-setup_kwargs = {
-    'name': 'nlp-service',
-    'version': '1.3.9',
-    'description': 'Microservice for NLP tasks using gRPC',
-    'long_description': '# NLP Microservice\n\nThe goal of this project is to provide a [gRPC](https://grpc.io) server for resource-heavy NLP tasks&mdash;for instance, computing vectors/embeddings for words or sentences.\nBy using [protobuf](https://developers.google.com/protocol-buffers) internally, our NLP server provides native and strongly typed interfaces for many programming languages.\nThere are multiple advantages that arise from outsourcing such computations to such a server:\n\n- If multiple apps rely on NLP, the underlying models (which are usually quite large) only need to be loaded once into the main memory.\n- All programming languages supported by gRPC get easy access to state-of-the-art NLP architectures (e.g., transformers).\n- The logic is consolidated at a central place, drastically decreasing the maintenance effort required.\n\nIn addition to the server, we also provide a client containing convenience functions.\nThis makes it easier for python applications to interact with the gRPC server.\nWe will discuss the client at the end of this README.\n\n## Installation and Setup\n\nWe are using [poetry](https://python-poetry.org) to manage the dependencies.\nFor easier setup, we also provide a `Dockerfile` and a `docker-compose` specification.\n\n### Docker-Compose (recommended)\n\nYou first need to pull this repository.\nThen execute the following in the project directory:\n\n```sh\ndocker-compose build cpu\n# OR, if you need extras:\ndocker-compose build --build-arg EXTRAS="levenshtein transformers" cpu\n# Start the CPU-only container\ndocker-compose up cpu\n```\n\nIn case you have a **CUDA-enabled GPU**, you can replace `cpu` with `cuda` in the above commands and make full use of your card for advanced models like BERT.\n\n### Poetry (advanced)\n\n```sh\n# The server dependencies are optional, thus they have to be installed explicitly.\npoetry install --extras server\n# To get startet, we recommend to use the default spacy model.\n# In case you are dealing with English texts, you can run.\npoetry run python -m spacy download core_en_web_lg\n# To run the server, you need to specify the address it should listen on.\n# In this example, it should liston on port 5678 on localhost.\npoetry run python -m nlp_service "127.0.0.1:50100"\n```\n\n## General Usage\n\nOnce the server is running, you are free to call any of the functions defined in the underlying [protobuf file](https://github.com/recap-utr/arg-services/blob/main/arg_services/nlp/v1/nlp.proto).\nThe corresponding documentation is located at the [Buf Schema Registry](https://buf.build/recap/arg-services/docs/main:arg_services.nlp.v1).\n_Please note:_ The examples here use the Python programming language, but are also directly applicable to any other language supported by gRPC.\n\n```python\nimport grpc\nfrom arg_services.nlp.v1 import nlp_pb2, nlp_pb2_grpc\n\n# First of all, we are creating a channel (i.e., establish a connection to our server)\nchannel = grpc.insecure_channel("127.0.0.1:5678")\n\n# The channel can now be used to create the actual client (allowing us to call all available functions)\nclient = nlp_pb2_grpc.NlpServiceStub(channel)\n\n# Now the time has come to prepare our actual function call.\n# We will start by creating a very simple NlpConfig with the default spacy model.\n# FOr details about the parameters, please have a look at the next section.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  spacy_model="en_core_web_lg",\n)\n\n# Next, we will build a request to query vectors from our server.\nrequest = nlp_pb2.VectorsRequest(\n  # The first parameter is a list of strings that shall be embedded by our server.\n  texts=["What a great tutorial!", "I will definitely recommend this to my friends."],\n  # Now we need to specify which embeddings have to be computed. In this example, we create one vector for each text\n  embedding_levels=[nlp_pb2.EmbeddingLevel.EMBEDDING_LEVEL_DOCUMENT],\n  # The only thing missing now is the spacy configuration we created in the previous step.\n  config=config\n)\n\n# Having created the request, we can now send it to the server and retrieve the corresponding response.\nresponse = client.Vectors(request)\n\n# Due to technical constraints, we cannot directly transfer numpy arrays, thus we convert our response.\nvectors = [np.array(entry.document.vector) for entry in response.vectors]\n```\n\n<!-- TODO: Prefer Vectors instead of Similarities for Python to increase performacne. -->\n\n## Advanced Usage\n\nA central piece for all available function is the `NlpConfig` message, allowing you to create even complex embedding models easily.\nIn addition to [its documentation](https://buf.build/recap/arg-services/docs/main:arg_services.nlp.v1), we will in the following present some examples to demonstrate the possibilities you have.\n\n```python\nfrom arg_services.nlp.v1 import nlp_pb2\n\n# In the example above, we already introduced a quite basic config:\nconfig = nlp_pb2.NlpConfig(\n  # You have to provide a language for every config: https://spacy.io/usage/models#languages\n  language="en",\n  # Also, you need to specify the model that spacy should load: https://spacy.io/models/en\n  spacy_model="en_core_web_lg",\n)\n\n# A central feature of our library is the possibility to combine multiple embedding models, potentially capturing more contextual information.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  # This parameter expects a list of models. If you pass more than one, the respective vectors are **concatenated** to each other\n  # (e.g., two 300-dimensional embeddings will result in a 600-dimensional one).\n  # This approach is based on https://arxiv.org/abs/1803.01400\n  embedding_models=[\n    nlp_pb2.EmbeddingModel(\n      # First select the type of model you would like to use (e.g., SBERT/Sentence Transformers).\n      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SENTENCE_TRANSFORMERS,\n      # Then select the actual model.\n      # Any of those specified on the website (https://www.sbert.net/docs/pretrained_models.html) are allowed.\n      model_name="all-mpnet-base-v2"\n    ),\n    nlp_pb2.EmbeddingModel(\n      # It is also possible to use a standard spacy model\n      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY,\n      model_name="en_core_web_lg",\n      # Since we have selected a word embedding (i.e., it cannot directly encode sentences), the token vectors need to be aggregated somehow.\n      # The default strategy is to use the arithmetic mean, but you are free to use other strategies (e.g., the geometric mean).\n      pooling_type=nlp_pb2.Pooling.POOLING_GMEAN\n    ),\n    nlp_pb2.EmbeddingModel(\n      model_type=nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY,\n      model_name="en_core_web_lg",\n      # Alternatively, it is also possible to use the generalized mean / power mean.\n      # In this example, the selected pmean corresponds to the geometic mean (thus this embedding is identical to the previous one).\n      # This approach is based on https://arxiv.org/abs/1803.01400\n      pmean=0\n    )\n  ]\n  # This setting is now optional and only needed if you need spacy features (e.g., POS tagging) besides embeddings.\n  # spacy_model="en_core_web_lg",\n)\n\n# If computing the similarity between strings, you get one additional parameter.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  # To keep the example simple, we will now only use a single spacy model instead of the more powerful embedding models.\n  # However, it is of course possible to use them here as well.\n  spacy_model="en_core_web_lg",\n  # If not specified, we will always use the cosine similarity when comparing two strings.\n  # As indicated in a recent paper (https://arxiv.org/abs/1904.13264), you may achieve better results with alternative approaches like DynaMax Jaccard.\n  # Please note that this particular method ignores your selected pooling method due to the fact that even plain word embeddings are not pooled at all.\n  similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_DYNAMAX_JACCARD\n)\n\n# It is also possible to determine a similarity score without the use of embeddings.\nconfig = nlp_pb2.NlpConfig(\n  language="en",\n  spacy_model="en_core_web_lg",\n  # Traditional metric (Jaccard similarity and Levenshtein edit distance) are also available\n  similarity_method=nlp_pb2.SimilarityMethod.SIMILARITY_METHOD_EDIT\n)\n```\n',
-    'author': 'Mirko Lenz',
-    'author_email': 'info@mirko-lenz.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'http://recap.uni-trier.de',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

