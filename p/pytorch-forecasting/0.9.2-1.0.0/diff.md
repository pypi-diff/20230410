# Comparing `tmp/pytorch_forecasting-0.9.2.tar.gz` & `tmp/pytorch_forecasting-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch_forecasting-0.9.2.tar", max compression
+gzip compressed data, was "pytorch_forecasting-1.0.0.tar", max compression
```

## Comparing `pytorch_forecasting-0.9.2.tar` & `pytorch_forecasting-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,34 @@
--rw-r--r--   0        0        0     1068 2021-11-29 19:54:54.431843 pytorch_forecasting-0.9.2/LICENSE
--rwxr-xr-x   0        0        0     9281 2021-11-29 19:54:54.431843 pytorch_forecasting-0.9.2/README.md
--rw-r--r--   0        0        0     2576 2021-11-29 19:55:03.903905 pytorch_forecasting-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2239 2021-11-29 19:55:03.903905 pytorch_forecasting-0.9.2/pytorch_forecasting/__init__.py
--rw-r--r--   0        0        0      642 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/data/__init__.py
--rw-r--r--   0        0        0    34976 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/data/encoders.py
--rw-r--r--   0        0        0     3361 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/data/examples.py
--rw-r--r--   0        0        0    90596 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/data/timeseries.py
--rw-r--r--   0        0        0    41897 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/metrics.py
--rw-r--r--   0        0        0      978 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/__init__.py
--rw-r--r--   0        0        0    88439 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/base_model.py
--rw-r--r--   0        0        0     2377 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/baseline.py
--rw-r--r--   0        0        0    11096 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/basic_rnn/__init__.py
--rw-r--r--   0        0        0    19233 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/deepar/__init__.py
--rw-r--r--   0        0        0     7347 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/mlp/__init__.py
--rw-r--r--   0        0        0     1564 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/mlp/submodules.py
--rw-r--r--   0        0        0    16214 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/nbeats/__init__.py
--rw-r--r--   0        0        0     6395 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/nbeats/sub_modules.py
--rw-r--r--   0        0        0      217 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/nn/__init__.py
--rw-r--r--   0        0        0     3406 2021-11-29 19:54:54.467843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/nn/embeddings.py
--rw-r--r--   0        0        0     7736 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/nn/rnn.py
--rw-r--r--   0        0        0    13422 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/rnn/__init__.py
--rw-r--r--   0        0        0    36906 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/temporal_fusion_transformer/__init__.py
--rw-r--r--   0        0        0    15911 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/temporal_fusion_transformer/sub_modules.py
--rw-r--r--   0        0        0     9865 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/models/temporal_fusion_transformer/tuning.py
--rw-r--r--   0        0        0     8649 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/optim.py
--rw-r--r--   0        0        0    12974 2021-11-29 19:54:54.471843 pytorch_forecasting-0.9.2/pytorch_forecasting/utils.py
--rw-r--r--   0        0        0    10777 2021-11-29 19:55:04.469378 pytorch_forecasting-0.9.2/setup.py
--rw-r--r--   0        0        0    10904 2021-11-29 19:55:04.470124 pytorch_forecasting-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-10 19:56:30.807288 pytorch_forecasting-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     9637 2023-04-10 19:56:30.807288 pytorch_forecasting-1.0.0/README.md
+-rw-r--r--   0        0        0     2963 2023-04-10 19:56:56.435579 pytorch_forecasting-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2373 2023-04-10 19:56:56.435579 pytorch_forecasting-1.0.0/pytorch_forecasting/__init__.py
+-rw-r--r--   0        0        0      687 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/data/__init__.py
+-rw-r--r--   0        0        0    47622 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/data/encoders.py
+-rw-r--r--   0        0        0     3357 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/data/examples.py
+-rw-r--r--   0        0        0     5633 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/data/samplers.py
+-rw-r--r--   0        0        0    90005 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/data/timeseries.py
+-rw-r--r--   0        0        0     1324 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/__init__.py
+-rw-r--r--   0        0        0    17629 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/_mqf2_utils.py
+-rw-r--r--   0        0        0    36785 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/base_metrics.py
+-rw-r--r--   0        0        0    22296 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/distributions.py
+-rw-r--r--   0        0        0    10491 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/point.py
+-rw-r--r--   0        0        0     1845 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/quantile.py
+-rw-r--r--   0        0        0     1042 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/__init__.py
+-rw-r--r--   0        0        0   102654 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/base_model.py
+-rw-r--r--   0        0        0     2377 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/baseline.py
+-rw-r--r--   0        0        0    19790 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/deepar/__init__.py
+-rw-r--r--   0        0        0     7328 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/mlp/__init__.py
+-rw-r--r--   0        0        0     1564 2023-04-10 19:56:30.867288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/mlp/submodules.py
+-rw-r--r--   0        0        0    16638 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nbeats/__init__.py
+-rw-r--r--   0        0        0     6391 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nbeats/sub_modules.py
+-rw-r--r--   0        0        0    25154 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nhits/__init__.py
+-rw-r--r--   0        0        0    13655 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nhits/sub_modules.py
+-rw-r--r--   0        0        0      380 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nn/__init__.py
+-rw-r--r--   0        0        0     8969 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nn/embeddings.py
+-rw-r--r--   0        0        0     7736 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/nn/rnn.py
+-rw-r--r--   0        0        0    13439 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/rnn/__init__.py
+-rw-r--r--   0        0        0    39159 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/temporal_fusion_transformer/__init__.py
+-rw-r--r--   0        0        0    15926 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/temporal_fusion_transformer/sub_modules.py
+-rw-r--r--   0        0        0     9349 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/models/temporal_fusion_transformer/tuning.py
+-rw-r--r--   0        0        0    18287 2023-04-10 19:56:30.871288 pytorch_forecasting-1.0.0/pytorch_forecasting/utils.py
+-rw-r--r--   0        0        0    11608 1970-01-01 00:00:00.000000 pytorch_forecasting-1.0.0/PKG-INFO
```

### Comparing `pytorch_forecasting-0.9.2/LICENSE` & `pytorch_forecasting-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_forecasting-0.9.2/README.md` & `pytorch_forecasting-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 - A timeseries dataset class which abstracts handling variable transformations, missing values,
   randomized subsampling, multiple history lengths, etc.
 - A base model class which provides basic training of timeseries models along with logging in tensorboard
   and generic visualizations such actual vs predictions and dependency plots
 - Multiple neural network architectures for timeseries forecasting that have been enhanced
   for real-world deployment and come with in-built interpretation capabilities
 - Multi-horizon timeseries metrics
-- Ranger optimizer for faster model training
 - Hyperparameter tuning with [optuna](https://optuna.readthedocs.io/)
 
 The package is built on [pytorch-lightning](https://pytorch-lightning.readthedocs.io/) to allow training on CPUs, single and multiple GPUs out-of-the-box.
 
 # Installation
 
 If you are working on windows, you need to first install PyTorch with
@@ -51,46 +50,51 @@
 
 Alternatively, you can install the package via conda
 
 `conda install pytorch-forecasting pytorch -c pytorch>=1.7 -c conda-forge`
 
 PyTorch Forecasting is now installed from the conda-forge channel while PyTorch is install from the pytorch channel.
 
+To use the MQF2 loss (multivariate quantile loss), also install
+`pip install pytorch-forecasting[mqf2]`
+
 # Documentation
 
 Visit [https://pytorch-forecasting.readthedocs.io](https://pytorch-forecasting.readthedocs.io) to read the
 documentation with detailed tutorials.
 
 # Available models
 
 The documentation provides a [comparison of available models](https://pytorch-forecasting.readthedocs.io/en/latest/models.html).
 
 - [Temporal Fusion Transformers for Interpretable Multi-horizon Time Series Forecasting](https://arxiv.org/pdf/1912.09363.pdf)
   which outperforms DeepAR by Amazon by 36-69% in benchmarks
 - [N-BEATS: Neural basis expansion analysis for interpretable time series forecasting](http://arxiv.org/abs/1905.10437)
   which has (if used as ensemble) outperformed all other methods including ensembles of traditional statical
   methods in the M4 competition. The M4 competition is arguably the most important benchmark for univariate time series forecasting.
+- [N-HiTS: Neural Hierarchical Interpolation for Time Series Forecasting](http://arxiv.org/abs/2201.12886) which supports covariates and has consistently beaten N-BEATS. It is also particularly well-suited for long-horizon forecasting.
 - [DeepAR: Probabilistic forecasting with autoregressive recurrent networks](https://www.sciencedirect.com/science/article/pii/S0169207019301888)
   which is the one of the most popular forecasting algorithms and is often used as a baseline
 - Simple standard networks for baselining: LSTM and GRU networks as well as a MLP on the decoder
 - A baseline model that always predicts the latest known value
 
 To implement new models or other custom components, see the [How to implement new models tutorial](https://pytorch-forecasting.readthedocs.io/en/latest/tutorials/building.html). It covers basic as well as advanced architectures.
 
 # Usage example
 
 Networks can be trained with the [PyTorch Lighning Trainer](https://pytorch-lightning.readthedocs.io/en/latest/common/trainer.html) on [pandas Dataframes](https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe) which are first converted to a [TimeSeriesDataSet](https://pytorch-forecasting.readthedocs.io/en/latest/data.html).
 
 ```python
 # imports for training
-import pytorch_lightning as pl
-from pytorch_lightning.loggers import TensorBoardLogger
-from pytorch_lightning.callbacks import EarlyStopping, LearningRateMonitor
+import lightning.pytorch as pl
+from lightning.pytorch.loggers import TensorBoardLogger
+from lightning.pytorch.callbacks import EarlyStopping, LearningRateMonitor
 # import dataset, network to train and metric to optimize
 from pytorch_forecasting import TimeSeriesDataSet, TemporalFusionTransformer, QuantileLoss
+from lightning.pytorch.tuner import Tuner
 
 # load data: this is pandas dataframe with at least a column for
 # * the target (what you want to predict)
 # * the timeseries ID (which should be a unique string to identify each timeseries)
 # * the time of the observation (which should be a monotonically increasing integer)
 data = ...
 
@@ -125,15 +129,15 @@
 val_dataloader = validation.to_dataloader(train=False, batch_size=batch_size, num_workers=2)
 
 # create PyTorch Lighning Trainer with early stopping
 early_stop_callback = EarlyStopping(monitor="val_loss", min_delta=1e-4, patience=1, verbose=False, mode="min")
 lr_logger = LearningRateMonitor()
 trainer = pl.Trainer(
     max_epochs=100,
-    gpus=0,  # run on CPU, if on multiple GPUs, use accelerator="ddp"
+    accelerator="auto",  # run on CPU, if on multiple GPUs, use strategy="ddp"
     gradient_clip_val=0.1,
     limit_train_batches=30,  # 30 batches per epoch
     callbacks=[lr_logger, early_stop_callback],
     logger=TensorBoardLogger("lightning_logs")
 )
 
 # define network to train - the architecture is mostly inferred from the dataset, so that only a few hyperparameters have to be set by the user
@@ -152,20 +156,20 @@
     # optimizer parameters
     learning_rate=0.03,
     reduce_on_plateau_patience=4
 )
 print(f"Number of parameters in network: {tft.size()/1e3:.1f}k")
 
 # find the optimal learning rate
-res = trainer.lr_find(
-    tft, train_dataloader=train_dataloader, val_dataloaders=val_dataloader, early_stop_threshold=1000.0, max_lr=0.3,
+res = Tuner(trainer).lr_find(
+    tft, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader, early_stop_threshold=1000.0, max_lr=0.3,
 )
 # and plot the result - always visually confirm that the suggested learning rate makes sense
 print(f"suggested learning rate: {res.suggestion()}")
 fig = res.plot(show=True, suggest=True)
 fig.show()
 
 # fit the model on the data - redefine the model with the correct learning rate if necessary
 trainer.fit(
-    tft, train_dataloader=train_dataloader, val_dataloaders=val_dataloader,
+    tft, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader,
 )
 ```
```

### Comparing `pytorch_forecasting-0.9.2/pyproject.toml` & `pytorch_forecasting-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.nbqa.mutate]
 isort = 1
 black = 1
 
 [tool.poetry]
 name = "pytorch_forecasting"
 readme = "README.md"  # Markdown files are supported
-version = "0.9.2"  # is being replaced automatically
+version = "1.0.0"  # is being replaced automatically
 
 authors = ["Jan Beitner"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
@@ -48,30 +48,35 @@
     "License :: OSI Approved :: MIT License"]
 description = "Forecasting timeseries with PyTorch - dataloaders, normalizers, metrics and models"
 repository = "https://github.com/jdb78/pytorch-forecasting"
 documentation = "https://pytorch-forecasting.readthedocs.io"
 homepage = "https://pytorch-forecasting.readthedocs.io"
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
+python = ">=3.8,<3.11"
 
-torch = "^1.7"
-pytorch-lightning = "^1.2.4"
-optuna = "^2.3.0"
-scipy = "*"
-pandas = "^1.3.0"
-scikit-learn = ">=0.24,<1.1"
+torch = "^2.0.0"
+lightning = "^2.0.0"
+optuna = "^3.1.0"
+scipy = "^1.8"
+pandas = ">=1.3.0,<=3.0.0"
+scikit-learn = "^1.2"
 matplotlib = "*"
 statsmodels = "*"
 
 pytest-github-actions-annotate-failures = {version = "*", optional = true}
+networkx = {version = "^3.0.0", optional = true}
+cpflows = {version="^0.1.2", optional = true}
+fastapi = ">=0.80"
+pytorch-optimizer = "^2.5.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+pydocstyle = "^6.1.1"
 # checks and make tools
-pre-commit = "^2.15.0"
+pre-commit = "^3.2.0"
 
 invoke = "*"
 flake8 = "*"
 mypy = "*"
 pylint = "*"
 isort = "*"
 
@@ -81,29 +86,35 @@
 pytest-cov = "*"
 pytest-sugar = "*"
 coverage = "*"
 pyarrow = "*"
 
 # jupyter notebook
 ipykernel = "*"
-black = { version = "*", allow-prereleases = true }
+black = { version = "*", allow-prereleases = true, extras = ["jupyter"] }
 
 # documentatation
 sphinx = "*"
 pydata-sphinx-theme = "*"
 nbsphinx = "*"
-pandoc = "*"
+# pandoc = "*"  # todo: bring back later when install works again
 recommonmark = "*"
+ipywidgets = "^8.0.1"
+pytest-dotenv = "^0.5.2"
+tensorboard = "^2.12.1"
+pandoc = "^2.3"
 
 
 [tool.poetry.extras]  # extras
 github-actions = ["pytest-github-actions-annotate-failures"]
+graph = ["networkx"]
+mqf2 = ["cpflows"]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 dirty = false
 style = "semver"  # semantic versioning
 
 [build-system]  # make the package pip installable
-requires = ["poetry_core>=1.1.0", "poetry-dynamic-versioning>=0.9.0"]
-build-backend = "poetry.core.masonry.api"
+requires = ["poetry-core>=1.0.7", "poetry-dynamic-versioning>=0.13.1"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 )
 from pytorch_forecasting.metrics import (
     MAE,
     MAPE,
     MASE,
     RMSE,
     SMAPE,
-    AggregationMetric,
     BetaDistributionLoss,
-    CompositeMetric,
     CrossEntropy,
     DistributionLoss,
+    ImplicitQuantileNetworkDistributionLoss,
     LogNormalDistributionLoss,
-    Metric,
+    MQF2DistributionLoss,
     MultiHorizonMetric,
     MultiLoss,
+    MultivariateNormalDistributionLoss,
     NegativeBinomialDistributionLoss,
     NormalDistributionLoss,
     PoissonLoss,
     QuantileLoss,
 )
 from pytorch_forecasting.models import (
     GRU,
@@ -36,14 +36,15 @@
     Baseline,
     BaseModel,
     BaseModelWithCovariates,
     DecoderMLP,
     DeepAR,
     MultiEmbedding,
     NBeats,
+    NHiTS,
     RecurrentNetwork,
     TemporalFusionTransformer,
     get_rnn,
 )
 from pytorch_forecasting.utils import (
     apply_to_list,
     autocorrelation,
@@ -62,34 +63,35 @@
     "TimeSeriesDataSet",
     "GroupNormalizer",
     "EncoderNormalizer",
     "NaNLabelEncoder",
     "MultiNormalizer",
     "TemporalFusionTransformer",
     "NBeats",
+    "NHiTS",
     "Baseline",
     "DeepAR",
     "BaseModel",
     "BaseModelWithCovariates",
     "AutoRegressiveBaseModel",
     "AutoRegressiveBaseModelWithCovariates",
     "MultiHorizonMetric",
     "MultiLoss",
     "MAE",
     "MAPE",
     "MASE",
     "SMAPE",
-    "Metric",
-    "AggregationMetric",
-    "CompositeMetric",
     "DistributionLoss",
     "BetaDistributionLoss",
     "LogNormalDistributionLoss",
     "NegativeBinomialDistributionLoss",
     "NormalDistributionLoss",
+    "ImplicitQuantileNetworkDistributionLoss",
+    "MultivariateNormalDistributionLoss",
+    "MQF2DistributionLoss",
     "CrossEntropy",
     "PoissonLoss",
     "QuantileLoss",
     "RMSE",
     "get_rnn",
     "LSTM",
     "GRU",
@@ -105,8 +107,8 @@
     "move_to_device",
     "integer_histogram",
     "groupby_apply",
     "profile",
     "unpack_sequence",
 ]
 
-__version__ = "0.9.2"
+__version__ = "1.0.0"
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/data/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/data/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from pytorch_forecasting.data.encoders import (
     EncoderNormalizer,
     GroupNormalizer,
     MultiNormalizer,
     NaNLabelEncoder,
     TorchNormalizer,
 )
-from pytorch_forecasting.data.timeseries import TimeSeriesDataSet, TimeSynchronizedBatchSampler
+from pytorch_forecasting.data.samplers import TimeSynchronizedBatchSampler
+from pytorch_forecasting.data.timeseries import TimeSeriesDataSet
 
 __all__ = [
     "TimeSeriesDataSet",
     "NaNLabelEncoder",
     "GroupNormalizer",
     "TorchNormalizer",
     "EncoderNormalizer",
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/data/encoders.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/data/encoders.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,220 @@
 """
 Encoders for encoding categorical variables and scaling continuous data.
 """
-from typing import Callable, Dict, Iterable, List, Tuple, Union
+
+from typing import Any, Callable, Dict, Iterable, List, Tuple, Union
 import warnings
 
 import numpy as np
 import pandas as pd
-from pandas.core.algorithms import isin
 from sklearn.base import BaseEstimator, TransformerMixin
 import torch
+from torch.distributions import constraints
+from torch.distributions.transforms import (
+    ExpTransform,
+    PowerTransform,
+    SigmoidTransform,
+    Transform,
+    _clipped_sigmoid,
+    identity_transform,
+)
 import torch.nn.functional as F
 from torch.nn.utils import rnn
 
+from pytorch_forecasting.utils import InitialParameterRepresenterMixIn
+
+
+def _plus_one(x):
+    return x + 1
+
+
+def _minus_one(x):
+    return x - 1
+
+
+def _identity(x):
+    return x
+
+
+def _clipped_logit(x):
+    finfo = torch.finfo(x.dtype)
+    x = x.clamp(min=finfo.eps, max=1.0 - finfo.eps)
+    return x.log() - (-x).log1p()
+
+
+def softplus_inv(y):
+    finfo = torch.finfo(y.dtype)
+    return y.where(y > 20.0, y + (y + finfo.eps).neg().expm1().neg().log())
+
+
+def _square(y):
+    return torch.pow(y, 2.0)
+
+
+def _clipped_log(y):
+    finfo = torch.finfo(y.dtype)
+    return y.log().clamp(min=-1 / finfo.eps)
+
+
+class SoftplusTransform(Transform):
+    r"""
+    Transform via the mapping :math:`\text{Softplus}(x) = \log(1 + \exp(x))`.
+    The implementation reverts to the linear function when :math:`x > 20`.
+    """
+    domain = constraints.real
+    codomain = constraints.positive
+    bijective = True
+    sign = +1
+
+    def __eq__(self, other):
+        return isinstance(other, SoftplusTransform)
+
+    def _call(self, x):
+        return F.softplus(x)
+
+    def _inverse(self, y):
+        return softplus_inv(y)
+
+    def log_abs_det_jacobian(self, x, y):
+        return -F.softplus(-x)
+
+
+class Expm1Transform(ExpTransform):
+    codomain = constraints.greater_than_eq(-1.0)
+
+    def _call(self, x):
+        return super()._call(x) - 1.0
+
+    def _inverse(self, y):
+        return super()._inverse(y + 1.0)
+
+
+class MinusOneTransform(Transform):
+    r"""
+    Transform x -> x - 1.
+    """
+    domain = constraints.real
+    codomain = constraints.real
+    sign: int = 1
+    bijective: bool = True
+
+    def _call(self, x):
+        return x - 1.0
+
+    def _inverse(self, y):
+        return y + 1.0
+
+    def log_abs_det_jacobian(self, x, y):
+        return 0.0
+
+
+class ReLuTransform(Transform):
+    r"""
+    Transform x -> max(0, x).
+    """
+    domain = constraints.real
+    codomain = constraints.nonnegative
+    sign: int = 1
+    bijective: bool = False
+
+    def _call(self, x):
+        return F.relu(x)
+
+    def _inverse(self, y):
+        return y
+
+    def log_abs_det_jacobian(self, x, y):
+        return 0.0
+
+
+class TransformMixIn:
+    """Mixin for providing pre- and post-processing capabilities to encoders.
+
+    Class should have a ``transformation`` attribute to indicate how to preprocess data.
+    """
+
+    # dict of PyTorch functions that transforms and inversely transforms values.
+    # inverse entry required if "reverse" is not the "inverse" of "forward".
+    TRANSFORMATIONS = {
+        "log": dict(forward=_clipped_log, reverse=torch.exp, inverse_torch=ExpTransform()),
+        "log1p": dict(forward=torch.log1p, reverse=torch.exp, inverse=torch.expm1, inverse_torch=Expm1Transform()),
+        "logit": dict(forward=_clipped_logit, reverse=_clipped_sigmoid, inverse_torch=SigmoidTransform()),
+        "count": dict(forward=_plus_one, reverse=F.softplus, inverse=_minus_one, inverse_torch=MinusOneTransform()),
+        "softplus": dict(forward=softplus_inv, reverse=F.softplus, inverse_torch=SoftplusTransform()),
+        "relu": dict(forward=_identity, reverse=F.relu, inverse=_identity, inverse_torch=ReLuTransform()),
+        "sqrt": dict(forward=torch.sqrt, reverse=_square, inverse_torch=PowerTransform(exponent=2.0)),
+    }
+
+    @classmethod
+    def get_transform(cls, transformation: Union[str, Dict[str, Callable]]) -> Dict[str, Callable]:
+        """Return transformation functions.
+
+        Args:
+            transformation (Union[str, Dict[str, Callable]]): name of transformation or
+                dictionary with transformation information.
+
+        Returns:
+            Dict[str, Callable]: dictionary with transformation functions (forward, reverse, inverse and inverse_torch)
+        """
+        if isinstance(transformation, str):
+            transform = cls.TRANSFORMATIONS[transformation]
+        else:
+            transform = transformation
+        transform.setdefault("forward", _identity)
+        transform.setdefault("reverse", _identity)
+        return transform
+
+    def preprocess(
+        self, y: Union[pd.Series, pd.DataFrame, np.ndarray, torch.Tensor]
+    ) -> Union[np.ndarray, torch.Tensor]:
+        """
+        Preprocess input data (e.g. take log).
+
+        Uses ``transform`` attribute to determine how to apply transform.
+
+        Returns:
+            Union[np.ndarray, torch.Tensor]: return rescaled series with type depending on input type
+        """
+        if self.transformation is None:
+            return y
+
+        if isinstance(y, torch.Tensor):
+            y = self.get_transform(self.transformation)["forward"](y)
+        else:
+            # convert first to tensor, then transform and then convert to numpy array
+            if isinstance(y, (pd.Series, pd.DataFrame)):
+                y = y.to_numpy()
+            y = torch.as_tensor(y)
+            y = self.get_transform(self.transformation)["forward"](y)
+            y = np.asarray(y)
+        return y
+
+    def inverse_preprocess(self, y: Union[pd.Series, np.ndarray, torch.Tensor]) -> Union[np.ndarray, torch.Tensor]:
+        """
+        Inverse preprocess re-scaled data (e.g. take exp).
+
+        Uses ``transform`` attribute to determine how to apply inverse transform.
+
+        Returns:
+            Union[np.ndarray, torch.Tensor]: return rescaled series with type depending on input type
+        """
+        if self.transformation is None:
+            pass
+        elif isinstance(y, torch.Tensor):
+            y = self.get_transform(self.transformation)["reverse"](y)
+        else:
+            # convert first to tensor, then transform and then convert to numpy array
+            y = torch.as_tensor(y)
+            y = self.get_transform(self.transformation)["reverse"](y)
+            y = np.asarray(y)
+        return y
+
 
-class NaNLabelEncoder(BaseEstimator, TransformerMixin):
+class NaNLabelEncoder(InitialParameterRepresenterMixIn, BaseEstimator, TransformerMixin, TransformMixIn):
     """
     Labelencoder that can optionally always encode nan and unknown classes (in transform) as class ``0``
     """
 
     def __init__(self, add_nan: bool = False, warn: bool = True):
         """
         init NaNLabelEncoder
@@ -52,15 +249,17 @@
 
         Args:
             y (pd.Series): series for which to carry out assessment
 
         Returns:
             bool: True if series is numeric
         """
-        return y.dtype.kind in "bcif" or (isinstance(y, pd.CategoricalDtype) and y.cat.categories.dtype.kind in "bcif")
+        return y.dtype.kind in "bcif" or (
+            isinstance(y.dtype, pd.CategoricalDtype) and y.cat.categories.dtype.kind in "bcif"
+        )
 
     def fit(self, y: pd.Series, overwrite: bool = False):
         """
         Fit transformer
 
         Args:
             y (pd.Series): input data to fit on
@@ -187,201 +386,150 @@
 
         Returns:
             np.ndarray: zero array.
         """
         return np.zeros(2, dtype=np.float64)
 
 
-def _plus_one(x):
-    return x + 1
-
-
-def _identity(x):
-    return x
-
-
-def _clamp_zero(x):
-    return x.clamp(0.0)
-
-
-class TorchNormalizer(BaseEstimator, TransformerMixin):
+class TorchNormalizer(InitialParameterRepresenterMixIn, BaseEstimator, TransformerMixin, TransformMixIn):
     """
     Basic target transformer that can be fit also on torch tensors.
     """
 
-    # transformation and inverse transformation
-    TRANSFORMATIONS = {
-        "log": (torch.log, torch.exp),
-        "log1p": (torch.log1p, torch.exp),
-        "logit": (torch.logit, torch.sigmoid),
-        "softplus": (_plus_one, F.softplus),
-        "relu": (_identity, _clamp_zero),
-    }
-
     def __init__(
         self,
         method: str = "standard",
         center: bool = True,
         transformation: Union[str, Tuple[Callable, Callable]] = None,
-        eps: float = 1e-8,
+        method_kwargs: Dict[str, Any] = {},
     ):
         """
-        Initialize
-
         Args:
             method (str, optional): method to rescale series. Either "identity", "standard" (standard scaling)
                 or "robust" (scale using quantiles 0.25-0.75). Defaults to "standard".
+            method_kwargs (Dict[str, Any], optional): Dictionary of method specific arguments as listed below
+                * "robust" method: "upper", "lower", "center" quantiles defaulting to 0.75, 0.25 and 0.5
             center (bool, optional): If to center the output to zero. Defaults to True.
-            transformation (Union[str, Tuple[Callable, Callable]] optional): Transform values before
+            transformation (Union[str, Dict[str, Callable]] optional): Transform values before
                 applying normalizer. Available options are
 
                 * None (default): No transformation of values
                 * log: Estimate in log-space leading to a multiplicative model
                 * logp1: Estimate in log-space but add 1 to values before transforming for stability
-                    (e.g. if many small values <<1 are present).
-                    Note, that inverse transform is still only `torch.exp()` and not `torch.expm1()`.
+                  (e.g. if many small values <<1 are present).
+                  Note, that inverse transform is still only `torch.exp()` and not `torch.expm1()`.
                 * logit: Apply logit transformation on values that are between 0 and 1
-                * softplus: Apply softplus to output (inverse transformation) and x + 1 to input (transformation)
+                * count: Apply softplus to output (inverse transformation) and x + 1 to input (transformation)
+                * softplus: Apply softplus to output (inverse transformation) and inverse softplus to input
+                    (transformation)
                 * relu: Apply max(0, x) to output
-                * Tuple[Callable, Callable] of PyTorch functions that transforms and inversely transforms values.
-
-            eps (float, optional): Number for numerical stability of calculations.
-                Defaults to 1e-8.
+                * Dict[str, Callable] of PyTorch functions that transforms and inversely transforms values.
+                  ``forward`` and ``reverse`` entries are required. ``inverse`` transformation is optional and
+                  should be defined if ``reverse`` is not the inverse of the forward transformation. ``inverse_torch``
+                  can be defined to provide a torch distribution transform for inverse transformations.
         """
         self.method = method
         assert method in ["standard", "robust", "identity"], f"method has invalid value {method}"
         self.center = center
-        self.eps = eps
         self.transformation = transformation
+        self.method_kwargs = method_kwargs
 
     def get_parameters(self, *args, **kwargs) -> torch.Tensor:
         """
         Returns parameters that were used for encoding.
 
         Returns:
             torch.Tensor: First element is center of data and second is scale
         """
         return torch.stack([torch.as_tensor(self.center_), torch.as_tensor(self.scale_)], dim=-1)
 
-    def preprocess(
-        self, y: Union[pd.Series, pd.DataFrame, np.ndarray, torch.Tensor]
-    ) -> Union[np.ndarray, torch.Tensor]:
-        """
-        Preprocess input data (e.g. take log).
-
-        Uses ``transform`` attribute to determine how to apply transform.
-
-        Returns:
-            Union[np.ndarray, torch.Tensor]: return rescaled series with type depending on input type
-        """
-        if self.transformation is None:
-            return y
-
-        # protect against numerical instabilities
-        if isinstance(self.transformation, str) and self.transformation == "logit":
-            # need to apply eps slightly differently
-            y = y / (1 + 2 * self.eps) + self.eps
-        else:
-            y = y + self.eps
-
-        if isinstance(y, torch.Tensor):
-            y = self.TRANSFORMATIONS.get(self.transformation, self.transformation)[0](y)
-        else:
-            # convert first to tensor, then transform and then convert to numpy array
-            if isinstance(y, (pd.Series, pd.DataFrame)):
-                y = y.to_numpy()
-            y = torch.as_tensor(y)
-            y = self.TRANSFORMATIONS.get(self.transformation, self.transformation)[0](y)
-            y = np.asarray(y)
-        return y
-
-    def inverse_preprocess(self, y: Union[pd.Series, np.ndarray, torch.Tensor]) -> Union[np.ndarray, torch.Tensor]:
-        """
-        Inverse preprocess re-scaled data (e.g. take exp).
-
-        Uses ``transform`` attribute to determine how to apply inverse transform.
-
-        Returns:
-            Union[np.ndarray, torch.Tensor]: return rescaled series with type depending on input type
-        """
-        if self.transformation is None:
-            pass
-        elif isinstance(y, torch.Tensor):
-            y = self.TRANSFORMATIONS.get(self.transformation, self.transformation)[1](y)
-        else:
-            # convert first to tensor, then transform and then convert to numpy array
-            y = torch.as_tensor(y)
-            y = self.TRANSFORMATIONS.get(self.transformation, self.transformation)[1](y)
-            y = np.asarray(y)
-        return y
-
     def fit(self, y: Union[pd.Series, np.ndarray, torch.Tensor]):
         """
         Fit transformer, i.e. determine center and scale of data
 
         Args:
             y (Union[pd.Series, np.ndarray, torch.Tensor]): input data
 
         Returns:
             TorchNormalizer: self
         """
         y = self.preprocess(y)
+        self._set_parameters(y_center=y, y_scale=y)
+        return self
 
+    def _set_parameters(
+        self, y_center: Union[pd.Series, np.ndarray, torch.Tensor], y_scale: Union[pd.Series, np.ndarray, torch.Tensor]
+    ):
+        """
+        Calculate parameters for scale and center based on input timeseries
+
+        Args:
+            y_center (Union[pd.Series, np.ndarray, torch.Tensor]): timeseries for calculating center
+            y_scale (Union[pd.Series, np.ndarray, torch.Tensor]): timeseries for calculating scale
+        """
+        if isinstance(y_center, torch.Tensor):
+            eps = torch.finfo(y_center.dtype).eps
+        else:
+            eps = np.finfo(np.float16).eps
         if self.method == "identity":
-            if isinstance(y, torch.Tensor):
-                self.center_ = torch.zeros(y.size()[:-1])
-                self.scale_ = torch.ones(y.size()[:-1])
-            elif isinstance(y, (np.ndarray, pd.Series, pd.DataFrame)):
-                self.center_ = np.zeros(y.shape[:-1])
-                self.scale_ = np.ones(y.shape[:-1])
+            if isinstance(y_center, torch.Tensor):
+                self.center_ = torch.zeros(y_center.size()[:-1])
+                self.scale_ = torch.ones(y_scale.size()[:-1])
+            elif isinstance(y_center, (np.ndarray, pd.Series, pd.DataFrame)):
+                # numpy default type is numpy.float64 while torch default type is torch.float32 (if not changed)
+                # therefore, we first generate torch tensors (with torch default type) and then
+                # convert them to numpy arrays
+                self.center_ = torch.zeros(y_center.shape[:-1]).numpy()
+                self.scale_ = torch.ones(y_scale.shape[:-1]).numpy()
             else:
                 self.center_ = 0.0
                 self.scale_ = 1.0
 
         elif self.method == "standard":
-            if isinstance(y, torch.Tensor):
-                self.center_ = torch.mean(y, dim=-1)
-                self.scale_ = torch.std(y, dim=-1) + self.eps
-            elif isinstance(y, np.ndarray):
-                self.center_ = np.mean(y, axis=-1)
-                self.scale_ = np.std(y, axis=-1) + self.eps
+            if isinstance(y_center, torch.Tensor):
+                self.center_ = torch.mean(y_center, dim=-1)
+                self.scale_ = torch.std(y_scale, dim=-1) + eps
+            elif isinstance(y_center, np.ndarray):
+                self.center_ = np.mean(y_center, axis=-1)
+                self.scale_ = np.std(y_scale, axis=-1) + eps
             else:
-                self.center_ = np.mean(y)
-                self.scale_ = np.std(y) + self.eps
+                self.center_ = np.mean(y_center)
+                self.scale_ = np.std(y_scale) + eps
+            # correct numpy scalar dtype promotion, e.g. fix type from `np.float32(0.0) + 1e-8` gives `np.float64(1e-8)`
+            if isinstance(self.scale_, np.ndarray):
+                self.scale_ = self.scale_.astype(y_scale.dtype)
 
         elif self.method == "robust":
-            if isinstance(y, torch.Tensor):
-                self.center_ = torch.median(y, dim=-1).values
-                q_75 = y.kthvalue(int(len(y) * 0.75), dim=-1).values
-                q_25 = y.kthvalue(int(len(y) * 0.25), dim=-1).values
-            elif isinstance(y, np.ndarray):
-                self.center_ = np.median(y, axis=-1)
-                q_75 = np.percentile(y, 75, axis=-1)
-                q_25 = np.percentile(y, 25, axis=-1)
-            else:
-                self.center_ = np.median(y)
-                q_75 = np.percentile(y, 75)
-                q_25 = np.percentile(y, 25)
-            self.scale_ = (q_75 - q_25) / 2.0 + self.eps
-        if not self.center:
+            if isinstance(y_center, torch.Tensor):
+                self.center_ = y_center.quantile(self.method_kwargs.get("center", 0.5), dim=-1)
+                q_75 = y_scale.quantile(self.method_kwargs.get("upper", 0.75), dim=-1)
+                q_25 = y_scale.quantile(self.method_kwargs.get("lower", 0.25), dim=-1)
+            elif isinstance(y_center, np.ndarray):
+                self.center_ = np.percentile(y_center, self.method_kwargs.get("center", 0.5) * 100, axis=-1)
+                q_75 = np.percentile(y_scale, self.method_kwargs.get("upper", 0.75) * 100, axis=-1)
+                q_25 = np.percentile(y_scale, self.method_kwargs.get("lower", 0.25) * 100, axis=-1)
+            else:
+                self.center_ = np.percentile(y_center, self.method_kwargs.get("center", 0.5) * 100, axis=-1)
+                q_75 = np.percentile(y_scale, self.method_kwargs.get("upper", 0.75) * 100)
+                q_25 = np.percentile(y_scale, self.method_kwargs.get("lower", 0.25) * 100)
+            self.scale_ = (q_75 - q_25) / 2.0 + eps
+        if not self.center and self.method != "identity":
             self.scale_ = self.center_
-            if isinstance(y, torch.Tensor):
+            if isinstance(y_center, torch.Tensor):
                 self.center_ = torch.zeros_like(self.center_)
             else:
                 self.center_ = np.zeros_like(self.center_)
 
         if (np.asarray(self.scale_) < 1e-7).any():
             warnings.warn(
                 "scale is below 1e-7 - consider not centering "
                 "the data or using data with higher variance for numerical stability",
                 UserWarning,
             )
 
-        return self
-
     def transform(
         self,
         y: Union[pd.Series, np.ndarray, torch.Tensor],
         return_norm: bool = False,
         target_scale: torch.Tensor = None,
     ) -> Union[Tuple[Union[np.ndarray, torch.Tensor], np.ndarray], Union[np.ndarray, torch.Tensor]]:
         """
@@ -403,15 +551,20 @@
         center = target_scale[..., 0]
         scale = target_scale[..., 1]
         if y.ndim > center.ndim:  # multiple batches -> expand size
             center = center.view(*center.size(), *(1,) * (y.ndim - center.ndim))
             scale = scale.view(*scale.size(), *(1,) * (y.ndim - scale.ndim))
 
         # transform
+        dtype = y.dtype
         y = (y - center) / scale
+        try:
+            y = y.astype(dtype)
+        except AttributeError:  # torch.Tensor has `.type()` instead of `.astype()`
+            y = y.type(dtype)
 
         # return with center and scale or without
         if return_norm:
             return y, target_scale
         else:
             return y
 
@@ -435,14 +588,17 @@
             data (Dict[str, torch.Tensor]): Dictionary with entries
                 * prediction: data to de-scale
                 * target_scale: center and scale of data
 
         Returns:
             torch.Tensor: de-scaled data
         """
+        # ensure output dtype matches input dtype
+        dtype = data["prediction"].dtype
+
         # inverse transformation with tensors
         norm = data["target_scale"]
 
         # use correct shape for norm
         if data["prediction"].ndim > norm.ndim:
             norm = norm.unsqueeze(-1)
 
@@ -450,26 +606,121 @@
         y = data["prediction"] * norm[:, 1, None] + norm[:, 0, None]
 
         y = self.inverse_preprocess(y)
 
         # return correct shape
         if data["prediction"].ndim == 1 and y.ndim > 1:
             y = y.squeeze(0)
-        return y
+        return y.type(dtype)
 
 
 class EncoderNormalizer(TorchNormalizer):
     """
     Special Normalizer that is fit on each encoding sequence.
 
     If used, this transformer will be fitted on each encoder sequence separately.
     This normalizer can be particularly useful as target normalizer.
     """
 
-    pass
+    def __init__(
+        self,
+        method: str = "standard",
+        center: bool = True,
+        max_length: Union[int, List[int]] = None,
+        transformation: Union[str, Tuple[Callable, Callable]] = None,
+        method_kwargs: Dict[str, Any] = {},
+    ):
+        """
+        Initialize
+
+        Args:
+            method (str, optional): method to rescale series. Either "identity", "standard" (standard scaling)
+                or "robust" (scale using quantiles 0.25-0.75). Defaults to "standard".
+            method_kwargs (Dict[str, Any], optional): Dictionary of method specific arguments as listed below
+                * "robust" method: "upper", "lower", "center" quantiles defaulting to 0.75, 0.25 and 0.5
+            center (bool, optional): If to center the output to zero. Defaults to True.
+            max_length(Union[int, List[int]], optional): Maximum length to take into account for calculating
+                parameters. If tuple, first length is maximum length for calculating center and second is maximum
+                length for calculating scale. Defaults to entire length of time series.
+            transformation (Union[str, Tuple[Callable, Callable]] optional): Transform values before
+                applying normalizer. Available options are
+
+                * None (default): No transformation of values
+                * log: Estimate in log-space leading to a multiplicative model
+                * logp1: Estimate in log-space but add 1 to values before transforming for stability
+                    (e.g. if many small values <<1 are present).
+                    Note, that inverse transform is still only `torch.exp()` and not `torch.expm1()`.
+                * logit: Apply logit transformation on values that are between 0 and 1
+                * count: Apply softplus to output (inverse transformation) and x + 1 to input (transformation)
+                * softplus: Apply softplus to output (inverse transformation) and inverse softplus to input
+                    (transformation)
+                * relu: Apply max(0, x) to output
+                * Dict[str, Callable] of PyTorch functions that transforms and inversely transforms values.
+                  ``forward`` and ``reverse`` entries are required. ``inverse`` transformation is optional and
+                  should be defined if ``reverse`` is not the inverse of the forward transformation. ``inverse_torch``
+                  can be defined to provide a torch distribution transform for inverse transformations.
+        """
+        super().__init__(method=method, center=center, transformation=transformation, method_kwargs=method_kwargs)
+        self.max_length = max_length
+
+    def fit(self, y: Union[pd.Series, np.ndarray, torch.Tensor]):
+        """
+        Fit transformer, i.e. determine center and scale of data
+
+        Args:
+            y (Union[pd.Series, np.ndarray, torch.Tensor]): input data
+
+        Returns:
+            TorchNormalizer: self
+        """
+        # reduce size of time series - take only max length
+        if self.max_length is None:
+            y_center = y_scale = self.preprocess(y)
+        elif isinstance(self.max_length, int):
+            y_center = y_scale = self.preprocess(self._slice(y, slice(-self.max_length, None)))
+        else:
+            y = self.preprocess(self._slice(y, slice(-max(self.max_length), None)))
+            if np.argmax(self.max_length) == 0:
+                y_center = y
+                y_scale = self._slice(y, slice(-self.max_length[1], None))
+            else:
+                y_center = self._slice(y, slice(-self.max_length[0], None))
+                y_scale = y
+        # set parameters for normalization
+        self._set_parameters(y_center=y_center, y_scale=y_scale)
+        return self
+
+    @property
+    def min_length(self):
+        if self.method == "identity":
+            return 0  # no timeseries properties used
+        elif self.center:
+            return 1  # only calculation of mean required
+        else:
+            return 2  # requires std, i.e. at least 2 entries
+
+    @staticmethod
+    def _slice(
+        x: Union[pd.DataFrame, pd.Series, np.ndarray, torch.Tensor], s: slice
+    ) -> Union[pd.DataFrame, pd.Series, np.ndarray, torch.Tensor]:
+        """
+        Slice pandas data frames, numpy arrays and tensors.
+
+        Args:
+            x (Union[pd.Series, np.ndarray, torch.Tensor]): object to slice
+            s (slice): slice, e.g. ``slice(None, -5)```
+
+        Returns:
+            Union[pd.Series, np.ndarray, torch.Tensor]: sliced object
+        """
+
+        if isinstance(x, (pd.DataFrame, pd.Series)):
+            return x[s]
+        else:
+            return x[..., s]
 
 
 class GroupNormalizer(TorchNormalizer):
     """
     Normalizer that scales by groups.
 
     For each group a scaler is fitted and applied. This scaler can be used as target normalizer or
@@ -479,134 +730,163 @@
     def __init__(
         self,
         method: str = "standard",
         groups: List[str] = [],
         center: bool = True,
         scale_by_group: bool = False,
         transformation: Union[str, Tuple[Callable, Callable]] = None,
-        eps: float = 1e-8,
+        method_kwargs: Dict[str, Any] = {},
     ):
         """
         Group normalizer to normalize a given entry by groups. Can be used as target normalizer.
 
         Args:
             method (str, optional): method to rescale series. Either "standard" (standard scaling) or "robust"
                 (scale using quantiles 0.25-0.75). Defaults to "standard".
+            method_kwargs (Dict[str, Any], optional): Dictionary of method specific arguments as listed below
+                * "robust" method: "upper", "lower", "center" quantiles defaulting to 0.75, 0.25 and 0.5
             groups (List[str], optional): Group names to normalize by. Defaults to [].
             center (bool, optional): If to center the output to zero. Defaults to True.
             scale_by_group (bool, optional): If to scale the output by group, i.e. norm is calculated as
                 ``(group1_norm * group2_norm * ...) ^ (1 / n_groups)``. Defaults to False.
             transformation (Union[str, Tuple[Callable, Callable]] optional): Transform values before
                 applying normalizer. Available options are
 
                 * None (default): No transformation of values
                 * log: Estimate in log-space leading to a multiplicative model
                 * logp1: Estimate in log-space but add 1 to values before transforming for stability
                     (e.g. if many small values <<1 are present).
                     Note, that inverse transform is still only `torch.exp()` and not `torch.expm1()`.
                 * logit: Apply logit transformation on values that are between 0 and 1
-                * softplus: Apply softplus to output (inverse transformation) and x + 1 to input (transformation)
+                * count: Apply softplus to output (inverse transformation) and x + 1 to input
+                    (transformation)
+                * softplus: Apply softplus to output (inverse transformation) and inverse softplus to input
+                    (transformation)
                 * relu: Apply max(0, x) to output
-                * Tuple[Callable, Callable] of PyTorch functions that transforms and inversely transforms values.
+                * Dict[str, Callable] of PyTorch functions that transforms and inversely transforms values.
+                  ``forward`` and ``reverse`` entries are required. ``inverse`` transformation is optional and
+                  should be defined if ``reverse`` is not the inverse of the forward transformation. ``inverse_torch``
+                  can be defined to provide a torch distribution transform for inverse transformations.
 
-            eps (float, optional): Number for numerical stability of calcualtions.
-                Defaults to 1e-8. For count data, 1.0 is recommended.
         """
         self.groups = groups
         self.scale_by_group = scale_by_group
-        super().__init__(
-            method=method,
-            center=center,
-            transformation=transformation,
-            eps=eps,
-        )
+        super().__init__(method=method, center=center, transformation=transformation, method_kwargs=method_kwargs)
 
     def fit(self, y: pd.Series, X: pd.DataFrame):
         """
         Determine scales for each group
 
         Args:
             y (pd.Series): input data
             X (pd.DataFrame): dataframe with columns for each group defined in ``groups`` parameter.
 
         Returns:
             self
         """
         y = self.preprocess(y)
+        eps = np.finfo(np.float16).eps
         if len(self.groups) == 0:
             assert not self.scale_by_group, "No groups are defined, i.e. `scale_by_group=[]`"
             if self.method == "standard":
-                self.norm_ = {"center": np.mean(y), "scale": np.std(y) + self.eps}  # center and scale
+                self.norm_ = {"center": np.mean(y), "scale": np.std(y) + eps}  # center and scale
             else:
-                quantiles = np.quantile(y, [0.25, 0.5, 0.75])
+                quantiles = np.quantile(
+                    y,
+                    [
+                        self.method_kwargs.get("lower", 0.25),
+                        self.method_kwargs.get("center", 0.5),
+                        self.method_kwargs.get("upper", 0.75),
+                    ],
+                )
                 self.norm_ = {
                     "center": quantiles[1],
-                    "scale": (quantiles[2] - quantiles[0]) / 2.0 + self.eps,
+                    "scale": (quantiles[2] - quantiles[0]) / 2.0 + eps,
                 }  # center and scale
             if not self.center:
-                self.norm_["scale"] = self.norm_["center"] + self.eps
+                self.norm_["scale"] = self.norm_["center"] + eps
                 self.norm_["center"] = 0.0
 
         elif self.scale_by_group:
             if self.method == "standard":
                 self.norm_ = {
                     g: X[[g]]
                     .assign(y=y)
                     .groupby(g, observed=True)
                     .agg(center=("y", "mean"), scale=("y", "std"))
-                    .assign(center=lambda x: x["center"], scale=lambda x: x.scale + self.eps)
+                    .assign(center=lambda x: x["center"], scale=lambda x: x.scale + eps)
                     for g in self.groups
                 }
             else:
                 self.norm_ = {
                     g: X[[g]]
                     .assign(y=y)
                     .groupby(g, observed=True)
-                    .y.quantile([0.25, 0.5, 0.75])
+                    .y.quantile(
+                        [
+                            self.method_kwargs.get("lower", 0.25),
+                            self.method_kwargs.get("center", 0.5),
+                            self.method_kwargs.get("upper", 0.75),
+                        ]
+                    )
                     .unstack(-1)
                     .assign(
-                        center=lambda x: x[0.5],
-                        scale=lambda x: (x[0.75] - x[0.25]) / 2.0 + self.eps,
+                        center=lambda x: x[self.method_kwargs.get("center", 0.5)],
+                        scale=lambda x: (
+                            x[self.method_kwargs.get("upper", 0.75)] - x[self.method_kwargs.get("lower", 0.25)]
+                        )
+                        / 2.0
+                        + eps,
                     )[["center", "scale"]]
                     for g in self.groups
                 }
             # calculate missings
             if not self.center:  # swap center and scale
 
                 def swap_parameters(norm):
-                    norm["scale"] = norm["center"] + self.eps
+                    norm["scale"] = norm["center"] + eps
                     norm["center"] = 0.0
                     return norm
 
                 self.norm_ = {g: swap_parameters(norm) for g, norm in self.norm_.items()}
             self.missing_ = {group: scales.median().to_dict() for group, scales in self.norm_.items()}
 
         else:
             if self.method == "standard":
                 self.norm_ = (
                     X[self.groups]
                     .assign(y=y)
                     .groupby(self.groups, observed=True)
                     .agg(center=("y", "mean"), scale=("y", "std"))
-                    .assign(center=lambda x: x["center"], scale=lambda x: x.scale + self.eps)
+                    .assign(center=lambda x: x["center"], scale=lambda x: x.scale + eps)
                 )
             else:
                 self.norm_ = (
                     X[self.groups]
                     .assign(y=y)
                     .groupby(self.groups, observed=True)
-                    .y.quantile([0.25, 0.5, 0.75])
+                    .y.quantile(
+                        [
+                            self.method_kwargs.get("lower", 0.25),
+                            self.method_kwargs.get("center", 0.5),
+                            self.method_kwargs.get("upper", 0.75),
+                        ]
+                    )
                     .unstack(-1)
                     .assign(
-                        center=lambda x: x[0.5],
-                        scale=lambda x: (x[0.75] - x[0.25]) / 2.0 + self.eps,
+                        center=lambda x: x[self.method_kwargs.get("center", 0.5)],
+                        scale=lambda x: (
+                            x[self.method_kwargs.get("upper", 0.75)] - x[self.method_kwargs.get("lower", 0.25)]
+                        )
+                        / 2.0
+                        + eps,
                     )[["center", "scale"]]
                 )
             if not self.center:  # swap center and scale
-                self.norm_["scale"] = self.norm_["center"] + self.eps
+                self.norm_["scale"] = self.norm_["center"] + eps
                 self.norm_["center"] = 0.0
             self.missing_ = self.norm_.median().to_dict()
 
         if (
             (self.scale_by_group and any([(self.norm_[group]["scale"] < 1e-7).any() for group in self.groups]))
             or (not self.scale_by_group and isinstance(self.norm_["scale"], float) and self.norm_["scale"] < 1e-7)
             or (
@@ -668,18 +948,21 @@
             return_norm (bool, optional): If to return . Defaults to False.
             target_scale (torch.Tensor): target scale to use instead of fitted center and scale
 
         Returns:
             Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]: Scaled data, if ``return_norm=True``, returns also scales
                 as second element
         """
+        # # check if arguments are wrong way round
+        if isinstance(y, pd.DataFrame) and not isinstance(X, pd.DataFrame):
+            raise ValueError("X and y is in wrong positions")
         if target_scale is None:
             assert X is not None, "either target_scale or X has to be passed"
             target_scale = self.get_norm(X)
-        return super().transform(y=y, return_norm=return_norm, target_scale=target_scale)
+        return super().transform(y, return_norm=return_norm, target_scale=target_scale)
 
     def get_parameters(self, groups: Union[torch.Tensor, list, tuple], group_names: List[str] = None) -> np.ndarray:
         """
         Get fitted scaling parameters for a given group.
 
         Args:
             groups (Union[torch.Tensor, list, tuple]): group ids for which to get parameters
@@ -775,15 +1058,15 @@
             MultiNormalizer: self
         """
         if isinstance(y, pd.DataFrame):
             y = y.to_numpy()
 
         for idx, normalizer in enumerate(self.normalizers):
             if isinstance(normalizer, GroupNormalizer):
-                normalizer.fit(y[:, idx], X=X)
+                normalizer.fit(y[:, idx], X)
             else:
                 normalizer.fit(y[:, idx])
 
         self.fitted_ = True
         return self
 
     def __getitem__(self, idx: int):
@@ -834,15 +1117,15 @@
         res = []
         for idx, normalizer in enumerate(self.normalizers):
             if target_scale is not None:
                 scale = target_scale[idx]
             else:
                 scale = None
             if isinstance(normalizer, GroupNormalizer):
-                r = normalizer.transform(y[idx], X=X, return_norm=return_norm, target_scale=scale)
+                r = normalizer.transform(y[idx], X, return_norm=return_norm, target_scale=scale)
             else:
                 r = normalizer.transform(y[idx], return_norm=return_norm, target_scale=scale)
             res.append(r)
 
         if return_norm:
             return [r[0] for r in res], [r[1] for r in res]
         else:
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/data/examples.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/data/examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import requests
 
-BASE_URL = "https://raw.github.com/jdb78/pytorch-forecasting/master/examples/data/"
+BASE_URL = "https://github.com/jdb78/pytorch-forecasting/raw/master/examples/data/"
 
 DATA_PATH = Path(__file__).parent
 
 
 def _get_data_by_filename(fname: str) -> Path:
     """
     Download file or used cached version.
@@ -83,21 +83,21 @@
 
     Returns:
         pd.DataFrame: data
     """
     # sample parameters
     np.random.seed(seed)
     linear_trends = np.random.normal(size=n_series)[:, None] / timesteps
-    quadratic_trends = np.random.normal(size=n_series)[:, None] / timesteps ** 2
+    quadratic_trends = np.random.normal(size=n_series)[:, None] / timesteps**2
     seasonalities = np.random.normal(size=n_series)[:, None]
     levels = level * np.random.normal(size=n_series)[:, None]
 
     # generate series
     x = np.arange(timesteps)[None, :]
-    series = (x * linear_trends + x ** 2 * quadratic_trends) * trend + seasonalities * np.sin(
+    series = (x * linear_trends + x**2 * quadratic_trends) * trend + seasonalities * np.sin(
         2 * np.pi * seasonality * x / timesteps
     )
     # add noise
     series = levels * series * (1 + noise * np.random.normal(size=series.shape))
     if exp:
         series = np.exp(series)
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/data/timeseries.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/data/timeseries.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,29 +11,30 @@
 import warnings
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from sklearn.exceptions import NotFittedError
 from sklearn.preprocessing import RobustScaler, StandardScaler
-from sklearn.utils import shuffle
 from sklearn.utils.validation import check_is_fitted
 import torch
 from torch.distributions import Beta
 from torch.nn.utils import rnn
 from torch.utils.data import DataLoader, Dataset
-from torch.utils.data.sampler import Sampler
+from torch.utils.data.sampler import Sampler, SequentialSampler
 
 from pytorch_forecasting.data.encoders import (
     EncoderNormalizer,
     GroupNormalizer,
     MultiNormalizer,
     NaNLabelEncoder,
     TorchNormalizer,
 )
+from pytorch_forecasting.data.samplers import TimeSynchronizedBatchSampler
+from pytorch_forecasting.utils import repr_class
 
 
 def _find_end_indices(diffs: np.ndarray, max_lengths: np.ndarray, min_length: int) -> Tuple[np.ndarray, np.ndarray]:
     """
     Identify end indices in series even if some values are missing.
 
     Args:
@@ -126,14 +127,55 @@
     * holding information about static and time-varying variables known and unknown in the future
     * holiding information about related categories (such as holidays)
     * downsampling for data augmentation
     * generating inference, validation and test datasets
     * etc.
     """
 
+    # todo: refactor:
+    # - creating base class with minimal functionality
+    # - "outsource" transformations -> use pytorch transformations as default
+
+    # todo: integrate graphs
+    # - add option to pass networkx graph to the dataset -> clearly defined
+    # - create method to create networkx graph for hierachies -> clearly defined
+    # - convert networkx graph to pytorch geometric graph
+    # - create sampler to sample from the graph
+    # - create option in `to_dataloader` method to use a graph sampler
+    #     -> automatically changing collate function which returns graphs
+    #     -> should incorporate entire dataset but be compatible with current approach
+    # - integrate hierachical loss somehow into loss metrics
+
+    # how to get there:
+    # - add networkx and pytorch_geometric to requirements BUT as extras
+    #     -> do we also need torch_sparse, etc.? -> can we avoid this? probably not
+    # - networkx graph: define what makes sense from user perspective
+    # - define conversion into pytorch geometric graph? is this a two-step process of
+    #     - encoding networkx graph and converting it into "unfilled" pytorch geometric graph
+    #     - then creating full graph in collate function on the fly?
+    #     - or is data already stored in pytorch geometric graph and we only cut through it?
+    #     - dataformat would change? Is is all timeseries data? + mask when valid?
+    #     - then making cuts through the graph in sampling?
+    #     - would it be best in this case to re-think the timeseries class and design it as series of transformations?
+    #     - what is the new master data? very off current state or very similar?
+    #     - current approach is storing data in long format which is memory efficient and using the index object to
+    #       make sense of it when accessing. graphs would require wide format?
+    # - do NOT overengineer, i.e. support only usecase of single static graph, but only subset might be relevant
+    #     -> however, should think what happens if we want a dynamic graph. would this completely change the
+    #        data format?
+
+    # decisions:
+    # - stay with long format and create graph on the fly even if hampering efficiency and performance
+    # - go with pytorch_geometric approach for future proofing
+    # - directly convert networkx into pytorch_geometric graph
+    # - sampling: support only time-synchronized.
+    #     - sample randomly an instance from index as now.
+    #     - then get additional samples as per graph (that has been created) and available data
+    #     - then collate into graph object
+
     def __init__(
         self,
         data: pd.DataFrame,
         time_idx: str,
         target: Union[str, List[str]],
         group_ids: List[str],
         weight: Union[str, None] = None,
@@ -432,15 +474,15 @@
 
         # preprocess data
         data = self._preprocess_data(data)
         for target in self.target_names:
             assert target not in self.scalers, "Target normalizer is separate and not in scalers."
 
         # create index
-        self.index = self._construct_index(data, predict_mode=predict_mode)
+        self.index = self._construct_index(data, predict_mode=self.predict_mode)
 
         # convert to torch tensor for high performance data loading later
         self.data = self._data_to_tensors(data)
 
     @property
     def dropout_categoricals(self) -> List[str]:
         """
@@ -544,16 +586,17 @@
                 self.target_normalizer = MultiNormalizer(normalizers)
             else:
                 self.target_normalizer = normalizers[0]
         elif isinstance(self.target_normalizer, (tuple, list)):
             self.target_normalizer = MultiNormalizer(self.target_normalizer)
         elif self.target_normalizer is None:
             self.target_normalizer = TorchNormalizer(method="identity")
-        assert self.min_encoder_length > 1 or not isinstance(
-            self.target_normalizer, EncoderNormalizer
+        assert (
+            not isinstance(self.target_normalizer, EncoderNormalizer)
+            or self.min_encoder_length >= self.target_normalizer.min_length
         ), "EncoderNormalizer is only allowed if min_encoder_length > 1"
         assert isinstance(
             self.target_normalizer, (TorchNormalizer, NaNLabelEncoder)
         ), f"target_normalizer has to be either None or of class TorchNormalizer but found {self.target_normalizer}"
         assert not self.multi_target or isinstance(self.target_normalizer, MultiNormalizer), (
             "multiple targets / list of targets requires MultiNormalizer as target_normalizer "
             f"but found {self.target_normalizer}"
@@ -700,15 +743,14 @@
             ), f"__target__{target} is a protected column and must not be present in data"
             data[f"__target__{target}"] = data[target]
         if self.weight is not None:
             data["__weight__"] = data[self.weight]
 
         # train target normalizer
         if self.target_normalizer is not None:
-
             # fit target normalizer
             try:
                 check_is_fitted(self.target_normalizer)
             except NotFittedError:
                 if isinstance(self.target_normalizer, EncoderNormalizer):
                     self.target_normalizer.fit(data[self.target])
                 elif isinstance(self.target_normalizer, (GroupNormalizer, MultiNormalizer)):
@@ -775,15 +817,15 @@
             elif name not in self.scalers:
                 self.scalers[name] = StandardScaler().fit(data[[name]])
             elif self.scalers[name] is not None:
                 try:
                     check_is_fitted(self.scalers[name])
                 except NotFittedError:
                     if isinstance(self.scalers[name], GroupNormalizer):
-                        self.scalers[name] = self.scalers[name].fit(data[[name]], data)
+                        self.scalers[name] = self.scalers[name].fit(data[name], data)
                     else:
                         self.scalers[name] = self.scalers[name].fit(data[[name]])
 
         # encode after fitting
         for name in self.reals:
             # targets are handled separately
             transformer = self.get_transformer(name)
@@ -1163,27 +1205,28 @@
         Create index of samples.
 
         Args:
             data (pd.DataFrame): preprocessed data
             predict_mode (bool): if to create one same per group with prediction length equals ``max_decoder_length``
 
         Returns:
-            pd.DataFrame: index dataframe
+            pd.DataFrame: index dataframe for timesteps and index dataframe for groups.
+                It contains a list of all possible subsequences.
         """
         g = data.groupby(self._group_ids, observed=True)
 
-        df_index_first = g["__time_idx__"].transform("nth", 0).to_frame("time_first")
-        df_index_last = g["__time_idx__"].transform("nth", -1).to_frame("time_last")
+        df_index_first = g["__time_idx__"].transform("first").to_frame("time_first")
+        df_index_last = g["__time_idx__"].transform("last").to_frame("time_last")
         df_index_diff_to_next = -g["__time_idx__"].diff(-1).fillna(-1).astype(int).to_frame("time_diff_to_next")
         df_index = pd.concat([df_index_first, df_index_last, df_index_diff_to_next], axis=1)
         df_index["index_start"] = np.arange(len(df_index))
         df_index["time"] = data["__time_idx__"]
         df_index["count"] = (df_index["time_last"] - df_index["time_first"]).astype(int) + 1
-        group_ids = g.ngroup()
-        df_index["group_id"] = group_ids
+        sequence_ids = g.ngroup()
+        df_index["sequence_id"] = sequence_ids
 
         min_sequence_length = self.min_prediction_length + self.min_encoder_length
         max_sequence_length = self.max_prediction_length + self.max_encoder_length
 
         # calculate maximum index to include from current index_start
         max_time = (df_index["time"] + max_sequence_length - 1).clip(upper=df_index["count"] + df_index.time_first - 1)
 
@@ -1223,19 +1266,19 @@
         if predict_mode:  # keep longest element per series (i.e. the first element that spans to the end of the series)
             # filter all elements that are longer than the allowed maximum sequence length
             df_index = df_index[
                 lambda x: (x["time_last"] - x["time"] + 1 <= max_sequence_length)
                 & (x["sequence_length"] >= min_sequence_length)
             ]
             # choose longest sequence
-            df_index = df_index.loc[df_index.groupby("group_id").sequence_length.idxmax()]
+            df_index = df_index.loc[df_index.groupby("sequence_id").sequence_length.idxmax()]
 
         # check that all groups/series have at least one entry in the index
-        if not group_ids.isin(df_index.group_id).all():
-            missing_groups = data.loc[~group_ids.isin(df_index.group_id), self._group_ids].drop_duplicates()
+        if not sequence_ids.isin(df_index.sequence_id).all():
+            missing_groups = data.loc[~sequence_ids.isin(df_index.sequence_id), self._group_ids].drop_duplicates()
             # decode values
             for name, id in self._group_ids_mapping.items():
                 missing_groups[id] = self.transform_values(name, missing_groups[id], inverse=True, group_id=True)
             warnings.warn(
                 "Min encoder length and/or min_prediction_idx and/or min prediction length and/or lags are "
                 "too large for "
                 f"{len(missing_groups)} series/groups which therefore are not present in the dataset index. "
@@ -1301,20 +1344,17 @@
             .apply(lambda x: self.transform_values(name=x.name, values=x, group_id=True, inverse=True))
             # add time index
             .assign(
                 time_idx_first=self.data["time"][index_start].numpy(),
                 time_idx_last=self.data["time"][index_last].numpy(),
                 # prediction index is last time index - decoder length + 1
                 time_idx_first_prediction=lambda x: x.time_idx_last
-                # decoder length is minimum of
-                - (
-                    x.time_idx_last - x.time_idx_first + 1 - self.min_encoder_length
-                )  # sequence lenght - min decoder length
-                .clip(upper=self.max_prediction_length)  # maximum prediction length
-                .clip(upper=x.time_idx_last - (self.min_prediction_idx - 1))  # not going beyond min prediction idx
+                - self.calculate_decoder_length(
+                    time_last=x.time_idx_last, sequence_length=x.time_idx_last - x.time_idx_first + 1
+                )
                 + 1,
             )
         )
         return index
 
     def plot_randomization(
         self, betas: Tuple[float, float] = None, length: int = None, min_length: int = None
@@ -1390,14 +1430,45 @@
 
     def reset_overwrite_values(self) -> None:
         """
         Reset values used to override sample features.
         """
         self._overwrite_values = None
 
+    def calculate_decoder_length(
+        self,
+        time_last: Union[int, pd.Series, np.ndarray],
+        sequence_length: Union[int, pd.Series, np.ndarray],
+    ) -> Union[int, pd.Series, np.ndarray]:
+        """
+        Calculate length of decoder.
+
+        Args:
+            time_last (Union[int, pd.Series, np.ndarray]): last time index of the sequence
+            sequence_length (Union[int, pd.Series, np.ndarray]): total length of the sequence
+
+        Returns:
+            Union[int, pd.Series, np.ndarray]: decoder length(s)
+        """
+        if isinstance(time_last, int):
+            decoder_length = min(
+                time_last - (self.min_prediction_idx - 1),  # not going beyond min prediction idx
+                self.max_prediction_length,  # maximum prediction length
+                sequence_length - self.min_encoder_length,  # sequence length - min decoder length
+            )
+        else:
+            decoder_length = np.min(
+                [
+                    time_last - (self.min_prediction_idx - 1),
+                    sequence_length - self.min_encoder_length,
+                ],
+                axis=0,
+            ).clip(max=self.max_prediction_length)
+        return decoder_length
+
     def __getitem__(self, idx: int) -> Tuple[Dict[str, torch.Tensor], torch.Tensor]:
         """
         Get sample for model
 
         Args:
             idx (int): index of prediction (between ``0`` and ``len(dataset) - 1``)
 
@@ -1459,19 +1530,15 @@
             sequence_length = len(target[0])
 
         # determine data window
         assert (
             sequence_length >= self.min_prediction_length
         ), "Sequence length should be at least minimum prediction length"
         # determine prediction/decode length and encode length
-        decoder_length = min(
-            time[-1] - (self.min_prediction_idx - 1),
-            self.max_prediction_length,
-            sequence_length - self.min_encoder_length,
-        )
+        decoder_length = self.calculate_decoder_length(time[-1], sequence_length)
         encoder_length = sequence_length - decoder_length
         assert (
             decoder_length >= self.min_prediction_length
         ), "Decoder length should be at least minimum prediction length"
         assert encoder_length >= self.min_encoder_length, "Encoder length should be at least minimum encoder length"
 
         if self.randomize_length is not None:  # randomization improves generalization
@@ -1598,16 +1665,17 @@
                 encoder_time_idx_start=time[0],
                 groups=groups,
                 target_scale=target_scale,
             ),
             (target, weight),
         )
 
+    @staticmethod
     def _collate_fn(
-        self, batches: List[Tuple[Dict[str, torch.Tensor], torch.Tensor]]
+        batches: List[Tuple[Dict[str, torch.Tensor], torch.Tensor]]
     ) -> Tuple[Dict[str, torch.Tensor], torch.Tensor]:
         """
         Collate function to combine items into mini-batch for dataloader.
 
         Args:
             batches (List[Tuple[Dict[str, torch.Tensor], torch.Tensor]]): List of samples generated with
                 :py:meth:`~__getitem__`.
@@ -1647,18 +1715,22 @@
             target_scale = torch.stack([batch[0]["target_scale"] for batch in batches])
         elif isinstance(batches[0][0]["target_scale"], (list, tuple)):
             target_scale = []
             for idx in range(len(batches[0][0]["target_scale"])):
                 if isinstance(batches[0][0]["target_scale"][idx], torch.Tensor):  # stack tensor
                     scale = torch.stack([batch[0]["target_scale"][idx] for batch in batches])
                 else:
-                    scale = torch.tensor([batch[0]["target_scale"][idx] for batch in batches], dtype=torch.float)
+                    scale = torch.from_numpy(
+                        np.array([batch[0]["target_scale"][idx] for batch in batches], dtype=np.float32),
+                    )
                 target_scale.append(scale)
         else:  # convert to tensor
-            target_scale = torch.tensor([batch[0]["target_scale"] for batch in batches], dtype=torch.float)
+            target_scale = torch.from_numpy(
+                np.array([batch[0]["target_scale"] for batch in batches], dtype=np.float32),
+            )
 
         # target and weight
         if isinstance(batches[0][1][0], (tuple, list)):
             target = [
                 rnn.pad_sequence([batch[1][0][idx] for batch in batches], batch_first=True)
                 for idx in range(len(batches[0][1][0]))
             ]
@@ -1773,15 +1845,18 @@
         default_kwargs.update(kwargs)
         kwargs = default_kwargs
         if kwargs["batch_sampler"] is not None:
             sampler = kwargs["batch_sampler"]
             if isinstance(sampler, str):
                 if sampler == "synchronized":
                     kwargs["batch_sampler"] = TimeSynchronizedBatchSampler(
-                        self, batch_size=kwargs["batch_size"], shuffle=kwargs["shuffle"], drop_last=kwargs["drop_last"]
+                        SequentialSampler(self),
+                        batch_size=kwargs["batch_size"],
+                        shuffle=kwargs["shuffle"],
+                        drop_last=kwargs["drop_last"],
                     )
                 else:
                     raise ValueError(f"batch_sampler {sampler} unknown - see docstring for valid batch_sampler")
             del kwargs["batch_size"]
             del kwargs["shuffle"]
             del kwargs["drop_last"]
 
@@ -1801,111 +1876,9 @@
         for id in self.group_ids:
             index_data[id] = x["groups"][:, self.group_ids.index(id)].cpu()
             # decode if possible
             index_data[id] = self.transform_values(id, index_data[id], inverse=True, group_id=True)
         index = pd.DataFrame(index_data)
         return index
 
-
-class TimeSynchronizedBatchSampler(Sampler):
-    """
-    Samples mini-batches randomly but in a time-synchronised manner.
-
-    Time-synchornisation means that the time index of the first decoder samples are aligned across the batch.
-    This sampler does not support missing values in the dataset.
-    """
-
-    def __init__(
-        self,
-        data_source: TimeSeriesDataSet,
-        batch_size: int = 64,
-        shuffle: bool = False,
-        drop_last: bool = False,
-    ):
-        """
-        Initialize TimeSynchronizedBatchSampler.
-
-        Args:
-            data_source (TimeSeriesDataSet): timeseries dataset.
-            drop_last (bool): if to drop last mini-batch from a group if it is smaller than batch_size.
-                Defaults to False.
-            shuffle (bool): if to shuffle dataset. Defaults to False.
-            batch_size (int, optional): Number of samples in a mini-batch. This is rather the maximum number
-                of samples. Because mini-batches are grouped by prediction time, chances are that there
-                are multiple where batch size will be smaller than the maximum. Defaults to 64.
-        """
-        # Since collections.abc.Iterable does not check for `__getitem__`, which
-        # is one way for an object to be an iterable, we don't do an `isinstance`
-        # check here.
-        if not isinstance(batch_size, int) or isinstance(batch_size, bool) or batch_size <= 0:
-            raise ValueError(
-                "batch_size should be a positive integer value, " "but got batch_size={}".format(batch_size)
-            )
-        if not isinstance(drop_last, bool):
-            raise ValueError("drop_last should be a boolean value, but got " "drop_last={}".format(drop_last))
-        self.data_source = data_source
-        self.batch_size = batch_size
-        self.drop_last = drop_last
-        self.shuffle = shuffle
-        assert (
-            not self.data_source.allow_missing_timesteps
-        ), "allow_missing_timesteps should be False for time-synchronized mini-batches"
-
-        # construct index from which can be sampled
-        self.construct_batch_groups()
-
-    def construct_batch_groups(self):
-        """
-        Construct index of batches from which can be sampled
-        """
-        index = self.data_source.index
-        # get groups, i.e. group all samples by first predict time
-        decoder_lengths = np.min(
-            [
-                index.time_last - (self.data_source.min_prediction_idx - 1),
-                index.sequence_length - self.data_source.min_encoder_length,
-            ],
-            axis=0,
-        ).clip(max=self.data_source.max_prediction_length)
-        first_prediction_time = index.time + index.sequence_length - decoder_lengths + 1
-        self._groups = pd.RangeIndex(0, len(index.index)).groupby(first_prediction_time)
-
-        # calculate sizes of groups
-        self._group_sizes = {}
-        warns = []
-        for name, group in self._groups.items():  # iterate over groups
-            if self.drop_last:
-                self._group_sizes[name] = len(group) // self.batch_size
-            else:
-                self._group_sizes[name] = (len(group) + self.batch_size - 1) // self.batch_size
-            if self._group_sizes[name] == 0:
-                self._group_sizes[name] = 1
-                warns.append(name)
-        if len(warns) > 0:
-            warnings.warn(
-                f"Less than {self.batch_size} samples available for {len(warns)} prediction times. "
-                f"Use batch size smaller than {self.batch_size}. "
-                f"First 10 prediction times with small batch sizes: {warns[:10]}"
-            )
-        # create index from which can be sampled: index is equal to number of batches
-        # associate index with prediction time
-        self._group_index = np.repeat(list(self._group_sizes.keys()), list(self._group_sizes.values()))
-        # associate index with batch within prediction time group
-        self._sub_group_index = np.concatenate([np.arange(size) for size in self._group_sizes.values()])
-
-    def __iter__(self):
-        if self.shuffle:  # shuffle samples
-            groups = {name: shuffle(group) for name, group in self._groups.items()}
-        else:
-            groups = self._groups
-
-        batch_samples = np.random.permutation(len(self))
-        for idx in batch_samples:
-            name = self._group_index[idx]
-            sub_group = self._sub_group_index[idx]
-            sub_group_start = sub_group * self.batch_size
-            sub_group_end = sub_group_start + self.batch_size
-            batch = groups[name][sub_group_start:sub_group_end]
-            yield batch
-
-    def __len__(self):
-        return len(self._group_index)
+    def __repr__(self) -> str:
+        return repr_class(self, attributes=self.get_parameters(), extra_attributes=dict(length=len(self)))
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/metrics.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/metrics/base_metrics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
-Implementation of metrics for (mulit-horizon) timeseries forecasting.
+Base classes for metrics - only for inheritance.
 """
-from typing import Dict, List, Tuple, Union
+import inspect
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 import warnings
 
-import scipy.stats
 from sklearn.base import BaseEstimator
 import torch
 from torch import distributions
-import torch.nn.functional as F
 from torch.nn.utils import rnn
 from torchmetrics import Metric as LightningMetric
 
 from pytorch_forecasting.utils import create_mask, unpack_sequence, unsqueeze_like
 
 
 class Metric(LightningMetric):
@@ -20,29 +19,33 @@
     Base metric class that has basic functions that can handle predicting quantiles and operate in log space.
     See the `Lightning documentation <https://pytorch-lightning.readthedocs.io/en/latest/metrics.html>`_
     for details of how to implement a new metric
 
     Other metrics should inherit from this base class
     """
 
-    def __init__(self, name: str = None, quantiles: List[float] = None, reduction="mean"):
+    full_state_update = False
+    higher_is_better = False
+    is_differentiable = True
+
+    def __init__(self, name: str = None, quantiles: List[float] = None, reduction="mean", **kwargs):
         """
         Initialize metric
 
         Args:
             name (str): metric name. Defaults to class name.
             quantiles (List[float], optional): quantiles for probability range. Defaults to None.
             reduction (str, optional): Reduction, "none", "mean" or "sqrt-mean". Defaults to "mean".
         """
         self.quantiles = quantiles
         self.reduction = reduction
         if name is None:
             name = self.__class__.__name__
         self.name = name
-        super().__init__()
+        super().__init__(**kwargs)
 
     def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor):
         raise NotImplementedError()
 
     def compute(self) -> torch.Tensor:
         """
         Abstract method that calcualtes metric
@@ -122,34 +125,142 @@
         new_metric = composite_metric + metric
         return new_metric
 
     def __mul__(self, multiplier: float):
         new_metric = CompositeMetric(metrics=[self], weights=[multiplier])
         return new_metric
 
+    def extra_repr(self) -> str:
+        forbidden_attributes = ["name", "reduction"]
+        attributes = list(inspect.signature(self.__class__).parameters.keys())
+        return ", ".join(
+            [
+                f"{name}={repr(getattr(self, name))}"
+                for name in attributes
+                if hasattr(self, name) and name not in forbidden_attributes
+            ]
+        )
+
     __rmul__ = __mul__
 
 
+class TorchMetricWrapper(Metric):
+    """
+    Wrap a torchmetric to work with PyTorch Forecasting.
+
+    Does not support weighting of errors and only supports metrics for point predictions.
+    """
+
+    def __init__(self, torchmetric: LightningMetric, reduction: str = None, **kwargs):
+        """
+        Args:
+            torchmetric (LightningMetric): Torchmetric to wrap.
+            reduction (str, optional): use reduction with torchmetric directly. Defaults to None.
+        """
+        super().__init__(**kwargs)
+        if reduction is not None:
+            raise ValueError("use reduction with torchmetric directly")
+        self.torchmetric = torchmetric
+
+    def _sync_dist(self, dist_sync_fn=None, process_group=None) -> None:
+        # No syncing required here. syncing will be done in metric_a and metric_b
+        pass
+
+    def _wrap_compute(self, compute: Callable) -> Callable:
+        return compute
+
+    def reset(self) -> None:
+        self.torchmetric.reset()
+
+    def persistent(self, mode: bool = False) -> None:
+        self.torchmetric.persistent(mode=mode)
+
+    def _convert(self, y_pred: torch.Tensor, target: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
+        # unpack target into target and weights
+        if isinstance(target, (list, tuple)) and not isinstance(target, rnn.PackedSequence):
+            target, weight = target
+            if weight is not None:
+                raise NotImplementedError(
+                    "Weighting is not supported for pure torchmetrics - "
+                    "implement a custom version or use pytorch-forecasting metrics"
+                )
+
+        # convert to point prediction - limits applications of class
+        y_pred = self.to_prediction(y_pred)
+
+        # unpack target if it is PackedSequence
+        if isinstance(target, rnn.PackedSequence):
+            target, lengths = unpack_sequence(target)
+            # create mask for different lengths
+            length_mask = create_mask(target.size(1), lengths, inverse=True)
+            target = target.masked_select(length_mask)
+            y_pred = y_pred.masked_select(length_mask)
+
+        y_pred = y_pred.flatten()
+        target = target.flatten()
+        return y_pred, target
+
+    def update(self, y_pred: torch.Tensor, target: torch.Tensor, **kwargs) -> torch.Tensor:
+        # flatten target and prediction
+        y_pred_flattened, target_flattened = self._convert(y_pred, target)
+
+        # update metric
+        self.torchmetric.update(y_pred_flattened, target_flattened, **kwargs)
+
+    def forward(self, y_pred, target, **kwargs):
+        # need this explicitly to avoid backpropagation errors because of sketchy caching
+        y_pred_flattened, target_flattened = self._convert(y_pred, target)
+        return self.torchmetric.forward(y_pred_flattened, target_flattened, **kwargs)
+
+    def compute(self):
+        res = self.torchmetric.compute()
+        return res
+
+    def __repr__(self):
+        return f"WrappedTorchmetric({repr(self.torchmetric)})"
+
+
+def convert_torchmetric_to_pytorch_forecasting_metric(metric: LightningMetric) -> Metric:
+    """
+    If necessary, convert a torchmetric to a PyTorch Forecasting metric that
+    works with PyTorch Forecasting models.
+
+    Args:
+        metric (LightningMetric): metric to (potentially) convert
+
+    Returns:
+        Metric: PyTorch Forecasting metric
+    """
+    if not isinstance(metric, (Metric, MultiLoss, CompositeMetric)):
+        return TorchMetricWrapper(metric)
+    else:
+        return metric
+
+
 class MultiLoss(LightningMetric):
     """
     Metric that can be used with muliple metrics.
     """
 
+    full_state_update = False
+    higher_is_better = False
+    is_differentiable = True
+
     def __init__(self, metrics: List[LightningMetric], weights: List[float] = None):
         """
         Args:
             metrics (List[LightningMetric], optional): list of metrics to combine.
             weights (List[float], optional): list of weights / multipliers for weights. Defaults to 1.0 for all metrics.
         """
         assert len(metrics) > 0, "at least one metric has to be specified"
         if weights is None:
             weights = [1.0 for _ in metrics]
         assert len(weights) == len(metrics), "Number of weights has to match number of metrics"
 
-        self.metrics = metrics
+        self.metrics = [convert_torchmetric_to_pytorch_forecasting_metric(m) for m in metrics]
         self.weights = weights
 
         super().__init__()
 
     def __repr__(self):
         name = (
             f"{self.__class__.__name__}("
@@ -169,27 +280,35 @@
         Number of metrics.
 
         Returns:
             int: number of metrics
         """
         return len(self.metrics)
 
-    def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor):
+    def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor, **kwargs) -> None:
         """
         Update composite metric
 
         Args:
             y_pred: network output
             y_actual: actual values
-
-        Returns:
-            torch.Tensor: metric value on which backpropagation can be applied
+            **kwargs: arguments to update function
         """
         for idx, metric in enumerate(self.metrics):
-            metric.update(y_pred[idx], (y_actual[0][idx], y_actual[1]))
+            try:
+                metric.update(
+                    y_pred[idx],
+                    (y_actual[0][idx], y_actual[1]),
+                    **{
+                        name: value[idx] if isinstance(value, (list, tuple)) else value
+                        for name, value in kwargs.items()
+                    },
+                )
+            except TypeError:  # silently update without kwargs if not supported
+                metric.update(y_pred[idx], (y_actual[0][idx], y_actual[1]))
 
     def compute(self) -> torch.Tensor:
         """
         Get metric
 
         Returns:
             torch.Tensor: metric
@@ -200,14 +319,63 @@
 
         if len(results) == 1:
             results = results[0]
         else:
             results = torch.stack(results, dim=0).sum(0)
         return results
 
+    @torch.jit.unused
+    def forward(self, y_pred: torch.Tensor, y_actual: torch.Tensor, **kwargs):
+        """
+        Calculate composite metric
+
+        Args:
+            y_pred: network output
+            y_actual: actual values
+            **kwargs: arguments to update function
+
+        Returns:
+            torch.Tensor: metric value on which backpropagation can be applied
+        """
+        results = []
+        for idx, metric in enumerate(self.metrics):
+            try:
+                res = metric(
+                    y_pred[idx],
+                    (y_actual[0][idx], y_actual[1]),
+                    **{
+                        name: value[idx] if isinstance(value, (list, tuple)) else value
+                        for name, value in kwargs.items()
+                    },
+                )
+            except TypeError:  # silently update without kwargs if not supported
+                res = metric(y_pred[idx], (y_actual[0][idx], y_actual[1]))
+            results.append(res * self.weights[idx])
+
+        if len(results) == 1:
+            results = results[0]
+        else:
+            results = torch.stack(results, dim=0).sum(0)
+        return results
+
+    def _wrap_compute(self, compute: Callable) -> Callable:
+        return compute
+
+    def _sync_dist(self, dist_sync_fn: Optional[Callable] = None, process_group: Optional[Any] = None) -> None:
+        # No syncing required here. syncing will be done in metrics
+        pass
+
+    def reset(self) -> None:
+        for metric in self.metrics:
+            metric.reset()
+
+    def persistent(self, mode: bool = False) -> None:
+        for metric in self.metrics:
+            metric.persistent(mode=mode)
+
     def to_prediction(self, y_pred: torch.Tensor, **kwargs) -> torch.Tensor:
         """
         Convert network prediction into a point prediction.
 
         Will use first metric in ``metrics`` attribute to calculate result.
 
         Args:
@@ -320,14 +488,18 @@
     Example:
 
         .. code-block:: python
 
             composite_metric = SMAPE() + 0.4 * MAE()
     """
 
+    full_state_update = False
+    higher_is_better = False
+    is_differentiable = True
+
     def __init__(self, metrics: List[LightningMetric] = [], weights: List[float] = None):
         """
         Args:
             metrics (List[LightningMetric], optional): list of metrics to combine. Defaults to [].
             weights (List[float], optional): list of weights / multipliers for weights. Defaults to 1.0 for all metrics.
         """
         if weights is None:
@@ -339,27 +511,30 @@
 
         super().__init__()
 
     def __repr__(self):
         name = " + ".join([f"{w:.3g} * {repr(m)}" if w != 1.0 else repr(m) for w, m in zip(self.weights, self.metrics)])
         return name
 
-    def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor):
+    def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor, **kwargs):
         """
         Update composite metric
 
         Args:
             y_pred: network output
             y_actual: actual values
 
         Returns:
             torch.Tensor: metric value on which backpropagation can be applied
         """
         for metric in self.metrics:
-            metric.update(y_pred, y_actual)
+            try:
+                metric.update(y_pred, y_actual, **kwargs)
+            except TypeError:
+                metric.update(y_pred, y_actual)
 
     def compute(self) -> torch.Tensor:
         """
         Get metric
 
         Returns:
             torch.Tensor: metric
@@ -370,14 +545,55 @@
 
         if len(results) == 1:
             results = results[0]
         else:
             results = torch.stack(results, dim=0).sum(0)
         return results
 
+    @torch.jit.unused
+    def forward(self, y_pred: torch.Tensor, y_actual: torch.Tensor, **kwargs):
+        """
+        Calculate composite metric
+
+        Args:
+            y_pred: network output
+            y_actual: actual values
+            **kwargs: arguments to update function
+
+        Returns:
+            torch.Tensor: metric value on which backpropagation can be applied
+        """
+        results = []
+        for weight, metric in zip(self.weights, self.metrics):
+            try:
+                results.append(metric(y_pred, y_actual, **kwargs) * weight)
+            except TypeError:
+                results.append(metric(y_pred, y_actual) * weight)
+
+        if len(results) == 1:
+            results = results[0]
+        else:
+            results = torch.stack(results, dim=0).sum(0)
+        return results
+
+    def _wrap_compute(self, compute: Callable) -> Callable:
+        return compute
+
+    def _sync_dist(self, dist_sync_fn: Optional[Callable] = None, process_group: Optional[Any] = None) -> None:
+        # No syncing required here. syncing will be done in metrics
+        pass
+
+    def reset(self) -> None:
+        for metric in self.metrics:
+            metric.reset()
+
+    def persistent(self, mode: bool = False) -> None:
+        for metric in self.metrics:
+            metric.persistent(mode=mode)
+
     def to_prediction(self, y_pred: torch.Tensor, **kwargs) -> torch.Tensor:
         """
         Convert network prediction into a point prediction.
 
         Will use first metric in ``metrics`` attribute to calculate result.
 
         Args:
@@ -430,25 +646,31 @@
         """
         Args:
             metric (Metric): metric which to calculate on aggreation.
         """
         super().__init__(**kwargs)
         self.metric = metric
 
-    def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor) -> torch.Tensor:
+    def update(self, y_pred: torch.Tensor, y_actual: torch.Tensor, **kwargs) -> torch.Tensor:
         """
         Calculate composite metric
 
         Args:
             y_pred: network output
             y_actual: actual values
 
         Returns:
             torch.Tensor: metric value on which backpropagation can be applied
         """
+        y_pred_mean, y_mean = self._calculate_mean(y_pred, y_actual)
+        # update metric. unsqueeze first batch dimension (as batches are collapsed)
+        self.metric.update(y_pred_mean, y_mean, **kwargs)
+
+    @staticmethod
+    def _calculate_mean(y_pred: torch.Tensor, y_actual: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         # extract target and weight
         if isinstance(y_actual, (tuple, list)) and not isinstance(y_actual, rnn.PackedSequence):
             target, weight = y_actual
         else:
             target = y_actual
             weight = None
 
@@ -467,27 +689,53 @@
             else:
                 weight = weight * length_mask
 
         if weight is None:
             y_mean = target.mean(0)
             y_pred_mean = y_pred.mean(0)
         else:
-
             # calculate weighted sums
             y_mean = (target * unsqueeze_like(weight, y_pred)).sum(0) / weight.sum(0)
 
             y_pred_sum = (y_pred * unsqueeze_like(weight, y_pred)).sum(0)
             y_pred_mean = y_pred_sum / unsqueeze_like(weight.sum(0), y_pred_sum)
-
-        # update metric. unsqueeze first batch dimension (as batches are collapsed)
-        self.metric.update(y_pred_mean.unsqueeze(0), y_mean.unsqueeze(0))
+        return y_pred_mean.unsqueeze(0), y_mean.unsqueeze(0)
 
     def compute(self):
         return self.metric.compute()
 
+    @torch.jit.unused
+    def forward(self, y_pred: torch.Tensor, y_actual: torch.Tensor, **kwargs):
+        """
+        Calculate composite metric
+
+        Args:
+            y_pred: network output
+            y_actual: actual values
+            **kwargs: arguments to update function
+
+        Returns:
+            torch.Tensor: metric value on which backpropagation can be applied
+        """
+        y_pred_mean, y_mean = self._calculate_mean(y_pred, y_actual)
+        return self.metric(y_pred_mean, y_mean, **kwargs)
+
+    def _wrap_compute(self, compute: Callable) -> Callable:
+        return compute
+
+    def _sync_dist(self, dist_sync_fn: Optional[Callable] = None, process_group: Optional[Any] = None) -> None:
+        # No syncing required here. syncing will be done in metrics
+        pass
+
+    def reset(self) -> None:
+        self.metrics.reset()
+
+    def persistent(self, mode: bool = False) -> None:
+        self.metric.persistent(mode=mode)
+
 
 class MultiHorizonMetric(Metric):
     """
     Abstract class for defining metric for a multihorizon forecast
     """
 
     def __init__(self, reduction: str = "mean", **kwargs) -> None:
@@ -618,292 +866,14 @@
         )
         assert torch.isfinite(
             loss
         ), "Loss should not be infinite - i.e. something went wrong (e.g. input is not in log space)"
         return loss
 
 
-class PoissonLoss(MultiHorizonMetric):
-    """
-    Poisson loss for count data
-    """
-
-    def loss(self, y_pred: Dict[str, torch.Tensor], target: torch.Tensor) -> torch.Tensor:
-        return F.poisson_nll_loss(
-            super().to_prediction(y_pred), target, log_input=True, full=False, eps=1e-6, reduction="none"
-        )
-
-    def to_prediction(self, out: Dict[str, torch.Tensor]):
-        rate = torch.exp(super().to_prediction(out))
-        return rate
-
-    def to_quantiles(self, out: Dict[str, torch.Tensor], quantiles=None):
-        if quantiles is None:
-            if self.quantiles is None:
-                quantiles = [0.5]
-            else:
-                quantiles = self.quantiles
-        predictions = super().to_prediction(out)
-        return torch.stack([torch.tensor(scipy.stats.poisson(predictions.cpu()).ppf(q)) for q in quantiles], dim=-1).to(
-            predictions.device
-        )
-
-
-class QuantileLoss(MultiHorizonMetric):
-    """
-    Quantile loss, i.e. a quantile of ``q=0.5`` will give half of the mean absolute error as it is calcualted as
-
-    Defined as ``max(q * (y-y_pred), (1-q) * (y_pred-y))``
-    """
-
-    def __init__(
-        self,
-        quantiles: List[float] = [0.02, 0.1, 0.25, 0.5, 0.75, 0.9, 0.98],
-        **kwargs,
-    ):
-        """
-        Quantile loss
-
-        Args:
-            quantiles: quantiles for metric
-        """
-        super().__init__(quantiles=quantiles, **kwargs)
-
-    def loss(self, y_pred: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        # calculate quantile loss
-        losses = []
-        for i, q in enumerate(self.quantiles):
-            errors = target - y_pred[..., i]
-            losses.append(torch.max((q - 1) * errors, q * errors).unsqueeze(-1))
-        losses = torch.cat(losses, dim=2)
-
-        return losses
-
-    def to_prediction(self, y_pred: torch.Tensor) -> torch.Tensor:
-        """
-        Convert network prediction into a point prediction.
-
-        Args:
-            y_pred: prediction output of network
-
-        Returns:
-            torch.Tensor: point prediction
-        """
-        if y_pred.ndim == 3:
-            idx = self.quantiles.index(0.5)
-            y_pred = y_pred[..., idx]
-        return y_pred
-
-    def to_quantiles(self, y_pred: torch.Tensor) -> torch.Tensor:
-        """
-        Convert network prediction into a quantile prediction.
-
-        Args:
-            y_pred: prediction output of network
-
-        Returns:
-            torch.Tensor: prediction quantiles
-        """
-        return y_pred
-
-
-class SMAPE(MultiHorizonMetric):
-    """
-    Symmetric mean absolute percentage. Assumes ``y >= 0``.
-
-    Defined as ``2*(y - y_pred).abs() / (y.abs() + y_pred.abs())``
-    """
-
-    def loss(self, y_pred, target):
-        y_pred = self.to_prediction(y_pred)
-        loss = 2 * (y_pred - target).abs() / (y_pred.abs() + target.abs() + 1e-8)
-        return loss
-
-
-class MAPE(MultiHorizonMetric):
-    """
-    Mean absolute percentage. Assumes ``y >= 0``.
-
-    Defined as ``(y - y_pred).abs() / y.abs()``
-    """
-
-    def loss(self, y_pred, target):
-        loss = (self.to_prediction(y_pred) - target).abs() / (target.abs() + 1e-8)
-        return loss
-
-
-class MAE(MultiHorizonMetric):
-    """
-    Mean average absolute error.
-
-    Defined as ``(y_pred - target).abs()``
-    """
-
-    def loss(self, y_pred, target):
-        loss = (self.to_prediction(y_pred) - target).abs()
-        return loss
-
-
-class CrossEntropy(MultiHorizonMetric):
-    """
-    Cross entropy loss for classification.
-    """
-
-    def loss(self, y_pred, target):
-
-        loss = F.cross_entropy(y_pred.view(-1, y_pred.size(-1)), target.view(-1), reduction="none").view(
-            -1, target.size(-1)
-        )
-        return loss
-
-    def to_prediction(self, y_pred: torch.Tensor) -> torch.Tensor:
-        """
-        Convert network prediction into a point prediction.
-
-        Returns best label
-
-        Args:
-            y_pred: prediction output of network
-
-        Returns:
-            torch.Tensor: point prediction
-        """
-        return y_pred.argmax(dim=-1)
-
-    def to_quantiles(self, y_pred: torch.Tensor, quantiles: List[float] = None) -> torch.Tensor:
-        """
-        Convert network prediction into a quantile prediction.
-
-        Args:
-            y_pred: prediction output of network
-            quantiles (List[float], optional): quantiles for probability range. Defaults to quantiles as
-                as defined in the class initialization.
-
-        Returns:
-            torch.Tensor: prediction quantiles
-        """
-        return y_pred
-
-
-class RMSE(MultiHorizonMetric):
-    """
-    Root mean square error
-
-    Defined as ``(y_pred - target)**2``
-    """
-
-    def __init__(self, reduction="sqrt-mean", **kwargs):
-        super().__init__(reduction=reduction, **kwargs)
-
-    def loss(self, y_pred: Dict[str, torch.Tensor], target):
-        loss = torch.pow(self.to_prediction(y_pred) - target, 2)
-        return loss
-
-
-class MASE(MultiHorizonMetric):
-    """
-    Mean absolute scaled error
-
-    Defined as ``(y_pred - target).abs() / all_targets[:, :-1] - all_targets[:, 1:]).mean(1)``.
-    ``all_targets`` are here the concatenated encoder and decoder targets
-    """
-
-    def update(
-        self,
-        y_pred,
-        target,
-        encoder_target,
-        encoder_lengths=None,
-    ) -> torch.Tensor:
-        """
-        Update metric that handles masking of values.
-
-        Args:
-            y_pred (Dict[str, torch.Tensor]): network output
-            target (Tuple[Union[torch.Tensor, rnn.PackedSequence], torch.Tensor]): tuple of actual values and weights
-            encoder_target (Union[torch.Tensor, rnn.PackedSequence]): historic actual values
-            encoder_lengths (torch.Tensor): optional encoder lengths, not necessary if encoder_target
-                is rnn.PackedSequence. Assumed encoder_target is torch.Tensor
-
-        Returns:
-            torch.Tensor: loss as a single number for backpropagation
-        """
-        # unpack weight
-        if isinstance(target, (list, tuple)):
-            weight = target[1]
-            target = target[0]
-        else:
-            weight = None
-
-        # unpack target
-        if isinstance(target, rnn.PackedSequence):
-            target, lengths = unpack_sequence(target)
-        else:
-            lengths = torch.full((target.size(0),), fill_value=target.size(1), dtype=torch.long, device=target.device)
-
-        # determine lengths for encoder
-        if encoder_lengths is None:
-            encoder_target, encoder_lengths = unpack_sequence(target)
-        else:
-            assert isinstance(encoder_target, torch.Tensor)
-        assert not target.requires_grad
-
-        # calculate loss with "none" reduction
-        scaling = self.calculate_scaling(target, lengths, encoder_target, encoder_lengths)
-        losses = self.loss(y_pred, target, scaling)
-
-        # weight samples
-        if weight is not None:
-            losses = losses * weight.unsqueeze(-1)
-
-        self._update_losses_and_lengths(losses, lengths)
-
-    def loss(self, y_pred, target, scaling):
-        return (y_pred - target).abs() / scaling.unsqueeze(-1)
-
-    def calculate_scaling(self, target, lengths, encoder_target, encoder_lengths):
-        # calcualte mean(abs(diff(targets)))
-        eps = 1e-6
-        batch_size = target.size(0)
-        total_lengths = lengths + encoder_lengths
-        assert (total_lengths > 1).all(), "Need at least 2 target values to be able to calculate MASE"
-        max_length = target.size(1) + encoder_target.size(1)
-        if (total_lengths != max_length).any():  # if decoder or encoder targets have sequences of different lengths
-            targets = torch.cat(
-                [
-                    encoder_target,
-                    torch.zeros(batch_size, target.size(1), device=target.device, dtype=encoder_target.dtype),
-                ],
-                dim=1,
-            )
-            target_index = torch.arange(target.size(1), device=target.device, dtype=torch.long).unsqueeze(0).expand(
-                batch_size, -1
-            ) + encoder_lengths.unsqueeze(-1)
-            targets.scatter_(dim=1, src=target, index=target_index)
-        else:
-            targets = torch.cat([encoder_target, target], dim=1)
-
-        # take absolute difference
-        diffs = (targets[:, :-1] - targets[:, 1:]).abs()
-
-        # set last difference to 0
-        not_maximum_length = total_lengths != max_length
-        zero_correction_indices = total_lengths[not_maximum_length] - 1
-        if len(zero_correction_indices) > 0:
-            diffs[
-                torch.arange(batch_size, dtype=torch.long, device=diffs.device)[not_maximum_length],
-                zero_correction_indices,
-            ] = 0.0
-
-        # calculate mean over differences
-        scaling = diffs.sum(1) / total_lengths + eps
-
-        return scaling
-
-
 class DistributionLoss(MultiHorizonMetric):
     """
     DistributionLoss base class.
 
     Class should be inherited for all distribution losses, i.e. if a network predicts
     the parameters of a probability distribution, DistributionLoss can be used to
     score those parameters and calculate loss for given true values.
@@ -958,27 +928,29 @@
         Returns:
             torch.Tensor: metric value on which backpropagation can be applied
         """
         distribution = self.map_x_to_distribution(y_pred)
         loss = -distribution.log_prob(y_actual)
         return loss
 
-    def to_prediction(self, y_pred: torch.Tensor) -> torch.Tensor:
+    def to_prediction(self, y_pred: torch.Tensor, n_samples: int = 100) -> torch.Tensor:
         """
         Convert network prediction into a point prediction.
 
         Args:
             y_pred: prediction output of network
 
         Returns:
             torch.Tensor: mean prediction
         """
         distribution = self.map_x_to_distribution(y_pred)
-
-        return distribution.mean
+        try:
+            return distribution.mean
+        except NotImplementedError:
+            return self.sample(y_pred, n_samples=n_samples).mean(-1)
 
     def sample(self, y_pred, n_samples: int) -> torch.Tensor:
         """
         Sample from distribution.
 
         Args:
             y_pred: prediction output of network (shape batch_size x n_timesteps x n_paramters)
@@ -1015,169 +987,47 @@
             quantiles = distribution.icdf(torch.tensor(quantiles, device=y_pred.device)[:, None, None]).permute(1, 2, 0)
         except NotImplementedError:  # resort to derive quantiles empirically
             samples = torch.sort(self.sample(y_pred, n_samples), -1).values
             quantiles = torch.quantile(samples, torch.tensor(quantiles, device=samples.device), dim=2).permute(1, 2, 0)
         return quantiles
 
 
-class NormalDistributionLoss(DistributionLoss):
-    """
-    Normal distribution loss.
+class MultivariateDistributionLoss(DistributionLoss):
+    """Base class for multivariate distribution losses.
 
-    Requirements for original target normalizer:
-        * not normalized in log space (use :py:class:`~LogNormalDistributionLoss`)
-        * not coerced to be positive
+    Class should be inherited for all multivariate distribution losses, i.e. if a batch of values
+    is predicted in one go and the batch dimension is not independent, but the time dimension still
+    remains independent.
     """
 
-    distribution_class = distributions.Normal
-    distribution_arguments = ["loc", "scale"]
-
-    def map_x_to_distribution(self, x: torch.Tensor) -> distributions.Normal:
-        return self.distribution_class(loc=x[..., 0], scale=x[..., 1])
-
-    def rescale_parameters(
-        self, parameters: torch.Tensor, target_scale: torch.Tensor, encoder: BaseEstimator
-    ) -> torch.Tensor:
-        assert encoder.transformation not in ["log", "log1p"], "Use LogNormalDistributionLoss for log scaled data"
-        assert encoder.transformation not in [
-            "softplus",
-            "relu",
-        ], "Cannot use NormalDistributionLoss for positive data"
-        assert encoder.transformation not in ["logit"], "Cannot use bound transformation such as 'logit'"
-        loc = encoder(dict(prediction=parameters[..., 0], target_scale=target_scale))
-        scale = F.softplus(parameters[..., 1]) * target_scale[..., 1].unsqueeze(1)
-        return torch.stack([loc, scale], dim=-1)
-
-
-class NegativeBinomialDistributionLoss(DistributionLoss):
-    """
-    Negative binomial loss, e.g. for count data.
-
-    Requirements for original target normalizer:
-        * not centered normalization (only rescaled)
-    """
-
-    distribution_class = distributions.NegativeBinomial
-    distribution_arguments = ["mean", "shape"]
-
-    def map_x_to_distribution(self, x: torch.Tensor) -> distributions.NegativeBinomial:
-        mean = x[..., 0]
-        shape = x[..., 1]
-        r = 1.0 / shape
-        p = mean / (mean + r)
-        return self.distribution_class(total_count=r, probs=p)
-
-    def rescale_parameters(
-        self, parameters: torch.Tensor, target_scale: torch.Tensor, encoder: BaseEstimator
-    ) -> torch.Tensor:
-        assert not encoder.center, "NegativeBinomialDistributionLoss is not compatible with `center=True` normalization"
-        assert encoder.transformation not in ["logit"], "Cannot use bound transformation such as 'logit'"
-        if encoder.transformation in ["log", "log1p"]:
-            mean = torch.exp(parameters[..., 0] * target_scale[..., 1].unsqueeze(-1))
-            shape = (
-                F.softplus(torch.exp(parameters[..., 1]))
-                / torch.exp(target_scale[..., 1].unsqueeze(-1)).sqrt()  # todo: is this correct?
-            )
-        else:
-            mean = F.softplus(parameters[..., 0]) * target_scale[..., 1].unsqueeze(-1)
-            shape = F.softplus(parameters[..., 1]) / target_scale[..., 1].unsqueeze(-1).sqrt()
-        return torch.stack([mean, shape], dim=-1)
-
-    def to_prediction(self, y_pred: torch.Tensor) -> torch.Tensor:
+    def sample(self, y_pred, n_samples: int) -> torch.Tensor:
         """
-        Convert network prediction into a point prediction. In the case of this distribution prediction we
-        need to derive the mean (as a point prediction) from the distribution parameters
+        Sample from distribution.
 
         Args:
-            y_pred: prediction output of network
-            in this case the two parameters for the negative binomial
+            y_pred: prediction output of network (shape batch_size x n_timesteps x n_paramters)
+            n_samples (int): number of samples to draw
 
         Returns:
-            torch.Tensor: mean prediction
+            torch.Tensor: tensor with samples  (shape batch_size x n_timesteps x n_samples)
         """
-        return y_pred[..., 0]
-
-
-class LogNormalDistributionLoss(DistributionLoss):
-    """
-    Log-normal loss.
-
-    Requirements for original target normalizer:
-        * normalized target in log space
-    """
-
-    distribution_class = distributions.LogNormal
-    distribution_arguments = ["loc", "scale"]
-
-    def map_x_to_distribution(self, x: torch.Tensor) -> distributions.LogNormal:
-        return self.distribution_class(loc=x[..., 0], scale=x[..., 1])
-
-    def rescale_parameters(
-        self, parameters: torch.Tensor, target_scale: torch.Tensor, encoder: BaseEstimator
-    ) -> torch.Tensor:
-        assert isinstance(encoder.transformation, str) and encoder.transformation in [
-            "log",
-            "log1p",
-        ], f"Log distribution requires log scaling but found `transformation={encoder.transform}`"
-
-        assert encoder.transformation not in ["logit"], "Cannot use bound transformation such as 'logit'"
-
-        scale = F.softplus(parameters[..., 1]) * target_scale[..., 1].unsqueeze(-1)
-        loc = parameters[..., 0] * target_scale[..., 1].unsqueeze(-1) + target_scale[..., 0].unsqueeze(-1)
-
-        return torch.stack([loc, scale], dim=-1)
-
-
-class BetaDistributionLoss(DistributionLoss):
-    """
-    Beta distribution loss for unit interval data.
-
-    Requirements for original target normalizer:
-        * logit transformation
-    """
-
-    distribution_class = distributions.Beta
-    distribution_arguments = ["mean", "shape"]
-    eps = 1e-4
-
-    def map_x_to_distribution(self, x: torch.Tensor) -> distributions.Beta:
-        mean = x[..., 0]
-        shape = x[..., 1]
-        return self.distribution_class(concentration0=(1 - mean) * shape, concentration1=mean * shape)
+        dist = self.map_x_to_distribution(y_pred)
+        samples = dist.sample((n_samples,)).permute(
+            2, 1, 0
+        )  # returned as (n_samples, n_timesteps, batch_size), so reshape to (batch_size, n_timesteps, n_samples)
+        return samples
 
     def loss(self, y_pred: torch.Tensor, y_actual: torch.Tensor) -> torch.Tensor:
         """
         Calculate negative likelihood
 
         Args:
             y_pred: network output
             y_actual: actual values
 
         Returns:
             torch.Tensor: metric value on which backpropagation can be applied
         """
         distribution = self.map_x_to_distribution(y_pred)
-        # clip y_actual to avoid infinite losses
-        loss = -distribution.log_prob(y_actual.clip(self.eps, 1 - self.eps))
+        # calculate one number and scale with batch size
+        loss = -distribution.log_prob(y_actual.transpose(0, 1)).sum() * y_actual.size(0)
         return loss
-
-    def rescale_parameters(
-        self, parameters: torch.Tensor, target_scale: torch.Tensor, encoder: BaseEstimator
-    ) -> torch.Tensor:
-        assert encoder.transformation in ["logit"], "Beta distribution is only compatible with logit transformation"
-        assert encoder.center, "Beta distribution requires normalizer to center data"
-
-        scaled_mean = encoder(dict(prediction=parameters[..., 0], target_scale=target_scale))
-        # need to first transform target scale standard deviation in logit space to real space
-        # we assume a normal distribution in logit space (we used a logit transform and a standard scaler)
-        # and know that the variance of the beta distribution is limited by `scaled_mean * (1 - scaled_mean)`
-        scaled_mean = scaled_mean * (1 - 2 * self.eps) + self.eps  # ensure that mean is not exactly 0 or 1
-        mean_derivative = scaled_mean * (1 - scaled_mean)
-
-        # we can approximate variance as
-        # torch.pow(torch.tanh(target_scale[..., 1].unsqueeze(1) * torch.sqrt(mean_derivative)), 2) * mean_derivative
-        # shape is (positive) parameter * mean_derivative / var
-        shape_scaler = (
-            torch.pow(torch.tanh(target_scale[..., 1].unsqueeze(1) * torch.sqrt(mean_derivative)), 2) + self.eps
-        )
-        scaled_shape = F.softplus(parameters[..., 1]) / shape_scaler
-        return torch.stack([scaled_mean, scaled_shape], dim=-1)
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     BaseModel,
     BaseModelWithCovariates,
 )
 from pytorch_forecasting.models.baseline import Baseline
 from pytorch_forecasting.models.deepar import DeepAR
 from pytorch_forecasting.models.mlp import DecoderMLP
 from pytorch_forecasting.models.nbeats import NBeats
+from pytorch_forecasting.models.nhits import NHiTS
 from pytorch_forecasting.models.nn import GRU, LSTM, MultiEmbedding, get_rnn
 from pytorch_forecasting.models.rnn import RecurrentNetwork
 from pytorch_forecasting.models.temporal_fusion_transformer import TemporalFusionTransformer
 
 __all__ = [
     "NBeats",
+    "NHiTS",
     "TemporalFusionTransformer",
     "RecurrentNetwork",
     "DeepAR",
     "BaseModel",
     "Baseline",
     "BaseModelWithCovariates",
     "AutoRegressiveBaseModel",
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/base_model.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/base_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 """
 Timeseries models share a number of common characteristics. This module implements these in a common base class.
 """
 from collections import namedtuple
 import copy
 from copy import deepcopy
 import inspect
-from typing import Any, Callable, Dict, Iterable, List, Tuple, Union
-
+import logging
+import os
+from typing import Any, Callable, Dict, Iterable, List, Literal, Optional, Tuple, Union
+import warnings
+
+import lightning.pytorch as pl
+from lightning.pytorch import LightningModule, Trainer
+from lightning.pytorch.callbacks import BasePredictionWriter, LearningRateFinder
+from lightning.pytorch.trainer.states import RunningStage
+from lightning.pytorch.utilities.parsing import AttributeDict, get_init_args
 import matplotlib.pyplot as plt
 import numpy as np
 from numpy.lib.function_base import iterable
 import pandas as pd
-from pytorch_lightning import LightningModule
-from pytorch_lightning.trainer.states import RunningStage
-from pytorch_lightning.utilities.parsing import AttributeDict, get_init_args
+import pytorch_optimizer
+from pytorch_optimizer import Ranger21
 import scipy.stats
 import torch
 import torch.nn as nn
 from torch.nn.utils import rnn
 from torch.optim.lr_scheduler import LambdaLR, ReduceLROnPlateau
 from torch.utils.data import DataLoader
 from tqdm.autonotebook import tqdm
@@ -26,30 +33,35 @@
 from pytorch_forecasting.data import TimeSeriesDataSet
 from pytorch_forecasting.data.encoders import EncoderNormalizer, GroupNormalizer, MultiNormalizer, NaNLabelEncoder
 from pytorch_forecasting.metrics import (
     MAE,
     MASE,
     SMAPE,
     DistributionLoss,
-    Metric,
     MultiHorizonMetric,
     MultiLoss,
     QuantileLoss,
+    convert_torchmetric_to_pytorch_forecasting_metric,
 )
-from pytorch_forecasting.optim import Ranger
+from pytorch_forecasting.metrics.base_metrics import Metric
+from pytorch_forecasting.models.nn.embeddings import MultiEmbedding
 from pytorch_forecasting.utils import (
+    InitialParameterRepresenterMixIn,
     OutputMixIn,
+    TupleOutputMixIn,
     apply_to_list,
+    concat_sequences,
     create_mask,
     get_embedding_size,
     groupby_apply,
-    move_to_device,
     to_list,
 )
 
+# todo: compile models
+
 
 def _torch_cat_na(x: List[torch.Tensor]) -> torch.Tensor:
     """
     Concatenate tensor along ``dim=0`` and add nans along ``dim=1`` if necessary.
 
     Allows concatenation of tensors where ``dim=1`` are not equal.
     Missing values are filled up with ``nan``.
@@ -64,19 +76,42 @@
         first_lens = [xi.shape[1] for xi in x]
         max_first_len = max(first_lens)
         if max_first_len > min(first_lens):
             x = [
                 xi
                 if xi.shape[1] == max_first_len
                 else torch.cat(
-                    [xi, torch.full((xi.shape[0], max_first_len - xi.shape[1], *xi.shape[2:]), float("nan"))], dim=1
+                    [
+                        xi,
+                        torch.full(
+                            (xi.shape[0], max_first_len - xi.shape[1], *xi.shape[2:]), float("nan"), device=xi.device
+                        ),
+                    ],
+                    dim=1,
                 )
                 for xi in x
             ]
-    return torch.cat(x, dim=0)
+
+    # check if remaining dimensions are all equal
+    if x[0].ndim > 2:
+        remaining_dimensions_equal = all([all([xi.size(i) == x[0].size(i) for xi in x]) for i in range(2, x[0].ndim)])
+    else:
+        remaining_dimensions_equal = True
+
+    # deaggregate
+    if remaining_dimensions_equal:
+        return torch.cat(x, dim=0)
+    else:
+        # make list instead but warn
+        warnings.warn(
+            f"Not all dimensions are equal for tensors shapes. Example tensor {x[0].shape}. "
+            "Returning list instead of torch.Tensor.",
+            UserWarning,
+        )
+        return [xii for xi in x for xii in xi]
 
 
 def _concatenate_output(
     output: List[Dict[str, List[Union[List[torch.Tensor], torch.Tensor, bool, int, str, np.ndarray]]]]
 ) -> Dict[str, Union[torch.Tensor, np.ndarray, List[Union[torch.Tensor, int, bool, str]]]]:
     """
     Concatenate multiple batches of output dictionary.
@@ -125,16 +160,190 @@
     RunningStage.TRAINING: "train",
     RunningStage.VALIDATING: "val",
     RunningStage.TESTING: "test",
     RunningStage.PREDICTING: "predict",
     RunningStage.SANITY_CHECKING: "sanity_check",
 }
 
+# return type of predict function
+PredictTuple = namedtuple(
+    "prediction", ["output", "x", "index", "decoder_lengths", "y"], defaults=(None, None, None, None, None)
+)
+
+
+class Prediction(PredictTuple, OutputMixIn):
+    pass
+
+
+class PredictCallback(BasePredictionWriter):
+    """Internally used callback to capture predictions and optionally write them to disk."""
+
+    # see base class predict function for documentation of parameters
+    def __init__(
+        self,
+        mode: Union[str, Tuple[str, str]] = "prediction",
+        return_index: bool = False,
+        return_decoder_lengths: bool = False,
+        return_y: bool = False,
+        write_interval: Literal["batch", "epoch", "batch_and_epoch"] = "batch",
+        return_x: bool = False,
+        mode_kwargs: Dict[str, Any] = None,
+        output_dir: Optional[str] = None,
+        predict_kwargs: Dict[str, Any] = None,
+    ) -> None:
+        super().__init__(write_interval=write_interval)
+        self.mode = mode
+        self.return_decoder_lengths = return_decoder_lengths
+        self.return_x = return_x
+        self.return_index = return_index
+        self.return_y = return_y
+        self.mode_kwargs = mode_kwargs if mode_kwargs is not None else {}
+        self.predict_kwargs = predict_kwargs if predict_kwargs is not None else {}
+        self.output_dir = output_dir
+        self._reset_data()
+
+    def _reset_data(self, result: bool = True):
+        # reset data objects to save results into
+        self._output = []
+        self._decode_lenghts = []
+        self._x_list = []
+        self._index = []
+        self._y = []
+        if result:
+            self._result = []
+
+    def on_predict_batch_end(
+        self,
+        trainer: Trainer,
+        pl_module: LightningModule,
+        outputs: Any,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int = 0,
+    ) -> None:
+        # extract predictions form output
+        x = batch[0]
+        out = outputs
+
+        lengths = x["decoder_lengths"]
+
+        nan_mask = create_mask(lengths.max(), lengths)
+        if isinstance(self.mode, (tuple, list)):
+            if self.mode[0] == "raw":
+                out = out[self.mode[1]]
+            else:
+                raise ValueError(
+                    f"If a tuple is specified, the first element must be 'raw' - got {self.mode[0]} instead"
+                )
+        elif self.mode == "prediction":
+            out = pl_module.to_prediction(out, **self.mode_kwargs)
+            # mask non-predictions
+            if isinstance(out, (list, tuple)):
+                out = [
+                    o.masked_fill(nan_mask, torch.tensor(float("nan"))) if o.dtype == torch.float else o for o in out
+                ]
+            elif out.dtype == torch.float:  # only floats can be filled with nans
+                out = out.masked_fill(nan_mask, torch.tensor(float("nan")))
+        elif self.mode == "quantiles":
+            out = pl_module.to_quantiles(out, **self.mode_kwargs)
+            # mask non-predictions
+            if isinstance(out, (list, tuple)):
+                out = [
+                    o.masked_fill(nan_mask.unsqueeze(-1), torch.tensor(float("nan"))) if o.dtype == torch.float else o
+                    for o in out
+                ]
+            elif out.dtype == torch.float:
+                out = out.masked_fill(nan_mask.unsqueeze(-1), torch.tensor(float("nan")))
+        elif self.mode == "raw":
+            pass
+        else:
+            raise ValueError(f"Unknown mode {self.mode} - see docs for valid arguments")
+
+        self._output.append(out)
+        out = dict(output=out)
+        if self.return_x:
+            self._x_list.append(x)
+            out["x"] = self._x_list[-1]
+        if self.return_index:
+            self._index.append(trainer.predict_dataloaders.dataset.x_to_index(x))
+            out["index"] = self._index[-1]
+        if self.return_decoder_lengths:
+            self._decode_lenghts.append(lengths)
+            out["decoder_lengths"] = self._decode_lenghts[-1]
+        if self.return_y:
+            self._y.append(batch[1])
+            out["y"] = self._y[-1]
+
+        if isinstance(out, dict):
+            out = Prediction(**out)
+        # write to disk
+        if self.output_dir is not None:
+            super().on_predict_batch_end(trainer, pl_module, out, batch, batch_idx, dataloader_idx)
+
+    def write_on_batch_end(self, trainer, pl_module, prediction, batch_indices, batch, batch_idx, dataloader_idx):
+        torch.save(prediction, os.path.join(self.output_dir, f"predictions_{batch_idx}.pt"))
+        self._reset_data()
+
+    def write_on_epoch_end(self, trainer, pl_module, predictions, batch_indices):
+        torch.save(predictions, os.path.join(self.output_dir, "predictions.pt"))
+        self._reset_data()
+
+    def on_predict_epoch_end(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule") -> None:
+        output = self._output
+        if len(output) > 0:
+            # concatenate output (of different batches)
+            if isinstance(self.mode, (tuple, list)) or self.mode != "raw":
+                if (
+                    isinstance(output[0], (tuple, list))
+                    and len(output[0]) > 0
+                    and isinstance(output[0][0], torch.Tensor)
+                ):
+                    output = [_torch_cat_na([out[idx] for out in output]) for idx in range(len(output[0]))]
+                else:
+                    output = _torch_cat_na(output)
+            elif self.mode == "raw":
+                output = _concatenate_output(output)
+
+            # if len(output) > 0:
+            # generate output
+            if self.return_x or self.return_index or self.return_decoder_lengths or self.return_y:
+                output = dict(output=output)
+            if self.return_x:
+                output["x"] = _concatenate_output(self._x_list)
+            if self.return_index:
+                output["index"] = pd.concat(self._index, axis=0, ignore_index=True)
+            if self.return_decoder_lengths:
+                output["decoder_lengths"] = torch.cat(self._decode_lenghts, dim=0)
+            if self.return_y:
+                y = concat_sequences([yi[0] for yi in self._y])
+                if self._y[-1][1] is None:
+                    weight = None
+                else:
+                    weight = concat_sequences([yi[1] for yi in self._y])
 
-class BaseModel(LightningModule):
+                output["y"] = (y, weight)
+            if isinstance(output, dict):
+                output = Prediction(**output)  # save for later writing or outputting
+            self._result = output
+
+            # write to disk
+            if self.interval.on_epoch:
+                self.write_on_epoch_end(trainer, pl_module, self._output, trainer.predict_loop.epoch_batch_indices)
+            self._reset_data(result=False)
+
+    @property
+    def result(self) -> Prediction:
+        if self.output_dir is None:
+            return self._result
+        else:
+            assert len(self._result) == 0, "Cannot return result if output_dir is set"
+            return None
+
+
+class BaseModel(InitialParameterRepresenterMixIn, LightningModule, TupleOutputMixIn):
     """
     BaseModel from which new timeseries models should inherit from.
     The ``hparams`` of the created object will default to the parameters indicated in :py:meth:`~__init__`.
 
     The :py:meth:`~BaseModel.forward` method should return a named tuple with at least the entry ``prediction``
     that contains the network's output. See the function's documentation for more details.
 
@@ -150,16 +359,16 @@
           space. Override it to pass additional arguments to the __init__ method of your network that depend on your
           dataset.
         * The :py:meth:`~BaseModel.transform_output` method rescales the network output using the target normalizer
           from thedataset.
         * The :py:meth:`~BaseModel.step` method takes care of calculating the loss, logging additional metrics defined
           in the ``logging_metrics`` attribute and plots of sample predictions. You can override this method to add
           custom interpretations or pass extra arguments to the networks forward method.
-        * The :py:meth:`~BaseModel.epoch_end` method can be used to calculate summaries of each epoch such as
-          statistics on the encoder length, etc.
+        * The :py:meth:`~BaseModel.on_epoch_end` method can be used to calculate summaries of each epoch such as
+          statistics on the encoder length, etc and needs to return the outputs.
         * The :py:meth:`~BaseModel.predict` method makes predictions using a dataloader or dataset. Override it if you
           need to pass additional arguments to ``forward`` by default.
 
     To implement your own architecture, it is best to
     go throught the :ref:`Using custom data and implementing custom models <new-model-tutorial>` and
     to look at existing ones to understand what might be a good approach.
 
@@ -187,20 +396,21 @@
         log_interval: Union[int, float] = -1,
         log_val_interval: Union[int, float] = None,
         learning_rate: Union[float, List[float]] = 1e-3,
         log_gradient_flow: bool = False,
         loss: Metric = SMAPE(),
         logging_metrics: nn.ModuleList = nn.ModuleList([]),
         reduce_on_plateau_patience: int = 1000,
+        reduce_on_plateau_reduction: float = 2.0,
         reduce_on_plateau_min_lr: float = 1e-5,
         weight_decay: float = 0.0,
         optimizer_params: Dict[str, Any] = None,
         monotone_constaints: Dict[str, int] = {},
         output_transformer: Callable = None,
-        optimizer="ranger",
+        optimizer="Ranger",
     ):
         """
         BaseModel for timeseries forecasting from which to inherit from
 
         Args:
             log_interval (Union[int, float], optional): Batches after which predictions are logged. If < 1.0, will log
                 multiple entries per batch. Defaults to -1.
@@ -210,29 +420,31 @@
             log_gradient_flow (bool): If to log gradient flow, this takes time and should be only done to diagnose
                 training failures. Defaults to False.
             loss (Metric, optional): metric to optimize, can also be list of metrics. Defaults to SMAPE().
             logging_metrics (nn.ModuleList[MultiHorizonMetric]): list of metrics that are logged during training.
                 Defaults to [].
             reduce_on_plateau_patience (int): patience after which learning rate is reduced by a factor of 10. Defaults
                 to 1000
+            reduce_on_plateau_reduction (float): reduction in learning rate when encountering plateau. Defaults to 2.0.
             reduce_on_plateau_min_lr (float): minimum learning rate for reduce on plateua learning rate scheduler.
                 Defaults to 1e-5
             weight_decay (float): weight decay. Defaults to 0.0.
             optimizer_params (Dict[str, Any]): additional parameters for the optimizer. Defaults to {}.
             monotone_constaints (Dict[str, int]): dictionary of monotonicity constraints for continuous decoder
                 variables mapping
                 position (e.g. ``"0"`` for first position) to constraint (``-1`` for negative and ``+1`` for positive,
                 larger numbers add more weight to the constraint vs. the loss but are usually not necessary).
                 This constraint significantly slows down training. Defaults to {}.
             output_transformer (Callable): transformer that takes network output and transforms it to prediction space.
                 Defaults to None which is equivalent to ``lambda out: out["prediction"]``.
-            optimizer (str): Optimizer, "ranger", "sgd", "adam", "adamw" or class name of optimizer in ``torch.optim``.
+            optimizer (str): Optimizer, "ranger", "sgd", "adam", "adamw" or class name of optimizer in ``torch.optim``
+                or ``pytorch_optimizer``.
                 Alternatively, a class or function can be passed which takes parameters as first argument and
-                a `lr` argument (optionally also `weight_decay`)
-                Defaults to "ranger".
+                a `lr` argument (optionally also `weight_decay`). Defaults to
+                `"ranger" <https://pytorch-optimizers.readthedocs.io/en/latest/optimizer_api.html#ranger21>`_.
         """
         super().__init__()
         # update hparams
         frame = inspect.currentframe()
         init_args = get_init_args(frame)
         self.save_hyperparameters(
             {name: val for name, val in init_args.items() if name not in self.hparams and name not in ["self"]}
@@ -240,19 +452,21 @@
 
         # update log interval if not defined
         if self.hparams.log_val_interval is None:
             self.hparams.log_val_interval = self.hparams.log_interval
 
         if not hasattr(self, "loss"):
             if isinstance(loss, (tuple, list)):
-                self.loss = MultiLoss(metrics=loss)
+                self.loss = MultiLoss(metrics=[convert_torchmetric_to_pytorch_forecasting_metric(l) for l in loss])
             else:
-                self.loss = loss
+                self.loss = convert_torchmetric_to_pytorch_forecasting_metric(loss)
         if not hasattr(self, "logging_metrics"):
-            self.logging_metrics = nn.ModuleList([l for l in logging_metrics])
+            self.logging_metrics = nn.ModuleList(
+                [convert_torchmetric_to_pytorch_forecasting_metric(l) for l in logging_metrics]
+            )
         if not hasattr(self, "output_transformer"):
             self.output_transformer = output_transformer
         if not hasattr(self, "optimizer"):  # callables are removed from hyperparameters, so better to save them
             self.optimizer = self.hparams.optimizer
 
         # delete everything from hparams that cannot be serialized with yaml.dump
         # which is particularly important for tensorboard logging
@@ -266,22 +480,36 @@
                     setattr(self, k, v)
 
         self.hparams_special = getattr(self, "hparams_special", [])
         self.hparams_special.extend(hparams_to_delete)
         for k in hparams_to_delete:
             del self._hparams[k]
             del self._hparams_initial[k]
+        # epoch outputs
+        self.training_step_outputs = []
+        self.validation_step_outputs = []
+        self.testing_step_outputs = []
+
+    def log(self, *args, **kwargs):
+        """See :meth:`lightning.pytorch.core.lightning.LightningModule.log`."""
+        # never log for prediction
+        if not self.predicting:
+            super().log(*args, **kwargs)
+
+    @property
+    def predicting(self) -> bool:
+        return self.current_stage is None or self.current_stage == "predict"
 
     @property
     def current_stage(self) -> str:
         """
         Available inside lightning loops.
         :return: current trainer stage. One of ["train", "val", "test", "predict", "sanity_check"]
         """
-        return STAGE_STATES[self.trainer.state.stage]
+        return STAGE_STATES.get(self.trainer.state.stage, None)
 
     @property
     def n_targets(self) -> int:
         """
         Number of targets to forecast.
 
         Based on loss function.
@@ -291,34 +519,40 @@
         """
         if isinstance(self.loss, MultiLoss):
             return len(self.loss.metrics)
         else:
             return 1
 
     def transform_output(
-        self, prediction: Union[torch.Tensor, List[torch.Tensor]], target_scale: Union[torch.Tensor, List[torch.Tensor]]
+        self,
+        prediction: Union[torch.Tensor, List[torch.Tensor]],
+        target_scale: Union[torch.Tensor, List[torch.Tensor]],
+        loss: Optional[Metric] = None,
     ) -> torch.Tensor:
         """
         Extract prediction from network output and rescale it to real space / de-normalize it.
 
         Args:
             prediction (Union[torch.Tensor, List[torch.Tensor]]): normalized prediction
             target_scale (Union[torch.Tensor, List[torch.Tensor]]): scale to rescale prediction
+            loss (Optional[Metric]): metric to use for transform
 
         Returns:
             torch.Tensor: rescaled prediction
         """
-        if isinstance(self.loss, MultiLoss):
-            out = self.loss.rescale_parameters(
+        if loss is None:
+            loss = self.loss
+        if isinstance(loss, MultiLoss):
+            out = loss.rescale_parameters(
                 prediction,
                 target_scale=target_scale,
                 encoder=self.output_transformer.normalizers,  # need to use normalizer per encoder
             )
         else:
-            out = self.loss.rescale_parameters(prediction, target_scale=target_scale, encoder=self.output_transformer)
+            out = loss.rescale_parameters(prediction, target_scale=target_scale, encoder=self.output_transformer)
         return out
 
     @staticmethod
     def deduce_default_output_parameters(
         dataset: TimeSeriesDataSet, kwargs: Dict[str, Any], default_loss: MultiHorizonMetric = None
     ) -> Dict[str, Any]:
         """
@@ -331,14 +565,15 @@
             kwargs (Dict[str, Any]): current hyperparameters
             default_loss (MultiHorizonMetric, optional): default loss function.
                 Defaults to :py:class:`~pytorch_forecasting.metrics.MAE`.
 
         Returns:
             Dict[str, Any]: dictionary with ``output_size`` and ``loss``.
         """
+
         # infer output size
         def get_output_size(normalizer, loss):
             if isinstance(loss, QuantileLoss):
                 return len(loss.quantiles)
             elif isinstance(normalizer, NaNLabelEncoder):
                 return len(normalizer.classes_)
             elif isinstance(loss, DistributionLoss):
@@ -373,37 +608,48 @@
 
     def training_step(self, batch, batch_idx):
         """
         Train on batch.
         """
         x, y = batch
         log, out = self.step(x, y, batch_idx)
-        log.update(self.create_log(x, y, out, batch_idx))
+        self.training_step_outputs.append(log)
         return log
 
-    def training_epoch_end(self, outputs):
-        self.epoch_end(outputs)
+    def on_train_epoch_end(self):
+        self.on_epoch_end(self.training_step_outputs)
+        self.training_step_outputs.clear()
+
+    def predict_step(self, batch, batch_idx):
+        predict_callback = [c for c in self.trainer.callbacks if isinstance(c, PredictCallback)][0]
+        x, y = batch
+        _, out = self.step(x, y, batch_idx, **predict_callback.predict_kwargs)
+        return out  # need to return output to be able to use predict callback
 
     def validation_step(self, batch, batch_idx):
         x, y = batch
         log, out = self.step(x, y, batch_idx)
         log.update(self.create_log(x, y, out, batch_idx))
+        self.validation_step_outputs.append(log)
         return log
 
-    def validation_epoch_end(self, outputs):
-        self.epoch_end(outputs)
+    def on_validation_epoch_end(self):
+        self.on_epoch_end(self.validation_step_outputs)
+        self.validation_step_outputs.clear()
 
     def test_step(self, batch, batch_idx):
         x, y = batch
         log, out = self.step(x, y, batch_idx)
         log.update(self.create_log(x, y, out, batch_idx))
+        self.testing_step_outputs.append(log)
         return log
 
-    def test_epoch_end(self, outputs):
-        self.epoch_end(outputs)
+    def on_test_epoch_end(self):
+        self.on_epoch_end(self.testing_step_outputs)
+        self.testing_step_outputs.clear()
 
     def create_log(
         self,
         x: Dict[str, torch.Tensor],
         y: Tuple[torch.Tensor, torch.Tensor],
         out: Dict[str, torch.Tensor],
         batch_idx: int,
@@ -423,14 +669,20 @@
             quantiles_kwargs (Dict[str, Any], optional):
                 :py:meth:`~pytorch_forcasting.models.base_model.BaseModel.to_quantiles`. Defaults to {}.
 
         Returns:
             Dict[str, Any]: log dictionary to be returned by training and validation steps
         """
         # log
+        if isinstance(self.loss, DistributionLoss):
+            prediction_kwargs.setdefault("n_samples", 20)
+            prediction_kwargs.setdefault("use_metric", True)
+            quantiles_kwargs.setdefault("n_samples", 20)
+            quantiles_kwargs.setdefault("use_metric", True)
+
         self.log_metrics(x, y, out, prediction_kwargs=prediction_kwargs)
         if self.log_interval > 0:
             self.log_prediction(
                 x, out, batch_idx, prediction_kwargs=prediction_kwargs, quantiles_kwargs=quantiles_kwargs
             )
         return {}
 
@@ -445,15 +697,15 @@
             y (Tuple[torch.Tensor, torch.Tensor]): y as passed to the loss function by the dataloader
             batch_idx (int): batch number
             **kwargs: additional arguments to pass to the network apart from ``x``
 
         Returns:
             Tuple[Dict[str, torch.Tensor], Dict[str, torch.Tensor]]: tuple where the first
                 entry is a dictionary to which additional logging results can be added for consumption in the
-                ``epoch_end`` hook and the second entry is the model's output.
+                ``on_epoch_end`` hook and the second entry is the model's output.
         """
         # pack y sequence if different encoder lengths exist
         if (x["decoder_lengths"] < x["decoder_lengths"].max()).any():
             if isinstance(y[0], (list, tuple)):
                 y = (
                     [
                         rnn.pack_padded_sequence(
@@ -482,56 +734,70 @@
             prediction = out["prediction"]
 
             # handle multiple targets
             prediction_list = to_list(prediction)
             gradient = 0
             # todo: should monotone constrains be applicable to certain targets?
             for pred in prediction_list:
-                gradient = gradient + torch.autograd.grad(
-                    outputs=pred,
-                    inputs=x["decoder_cont"],
-                    grad_outputs=torch.ones_like(pred),  # t
-                    create_graph=True,  # allows usage in graph
-                    allow_unused=True,
-                )[0]
+                gradient = (
+                    gradient
+                    + torch.autograd.grad(
+                        outputs=pred,
+                        inputs=x["decoder_cont"],
+                        grad_outputs=torch.ones_like(pred),  # t
+                        create_graph=True,  # allows usage in graph
+                        allow_unused=True,
+                    )[0]
+                )
 
             # select relevant features
             indices = torch.tensor(
                 [self.hparams.x_reals.index(name) for name in self.hparams.monotone_constaints.keys()]
             )
             monotonicity = torch.tensor(
                 [val for val in self.hparams.monotone_constaints.values()], dtype=gradient.dtype, device=gradient.device
             )
             # add additionl loss if gradient points in wrong direction
             gradient = gradient[..., indices] * monotonicity[None, None]
             monotinicity_loss = gradient.clamp_max(0).mean()
             # multiply monotinicity loss by large number to ensure relevance and take to the power of 2
             # for smoothness of loss function
             monotinicity_loss = 10 * torch.pow(monotinicity_loss, 2)
-            if isinstance(self.loss, MASE):
-                loss = self.loss(
-                    prediction, y, encoder_target=x["encoder_target"], encoder_lengths=x["encoder_lengths"]
-                )
-            else:
-                loss = self.loss(prediction, y)
+            if not self.predicting:
+                if isinstance(self.loss, (MASE, MultiLoss)):
+                    loss = self.loss(
+                        prediction, y, encoder_target=x["encoder_target"], encoder_lengths=x["encoder_lengths"]
+                    )
+                else:
+                    loss = self.loss(prediction, y)
 
-            loss = loss * (1 + monotinicity_loss)
+                loss = loss * (1 + monotinicity_loss)
+            else:
+                loss = None
         else:
             out = self(x, **kwargs)
 
             # calculate loss
             prediction = out["prediction"]
-            if isinstance(self.loss, MASE):
-                loss = self.loss(
-                    prediction, y, encoder_target=x["encoder_target"], encoder_lengths=x["encoder_lengths"]
-                )
+            if not self.predicting:
+                if isinstance(self.loss, (MASE, MultiLoss)):
+                    mase_kwargs = dict(encoder_target=x["encoder_target"], encoder_lengths=x["encoder_lengths"])
+                    loss = self.loss(prediction, y, **mase_kwargs)
+                else:
+                    loss = self.loss(prediction, y)
             else:
-                loss = self.loss(prediction, y)
-
-        self.log(f"{self.current_stage}_loss", loss, on_step=self.training, on_epoch=True, prog_bar=True)
+                loss = None
+        self.log(
+            f"{self.current_stage}_loss",
+            loss,
+            on_step=self.training,
+            on_epoch=True,
+            prog_bar=True,
+            batch_size=len(x["decoder_target"]),
+        )
         log = {"loss": loss, "n_samples": x["decoder_lengths"].size(0)}
         return log, out
 
     def log_metrics(
         self,
         x: Dict[str, torch.Tensor],
         y: torch.Tensor,
@@ -575,37 +841,17 @@
                 else:
                     target_tag = ""
                 self.log(
                     f"{target_tag}{self.current_stage}_{metric.name}",
                     loss_value,
                     on_step=self.training,
                     on_epoch=True,
+                    batch_size=len(x["decoder_target"]),
                 )
 
-    def to_network_output(self, **results):
-        """
-        Convert output into a named (and immuatable) tuple.
-
-        This allows tracing the modules as graphs and prevents modifying the output.
-
-        Returns:
-            named tuple
-        """
-        if hasattr(self, "_output_class"):
-            Output = self._output_class
-        else:
-            OutputTuple = namedtuple("output", results)
-
-            class Output(OutputMixIn, OutputTuple):
-                pass
-
-            self._output_class = Output
-
-        return self._output_class(**results)
-
     def forward(
         self, x: Dict[str, Union[torch.Tensor, List[torch.Tensor]]]
     ) -> Dict[str, Union[torch.Tensor, List[torch.Tensor]]]:
         """
         Network forward pass.
 
         Args:
@@ -642,32 +888,32 @@
                     prediction = self.transform_output(prediction, target_scale=x["target_scale"])
 
                     # We need to return a dictionary that at least contains the prediction
                     # The parameter can be directly forwarded from the input.
                     # The conversion to a named tuple can be directly achieved with the `to_network_output` function.
                     return self.to_network_output(prediction=prediction)
 
-
-
         """
         raise NotImplementedError()
 
-    def epoch_end(self, outputs):
+    def on_epoch_end(self, outputs):
         """
         Run at epoch end for training or validation. Can be overriden in models.
         """
         pass
 
     @property
     def log_interval(self) -> float:
         """
         Log interval depending if training or validating
         """
         if self.training:
             return self.hparams.log_interval
+        elif self.predicting:
+            return -1
         else:
             return self.hparams.log_val_interval
 
     def log_prediction(
         self, x: Dict[str, torch.Tensor], out: Dict[str, torch.Tensor], batch_idx: int, **kwargs
     ) -> None:
         """
@@ -712,16 +958,16 @@
         self,
         x: Dict[str, torch.Tensor],
         out: Dict[str, torch.Tensor],
         idx: int = 0,
         add_loss_to_title: Union[Metric, torch.Tensor, bool] = False,
         show_future_observed: bool = True,
         ax=None,
-        quantiles_kwargs: Dict[str, Any] = None,
-        prediction_kwargs: Dict[str, Any] = None,
+        quantiles_kwargs: Dict[str, Any] = {},
+        prediction_kwargs: Dict[str, Any] = {},
     ) -> plt.Figure:
         """
         Plot prediction of prediction vs actuals
 
         Args:
             x: network input
             out: network output
@@ -737,31 +983,23 @@
         Returns:
             matplotlib figure
         """
         # all true values for y of the first sample in batch
         encoder_targets = to_list(x["encoder_target"])
         decoder_targets = to_list(x["decoder_target"])
 
-        # get predictions
-        if prediction_kwargs is None:
-            prediction_kwargs = {}
-
-        if quantiles_kwargs is None:
-            quantiles_kwargs = {}
-
         y_raws = to_list(out["prediction"])  # raw predictions - used for calculating loss
         y_hats = to_list(self.to_prediction(out, **prediction_kwargs))
         y_quantiles = to_list(self.to_quantiles(out, **quantiles_kwargs))
 
         # for each target, plot
         figs = []
         for y_raw, y_hat, y_quantile, encoder_target, decoder_target in zip(
             y_raws, y_hats, y_quantiles, encoder_targets, decoder_targets
         ):
-
             y_all = torch.cat([encoder_target[idx], decoder_target[idx]])
             max_encoder_length = x["encoder_lengths"].max()
             y = torch.cat(
                 (
                     y_all[: x["encoder_lengths"][idx]],
                     y_all[max_encoder_length : (max_encoder_length + x["decoder_lengths"][idx])],
                 ),
@@ -813,27 +1051,31 @@
                     ax.errorbar(
                         x_pred,
                         y[[-n_pred]],
                         yerr=quantiles - y[-n_pred],
                         c=pred_color,
                         capsize=1.0,
                     )
+
             if add_loss_to_title is not False:
                 if isinstance(add_loss_to_title, bool):
                     loss = self.loss
                 elif isinstance(add_loss_to_title, torch.Tensor):
                     loss = add_loss_to_title.detach()[idx].item()
                 elif isinstance(add_loss_to_title, Metric):
                     loss = add_loss_to_title
                 else:
                     raise ValueError(f"add_loss_to_title '{add_loss_to_title}'' is unkown")
                 if isinstance(loss, MASE):
                     loss_value = loss(y_raw[None], (y[-n_pred:][None], None), y[:n_pred][None])
                 elif isinstance(loss, Metric):
-                    loss_value = loss(y_raw[None], (y[-n_pred:][None], None))
+                    try:
+                        loss_value = loss(y_raw[None], (y[-n_pred:][None], None))
+                    except Exception:
+                        loss_value = "-"
                 else:
                     loss_value = loss
                 ax.set_title(f"Loss {loss_value}")
             ax.set_xlabel("Time index")
             fig.legend()
             figs.append(fig)
 
@@ -848,15 +1090,15 @@
         log distribution of gradients to identify exploding / vanishing gradients
         """
         ave_grads = []
         layers = []
         for name, p in named_parameters:
             if p.grad is not None and p.requires_grad and "bias" not in name:
                 layers.append(name)
-                ave_grads.append(p.grad.abs().mean())
+                ave_grads.append(p.grad.abs().cpu().mean())
                 self.logger.experiment.add_histogram(tag=name, values=p.grad, global_step=self.global_step)
         fig, ax = plt.subplots()
         ax.plot(ave_grads)
         ax.set_xlabel("Layers")
         ax.set_ylabel("Average gradient")
         ax.set_yscale("log")
         ax.set_title("Gradient flow")
@@ -898,35 +1140,62 @@
             try:
                 optimizer = self.optimizer(
                     self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params
                 )
             except TypeError:  # in case there is no weight decay
                 optimizer = self.optimizer(self.parameters(), lr=lr, **optimizer_params)
         elif self.hparams.optimizer == "adam":
-            optimizer = torch.optim.Adam(self.parameters(), lr=lr)
+            optimizer = torch.optim.Adam(
+                self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params
+            )
         elif self.hparams.optimizer == "adamw":
-            optimizer = torch.optim.AdamW(self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay)
+            optimizer = torch.optim.AdamW(
+                self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params
+            )
         elif self.hparams.optimizer == "ranger":
-            optimizer = Ranger(self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay)
+            if any([isinstance(c, LearningRateFinder) for c in self.trainer.callbacks]):
+                # if finding learning rate, switch off warm up and cool down
+                optimizer_params.setdefault("num_warm_up_iterations", 0)
+                optimizer_params.setdefault("num_warm_down_iterations", 0)
+                optimizer_params.setdefault("lookahead_merge_time", 1e6)
+                optimizer_params.setdefault("num_iterations", 100)
+            elif self.trainer.limit_train_batches is not None:
+                # if finding limiting train batches, set iterations to it
+                optimizer_params.setdefault(
+                    "num_iterations", min(self.trainer.num_training_batches, self.trainer.limit_train_batches)
+                )
+            else:
+                # if finding not limiting train batches, set iterations to dataloader length
+                optimizer_params.setdefault("num_iterations", self.trainer.num_training_batches)
+            optimizer = Ranger21(self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params)
         elif self.hparams.optimizer == "sgd":
             optimizer = torch.optim.SGD(
                 self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params
             )
         elif hasattr(torch.optim, self.hparams.optimizer):
             try:
                 optimizer = getattr(torch.optim, self.hparams.optimizer)(
                     self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params
                 )
             except TypeError:  # in case there is no weight decay
                 optimizer = getattr(torch.optim, self.hparams.optimizer)(self.parameters(), lr=lr, **optimizer_params)
+        elif hasattr(pytorch_optimizer, self.hparams.optimizer):
+            try:
+                optimizer = getattr(pytorch_optimizer, self.hparams.optimizer)(
+                    self.parameters(), lr=lr, weight_decay=self.hparams.weight_decay, **optimizer_params
+                )
+            except TypeError:  # in case there is no weight decay
+                optimizer = getattr(pytorch_optimizer, self.hparams.optimizer)(
+                    self.parameters(), lr=lr, **optimizer_params
+                )
         else:
             raise ValueError(f"Optimizer of self.hparams.optimizer={self.hparams.optimizer} unknown")
 
         # set scheduler
-        if isinstance(lr, (list, tuple)):  # change for each epoch
+        if isinstance(lrs, (list, tuple)):  # change for each epoch
             # normalize lrs
             lrs = np.array(lrs) / lrs[0]
             scheduler_config = {
                 "scheduler": LambdaLR(optimizer, lambda epoch: lrs[min(epoch, len(lrs) - 1)]),
                 "interval": "epoch",
                 "frequency": 1,
                 "strict": False,
@@ -934,15 +1203,15 @@
         elif self.hparams.reduce_on_plateau_patience is None:
             scheduler_config = {}
         else:  # find schedule based on validation loss
             scheduler_config = {
                 "scheduler": ReduceLROnPlateau(
                     optimizer,
                     mode="min",
-                    factor=0.2,
+                    factor=1.0 / self.hparams.reduce_on_plateau_reduction,
                     patience=self.hparams.reduce_on_plateau_patience,
                     cooldown=self.hparams.reduce_on_plateau_patience,
                     min_lr=self.hparams.reduce_on_plateau_min_lr,
                 ),
                 "monitor": "val_loss",  # Default: val_loss
                 "interval": "epoch",
                 "frequency": 1,
@@ -1017,16 +1286,16 @@
             use_metric (bool): if to use metric to convert for conversion, if False,
                 simply take the average over ``out["prediction"]``
             **kwargs: arguments to metric ``to_quantiles`` method
 
         Returns:
             torch.Tensor: predictions of shape batch_size x timesteps
         """
-        # if samples were already drawn directly take mean
         if not use_metric:
+            # if samples were already drawn directly take mean
             # todo: support classification
             if isinstance(self.loss, MultiLoss):
                 out = [Metric.to_prediction(loss, out["prediction"][idx]) for idx, loss in enumerate(self.loss)]
             else:
                 out = Metric.to_prediction(self.loss, out["prediction"])
         else:
             try:
@@ -1073,42 +1342,48 @@
         data: Union[DataLoader, pd.DataFrame, TimeSeriesDataSet],
         mode: Union[str, Tuple[str, str]] = "prediction",
         return_index: bool = False,
         return_decoder_lengths: bool = False,
         batch_size: int = 64,
         num_workers: int = 0,
         fast_dev_run: bool = False,
-        show_progress_bar: bool = False,
         return_x: bool = False,
+        return_y: bool = False,
         mode_kwargs: Dict[str, Any] = None,
+        trainer_kwargs: Optional[Dict[str, Any]] = None,
+        write_interval: Literal["batch", "epoch", "batch_and_epoch"] = "batch",
+        output_dir: Optional[str] = None,
         **kwargs,
-    ):
+    ) -> Prediction:
         """
         Run inference / prediction.
 
         Args:
             dataloader: dataloader, dataframe or dataset
             mode: one of "prediction", "quantiles", or "raw", or tuple ``("raw", output_name)`` where output_name is
                 a name in the dictionary returned by ``forward()``
             return_index: if to return the prediction index (in the same order as the output, i.e. the row of the
                 dataframe corresponds to the first dimension of the output and the given time index is the time index
                 of the first prediction)
             return_decoder_lengths: if to return decoder_lengths (in the same order as the output
             batch_size: batch size for dataloader - only used if data is not a dataloader is passed
             num_workers: number of workers for dataloader - only used if data is not a dataloader is passed
             fast_dev_run: if to only return results of first batch
-            show_progress_bar: if to show progress bar. Defaults to False.
             return_x: if to return network inputs (in the same order as prediction output)
+            return_y: if to return network targets (in the same order as prediction output)
             mode_kwargs (Dict[str, Any]): keyword arguments for ``to_prediction()`` or ``to_quantiles()``
                 for modes "prediction" and "quantiles"
+            trainer_kwargs (Dict[str, Any], optional): keyword arguments for the trainer
+            write_interval: interval to write predictions to disk
+            output_dir: directory to write predictions to. Defaults to None. If set function will return empty list
             **kwargs: additional arguments to network's forward method
 
         Returns:
-            output, x, index, decoder_lengths: some elements might not be present depending on what is configured
-                to be returned
+            Prediction: if one of the ```return`` arguments is present,
+                prediction tuple with fields ``prediction``, ``x``, ``y``, ``index`` and ``decoder_lengths``
         """
         # convert to dataloader
         if isinstance(data, pd.DataFrame):
             data = TimeSeriesDataSet.from_parameters(self.dataset_parameters, data, predict=True)
         if isinstance(data, TimeSeriesDataSet):
             dataloader = data.to_dataloader(batch_size=batch_size, train=False, num_workers=num_workers)
         else:
@@ -1117,102 +1392,43 @@
         # mode kwargs default to None
         if mode_kwargs is None:
             mode_kwargs = {}
 
         # ensure passed dataloader is correct
         assert isinstance(dataloader.dataset, TimeSeriesDataSet), "dataset behind dataloader mut be TimeSeriesDataSet"
 
-        # prepare model
-        self.eval()  # no dropout, etc. no gradients
-
-        # run predictions
-        output = []
-        decode_lenghts = []
-        x_list = []
-        index = []
-        progress_bar = tqdm(desc="Predict", unit=" batches", total=len(dataloader), disable=not show_progress_bar)
-        with torch.no_grad():
-            for x, _ in dataloader:
-                # move data to appropriate device
-                data_device = x["encoder_cont"].device
-                if data_device != self.device:
-                    x = move_to_device(x, self.device)
-
-                # make prediction
-                out = self(x, **kwargs)  # raw output is dictionary
-
-                lengths = x["decoder_lengths"]
-                if return_decoder_lengths:
-                    decode_lenghts.append(lengths)
-                nan_mask = create_mask(lengths.max(), lengths)
-                if isinstance(mode, (tuple, list)):
-                    if mode[0] == "raw":
-                        out = out[mode[1]]
-                    else:
-                        raise ValueError(
-                            f"If a tuple is specified, the first element must be 'raw' - got {mode[0]} instead"
-                        )
-                elif mode == "prediction":
-                    out = self.to_prediction(out, **mode_kwargs)
-                    # mask non-predictions
-                    if isinstance(out, (list, tuple)):
-                        out = [
-                            o.masked_fill(nan_mask, torch.tensor(float("nan"))) if o.dtype == torch.float else o
-                            for o in out
-                        ]
-                    elif out.dtype == torch.float:  # only floats can be filled with nans
-                        out = out.masked_fill(nan_mask, torch.tensor(float("nan")))
-                elif mode == "quantiles":
-                    out = self.to_quantiles(out, **mode_kwargs)
-                    # mask non-predictions
-                    if isinstance(out, (list, tuple)):
-                        out = [
-                            o.masked_fill(nan_mask.unsqueeze(-1), torch.tensor(float("nan")))
-                            if o.dtype == torch.float
-                            else o
-                            for o in out
-                        ]
-                    elif out.dtype == torch.float:
-                        out = out.masked_fill(nan_mask.unsqueeze(-1), torch.tensor(float("nan")))
-                elif mode == "raw":
-                    pass
-                else:
-                    raise ValueError(f"Unknown mode {mode} - see docs for valid arguments")
-
-                out = move_to_device(out, device="cpu")
-
-                output.append(out)
-                if return_x:
-                    x = move_to_device(x, "cpu")
-                    x_list.append(x)
-                if return_index:
-                    index.append(dataloader.dataset.x_to_index(x))
-                progress_bar.update()
-                if fast_dev_run:
-                    break
-
-        # concatenate output (of different batches)
-        if isinstance(mode, (tuple, list)) or mode != "raw":
-            if isinstance(output[0], (tuple, list)) and len(output[0]) > 0 and isinstance(output[0][0], torch.Tensor):
-                output = [_torch_cat_na([out[idx] for out in output]) for idx in range(len(output[0]))]
-            else:
-                output = _torch_cat_na(output)
-        elif mode == "raw":
-            output = _concatenate_output(output)
+        predict_callback = PredictCallback(
+            mode=mode,
+            return_index=return_index,
+            return_decoder_lengths=return_decoder_lengths,
+            write_interval=write_interval,
+            return_x=return_x,
+            mode_kwargs=mode_kwargs,
+            output_dir=output_dir,
+            predict_kwargs=kwargs,
+            return_y=return_y,
+        )
+        if trainer_kwargs is None:
+            trainer_kwargs = {}
+        trainer_kwargs.setdefault("callbacks", trainer_kwargs.get("callbacks", []) + [predict_callback])
+        trainer_kwargs.setdefault("enable_progress_bar", False)
+        trainer_kwargs.setdefault("inference_mode", False)
+        assert (
+            "fast_dev_run" not in trainer_kwargs
+        ), "fast_dev_run should be passed as argument to predict and not in trainer_kwargs"
+        log_level_lighting = logging.getLogger("lightning").getEffectiveLevel()
+        log_level_pytorch_lightning = logging.getLogger("pytorch_lightning").getEffectiveLevel()
+        logging.getLogger("lightning").setLevel(logging.WARNING)
+        logging.getLogger("pytorch_lightning").setLevel(logging.WARNING)
+        trainer = Trainer(fast_dev_run=fast_dev_run, **trainer_kwargs)
+        trainer.predict(self, dataloader)
+        logging.getLogger("lightning").setLevel(log_level_lighting)
+        logging.getLogger("pytorch_lightning").setLevel(log_level_pytorch_lightning)
 
-        # generate output
-        if return_x or return_index or return_decoder_lengths:
-            output = [output]
-        if return_x:
-            output.append(_concatenate_output(x_list))
-        if return_index:
-            output.append(pd.concat(index, axis=0, ignore_index=True))
-        if return_decoder_lengths:
-            output.append(torch.cat(decode_lenghts, dim=0))
-        return output
+        return predict_callback.result
 
     def predict_dependency(
         self,
         data: Union[DataLoader, pd.DataFrame, TimeSeriesDataSet],
         variable: str,
         values: Iterable,
         mode: str = "dataframe",
@@ -1256,42 +1472,42 @@
         for idx, value in enumerate(values):
             # set values
             data.set_overwrite_values(variable=variable, values=value, target=target)
             # predict
             kwargs.setdefault("mode", "prediction")
 
             if idx == 0 and mode == "dataframe":  # need index for returning as dataframe
-                res, index = self.predict(data, return_index=True, **kwargs)
-                results.append(res)
+                res = self.predict(data, return_index=True, **kwargs)
+                results.append(res.output)
             else:
                 results.append(self.predict(data, **kwargs))
             # increment progress
             progress_bar.update()
 
         data.reset_overwrite_values()  # reset overwrite values to avoid side-effect
 
         # results to one tensor
         results = torch.stack(results, dim=0)
 
         # convert results to requested output format
         if mode == "series":
             results = results[:, ~torch.isnan(results[0])].mean(1)  # average samples and prediction horizon
-            results = pd.Series(results, index=values)
+            results = pd.Series(results.cpu().numpy(), index=values)
 
         elif mode == "dataframe":
             # take mean over time
             is_nan = torch.isnan(results)
             results[is_nan] = 0
             results = results.sum(-1) / (~is_nan).float().sum(-1)
 
             # create dataframe
             dependencies = (
-                index.iloc[np.tile(np.arange(len(index)), len(values))]
+                res.index.iloc[np.tile(np.arange(len(res.index)), len(values))]
                 .reset_index(drop=True)
-                .assign(prediction=results.flatten())
+                .assign(prediction=results.flatten().cpu().numpy())
             )
             dependencies[variable] = values.repeat(len(data))
             first_prediction = dependencies.groupby(data.group_ids, observed=True).prediction.transform("first")
             dependencies["normalized_prediction"] = dependencies["prediction"] / first_prediction
             dependencies["id"] = dependencies.groupby(data.group_ids, observed=True).ngroup()
             results = dependencies
 
@@ -1326,14 +1542,33 @@
              embedding vector filled with zeros
         categorical_groups (Dict[str, List[str]]): dictionary of categorical variables that are grouped together and
             can also take multiple values simultaneously (e.g. holiday during octoberfest). They should be implemented
             as bag of embeddings
     """
 
     @property
+    def target_positions(self) -> torch.LongTensor:
+        """
+        Positions of target variable(s) in covariates.
+
+        Returns:
+            torch.LongTensor: tensor of positions.
+        """
+        # todo: expand for categorical targets
+        if "target" in self.hparams:
+            target = self.hparams.target
+        else:
+            target = self.dataset_parameters["target"]
+        return torch.tensor(
+            [self.hparams.x_reals.index(name) for name in to_list(target)],
+            device=self.device,
+            dtype=torch.long,
+        )
+
+    @property
     def reals(self) -> List[str]:
         """List of all continuous variables in model"""
         return list(
             dict.fromkeys(
                 self.hparams.static_reals
                 + self.hparams.time_varying_reals_encoder
                 + self.hparams.time_varying_reals_decoder
@@ -1432,14 +1667,55 @@
             embedding_labels=embedding_labels,
             embedding_paddings=embedding_paddings,
             categorical_groups=dataset.variable_groups,
         )
         new_kwargs.update(kwargs)
         return super().from_dataset(dataset, **new_kwargs)
 
+    def extract_features(
+        self,
+        x,
+        embeddings: MultiEmbedding = None,
+        period: str = "all",
+    ) -> torch.Tensor:
+        """
+        Extract features
+
+        Args:
+            x (Dict[str, torch.Tensor]): input from the dataloader
+            embeddings (MultiEmbedding): embeddings for categorical variables
+            period (str, optional): One of "encoder", "decoder" or "all". Defaults to "all".
+
+        Returns:
+            torch.Tensor: tensor with selected variables
+        """
+        # select period
+        if period == "encoder":
+            x_cat = x["encoder_cat"]
+            x_cont = x["encoder_cont"]
+        elif period == "decoder":
+            x_cat = x["decoder_cat"]
+            x_cont = x["decoder_cont"]
+        elif period == "all":
+            x_cat = torch.cat([x["encoder_cat"], x["decoder_cat"]], dim=1)  # concatenate in time dimension
+            x_cont = torch.cat([x["encoder_cont"], x["decoder_cont"]], dim=1)  # concatenate in time dimension
+        else:
+            raise ValueError(f"Unknown type: {type}")
+
+        # create dictionary of encoded vectors
+        input_vectors = embeddings(x_cat)
+        input_vectors.update(
+            {
+                name: x_cont[..., idx].unsqueeze(-1)
+                for idx, name in enumerate(self.hparams.x_reals)
+                if name in self.reals
+            }
+        )
+        return input_vectors
+
     def calculate_prediction_actual_by_variable(
         self,
         x: Dict[str, torch.Tensor],
         y_pred: torch.Tensor,
         normalize: bool = True,
         bins: int = 95,
         std: float = 2.0,
@@ -1718,24 +1994,26 @@
         kwargs.setdefault("target_lags", {name: dataset._get_lagged_names(name) for name in lags})
         return super().from_dataset(dataset, **kwargs)
 
     def output_to_prediction(
         self,
         normalized_prediction_parameters: torch.Tensor,
         target_scale: Union[List[torch.Tensor], torch.Tensor],
+        n_samples: int = 1,
         **kwargs,
     ) -> Tuple[Union[List[torch.Tensor], torch.Tensor], torch.Tensor]:
         """
         Convert network output to rescaled and normalized prediction.
 
         Function is typically not called directly but via :py:meth:`~decode_autoregressive`.
 
         Args:
             normalized_prediction_parameters (torch.Tensor): network prediction output
             target_scale (Union[List[torch.Tensor], torch.Tensor]): target scale to rescale network output
+            n_samples (int, optional): Number of samples to draw independently. Defaults to 1.
             **kwargs: extra arguments for dictionary passed to :py:meth:`~transform_output` method.
 
         Returns:
             Tuple[Union[List[torch.Tensor], torch.Tensor], torch.Tensor]: tuple of rescaled prediction and
                 normalized prediction (e.g. for input into next auto-regressive step)
         """
         single_prediction = to_list(normalized_prediction_parameters)[0].ndim == 2
@@ -1747,15 +2025,23 @@
         )
         # todo: handle classification
         # sample value(s) from distribution and  select first sample
         if isinstance(self.loss, DistributionLoss) or (
             isinstance(self.loss, MultiLoss) and isinstance(self.loss[0], DistributionLoss)
         ):
             # todo: handle mixed losses
-            prediction = self.loss.sample(prediction_parameters, 1)
+            if n_samples > 1:
+                prediction_parameters = apply_to_list(
+                    prediction_parameters, lambda x: x.reshape(int(x.size(0) / n_samples), n_samples, -1)
+                )
+                prediction = self.loss.sample(prediction_parameters, 1)
+                prediction = apply_to_list(prediction, lambda x: x.reshape(x.size(0) * n_samples, 1, -1))
+            else:
+                prediction = self.loss.sample(normalized_prediction_parameters, 1)
+
         else:
             prediction = prediction_parameters
         # normalize prediction prediction
         normalized_prediction = self.output_transformer.transform(prediction, target_scale=target_scale)
         if isinstance(normalized_prediction, list):
             input_target = torch.cat(normalized_prediction, dim=-1)
         else:
@@ -1770,14 +2056,15 @@
     def decode_autoregressive(
         self,
         decode_one: Callable,
         first_target: Union[List[torch.Tensor], torch.Tensor],
         first_hidden_state: Any,
         target_scale: Union[List[torch.Tensor], torch.Tensor],
         n_decoder_steps: int,
+        n_samples: int = 1,
         **kwargs,
     ) -> Union[List[torch.Tensor], torch.Tensor]:
         """
         Make predictions in auto-regressive manner.
 
         Supports only continuous targets.
 
@@ -1795,14 +2082,16 @@
                 And returns tuple of (not rescaled) network prediction output and hidden state for next
                 auto-regressive step.
 
             first_target (Union[List[torch.Tensor], torch.Tensor]): first target value to use for decoding
             first_hidden_state (Any): first hidden state used for decoding
             target_scale (Union[List[torch.Tensor], torch.Tensor]): target scale as in ``x``
             n_decoder_steps (int): number of decoding/prediction steps
+            n_samples (int): number of independent samples to draw from the distribution -
+                only relevant for multivariate models. Defaults to 1.
             **kwargs: additional arguments that are passed to the decode_one function.
 
         Returns:
             Union[List[torch.Tensor], torch.Tensor]: re-scaled prediction
 
         Example:
 
@@ -1820,15 +2109,15 @@
                     )
                     # but this time fill in missing target from encoder_cont at the first time step instead of
                     # throwing it away
                     last_encoder_target = x["encoder_cont"][
                         torch.arange(x["encoder_cont"].size(0), device=x["encoder_cont"].device),
                         x["encoder_lengths"] - 1,
                         self.target_positions.unsqueeze(-1)
-                    ].T
+                    ].T.contiguous()
                     input_vector[:, 0, self.target_positions] = last_encoder_target
 
                     if self.training:  # training mode
                         decoder_output, _ = self.rnn(
                             x,
                             hidden_state,
                             lengths=x["decoder_lengths"],
@@ -1888,15 +2177,17 @@
         for idx in range(n_decoder_steps):
             # get lagged targets
             current_target, current_hidden_state = decode_one(
                 idx, lagged_targets=normalized_output, hidden_state=current_hidden_state, **kwargs
             )
 
             # get prediction and its normalized version for the next step
-            prediction, current_target = self.output_to_prediction(current_target, target_scale=target_scale)
+            prediction, current_target = self.output_to_prediction(
+                current_target, target_scale=target_scale, n_samples=n_samples
+            )
             # save normalized output for lagged targets
             normalized_output.append(current_target)
             # set output to unnormalized samples, append each target as n_batch_samples x n_random_samples
 
             output.append(prediction)
         if isinstance(self.hparams.target, str):
             output = torch.stack(output, dim=1)
@@ -1916,14 +2207,60 @@
         # todo: expand for categorical targets
         return torch.tensor(
             [0],
             device=self.device,
             dtype=torch.long,
         )
 
+    def plot_prediction(
+        self,
+        x: Dict[str, torch.Tensor],
+        out: Dict[str, torch.Tensor],
+        idx: int = 0,
+        add_loss_to_title: Union[Metric, torch.Tensor, bool] = False,
+        show_future_observed: bool = True,
+        ax=None,
+        quantiles_kwargs: Dict[str, Any] = {},
+        prediction_kwargs: Dict[str, Any] = {},
+    ) -> plt.Figure:
+        """
+        Plot prediction of prediction vs actuals
+
+        Args:
+            x: network input
+            out: network output
+            idx: index of prediction to plot
+            add_loss_to_title: if to add loss to title or loss function to calculate. Can be either metrics,
+                bool indicating if to use loss metric or tensor which contains losses for all samples.
+                Calcualted losses are determined without weights. Default to False.
+            show_future_observed: if to show actuals for future. Defaults to True.
+            ax: matplotlib axes to plot on
+            quantiles_kwargs (Dict[str, Any]): parameters for ``to_quantiles()`` of the loss metric.
+            prediction_kwargs (Dict[str, Any]): parameters for ``to_prediction()`` of the loss metric.
+
+        Returns:
+            matplotlib figure
+        """
+
+        # get predictions
+        if isinstance(self.loss, DistributionLoss):
+            prediction_kwargs.setdefault("use_metric", False)
+            quantiles_kwargs.setdefault("use_metric", False)
+
+        return super().plot_prediction(
+            x=x,
+            out=out,
+            idx=idx,
+            add_loss_to_title=add_loss_to_title,
+            show_future_observed=show_future_observed,
+            ax=ax,
+            quantiles_kwargs=quantiles_kwargs,
+            prediction_kwargs=prediction_kwargs,
+        )
+
     @property
     def lagged_target_positions(self) -> Dict[int, torch.LongTensor]:
         """
         Positions of lagged target variable(s) in covariates.
 
         Returns:
             Dict[int, torch.LongTensor]: dictionary mapping integer lags to tensor of variable positions.
@@ -1962,29 +2299,14 @@
              embedding vector filled with zeros
         categorical_groups (Dict[str, List[str]]): dictionary of categorical variables that are grouped together and
             can also take multiple values simultaneously (e.g. holiday during octoberfest). They should be implemented
             as bag of embeddings
     """
 
     @property
-    def target_positions(self) -> torch.LongTensor:
-        """
-        Positions of target variable(s) in covariates.
-
-        Returns:
-            torch.LongTensor: tensor of positions.
-        """
-        # todo: expand for categorical targets
-        return torch.tensor(
-            [self.hparams.x_reals.index(name) for name in to_list(self.hparams.target)],
-            device=self.device,
-            dtype=torch.long,
-        )
-
-    @property
     def lagged_target_positions(self) -> Dict[int, torch.LongTensor]:
         """
         Positions of lagged target variable(s) in covariates.
 
         Returns:
             Dict[int, torch.LongTensor]: dictionary mapping integer lags to tensor of variable positions.
         """
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/baseline.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/baseline.py`

 * *Files identical despite different names*

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/basic_rnn/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/rnn/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """
-Basic RNN model with LSTM or GRU cells
+Simple recurrent model - either with LSTM or GRU cells.
 """
+from copy import copy
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import torch
-from torch import nn
-from torch.nn.utils import rnn
+import torch.nn as nn
 
-from pytorch_forecasting.metrics import MultiHorizonMetric
+from pytorch_forecasting.data.encoders import MultiNormalizer, NaNLabelEncoder
+from pytorch_forecasting.data.timeseries import TimeSeriesDataSet
+from pytorch_forecasting.metrics import MAE, MAPE, MASE, RMSE, SMAPE, MultiHorizonMetric, MultiLoss, QuantileLoss
 from pytorch_forecasting.models.base_model import AutoRegressiveBaseModelWithCovariates
-from pytorch_forecasting.models.nn import MultiEmbedding, get_rnn
-from pytorch_forecasting.utils import to_list
+from pytorch_forecasting.models.nn import HiddenState, MultiEmbedding, get_rnn
+from pytorch_forecasting.utils import apply_to_list, to_list
 
 
-class LSTMModel(AutoRegressiveBaseModelWithCovariates):
-    """
-    Basic RNN network.
-    """
-
+class RecurrentNetwork(AutoRegressiveBaseModelWithCovariates):
     def __init__(
         self,
         cell_type: str = "LSTM",
         hidden_size: int = 10,
         rnn_layers: int = 2,
         dropout: float = 0.1,
         static_categoricals: List[str] = [],
@@ -33,22 +31,26 @@
         time_varying_reals_encoder: List[str] = [],
         time_varying_reals_decoder: List[str] = [],
         embedding_sizes: Dict[str, Tuple[int, int]] = {},
         embedding_paddings: List[str] = [],
         embedding_labels: Dict[str, np.ndarray] = {},
         x_reals: List[str] = [],
         x_categoricals: List[str] = [],
-        n_validation_samples: int = None,
-        n_plotting_samples: int = None,
+        output_size: Union[int, List[int]] = 1,
         target: Union[str, List[str]] = None,
+        target_lags: Dict[str, List[int]] = {},
         loss: MultiHorizonMetric = None,
         logging_metrics: nn.ModuleList = None,
         **kwargs,
     ):
         """
+        Recurrent Network.
+
+        Simple LSTM or GRU layer followed by output layer
+
         Args:
             cell_type (str, optional): Recurrent cell type ["LSTM", "GRU"]. Defaults to "LSTM".
             hidden_size (int, optional): hidden recurrent size - the most important hyperparameter along with
                 ``rnn_layers``. Defaults to 10.
             rnn_layers (int, optional): Number of RNN layers - important hyperparameter. Defaults to 2.
             dropout (float, optional): Dropout in RNN layers. Defaults to 0.1.
             static_categoricals: integer of positions of static categorical variables
@@ -62,150 +64,227 @@
                 variable which is the key in the dictionary
             x_reals: order of continuous variables in tensor passed to forward function
             x_categoricals: order of categorical variables in tensor passed to forward function
             embedding_sizes: dictionary mapping (string) indices to tuple of number of categorical classes and
                 embedding size
             embedding_paddings: list of indices for embeddings which transform the zero's embedding to a zero vector
             embedding_labels: dictionary mapping (string) indices to list of categorical labels
-            n_validation_samples (int, optional): Number of samples to use for calculating validation metrics.
-                Defaults to None, i.e. no sampling at validation stage and using "mean" of distribution for logging
-                metrics calculation.
-            n_plotting_samples (int, optional): Number of samples to generate for plotting predictions
-                during training. Defaults to ``n_validation_samples`` if not None or 100 otherwise.
+            output_size (Union[int, List[int]], optional): number of outputs (e.g. number of quantiles for
+                QuantileLoss and one target or list of output sizes).
             target (str, optional): Target variable or list of target variables. Defaults to None.
-            loss (DistributionLoss, optional): Distribution loss function. Keep in mind that each distribution
-                loss function might have specific requirements for target normalization.
-                Defaults to :py:class:`~pytorch_forecasting.metrics.NormalDistributionLoss`.
+            target_lags (Dict[str, Dict[str, int]]): dictionary of target names mapped to list of time steps by
+                which the variable should be lagged.
+                Lags can be useful to indicate seasonality to the models. If you know the seasonalit(ies) of your data,
+                add at least the target variables with the corresponding lags to improve performance.
+                Defaults to no lags, i.e. an empty dictionary.
+            loss (MultiHorizonMetric, optional): loss: loss function taking prediction and targets.
             logging_metrics (nn.ModuleList, optional): Metrics to log during training.
                 Defaults to nn.ModuleList([SMAPE(), MAE(), RMSE(), MAPE(), MASE()]).
         """
-        # saves arguments in signature to `.hparams` attribute, mandatory call - do not skip this
+        if loss is None:
+            loss = MAE()
+        if logging_metrics is None:
+            logging_metrics = nn.ModuleList([SMAPE(), MAE(), RMSE(), MAPE(), MASE()])
         self.save_hyperparameters()
-        # pass additional arguments to BaseModel.__init__, mandatory call - do not skip this
+        # store loss function separately as it is a module
         super().__init__(loss=loss, logging_metrics=logging_metrics, **kwargs)
 
-        assert set(self.encoder_variables) - set(to_list(target)) == set(
-            self.decoder_variables
-        ), "Encoder and decoder variables have to be the same apart from target variable"
-        for targeti in to_list(target):
-            assert (
-                targeti in time_varying_reals_encoder
-            ), f"target {targeti} has to be real"  # todo: remove this restriction
-
         self.embeddings = MultiEmbedding(
             embedding_sizes=embedding_sizes,
             embedding_paddings=embedding_paddings,
             categorical_groups=categorical_groups,
             x_categoricals=x_categoricals,
         )
 
-        time_series_rnn = get_rnn(cell_type)
+        lagged_target_names = [l for lags in target_lags.values() for l in lags]
+        assert set(self.encoder_variables) - set(to_list(target)) - set(lagged_target_names) == set(
+            self.decoder_variables
+        ) - set(lagged_target_names), "Encoder and decoder variables have to be the same apart from target variable"
+        for targeti in to_list(target):
+            assert (
+                targeti in time_varying_reals_encoder
+            ), f"target {targeti} has to be real"  # todo: remove this restriction
+        assert (isinstance(target, str) and isinstance(loss, MultiHorizonMetric)) or (
+            isinstance(target, (list, tuple)) and isinstance(loss, MultiLoss) and len(loss) == len(target)
+        ), "number of targets should be equivalent to number of loss metrics"
+
+        rnn_class = get_rnn(cell_type)
         cont_size = len(self.reals)
-        cat_size = sum([size[1] for size in self.hparams.embedding_sizes.values()])
+        cat_size = sum(self.embeddings.output_size.values())
         input_size = cont_size + cat_size
-        self.rnn = time_series_rnn(
+        self.rnn = rnn_class(
             input_size=input_size,
             hidden_size=self.hparams.hidden_size,
             num_layers=self.hparams.rnn_layers,
             dropout=self.hparams.dropout if self.hparams.rnn_layers > 1 else 0,
             batch_first=True,
         )
 
         # add linear layers for argument projects
         if isinstance(target, str):  # single target
-            self.output_projector = nn.Linear(self.hparams.hidden_size, 1)
+            self.output_projector = nn.Linear(self.hparams.hidden_size, self.hparams.output_size)
+            assert not isinstance(self.loss, QuantileLoss), "QuantileLoss does not work with recurrent network"
         else:  # multi target
-            self.output_projector = nn.ModuleList([nn.Linear(self.hparams.hidden_size, 1) for _ in target])
+            self.output_projector = nn.ModuleList(
+                [nn.Linear(self.hparams.hidden_size, size) for size in self.hparams.output_size]
+            )
+            for l in self.loss:
+                assert not isinstance(l, QuantileLoss), "QuantileLoss does not work with recurrent network"
 
-    @property
-    def target_position(self):
-        # position of target within reals vector: with covariates: self.hparams.x_reals.index(self.hparams.target)
-        return 0
-
-    def encode(self, x: Dict[str, torch.Tensor]):
-        # we need at least one encoding step as because the target needs to be lagged by one time step
-        # as we are lazy, we also require that the encoder length is at least 1, so we can easily generate a
-        # hidden state here. See the DeepAR implementation for how to use a minimal encoder length of 1
-        max_encoder_length = x["encoder_lengths"].max()
-        assert x["encoder_lengths"].min() > 0
-        if max_encoder_length > 1:
-            encoder_lengths = x["encoder_lengths"] - 1
-            rnn_encoder_lengths = encoder_lengths.where(encoder_lengths > 0, torch.ones_like(encoder_lengths))
-            input_vector = self.construct_input_vector(x["encoder_cat"], x["encoder_cont"])
-            _, hidden_state = self.rnn(
-                rnn.pack_padded_sequence(
-                    input_vector, rnn_encoder_lengths.cpu(), enforce_sorted=False, batch_first=True
-                )
-            )  # second ouput is not needed (hidden state)
-            # replace hidden cell with initial input if encoder_length is zero to determine correct initial state
-            no_encoding = (encoder_lengths == 0)[None, :, None]  # shape: n_lstm_layers x batch_size x hidden_size
-            hidden_state = self.rnn.handle_no_encoding(hidden_state, no_encoding)
+    @classmethod
+    def from_dataset(
+        cls,
+        dataset: TimeSeriesDataSet,
+        allowed_encoder_known_variable_names: List[str] = None,
+        **kwargs,
+    ):
+        """
+        Create model from dataset.
+
+        Args:
+            dataset: timeseries dataset
+            allowed_encoder_known_variable_names: List of known variables that are allowed in encoder, defaults to all
+            **kwargs: additional arguments such as hyperparameters for model (see ``__init__()``)
+
+        Returns:
+            Recurrent network
+        """
+        new_kwargs = copy(kwargs)
+        new_kwargs.update(cls.deduce_default_output_parameters(dataset=dataset, kwargs=kwargs, default_loss=MAE()))
+        assert not isinstance(dataset.target_normalizer, NaNLabelEncoder) and (
+            not isinstance(dataset.target_normalizer, MultiNormalizer)
+            or all([not isinstance(normalizer, NaNLabelEncoder) for normalizer in dataset.target_normalizer])
+        ), "target(s) should be continuous - categorical targets are not supported"  # todo: remove this restriction
+        return super().from_dataset(
+            dataset, allowed_encoder_known_variable_names=allowed_encoder_known_variable_names, **new_kwargs
+        )
+
+    def construct_input_vector(
+        self, x_cat: torch.Tensor, x_cont: torch.Tensor, one_off_target: torch.Tensor = None
+    ) -> torch.Tensor:
+        """
+        Create input vector into RNN network
+
+        Args:
+            one_off_target: tensor to insert into first position of target. If None (default), remove first time step.
+        """
+        # create input vector
+        if len(self.categoricals) > 0:
+            embeddings = self.embeddings(x_cat)
+            flat_embeddings = torch.cat([emb for emb in embeddings.values()], dim=-1)
+            input_vector = flat_embeddings
+
+        if len(self.reals) > 0:
+            input_vector = x_cont.clone()
+
+        if len(self.reals) > 0 and len(self.categoricals) > 0:
+            input_vector = torch.cat([x_cont, flat_embeddings], dim=-1)
+
+        # shift target by one
+        input_vector[..., self.target_positions] = torch.roll(
+            input_vector[..., self.target_positions], shifts=1, dims=1
+        )
+
+        if one_off_target is not None:  # set first target input (which is rolled over)
+            input_vector[:, 0, self.target_positions] = one_off_target
         else:
-            hidden_state = self.rnn.init_hidden_state(x, self.hparam.hidden_size)
+            input_vector = input_vector[:, 1:]
+
+        # shift target
+        return input_vector
+
+    def encode(self, x: Dict[str, torch.Tensor]) -> HiddenState:
+        """
+        Encode sequence into hidden state
+        """
+        # encode using rnn
+        assert x["encoder_lengths"].min() > 0
+        encoder_lengths = x["encoder_lengths"] - 1
+        input_vector = self.construct_input_vector(x["encoder_cat"], x["encoder_cont"])
+        _, hidden_state = self.rnn(
+            input_vector, lengths=encoder_lengths, enforce_sorted=False
+        )  # second ouput is not needed (hidden state)
         return hidden_state
 
-    def decode(self, x: Dict[str, torch.Tensor], hidden_state):
-        # again lag target by one
-        input_vector = x["decoder_cont"].clone()
-        input_vector[..., self.target_position] = torch.roll(input_vector[..., self.target_position], shifts=1, dims=1)
-        # but this time fill in missing target from encoder_cont at the first time step instead of throwing it away
-        last_encoder_target = x["encoder_cont"][
-            torch.arange(x["encoder_cont"].size(0)), x["encoder_lengths"] - 1, self.target_position
-        ]
-        input_vector[:, 0, self.target_position] = last_encoder_target
-
-        if self.training:  # training attribute is provided from PyTorch and indicates if module is in training model
-            packed_decoder = rnn.pack_padded_sequence(
-                input_vector, lengths=x["decoder_lengths"].cpu(), batch_first=True, enforce_sorted=False
+    def decode_all(
+        self,
+        x: torch.Tensor,
+        hidden_state: HiddenState,
+        lengths: torch.Tensor = None,
+    ):
+        decoder_output, hidden_state = self.rnn(x, hidden_state, lengths=lengths, enforce_sorted=False)
+        if isinstance(self.hparams.target, str):  # single target
+            output = self.output_projector(decoder_output)
+        else:
+            output = [projector(decoder_output) for projector in self.output_projector]
+        return output, hidden_state
+
+    def decode(
+        self,
+        input_vector: torch.Tensor,
+        target_scale: torch.Tensor,
+        decoder_lengths: torch.Tensor,
+        hidden_state: HiddenState,
+        n_samples: int = None,
+    ) -> Tuple[torch.Tensor, bool]:
+        """
+        Decode hidden state of RNN into prediction. If n_smaples is given,
+        decode not by using actual values but rather by
+        sampling new targets from past predictions iteratively
+        """
+        if self.training:
+            output, _ = self.decode_all(input_vector, hidden_state, lengths=decoder_lengths)
+            output = self.transform_output(output, target_scale=target_scale)
+        else:
+            # run in eval, i.e. simulation mode
+            target_pos = self.target_positions
+            lagged_target_positions = self.lagged_target_positions
+
+            # define function to run at every decoding step
+            def decode_one(
+                idx,
+                lagged_targets,
+                hidden_state,
+            ):
+                x = input_vector[:, [idx]]
+                x[:, 0, target_pos] = lagged_targets[-1]
+                for lag, lag_positions in lagged_target_positions.items():
+                    if idx > lag:
+                        x[:, 0, lag_positions] = lagged_targets[-lag]
+                prediction, hidden_state = self.decode_all(x, hidden_state)
+                prediction = apply_to_list(prediction, lambda x: x[:, 0])  # select first time step
+                return prediction, hidden_state
+
+            # make predictions which are fed into next step
+            output = self.decode_autoregressive(
+                decode_one,
+                first_target=input_vector[:, 0, target_pos],
+                first_hidden_state=hidden_state,
+                target_scale=target_scale,
+                n_decoder_steps=input_vector.size(1),
             )
-            # run through same lstm
-            lstm_output, _ = self.lstm(packed_decoder, hidden_state)
-            # unpack sequence
-            lstm_output, _ = rnn.pad_packed_sequence(lstm_output, batch_first=True)
-            # transform into right shape
-            prediction = self.output_layer(lstm_output)
-
-        else:  # if not training, need to predict in autoregressive manner
-            # predict one by one
-            max_decoder_length = x["decoder_lengths"].max()
-            # initialize previous target and hidden state
-            last_target = last_encoder_target
-            last_hidden_state = hidden_state
-
-            predictions = []
-
-            # for each time step run prediction
-            for i in range(max_decoder_length):
-                current_input_vector = input_vector[:, i].unsqueeze(1)  # select time step in decoder
-                current_input_vector[:, 0, self.target_position] = last_target  # insert previous target
-
-                # make lstm prediction
-                lstm_prediction, new_hidden_state = self.lstm(current_input_vector, last_hidden_state)
-                prediction = self.output_layer(lstm_prediction).squeeze(1)
-
-                # save prediction
-                predictions.append(prediction)
-
-                # prepare for next time step
-                last_hidden_state = new_hidden_state
-
-                # Prediction should be passed through transformer and then inversely transformed.
-                # The inverse transformation might be only approximately the inverse of the
-                # forward transformation making this step important.
-                rescaled_prediction = self.transform_output(
-                    prediction=prediction, target_scale=x["target_scale"]
-                )  # inverse transform
-                normalized_prediction = self.output_transformer.transform(
-                    rescaled_prediction, target_scale=x["target_scale"]
-                )  # transform
-
-                last_target = normalized_prediction.squeeze(1)
-
-            # stack all predictions
-            prediction = torch.stack(predictions, dim=1)
-
-        return prediction
-
-    def forward(self, x: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
-        hidden_state = self.encode(x)  # encode to hidden state
-        prediction = self.decode(x, hidden_state)  # decode leveraging hidden state
-        return self.to_network_output(prediction=prediction)
+        return output
+
+    def forward(self, x: Dict[str, torch.Tensor], n_samples: int = None) -> Dict[str, torch.Tensor]:
+        """
+        Forward network
+        """
+        hidden_state = self.encode(x)
+        # decode
+        input_vector = self.construct_input_vector(
+            x["decoder_cat"],
+            x["decoder_cont"],
+            one_off_target=x["encoder_cont"][
+                torch.arange(x["encoder_cont"].size(0), device=x["encoder_cont"].device),
+                x["encoder_lengths"] - 1,
+                self.target_positions.unsqueeze(-1),
+            ].T.contiguous(),
+        )
+
+        output = self.decode(
+            input_vector,
+            decoder_lengths=x["decoder_lengths"],
+            target_scale=x["target_scale"],
+            hidden_state=hidden_state,
+        )
+        # return relevant part
+        return self.to_network_output(prediction=output)
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/deepar/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/deepar/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 """
 `DeepAR: Probabilistic forecasting with autoregressive recurrent networks
 <https://www.sciencedirect.com/science/article/pii/S0169207019301888>`_
 which is the one of the most popular forecasting algorithms and is often used as a baseline
 """
 from copy import copy, deepcopy
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
-import matplotlib.pyplot as plt
-from matplotlib.pyplot import plot_date
 import numpy as np
 import pandas as pd
-from pytorch_lightning.core.lightning import LightningModule
 import torch
-import torch.distributions as dists
 import torch.nn as nn
-from torch.nn.utils import rnn
 from torch.utils.data.dataloader import DataLoader
 
 from pytorch_forecasting.data.encoders import EncoderNormalizer, MultiNormalizer, NaNLabelEncoder
 from pytorch_forecasting.data.timeseries import TimeSeriesDataSet
 from pytorch_forecasting.metrics import (
     MAE,
     MAPE,
     MASE,
     RMSE,
     SMAPE,
     DistributionLoss,
     Metric,
     MultiLoss,
+    MultivariateDistributionLoss,
     NormalDistributionLoss,
 )
-from pytorch_forecasting.models.base_model import AutoRegressiveBaseModelWithCovariates
+from pytorch_forecasting.models.base_model import AutoRegressiveBaseModelWithCovariates, Prediction
 from pytorch_forecasting.models.nn import HiddenState, MultiEmbedding, get_rnn
 from pytorch_forecasting.utils import apply_to_list, to_list
 
 
 class DeepAR(AutoRegressiveBaseModelWithCovariates):
     def __init__(
         self,
@@ -64,14 +60,18 @@
     ):
         """
         DeepAR Network.
 
         The code is based on the article `DeepAR: Probabilistic forecasting with autoregressive recurrent networks
         <https://www.sciencedirect.com/science/article/pii/S0169207019301888>`_.
 
+        By using a Multivariate Loss such as the
+        :py:class:`~pytorch_forecasting.metrics.MultivariateNormalDistributionLoss`,
+        the network is converted into a `DeepVAR network <http://arxiv.org/abs/1910.03002>`_.
+
         Args:
             cell_type (str, optional): Recurrent cell type ["LSTM", "GRU"]. Defaults to "LSTM".
             hidden_size (int, optional): hidden recurrent size - the most important hyperparameter along with
                 ``rnn_layers``. Defaults to 10.
             rnn_layers (int, optional): Number of RNN layers - important hyperparameter. Defaults to 2.
             dropout (float, optional): Dropout in RNN layers. Defaults to 0.1.
             static_categoricals: integer of positions of static categorical variables
@@ -125,26 +125,26 @@
             categorical_groups=categorical_groups,
             x_categoricals=x_categoricals,
         )
 
         lagged_target_names = [l for lags in target_lags.values() for l in lags]
         assert set(self.encoder_variables) - set(to_list(target)) - set(lagged_target_names) == set(
             self.decoder_variables
-        ), "Encoder and decoder variables have to be the same apart from target variable"
+        ) - set(lagged_target_names), "Encoder and decoder variables have to be the same apart from target variable"
         for targeti in to_list(target):
             assert (
                 targeti in time_varying_reals_encoder
             ), f"target {targeti} has to be real"  # todo: remove this restriction
         assert (isinstance(target, str) and isinstance(loss, DistributionLoss)) or (
             isinstance(target, (list, tuple)) and isinstance(loss, MultiLoss) and len(loss) == len(target)
         ), "number of targets should be equivalent to number of loss metrics"
 
         rnn_class = get_rnn(cell_type)
         cont_size = len(self.reals)
-        cat_size = sum([size[1] for size in self.hparams.embedding_sizes.values()])
+        cat_size = sum(self.embeddings.output_size.values())
         input_size = cont_size + cat_size
         self.rnn = rnn_class(
             input_size=input_size,
             hidden_size=self.hparams.hidden_size,
             num_layers=self.hparams.rnn_layers,
             dropout=self.hparams.dropout if self.hparams.rnn_layers > 1 else 0,
             batch_first=True,
@@ -180,14 +180,18 @@
         if dataset.multi_target:
             new_kwargs.setdefault("loss", MultiLoss([NormalDistributionLoss()] * len(dataset.target_names)))
         new_kwargs.update(kwargs)
         assert not isinstance(dataset.target_normalizer, NaNLabelEncoder) and (
             not isinstance(dataset.target_normalizer, MultiNormalizer)
             or all([not isinstance(normalizer, NaNLabelEncoder) for normalizer in dataset.target_normalizer])
         ), "target(s) should be continuous - categorical targets are not supported"  # todo: remove this restriction
+        if isinstance(new_kwargs.get("loss", None), MultivariateDistributionLoss):
+            assert (
+                dataset.min_prediction_length == dataset.max_prediction_length
+            ), "Multivariate models require constant prediction lenghts"
         return super().from_dataset(
             dataset, allowed_encoder_known_variable_names=allowed_encoder_known_variable_names, **new_kwargs
         )
 
     def construct_input_vector(
         self, x_cat: torch.Tensor, x_cont: torch.Tensor, one_off_target: torch.Tensor = None
     ) -> torch.Tensor:
@@ -291,14 +295,15 @@
             # make predictions which are fed into next step
             output = self.decode_autoregressive(
                 decode_one,
                 first_target=input_vector[:, 0, target_pos],
                 first_hidden_state=hidden_state,
                 target_scale=target_scale,
                 n_decoder_steps=input_vector.size(1),
+                n_samples=n_samples,
             )
             # reshape predictions for n_samples:
             # from n_samples * batch_size x time steps to batch_size x time steps x n_samples
             output = apply_to_list(output, lambda x: x.reshape(-1, n_samples, input_vector.size(1)).permute(0, 2, 1))
         return output
 
     def forward(self, x: Dict[str, torch.Tensor], n_samples: int = None) -> Dict[str, torch.Tensor]:
@@ -310,15 +315,15 @@
         input_vector = self.construct_input_vector(
             x["decoder_cat"],
             x["decoder_cont"],
             one_off_target=x["encoder_cont"][
                 torch.arange(x["encoder_cont"].size(0), device=x["encoder_cont"].device),
                 x["encoder_lengths"] - 1,
                 self.target_positions.unsqueeze(-1),
-            ].T,
+            ].T.contiguous(),
         )
 
         if self.training:
             assert n_samples is None, "cannot sample from decoder when training"
         output = self.decode(
             input_vector,
             decoder_lengths=x["decoder_lengths"],
@@ -337,43 +342,32 @@
             out,
             batch_idx,
             prediction_kwargs=dict(n_samples=n_samples),
             quantiles_kwargs=dict(n_samples=n_samples),
         )
         return log
 
-    def plot_prediction(
-        self,
-        x: Dict[str, torch.Tensor],
-        out: Dict[str, torch.Tensor],
-        idx: int,
-        add_loss_to_title: Union[Metric, torch.Tensor, bool] = False,
-        show_future_observed: bool = True,
-        ax=None,
-        **kwargs,
-    ) -> plt.Figure:
-        # workaround for not being able to compute loss for single sample without parameters of distribution
-        return super().plot_prediction(
-            x, out, idx=idx, add_loss_to_title=False, show_future_observed=show_future_observed, ax=ax, **kwargs
-        )
-
     def predict(
         self,
         data: Union[DataLoader, pd.DataFrame, TimeSeriesDataSet],
         mode: Union[str, Tuple[str, str]] = "prediction",
         return_index: bool = False,
         return_decoder_lengths: bool = False,
         batch_size: int = 64,
         num_workers: int = 0,
         fast_dev_run: bool = False,
-        show_progress_bar: bool = False,
         return_x: bool = False,
+        return_y: bool = False,
         mode_kwargs: Dict[str, Any] = None,
+        trainer_kwargs: Optional[Dict[str, Any]] = None,
+        write_interval: Literal["batch", "epoch", "batch_and_epoch"] = "batch",
+        output_dir: Optional[str] = None,
         n_samples: int = 100,
-    ):
+        **kwargs,
+    ) -> Prediction:
         """
         predict dataloader
 
         Args:
             dataloader: dataloader, dataframe or dataset
             mode: one of "prediction", "quantiles", "samples" or "raw", or tuple ``("raw", output_name)`` where
                 output_name is a name in the dictionary returned by ``forward()``
@@ -382,21 +376,25 @@
                 of the first prediction)
             return_decoder_lengths: if to return decoder_lengths (in the same order as the output
             batch_size: batch size for dataloader - only used if data is not a dataloader is passed
             num_workers: number of workers for dataloader - only used if data is not a dataloader is passed
             fast_dev_run: if to only return results of first batch
             show_progress_bar: if to show progress bar. Defaults to False.
             return_x: if to return network inputs (in the same order as prediction output)
+            return_y: if to return network targets (in the same order as prediction output)
             mode_kwargs (Dict[str, Any]): keyword arguments for ``to_prediction()`` or ``to_quantiles()``
                 for modes "prediction" and "quantiles"
+            trainer_kwargs (Dict[str, Any], optional): keyword arguments for the trainer
+            write_interval: interval to write predictions to disk
+            output_dir: directory to write predictions to. Defaults to None. If set function will return empty list
             n_samples: number of samples to draw. Defaults to 100.
 
         Returns:
-            output, x, index, decoder_lengths: some elements might not be present depending on what is configured
-                to be returned
+            Prediction: if one of the ```return`` arguments is present,
+                prediction tuple with fields ``prediction``, ``x``, ``y``, ``index`` and ``decoder_lengths``
         """
         if isinstance(mode, str):
             if mode in ["prediction", "quantiles"]:
                 if mode_kwargs is None:
                     mode_kwargs = dict(use_metric=False)
                 else:
                     mode_kwargs = deepcopy(mode_kwargs)
@@ -406,13 +404,17 @@
         return super().predict(
             data=data,
             mode=mode,
             return_decoder_lengths=return_decoder_lengths,
             return_index=return_index,
             n_samples=n_samples,  # new keyword that is passed to forward function
             return_x=return_x,
-            show_progress_bar=show_progress_bar,
             fast_dev_run=fast_dev_run,
             num_workers=num_workers,
             batch_size=batch_size,
             mode_kwargs=mode_kwargs,
+            trainer_kwargs=trainer_kwargs,
+            write_interval=write_interval,
+            output_dir=output_dir,
+            return_y=return_y,
+            **kwargs,
         )
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/mlp/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/mlp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         # define network
         if isinstance(self.hparams.output_size, int):
             mlp_output_size = self.hparams.output_size
         else:
             mlp_output_size = sum(self.hparams.output_size)
 
         cont_size = len(self.decoder_reals_positions)
-        cat_size = sum([emb.embedding_dim for emb in self.input_embeddings.values()])
+        cat_size = sum(self.input_embeddings.output_size.values())
         input_size = cont_size + cat_size
 
         self.mlp = FullyConnectedModule(
             dropout=dropout,
             norm=self.hparams.norm,
             activation_class=getattr(nn, self.hparams.activation_class),
             input_size=input_size,
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/mlp/submodules.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/mlp/submodules.py`

 * *Files identical despite different names*

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/nbeats/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/nbeats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         `N-BEATS: Neural basis expansion analysis for interpretable time series
         forecasting <http://arxiv.org/abs/1905.10437>`_. The network has (if used as ensemble) outperformed all
         other methods
         including ensembles of traditional statical methods in the M4 competition. The M4 competition is arguably
         the most
         important benchmark for univariate time series forecasting.
 
+        The :py:class:`~pytorch_forecasting.models.nhits.NHiTS` network has recently shown to consistently outperform
+        N-BEATS.
+
         Args:
             stack_types: One of the following values: “generic”, “seasonality" or “trend". A list of strings
                 of length 1 or ‘num_stacks’. Default and recommended value
                 for generic mode: [“generic”] Recommended value for interpretable mode: [“trend”,”seasonality”]
             num_blocks: The number of blocks per stack. A list of ints of length 1 or ‘num_stacks’.
                 Default and recommended value for generic mode: [1] Recommended value for interpretable mode: [3]
             num_block_layers: Number of fully connected layers with ReLu activation per block. A list of ints of length
@@ -220,28 +223,40 @@
 
     def step(self, x, y, batch_idx) -> Dict[str, torch.Tensor]:
         """
         Take training / validation step.
         """
         log, out = super().step(x, y, batch_idx=batch_idx)
 
-        if self.hparams.backcast_loss_ratio > 0:  # add loss from backcast
+        if self.hparams.backcast_loss_ratio > 0 and not self.predicting:  # add loss from backcast
             backcast = out["backcast"]
             backcast_weight = (
                 self.hparams.backcast_loss_ratio * self.hparams.prediction_length / self.hparams.context_length
             )
             backcast_weight = backcast_weight / (backcast_weight + 1)  # normalize
             forecast_weight = 1 - backcast_weight
             if isinstance(self.loss, MASE):
                 backcast_loss = self.loss(backcast, x["encoder_target"], x["decoder_target"]) * backcast_weight
             else:
                 backcast_loss = self.loss(backcast, x["encoder_target"]) * backcast_weight
             label = ["val", "train"][self.training]
-            self.log(f"{label}_backcast_loss", backcast_loss, on_epoch=True, on_step=self.training)
-            self.log(f"{label}_forecast_loss", log["loss"], on_epoch=True, on_step=self.training)
+            self.log(
+                f"{label}_backcast_loss",
+                backcast_loss,
+                on_epoch=True,
+                on_step=self.training,
+                batch_size=len(x["decoder_target"]),
+            )
+            self.log(
+                f"{label}_forecast_loss",
+                log["loss"],
+                on_epoch=True,
+                on_step=self.training,
+                batch_size=len(x["decoder_target"]),
+            )
             log["loss"] = log["loss"] * forecast_weight + backcast_loss
 
         self.log_interpretation(x, out, batch_idx=batch_idx)
         return log, out
 
     def log_interpretation(self, x, out, batch_idx):
         """
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/nbeats/sub_modules.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/nbeats/sub_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,18 +147,18 @@
             share_thetas=True,
             dropout=dropout,
         )
 
         backcast_linspace, forecast_linspace = linspace(backcast_length, forecast_length, centered=True)
         norm = np.sqrt(forecast_length / thetas_dim)  # ensure range of predictions is comparable to input
 
-        coefficients = torch.tensor([backcast_linspace ** i for i in range(thetas_dim)], dtype=torch.float32)
+        coefficients = torch.tensor([backcast_linspace**i for i in range(thetas_dim)], dtype=torch.float32)
         self.register_buffer("T_backcast", coefficients * norm)
 
-        coefficients = torch.tensor([forecast_linspace ** i for i in range(thetas_dim)], dtype=torch.float32)
+        coefficients = torch.tensor([forecast_linspace**i for i in range(thetas_dim)], dtype=torch.float32)
         self.register_buffer("T_forecast", coefficients * norm)
 
     def forward(self, x) -> Tuple[torch.Tensor, torch.Tensor]:
         x = super().forward(x)
         backcast = self.theta_b_fc(x).mm(self.T_backcast)
         forecast = self.theta_f_fc(x).mm(self.T_forecast)
         return backcast, forecast
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/nn/rnn.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/nn/rnn.py`

 * *Files identical despite different names*

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/temporal_fusion_transformer/__init__.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/temporal_fusion_transformer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     AddNorm,
     GateAddNorm,
     GatedLinearUnit,
     GatedResidualNetwork,
     InterpretableMultiHeadAttention,
     VariableSelectionNetwork,
 )
-from pytorch_forecasting.utils import autocorrelation, create_mask, detach, integer_histogram, padded_stack, to_list
+from pytorch_forecasting.utils import create_mask, detach, integer_histogram, masked_op, padded_stack, to_list
 
 
 class TemporalFusionTransformer(BaseModelWithCovariates):
     def __init__(
         self,
         hidden_size: int = 16,
         lstm_layers: int = 1,
@@ -53,14 +53,15 @@
         learning_rate: float = 1e-3,
         log_interval: Union[int, float] = -1,
         log_val_interval: Union[int, float] = None,
         log_gradient_flow: bool = False,
         reduce_on_plateau_patience: int = 1000,
         monotone_constaints: Dict[str, int] = {},
         share_single_variable_networks: bool = False,
+        causal_attention: bool = True,
         logging_metrics: nn.ModuleList = None,
         **kwargs,
     ):
         """
         Temporal Fusion Transformer for forecasting timeseries - use its :py:meth:`~from_dataset` method if possible.
 
         Implementation of the article
@@ -122,14 +123,16 @@
             monotone_constaints (Dict[str, int]): dictionary of monotonicity constraints for continuous decoder
                 variables mapping
                 position (e.g. ``"0"`` for first position) to constraint (``-1`` for negative and ``+1`` for positive,
                 larger numbers add more weight to the constraint vs. the loss but are usually not necessary).
                 This constraint significantly slows down training. Defaults to {}.
             share_single_variable_networks (bool): if to share the single variable networks between the encoder and
                 decoder. Defaults to False.
+            causal_attention (bool): If to attend only at previous timesteps in the decoder or also include future
+                predictions. Defaults to True.
             logging_metrics (nn.ModuleList[LightningMetric]): list of metrics that are logged during training.
                 Defaults to nn.ModuleList([SMAPE(), MAE(), RMSE(), MAPE()]).
             **kwargs: additional arguments to :py:class:`~BaseModel`.
         """
         if logging_metrics is None:
             logging_metrics = nn.ModuleList([SMAPE(), MAE(), RMSE(), MAPE()])
         if loss is None:
@@ -155,15 +158,17 @@
                 name: nn.Linear(1, self.hparams.hidden_continuous_sizes.get(name, self.hparams.hidden_continuous_size))
                 for name in self.reals
             }
         )
 
         # variable selection
         # variable selection for static variables
-        static_input_sizes = {name: self.hparams.embedding_sizes[name][1] for name in self.hparams.static_categoricals}
+        static_input_sizes = {
+            name: self.input_embeddings.output_size[name] for name in self.hparams.static_categoricals
+        }
         static_input_sizes.update(
             {
                 name: self.hparams.hidden_continuous_sizes.get(name, self.hparams.hidden_continuous_size)
                 for name in self.hparams.static_reals
             }
         )
         self.static_variable_selection = VariableSelectionNetwork(
@@ -172,25 +177,25 @@
             input_embedding_flags={name: True for name in self.hparams.static_categoricals},
             dropout=self.hparams.dropout,
             prescalers=self.prescalers,
         )
 
         # variable selection for encoder and decoder
         encoder_input_sizes = {
-            name: self.hparams.embedding_sizes[name][1] for name in self.hparams.time_varying_categoricals_encoder
+            name: self.input_embeddings.output_size[name] for name in self.hparams.time_varying_categoricals_encoder
         }
         encoder_input_sizes.update(
             {
                 name: self.hparams.hidden_continuous_sizes.get(name, self.hparams.hidden_continuous_size)
                 for name in self.hparams.time_varying_reals_encoder
             }
         )
 
         decoder_input_sizes = {
-            name: self.hparams.embedding_sizes[name][1] for name in self.hparams.time_varying_categoricals_decoder
+            name: self.input_embeddings.output_size[name] for name in self.hparams.time_varying_categoricals_decoder
         }
         decoder_input_sizes.update(
             {
                 name: self.hparams.hidden_continuous_sizes.get(name, self.hparams.hidden_continuous_size)
                 for name in self.hparams.time_varying_reals_decoder
             }
         )
@@ -354,40 +359,41 @@
 
     def expand_static_context(self, context, timesteps):
         """
         add time dimension to static context
         """
         return context[:, None].expand(-1, timesteps, -1)
 
-    def get_attention_mask(self, encoder_lengths: torch.LongTensor, decoder_length: int):
+    def get_attention_mask(self, encoder_lengths: torch.LongTensor, decoder_lengths: torch.LongTensor):
         """
         Returns causal mask to apply for self-attention layer.
-
-        Args:
-            self_attn_inputs: Inputs to self attention layer to determine mask shape
         """
-        # indices to which is attended
-        attend_step = torch.arange(decoder_length, device=self.device)
-        # indices for which is predicted
-        predict_step = torch.arange(0, decoder_length, device=self.device)[:, None]
-        # do not attend to steps to self or after prediction
-        # todo: there is potential value in attending to future forecasts if they are made with knowledge currently
-        #   available
-        #   one possibility is here to use a second attention layer for future attention (assuming different effects
-        #   matter in the future than the past)
-        #   or alternatively using the same layer but allowing forward attention - i.e. only masking out non-available
-        #   data and self
-        decoder_mask = attend_step >= predict_step
+        decoder_length = decoder_lengths.max()
+        if self.hparams.causal_attention:
+            # indices to which is attended
+            attend_step = torch.arange(decoder_length, device=self.device)
+            # indices for which is predicted
+            predict_step = torch.arange(0, decoder_length, device=self.device)[:, None]
+            # do not attend to steps to self or after prediction
+            decoder_mask = (attend_step >= predict_step).unsqueeze(0).expand(encoder_lengths.size(0), -1, -1)
+        else:
+            # there is value in attending to future forecasts if they are made with knowledge currently
+            #   available
+            #   one possibility is here to use a second attention layer for future attention (assuming different effects
+            #   matter in the future than the past)
+            #   or alternatively using the same layer but allowing forward attention - i.e. only
+            #   masking out non-available data and self
+            decoder_mask = create_mask(decoder_length, decoder_lengths).unsqueeze(1).expand(-1, decoder_length, -1)
         # do not attend to steps where data is padded
-        encoder_mask = create_mask(encoder_lengths.max(), encoder_lengths)
+        encoder_mask = create_mask(encoder_lengths.max(), encoder_lengths).unsqueeze(1).expand(-1, decoder_length, -1)
         # combine masks along attended time - first encoder and then decoder
         mask = torch.cat(
             (
-                encoder_mask.unsqueeze(1).expand(-1, decoder_length, -1),
-                decoder_mask.unsqueeze(0).expand(encoder_lengths.size(0), -1, -1),
+                encoder_mask,
+                decoder_mask,
             ),
             dim=2,
         )
         return mask
 
     def forward(self, x: Dict[str, torch.Tensor]) -> Dict[str, torch.Tensor]:
         """
@@ -475,17 +481,15 @@
         )
 
         # Attention
         attn_output, attn_output_weights = self.multihead_attn(
             q=attn_input[:, max_encoder_length:],  # query only for predictions
             k=attn_input,
             v=attn_input,
-            mask=self.get_attention_mask(
-                encoder_lengths=encoder_lengths, decoder_length=timesteps - max_encoder_length
-            ),
+            mask=self.get_attention_mask(encoder_lengths=encoder_lengths, decoder_lengths=decoder_lengths),
         )
 
         # skip connection over attention
         attn_output = self.post_attn_gate_norm(attn_output, attn_input[:, max_encoder_length:])
 
         output = self.pos_wise_ff(attn_output)
 
@@ -495,15 +499,16 @@
         if self.n_targets > 1:  # if to use multi-target architecture
             output = [output_layer(output) for output_layer in self.output_layer]
         else:
             output = self.output_layer(output)
 
         return self.to_network_output(
             prediction=self.transform_output(output, target_scale=x["target_scale"]),
-            attention=attn_output_weights,
+            encoder_attention=attn_output_weights[..., :max_encoder_length],
+            decoder_attention=attn_output_weights[..., max_encoder_length:],
             static_variables=static_variable_selection,
             encoder_variables=encoder_sparse_weights,
             decoder_variables=decoder_sparse_weights,
             decoder_lengths=decoder_lengths,
             encoder_lengths=encoder_lengths,
         )
 
@@ -522,115 +527,155 @@
         interpretation = self.interpret_output(
             detach(out),
             reduction="sum",
             attention_prediction_horizon=0,  # attention only for first prediction horizon
         )
         return interpretation
 
-    def epoch_end(self, outputs):
+    def on_epoch_end(self, outputs):
         """
         run at epoch end for training or validation
         """
-        if self.log_interval > 0:
+        if self.log_interval > 0 and not self.training:
             self.log_interpretation(outputs)
 
     def interpret_output(
         self,
         out: Dict[str, torch.Tensor],
         reduction: str = "none",
         attention_prediction_horizon: int = 0,
-        attention_as_autocorrelation: bool = False,
     ) -> Dict[str, torch.Tensor]:
         """
         interpret output of model
 
         Args:
             out: output as produced by ``forward()``
             reduction: "none" for no averaging over batches, "sum" for summing attentions, "mean" for
                 normalizing by encode lengths
             attention_prediction_horizon: which prediction horizon to use for attention
-            attention_as_autocorrelation: if to record attention as autocorrelation - this should be set to true in
-                case of ``reduction != "none"`` and differing prediction times of the samples. Defaults to False
 
         Returns:
             interpretations that can be plotted with ``plot_interpretation()``
         """
+        # take attention and concatenate if a list to proper attention object
+        batch_size = len(out["decoder_attention"])
+        if isinstance(out["decoder_attention"], (list, tuple)):
+            # start with decoder attention
+            # assume issue is in last dimension, we need to find max
+            max_last_dimension = max(x.size(-1) for x in out["decoder_attention"])
+            first_elm = out["decoder_attention"][0]
+            # create new attention tensor into which we will scatter
+            decoder_attention = torch.full(
+                (batch_size, *first_elm.shape[:-1], max_last_dimension),
+                float("nan"),
+                dtype=first_elm.dtype,
+                device=first_elm.device,
+            )
+            # scatter into tensor
+            for idx, x in enumerate(out["decoder_attention"]):
+                decoder_length = out["decoder_lengths"][idx]
+                decoder_attention[idx, :, :, :decoder_length] = x[..., :decoder_length]
+        else:
+            decoder_attention = out["decoder_attention"].clone()
+            decoder_mask = create_mask(out["decoder_attention"].size(1), out["decoder_lengths"])
+            decoder_attention[decoder_mask[..., None, None].expand_as(decoder_attention)] = float("nan")
+
+        if isinstance(out["encoder_attention"], (list, tuple)):
+            # same game for encoder attention
+            # create new attention tensor into which we will scatter
+            first_elm = out["encoder_attention"][0]
+            encoder_attention = torch.full(
+                (batch_size, *first_elm.shape[:-1], self.hparams.max_encoder_length),
+                float("nan"),
+                dtype=first_elm.dtype,
+                device=first_elm.device,
+            )
+            # scatter into tensor
+            for idx, x in enumerate(out["encoder_attention"]):
+                encoder_length = out["encoder_lengths"][idx]
+                encoder_attention[idx, :, :, self.hparams.max_encoder_length - encoder_length :] = x[
+                    ..., :encoder_length
+                ]
+        else:
+            # roll encoder attention (so start last encoder value is on the right)
+            encoder_attention = out["encoder_attention"].clone()
+            shifts = encoder_attention.size(3) - out["encoder_lengths"]
+            new_index = (
+                torch.arange(encoder_attention.size(3), device=encoder_attention.device)[None, None, None].expand_as(
+                    encoder_attention
+                )
+                - shifts[:, None, None, None]
+            ) % encoder_attention.size(3)
+            encoder_attention = torch.gather(encoder_attention, dim=3, index=new_index)
+            # expand encoder_attentiont to full size
+            if encoder_attention.size(-1) < self.hparams.max_encoder_length:
+                encoder_attention = torch.concat(
+                    [
+                        torch.full(
+                            (
+                                *encoder_attention.shape[:-1],
+                                self.hparams.max_encoder_length - out["encoder_lengths"].max(),
+                            ),
+                            float("nan"),
+                            dtype=encoder_attention.dtype,
+                            device=encoder_attention.device,
+                        ),
+                        encoder_attention,
+                    ],
+                    dim=-1,
+                )
+
+        # combine attention vector
+        attention = torch.concat([encoder_attention, decoder_attention], dim=-1)
+        attention[attention < 1e-5] = float("nan")
 
         # histogram of decode and encode lengths
         encoder_length_histogram = integer_histogram(out["encoder_lengths"], min=0, max=self.hparams.max_encoder_length)
         decoder_length_histogram = integer_histogram(
             out["decoder_lengths"], min=1, max=out["decoder_variables"].size(1)
         )
 
         # mask where decoder and encoder where not applied when averaging variable selection weights
-        encoder_variables = out["encoder_variables"].squeeze(-2)
+        encoder_variables = out["encoder_variables"].squeeze(-2).clone()
         encode_mask = create_mask(encoder_variables.size(1), out["encoder_lengths"])
         encoder_variables = encoder_variables.masked_fill(encode_mask.unsqueeze(-1), 0.0).sum(dim=1)
         encoder_variables /= (
             out["encoder_lengths"]
             .where(out["encoder_lengths"] > 0, torch.ones_like(out["encoder_lengths"]))
             .unsqueeze(-1)
         )
 
-        decoder_variables = out["decoder_variables"].squeeze(-2)
+        decoder_variables = out["decoder_variables"].squeeze(-2).clone()
         decode_mask = create_mask(decoder_variables.size(1), out["decoder_lengths"])
         decoder_variables = decoder_variables.masked_fill(decode_mask.unsqueeze(-1), 0.0).sum(dim=1)
         decoder_variables /= out["decoder_lengths"].unsqueeze(-1)
 
         # static variables need no masking
         static_variables = out["static_variables"].squeeze(1)
         # attention is batch x time x heads x time_to_attend
         # average over heads + only keep prediction attention and attention on observed timesteps
-        attention = out["attention"][
-            :, attention_prediction_horizon, :, : out["encoder_lengths"].max() + attention_prediction_horizon
-        ].mean(1)
+        attention = masked_op(
+            attention[
+                :, attention_prediction_horizon, :, : self.hparams.max_encoder_length + attention_prediction_horizon
+            ],
+            op="mean",
+            dim=1,
+        )
 
         if reduction != "none":  # if to average over batches
             static_variables = static_variables.sum(dim=0)
             encoder_variables = encoder_variables.sum(dim=0)
             decoder_variables = decoder_variables.sum(dim=0)
 
-            # reorder attention or averaging
-            for i in range(len(attention)):  # very inefficient but does the trick
-                if 0 < out["encoder_lengths"][i] < attention.size(1) - attention_prediction_horizon - 1:
-                    relevant_attention = attention[
-                        i, : out["encoder_lengths"][i] + attention_prediction_horizon
-                    ].clone()
-                    if attention_as_autocorrelation:
-                        relevant_attention = autocorrelation(relevant_attention)
-                    attention[i, -out["encoder_lengths"][i] - attention_prediction_horizon :] = relevant_attention
-                    attention[i, : attention.size(1) - out["encoder_lengths"][i] - attention_prediction_horizon] = 0.0
-                elif attention_as_autocorrelation:
-                    attention[i] = autocorrelation(attention[i])
-
-            attention = attention.sum(dim=0)
-            if reduction == "mean":
-                attention = attention / encoder_length_histogram[1:].flip(0).cumsum(0).clamp(1)
-                attention = attention / attention.sum(-1).unsqueeze(-1)  # renormalize
-            elif reduction == "sum":
-                pass
-            else:
-                raise ValueError(f"Unknown reduction {reduction}")
-
-            attention = torch.zeros(
-                self.hparams.max_encoder_length + attention_prediction_horizon, device=self.device
-            ).scatter(
-                dim=0,
-                index=torch.arange(
-                    self.hparams.max_encoder_length + attention_prediction_horizon - attention.size(-1),
-                    self.hparams.max_encoder_length + attention_prediction_horizon,
-                    device=self.device,
-                ),
-                src=attention,
-            )
+            attention = masked_op(attention, dim=0, op=reduction)
         else:
-            attention = attention / attention.sum(-1).unsqueeze(-1)  # renormalize
+            attention = attention / masked_op(attention, dim=1, op="sum").unsqueeze(-1)  # renormalize
 
         interpretation = dict(
-            attention=attention,
+            attention=attention.masked_fill(torch.isnan(attention), 0.0),
             static_variables=static_variables,
             encoder_variables=encoder_variables,
             decoder_variables=decoder_variables,
             encoder_length_histogram=encoder_length_histogram,
             decoder_length_histogram=decoder_length_histogram,
         )
         return interpretation
@@ -671,23 +716,23 @@
             show_future_observed=show_future_observed,
             ax=ax,
             **kwargs,
         )
 
         # add attention on secondary axis
         if plot_attention:
-            interpretation = self.interpret_output(out)
+            interpretation = self.interpret_output(out.iget(slice(idx, idx + 1)))
             for f in to_list(fig):
                 ax = f.axes[0]
                 ax2 = ax.twinx()
                 ax2.set_ylabel("Attention")
-                encoder_length = x["encoder_lengths"][idx]
+                encoder_length = x["encoder_lengths"][0]
                 ax2.plot(
                     torch.arange(-encoder_length, 0),
-                    interpretation["attention"][idx, :encoder_length].detach().cpu(),
+                    interpretation["attention"][0, -encoder_length:].detach().cpu(),
                     alpha=0.2,
                     color="k",
                 )
                 f.tight_layout()
         return fig
 
     def plot_interpretation(self, interpretation: Dict[str, torch.Tensor]) -> Dict[str, plt.Figure]:
@@ -748,15 +793,15 @@
         interpretation = {
             # use padded_stack because decoder length histogram can be of different length
             name: padded_stack([x["interpretation"][name].detach() for x in outputs], side="right", value=0).sum(0)
             for name in outputs[0]["interpretation"].keys()
         }
         # normalize attention with length histogram squared to account for: 1. zeros in attention and
         # 2. higher attention due to less values
-        attention_occurances = interpretation["encoder_length_histogram"][1:].flip(0).cumsum(0).float()
+        attention_occurances = interpretation["encoder_length_histogram"][1:].flip(0).float().cumsum(0)
         attention_occurances = attention_occurances / attention_occurances.max()
         attention_occurances = torch.cat(
             [
                 attention_occurances,
                 torch.ones(
                     interpretation["attention"].size(0) - attention_occurances.size(0),
                     dtype=attention_occurances.dtype,
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/temporal_fusion_transformer/sub_modules.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/temporal_fusion_transformer/sub_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 class TimeDistributed(nn.Module):
     def __init__(self, module: nn.Module, batch_first: bool = False):
         super().__init__()
         self.module = module
         self.batch_first = batch_first
 
     def forward(self, x):
-
         if len(x.size()) <= 2:
             return self.module(x)
 
         # Squash samples and timesteps into a single axis
         x_reshape = x.contiguous().view(-1, x.size(-1))  # (samples * timesteps, input_size)
 
         y = self.module(x_reshape)
@@ -46,15 +45,14 @@
     def interpolate(self, x):
         upsampled = F.interpolate(x.unsqueeze(1), self.output_size, mode="linear", align_corners=True).squeeze(1)
         if self.trainable:
             upsampled = upsampled * self.gate(self.mask.unsqueeze(0)) * 2.0
         return upsampled
 
     def forward(self, x):
-
         if len(x.size()) <= 2:
             return self.interpolate(x)
 
         # Squash samples and timesteps into a single axis
         x_reshape = x.contiguous().view(-1, x.size(-1))  # (samples * timesteps, input_size)
 
         y = self.interpolate(x_reshape)
@@ -382,15 +380,15 @@
         self.softmax = nn.Softmax(dim=2)
         self.scale = scale
 
     def forward(self, q, k, v, mask=None):
         attn = torch.bmm(q, k.permute(0, 2, 1))  # query-key overlap
 
         if self.scale:
-            dimension = torch.sqrt(torch.tensor(k.shape[-1]).to(torch.float32))
+            dimension = torch.as_tensor(k.size(-1), dtype=attn.dtype, device=attn.device).sqrt()
             attn = attn / dimension
 
         if mask is not None:
             attn = attn.masked_fill(mask, -1e9)
         attn = self.softmax(attn)
 
         if self.dropout is not None:
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/models/temporal_fusion_transformer/tuning.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/models/temporal_fusion_transformer/tuning.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,47 +2,41 @@
 Hyperparameters can be efficiently tuned with `optuna <https://optuna.readthedocs.io/>`_.
 """
 import copy
 import logging
 import os
 from typing import Any, Dict, Tuple, Union
 
+import lightning.pytorch as pl
+from lightning.pytorch.callbacks import LearningRateMonitor, ModelCheckpoint
+from lightning.pytorch.loggers import TensorBoardLogger
+from lightning.pytorch.tuner import Tuner
 import numpy as np
 import optuna
-from optuna.integration import PyTorchLightningPruningCallback, TensorBoardCallback
+from optuna.integration import PyTorchLightningPruningCallback
 import optuna.logging
-import pytorch_lightning as pl
-from pytorch_lightning import Callback
-from pytorch_lightning.callbacks import LearningRateMonitor
-from pytorch_lightning.loggers import TensorBoardLogger
 import statsmodels.api as sm
 import torch
 from torch.utils.data import DataLoader
 
 from pytorch_forecasting import TemporalFusionTransformer
 from pytorch_forecasting.data import TimeSeriesDataSet
 from pytorch_forecasting.metrics import QuantileLoss
 
 optuna_logger = logging.getLogger("optuna")
 
 
-class MetricsCallback(Callback):
-    """PyTorch Lightning metric callback."""
-
-    def __init__(self):
-        super().__init__()
-        self.metrics = []
-
-    def on_validation_end(self, trainer, pl_module):
-        self.metrics.append(trainer.callback_metrics)
+# need to inherit from callback for this to work
+class PyTorchLightningPruningCallbackAdjusted(pl.Callback, PyTorchLightningPruningCallback):
+    pass
 
 
 def optimize_hyperparameters(
-    train_dataloader: DataLoader,
-    val_dataloader: DataLoader,
+    train_dataloaders: DataLoader,
+    val_dataloaders: DataLoader,
     model_path: str,
     max_epochs: int = 20,
     n_trials: int = 100,
     timeout: float = 3600 * 8.0,  # 8 hours
     gradient_clip_val_range: Tuple[float, float] = (0.01, 100.0),
     hidden_size_range: Tuple[int, int] = (16, 265),
     hidden_continuous_size_range: Tuple[int, int] = (8, 64),
@@ -60,16 +54,16 @@
     """
     Optimize Temporal Fusion Transformer hyperparameters.
 
     Run hyperparameter optimization. Learning rate for is determined with
     the PyTorch Lightning learning rate finder.
 
     Args:
-        train_dataloader (DataLoader): dataloader for training model
-        val_dataloader (DataLoader): dataloader for validating model
+        train_dataloaders (DataLoader): dataloader for training model
+        val_dataloaders (DataLoader): dataloader for validating model
         model_path (str): folder to which model checkpoints are saved
         max_epochs (int, optional): Maximum number of epochs to run training. Defaults to 20.
         n_trials (int, optional): Number of hyperparameter trials to run. Defaults to 100.
         timeout (float, optional): Time in seconds after which training is stopped regardless of number of epochs
             or validation metric. Defaults to 3600*8.0.
         hidden_size_range (Tuple[int, int], optional): Minimum and maximum of ``hidden_size`` hyperparameter. Defaults
             to (16, 265).
@@ -97,16 +91,16 @@
             Defaults to optuna.pruners.SuccessiveHalvingPruner().
 
         **kwargs: Additional arguments for the :py:class:`~TemporalFusionTransformer`.
 
     Returns:
         optuna.Study: optuna study results
     """
-    assert isinstance(train_dataloader.dataset, TimeSeriesDataSet) and isinstance(
-        val_dataloader.dataset, TimeSeriesDataSet
+    assert isinstance(train_dataloaders.dataset, TimeSeriesDataSet) and isinstance(
+        val_dataloaders.dataset, TimeSeriesDataSet
     ), "dataloaders must be built from timeseriesdataset"
 
     logging_level = {
         None: optuna.logging.get_verbosity(),
         0: optuna.logging.WARNING,
         1: optuna.logging.INFO,
         2: optuna.logging.DEBUG,
@@ -117,49 +111,44 @@
     loss = kwargs.get(
         "loss", QuantileLoss()
     )  # need a deepcopy of loss as it will otherwise propagate from one trial to the next
 
     # create objective function
     def objective(trial: optuna.Trial) -> float:
         # Filenames for each trial must be made unique in order to access each checkpoint.
-        checkpoint_callback = pl.callbacks.ModelCheckpoint(
+        checkpoint_callback = ModelCheckpoint(
             dirpath=os.path.join(model_path, "trial_{}".format(trial.number)), filename="{epoch}", monitor="val_loss"
         )
 
-        # The default logger in PyTorch Lightning writes to event files to be consumed by
-        # TensorBoard. We don't use any logger here as it requires us to implement several abstract
-        # methods. Instead we setup a simple callback, that saves metrics from each validation step.
-        metrics_callback = MetricsCallback()
         learning_rate_callback = LearningRateMonitor()
         logger = TensorBoardLogger(log_dir, name="optuna", version=trial.number)
         gradient_clip_val = trial.suggest_loguniform("gradient_clip_val", *gradient_clip_val_range)
         default_trainer_kwargs = dict(
-            gpus=[0] if torch.cuda.is_available() else None,
+            accelerator="auto",
             max_epochs=max_epochs,
             gradient_clip_val=gradient_clip_val,
             callbacks=[
-                metrics_callback,
                 learning_rate_callback,
                 checkpoint_callback,
-                PyTorchLightningPruningCallback(trial, monitor="val_loss"),
+                PyTorchLightningPruningCallbackAdjusted(trial, monitor="val_loss"),
             ],
             logger=logger,
-            progress_bar_refresh_rate=[0, 1][optuna_verbose < optuna.logging.INFO],
-            weights_summary=[None, "top"][optuna_verbose < optuna.logging.INFO],
+            enable_progress_bar=optuna_verbose < optuna.logging.INFO,
+            enable_model_summary=[False, True][optuna_verbose < optuna.logging.INFO],
         )
         default_trainer_kwargs.update(trainer_kwargs)
         trainer = pl.Trainer(
             **default_trainer_kwargs,
         )
 
         # create model
         hidden_size = trial.suggest_int("hidden_size", *hidden_size_range, log=True)
         kwargs["loss"] = copy.deepcopy(loss)
         model = TemporalFusionTransformer.from_dataset(
-            train_dataloader.dataset,
+            train_dataloaders.dataset,
             dropout=trial.suggest_uniform("dropout", *dropout_range),
             hidden_size=hidden_size,
             hidden_continuous_size=trial.suggest_int(
                 "hidden_continuous_size",
                 hidden_continuous_size_range[0],
                 min(hidden_continuous_size_range[1], hidden_size),
                 log=True,
@@ -168,23 +157,24 @@
             log_interval=-1,
             **kwargs,
         )
         # find good learning rate
         if use_learning_rate_finder:
             lr_trainer = pl.Trainer(
                 gradient_clip_val=gradient_clip_val,
-                gpus=[0] if torch.cuda.is_available() else None,
+                accelerator="auto",
                 logger=False,
-                progress_bar_refresh_rate=0,
-                weights_summary=None,
+                enable_progress_bar=False,
+                enable_model_summary=False,
             )
-            res = lr_trainer.tuner.lr_find(
+            tuner = Tuner(lr_trainer)
+            res = tuner.lr_find(
                 model,
-                train_dataloader=train_dataloader,
-                val_dataloaders=val_dataloader,
+                train_dataloaders=train_dataloaders,
+                val_dataloaders=val_dataloaders,
                 early_stop_threshold=10000,
                 min_lr=learning_rate_range[0],
                 num_training=100,
                 max_lr=learning_rate_range[1],
             )
 
             loss_finite = np.isfinite(res.results["loss"])
@@ -202,17 +192,17 @@
             optuna_logger.info(f"Using learning rate of {optimal_lr:.3g}")
             # add learning rate artificially
             model.hparams.learning_rate = trial.suggest_uniform("learning_rate", optimal_lr, optimal_lr)
         else:
             model.hparams.learning_rate = trial.suggest_loguniform("learning_rate", *learning_rate_range)
 
         # fit
-        trainer.fit(model, train_dataloader=train_dataloader, val_dataloaders=val_dataloader)
+        trainer.fit(model, train_dataloaders=train_dataloaders, val_dataloaders=val_dataloaders)
 
         # report result
-        return metrics_callback.metrics[-1]["val_loss"].item()
+        return trainer.callback_metrics["val_loss"].item()
 
     # setup optuna and run
     if study is None:
         study = optuna.create_study(direction="minimize", pruner=pruner)
     study.optimize(objective, n_trials=n_trials, timeout=timeout)
     return study
```

### Comparing `pytorch_forecasting-0.9.2/pytorch_forecasting/utils.py` & `pytorch_forecasting-1.0.0/pytorch_forecasting/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 Helper functions for PyTorch forecasting
 """
+from collections import namedtuple
 from contextlib import redirect_stdout
+import inspect
 import os
 from typing import Any, Callable, Dict, List, Tuple, Union
 
+import lightning.pytorch as pl
 import torch
+from torch import nn
 from torch.fft import irfft, rfft
 import torch.nn.functional as F
 from torch.nn.utils import rnn
 
 
 def integer_histogram(
     data: torch.LongTensor, min: Union[None, int] = None, max: Union[None, int] = None
@@ -105,15 +109,15 @@
         n (int): number of classes
         max_size (int, optional): maximum embedding size. Defaults to 100.
 
     Returns:
         int: embedding size
     """
     if n > 2:
-        return min(round(1.6 * n ** 0.56), max_size)
+        return min(round(1.6 * n**0.56), max_size)
     else:
         return 1
 
 
 def create_mask(size: int, lengths: torch.LongTensor, inverse: bool = False) -> torch.BoolTensor:
     """
     Create boolean masks of shape len(lenghts) x size.
@@ -222,14 +226,39 @@
         # batch sizes reside on the CPU by default -> we need to bring them to GPU
         lengths = lengths.to(sequence.device)
     else:
         lengths = torch.ones(sequence.size(0), device=sequence.device, dtype=torch.long) * sequence.size(1)
     return sequence, lengths
 
 
+def concat_sequences(
+    sequences: Union[List[torch.Tensor], List[rnn.PackedSequence]]
+) -> Union[torch.Tensor, rnn.PackedSequence]:
+    """
+    Concatenate RNN sequences.
+
+    Args:
+        sequences (Union[List[torch.Tensor], List[rnn.PackedSequence]): list of RNN packed sequences or tensors of which
+            first index are samples and second are timesteps
+
+    Returns:
+        Union[torch.Tensor, rnn.PackedSequence]: concatenated sequence
+    """
+    if isinstance(sequences[0], rnn.PackedSequence):
+        return rnn.pack_sequence(sequences, enforce_sorted=False)
+    elif isinstance(sequences[0], torch.Tensor):
+        return torch.cat(sequences, dim=1)
+    elif isinstance(sequences[0], (tuple, list)):
+        return tuple(
+            concat_sequences([sequences[ii][i] for ii in range(len(sequences))]) for i in range(len(sequences[0]))
+        )
+    else:
+        raise ValueError("Unsupported sequence type")
+
+
 def padded_stack(
     tensors: List[torch.Tensor], side: str = "right", mode: str = "constant", value: Union[int, float] = 0
 ) -> torch.Tensor:
     """
     Stack tensors along first dimension and pad them along last dimension to ensure their size is equal.
 
     Args:
@@ -333,14 +362,50 @@
 
     def items(self):
         return zip(self._fields, self)
 
     def keys(self):
         return self._fields
 
+    def iget(self, idx: Union[int, slice]):
+        """Select item(s) row-wise.
+
+        Args:
+            idx ([int, slice]): item to select
+
+        Returns:
+            Output of single item.
+        """
+        return self.__class__(*(x[idx] for x in self))
+
+
+class TupleOutputMixIn:
+    """MixIn to give output a namedtuple-like access capabilities with ``to_network_output() function``."""
+
+    def to_network_output(self, **results):
+        """
+        Convert output into a named (and immuatable) tuple.
+
+        This allows tracing the modules as graphs and prevents modifying the output.
+
+        Returns:
+            named tuple
+        """
+        if hasattr(self, "_output_class"):
+            Output = self._output_class
+        else:
+            OutputTuple = namedtuple("output", results)
+
+            class Output(OutputMixIn, OutputTuple):
+                pass
+
+            self._output_class = Output
+
+        return self._output_class(**results)
+
 
 def move_to_device(
     x: Union[
         Dict[str, Union[torch.Tensor, List[torch.Tensor], Tuple[torch.Tensor]]],
         torch.Tensor,
         List[torch.Tensor],
         Tuple[torch.Tensor],
@@ -406,7 +471,88 @@
         return {name: detach(xi) for name, xi in x.items()}
     elif isinstance(x, OutputMixIn):
         return x.__class__(**{name: detach(xi) for name, xi in x.items()})
     elif isinstance(x, (list, tuple)):
         return [detach(xi) for xi in x]
     else:
         return x
+
+
+def masked_op(tensor: torch.Tensor, op: str = "mean", dim: int = 0, mask: torch.Tensor = None) -> torch.Tensor:
+    """Calculate operation on masked tensor.
+
+    Args:
+        tensor (torch.Tensor): tensor to conduct operation over
+        op (str): operation to apply. One of ["mean", "sum"]. Defaults to "mean".
+        dim (int, optional): dimension to average over. Defaults to 0.
+        mask (torch.Tensor, optional): boolean mask to apply (True=will take mean, False=ignore).
+            Masks nan values by default.
+
+    Returns:
+        torch.Tensor: tensor with averaged out dimension
+    """
+    if mask is None:
+        mask = ~torch.isnan(tensor)
+    masked = tensor.masked_fill(~mask, 0.0)
+    summed = masked.sum(dim=dim)
+    if op == "mean":
+        return summed / mask.sum(dim=dim)  # Find the average
+    elif op == "sum":
+        return summed
+    else:
+        raise ValueError(f"unkown operation {op}")
+
+
+def repr_class(
+    obj,
+    attributes: Union[List[str], Dict[str, Any]],
+    max_characters_before_break: int = 100,
+    extra_attributes: Dict[str, Any] = {},
+) -> str:
+    """Print class name and parameters.
+
+    Args:
+        obj: class to format
+        attributes (Union[List[str], Dict[str]]): list of attributes to show or dictionary of attributes and values
+            to show max_characters_before_break (int): number of characters before breaking the into multiple lines
+        extra_attributes (Dict[str, Any]): extra attributes to show in angled brackets
+
+    Returns:
+        str
+    """
+    # get attributes
+    if isinstance(attributes, (tuple, list)):
+        attributes = {name: getattr(obj, name) for name in attributes if hasattr(obj, name)}
+    attributes_strings = [f"{name}={repr(value)}" for name, value in attributes.items()]
+    # get header
+    header_name = obj.__class__.__name__
+    # add extra attributes
+    if len(extra_attributes) > 0:
+        extra_attributes_strings = [f"{name}={repr(value)}" for name, value in extra_attributes.items()]
+        if len(header_name) + 2 + len(", ".join(extra_attributes_strings)) > max_characters_before_break:
+            header = f"{header_name}[\n\t" + ",\n\t".join(attributes_strings) + "\n]("
+        else:
+            header = f"{header_name}[{', '.join(extra_attributes_strings)}]("
+    else:
+        header = f"{header_name}("
+
+    # create final representation
+    attributes_string = ", ".join(attributes_strings)
+    if len(attributes_string) + len(header.split("\n")[-1]) + 1 > max_characters_before_break:
+        attributes_string = "\n\t" + ",\n\t".join(attributes_strings) + "\n"
+    return f"{header}{attributes_string})"
+
+
+class InitialParameterRepresenterMixIn:
+    def __repr__(self) -> str:
+        if isinstance(self, nn.Module):
+            return super().__repr__()
+        else:
+            attributes = list(inspect.signature(self.__class__).parameters.keys())
+            return repr_class(self, attributes=attributes)
+
+    def extra_repr(self) -> str:
+        if isinstance(self, pl.LightningModule):
+            return "\t" + repr(self.hparams).replace("\n", "\n\t")
+        else:
+            attributes = list(inspect.signature(self.__class__).parameters.keys())
+            return ", ".join([f"{name}={repr(getattr(self, name))}" for name in attributes if hasattr(self, name)])
```

### Comparing `pytorch_forecasting-0.9.2/setup.py` & `pytorch_forecasting-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,220 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pytorch-forecasting
+Version: 1.0.0
+Summary: Forecasting timeseries with PyTorch - dataloaders, normalizers, metrics and models
+Home-page: https://pytorch-forecasting.readthedocs.io
+Author: Jan Beitner
+Requires-Python: >=3.8,<3.11
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: github-actions
+Provides-Extra: graph
+Provides-Extra: mqf2
+Requires-Dist: cpflows (>=0.1.2,<0.2.0) ; extra == "mqf2"
+Requires-Dist: fastapi (>=0.80)
+Requires-Dist: lightning (>=2.0.0,<3.0.0)
+Requires-Dist: matplotlib
+Requires-Dist: networkx (>=3.0.0,<4.0.0) ; extra == "graph"
+Requires-Dist: optuna (>=3.1.0,<4.0.0)
+Requires-Dist: pandas (>=1.3.0,<=3.0.0)
+Requires-Dist: pytest-github-actions-annotate-failures ; extra == "github-actions"
+Requires-Dist: pytorch-optimizer (>=2.5.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.2,<2.0)
+Requires-Dist: scipy (>=1.8,<2.0)
+Requires-Dist: statsmodels
+Requires-Dist: torch (>=2.0.0,<3.0.0)
+Project-URL: Documentation, https://pytorch-forecasting.readthedocs.io
+Project-URL: Repository, https://github.com/jdb78/pytorch-forecasting
+Description-Content-Type: text/markdown
+
+![PyTorch Forecasting](./docs/source/_static/logo.svg)
+
+[pypi-image]: https://badge.fury.io/py/pytorch-forecasting.svg
+[pypi-url]: https://pypi.python.org/pypi/pytorch-forecasting
+[conda-image]: https://img.shields.io/conda/v/conda-forge/pytorch-forecasting
+[conda-url]: https://anaconda.org/conda-forge/pytorch-forecasting
+[build-image]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/test.yml/badge.svg?branch=master
+[build-url]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/test.yml?query=branch%3Amaster
+[linter-image]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/code_quality.yml/badge.svg?branch=master
+[linter-url]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/code_quality.yml?query=branch%3Amaster
+[docs-image]: https://readthedocs.org/projects/pytorch-forecasting/badge/?version=latest
+[docs-url]: https://pytorch-forecasting.readthedocs.io
+[coverage-image]: https://codecov.io/gh/jdb78/pytorch-forecasting/branch/master/graph/badge.svg
+[coverage-url]: https://codecov.io/github/jdb78/pytorch-forecasting?branch=master
+
+[![PyPI Version][pypi-image]][pypi-url] [![Conda Version][conda-image]][conda-url] [![Docs Status][docs-image]][docs-url] [![Linter Status][linter-image]][linter-url] [![Build Status][build-image]][build-url] [![Code Coverage][coverage-image]][coverage-url]
+
+**[Documentation](https://pytorch-forecasting.readthedocs.io)** | **[Tutorials](https://pytorch-forecasting.readthedocs.io/en/latest/tutorials.html)** | **[Release Notes](https://pytorch-forecasting.readthedocs.io/en/latest/CHANGELOG.html)**
+
+_PyTorch Forecasting_ is a PyTorch-based package for forecasting time series with state-of-the-art network architectures. It provides a high-level API for training networks on pandas data frames and leverages
+[PyTorch Lightning](https://pytorch-lightning.readthedocs.io/) for scalable training on (multiple) GPUs, CPUs and for automatic logging.
+
+---
+
+Our article on [Towards Data Science](https://towardsdatascience.com/introducing-pytorch-forecasting-64de99b9ef46) introduces the package and provides background information.
+
+PyTorch Forecasting aims to ease state-of-the-art timeseries forecasting with neural networks for real-world cases and research alike. The goal is to provide a high-level API with maximum flexibility for professionals and reasonable defaults for beginners.
+Specifically, the package provides
+
+- A timeseries dataset class which abstracts handling variable transformations, missing values,
+  randomized subsampling, multiple history lengths, etc.
+- A base model class which provides basic training of timeseries models along with logging in tensorboard
+  and generic visualizations such actual vs predictions and dependency plots
+- Multiple neural network architectures for timeseries forecasting that have been enhanced
+  for real-world deployment and come with in-built interpretation capabilities
+- Multi-horizon timeseries metrics
+- Hyperparameter tuning with [optuna](https://optuna.readthedocs.io/)
+
+The package is built on [pytorch-lightning](https://pytorch-lightning.readthedocs.io/) to allow training on CPUs, single and multiple GPUs out-of-the-box.
+
+# Installation
+
+If you are working on windows, you need to first install PyTorch with
+
+`pip install torch -f https://download.pytorch.org/whl/torch_stable.html`.
+
+Otherwise, you can proceed with
+
+`pip install pytorch-forecasting`
+
+Alternatively, you can install the package via conda
+
+`conda install pytorch-forecasting pytorch -c pytorch>=1.7 -c conda-forge`
+
+PyTorch Forecasting is now installed from the conda-forge channel while PyTorch is install from the pytorch channel.
+
+To use the MQF2 loss (multivariate quantile loss), also install
+`pip install pytorch-forecasting[mqf2]`
+
+# Documentation
+
+Visit [https://pytorch-forecasting.readthedocs.io](https://pytorch-forecasting.readthedocs.io) to read the
+documentation with detailed tutorials.
+
+# Available models
+
+The documentation provides a [comparison of available models](https://pytorch-forecasting.readthedocs.io/en/latest/models.html).
+
+- [Temporal Fusion Transformers for Interpretable Multi-horizon Time Series Forecasting](https://arxiv.org/pdf/1912.09363.pdf)
+  which outperforms DeepAR by Amazon by 36-69% in benchmarks
+- [N-BEATS: Neural basis expansion analysis for interpretable time series forecasting](http://arxiv.org/abs/1905.10437)
+  which has (if used as ensemble) outperformed all other methods including ensembles of traditional statical
+  methods in the M4 competition. The M4 competition is arguably the most important benchmark for univariate time series forecasting.
+- [N-HiTS: Neural Hierarchical Interpolation for Time Series Forecasting](http://arxiv.org/abs/2201.12886) which supports covariates and has consistently beaten N-BEATS. It is also particularly well-suited for long-horizon forecasting.
+- [DeepAR: Probabilistic forecasting with autoregressive recurrent networks](https://www.sciencedirect.com/science/article/pii/S0169207019301888)
+  which is the one of the most popular forecasting algorithms and is often used as a baseline
+- Simple standard networks for baselining: LSTM and GRU networks as well as a MLP on the decoder
+- A baseline model that always predicts the latest known value
+
+To implement new models or other custom components, see the [How to implement new models tutorial](https://pytorch-forecasting.readthedocs.io/en/latest/tutorials/building.html). It covers basic as well as advanced architectures.
+
+# Usage example
+
+Networks can be trained with the [PyTorch Lighning Trainer](https://pytorch-lightning.readthedocs.io/en/latest/common/trainer.html) on [pandas Dataframes](https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe) which are first converted to a [TimeSeriesDataSet](https://pytorch-forecasting.readthedocs.io/en/latest/data.html).
+
+```python
+# imports for training
+import lightning.pytorch as pl
+from lightning.pytorch.loggers import TensorBoardLogger
+from lightning.pytorch.callbacks import EarlyStopping, LearningRateMonitor
+# import dataset, network to train and metric to optimize
+from pytorch_forecasting import TimeSeriesDataSet, TemporalFusionTransformer, QuantileLoss
+from lightning.pytorch.tuner import Tuner
+
+# load data: this is pandas dataframe with at least a column for
+# * the target (what you want to predict)
+# * the timeseries ID (which should be a unique string to identify each timeseries)
+# * the time of the observation (which should be a monotonically increasing integer)
+data = ...
+
+# define the dataset, i.e. add metadata to pandas dataframe for the model to understand it
+max_encoder_length = 36
+max_prediction_length = 6
+training_cutoff = "YYYY-MM-DD"  # day for cutoff
+
+training = TimeSeriesDataSet(
+    data[lambda x: x.date <= training_cutoff],
+    time_idx= ...,  # column name of time of observation
+    target= ...,  # column name of target to predict
+    group_ids=[ ... ],  # column name(s) for timeseries IDs
+    max_encoder_length=max_encoder_length,  # how much history to use
+    max_prediction_length=max_prediction_length,  # how far to predict into future
+    # covariates static for a timeseries ID
+    static_categoricals=[ ... ],
+    static_reals=[ ... ],
+    # covariates known and unknown in the future to inform prediction
+    time_varying_known_categoricals=[ ... ],
+    time_varying_known_reals=[ ... ],
+    time_varying_unknown_categoricals=[ ... ],
+    time_varying_unknown_reals=[ ... ],
+)
+
+# create validation dataset using the same normalization techniques as for the training dataset
+validation = TimeSeriesDataSet.from_dataset(training, data, min_prediction_idx=training.index.time.max() + 1, stop_randomization=True)
+
+# convert datasets to dataloaders for training
+batch_size = 128
+train_dataloader = training.to_dataloader(train=True, batch_size=batch_size, num_workers=2)
+val_dataloader = validation.to_dataloader(train=False, batch_size=batch_size, num_workers=2)
+
+# create PyTorch Lighning Trainer with early stopping
+early_stop_callback = EarlyStopping(monitor="val_loss", min_delta=1e-4, patience=1, verbose=False, mode="min")
+lr_logger = LearningRateMonitor()
+trainer = pl.Trainer(
+    max_epochs=100,
+    accelerator="auto",  # run on CPU, if on multiple GPUs, use strategy="ddp"
+    gradient_clip_val=0.1,
+    limit_train_batches=30,  # 30 batches per epoch
+    callbacks=[lr_logger, early_stop_callback],
+    logger=TensorBoardLogger("lightning_logs")
+)
+
+# define network to train - the architecture is mostly inferred from the dataset, so that only a few hyperparameters have to be set by the user
+tft = TemporalFusionTransformer.from_dataset(
+    # dataset
+    training,
+    # architecture hyperparameters
+    hidden_size=32,
+    attention_head_size=1,
+    dropout=0.1,
+    hidden_continuous_size=16,
+    # loss metric to optimize
+    loss=QuantileLoss(),
+    # logging frequency
+    log_interval=2,
+    # optimizer parameters
+    learning_rate=0.03,
+    reduce_on_plateau_patience=4
+)
+print(f"Number of parameters in network: {tft.size()/1e3:.1f}k")
+
+# find the optimal learning rate
+res = Tuner(trainer).lr_find(
+    tft, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader, early_stop_threshold=1000.0, max_lr=0.3,
+)
+# and plot the result - always visually confirm that the suggested learning rate makes sense
+print(f"suggested learning rate: {res.suggestion()}")
+fig = res.plot(show=True, suggest=True)
+fig.show()
+
+# fit the model on the data - redefine the model with the correct learning rate if necessary
+trainer.fit(
+    tft, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader,
+)
+```
 
-packages = \
-['pytorch_forecasting',
- 'pytorch_forecasting.data',
- 'pytorch_forecasting.models',
- 'pytorch_forecasting.models.basic_rnn',
- 'pytorch_forecasting.models.deepar',
- 'pytorch_forecasting.models.mlp',
- 'pytorch_forecasting.models.nbeats',
- 'pytorch_forecasting.models.nn',
- 'pytorch_forecasting.models.rnn',
- 'pytorch_forecasting.models.temporal_fusion_transformer']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['matplotlib',
- 'optuna>=2.3.0,<3.0.0',
- 'pandas>=1.3.0,<2.0.0',
- 'pytorch-lightning>=1.2.4,<2.0.0',
- 'scikit-learn>=0.24,<1.1',
- 'scipy',
- 'statsmodels',
- 'torch>=1.7,<2.0']
-
-extras_require = \
-{'github-actions': ['pytest-github-actions-annotate-failures']}
-
-setup_kwargs = {
-    'name': 'pytorch-forecasting',
-    'version': '0.9.2',
-    'description': 'Forecasting timeseries with PyTorch - dataloaders, normalizers, metrics and models',
-    'long_description': '![PyTorch Forecasting](./docs/source/_static/logo.svg)\n\n[pypi-image]: https://badge.fury.io/py/pytorch-forecasting.svg\n[pypi-url]: https://pypi.python.org/pypi/pytorch-forecasting\n[conda-image]: https://img.shields.io/conda/v/conda-forge/pytorch-forecasting\n[conda-url]: https://anaconda.org/conda-forge/pytorch-forecasting\n[build-image]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/test.yml/badge.svg?branch=master\n[build-url]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/test.yml?query=branch%3Amaster\n[linter-image]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/code_quality.yml/badge.svg?branch=master\n[linter-url]: https://github.com/jdb78/pytorch-forecasting/actions/workflows/code_quality.yml?query=branch%3Amaster\n[docs-image]: https://readthedocs.org/projects/pytorch-forecasting/badge/?version=latest\n[docs-url]: https://pytorch-forecasting.readthedocs.io\n[coverage-image]: https://codecov.io/gh/jdb78/pytorch-forecasting/branch/master/graph/badge.svg\n[coverage-url]: https://codecov.io/github/jdb78/pytorch-forecasting?branch=master\n\n[![PyPI Version][pypi-image]][pypi-url] [![Conda Version][conda-image]][conda-url] [![Docs Status][docs-image]][docs-url] [![Linter Status][linter-image]][linter-url] [![Build Status][build-image]][build-url] [![Code Coverage][coverage-image]][coverage-url]\n\n**[Documentation](https://pytorch-forecasting.readthedocs.io)** | **[Tutorials](https://pytorch-forecasting.readthedocs.io/en/latest/tutorials.html)** | **[Release Notes](https://pytorch-forecasting.readthedocs.io/en/latest/CHANGELOG.html)**\n\n_PyTorch Forecasting_ is a PyTorch-based package for forecasting time series with state-of-the-art network architectures. It provides a high-level API for training networks on pandas data frames and leverages\n[PyTorch Lightning](https://pytorch-lightning.readthedocs.io/) for scalable training on (multiple) GPUs, CPUs and for automatic logging.\n\n---\n\nOur article on [Towards Data Science](https://towardsdatascience.com/introducing-pytorch-forecasting-64de99b9ef46) introduces the package and provides background information.\n\nPyTorch Forecasting aims to ease state-of-the-art timeseries forecasting with neural networks for real-world cases and research alike. The goal is to provide a high-level API with maximum flexibility for professionals and reasonable defaults for beginners.\nSpecifically, the package provides\n\n- A timeseries dataset class which abstracts handling variable transformations, missing values,\n  randomized subsampling, multiple history lengths, etc.\n- A base model class which provides basic training of timeseries models along with logging in tensorboard\n  and generic visualizations such actual vs predictions and dependency plots\n- Multiple neural network architectures for timeseries forecasting that have been enhanced\n  for real-world deployment and come with in-built interpretation capabilities\n- Multi-horizon timeseries metrics\n- Ranger optimizer for faster model training\n- Hyperparameter tuning with [optuna](https://optuna.readthedocs.io/)\n\nThe package is built on [pytorch-lightning](https://pytorch-lightning.readthedocs.io/) to allow training on CPUs, single and multiple GPUs out-of-the-box.\n\n# Installation\n\nIf you are working on windows, you need to first install PyTorch with\n\n`pip install torch -f https://download.pytorch.org/whl/torch_stable.html`.\n\nOtherwise, you can proceed with\n\n`pip install pytorch-forecasting`\n\nAlternatively, you can install the package via conda\n\n`conda install pytorch-forecasting pytorch -c pytorch>=1.7 -c conda-forge`\n\nPyTorch Forecasting is now installed from the conda-forge channel while PyTorch is install from the pytorch channel.\n\n# Documentation\n\nVisit [https://pytorch-forecasting.readthedocs.io](https://pytorch-forecasting.readthedocs.io) to read the\ndocumentation with detailed tutorials.\n\n# Available models\n\nThe documentation provides a [comparison of available models](https://pytorch-forecasting.readthedocs.io/en/latest/models.html).\n\n- [Temporal Fusion Transformers for Interpretable Multi-horizon Time Series Forecasting](https://arxiv.org/pdf/1912.09363.pdf)\n  which outperforms DeepAR by Amazon by 36-69% in benchmarks\n- [N-BEATS: Neural basis expansion analysis for interpretable time series forecasting](http://arxiv.org/abs/1905.10437)\n  which has (if used as ensemble) outperformed all other methods including ensembles of traditional statical\n  methods in the M4 competition. The M4 competition is arguably the most important benchmark for univariate time series forecasting.\n- [DeepAR: Probabilistic forecasting with autoregressive recurrent networks](https://www.sciencedirect.com/science/article/pii/S0169207019301888)\n  which is the one of the most popular forecasting algorithms and is often used as a baseline\n- Simple standard networks for baselining: LSTM and GRU networks as well as a MLP on the decoder\n- A baseline model that always predicts the latest known value\n\nTo implement new models or other custom components, see the [How to implement new models tutorial](https://pytorch-forecasting.readthedocs.io/en/latest/tutorials/building.html). It covers basic as well as advanced architectures.\n\n# Usage example\n\nNetworks can be trained with the [PyTorch Lighning Trainer](https://pytorch-lightning.readthedocs.io/en/latest/common/trainer.html) on [pandas Dataframes](https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dataframe) which are first converted to a [TimeSeriesDataSet](https://pytorch-forecasting.readthedocs.io/en/latest/data.html).\n\n```python\n# imports for training\nimport pytorch_lightning as pl\nfrom pytorch_lightning.loggers import TensorBoardLogger\nfrom pytorch_lightning.callbacks import EarlyStopping, LearningRateMonitor\n# import dataset, network to train and metric to optimize\nfrom pytorch_forecasting import TimeSeriesDataSet, TemporalFusionTransformer, QuantileLoss\n\n# load data: this is pandas dataframe with at least a column for\n# * the target (what you want to predict)\n# * the timeseries ID (which should be a unique string to identify each timeseries)\n# * the time of the observation (which should be a monotonically increasing integer)\ndata = ...\n\n# define the dataset, i.e. add metadata to pandas dataframe for the model to understand it\nmax_encoder_length = 36\nmax_prediction_length = 6\ntraining_cutoff = "YYYY-MM-DD"  # day for cutoff\n\ntraining = TimeSeriesDataSet(\n    data[lambda x: x.date <= training_cutoff],\n    time_idx= ...,  # column name of time of observation\n    target= ...,  # column name of target to predict\n    group_ids=[ ... ],  # column name(s) for timeseries IDs\n    max_encoder_length=max_encoder_length,  # how much history to use\n    max_prediction_length=max_prediction_length,  # how far to predict into future\n    # covariates static for a timeseries ID\n    static_categoricals=[ ... ],\n    static_reals=[ ... ],\n    # covariates known and unknown in the future to inform prediction\n    time_varying_known_categoricals=[ ... ],\n    time_varying_known_reals=[ ... ],\n    time_varying_unknown_categoricals=[ ... ],\n    time_varying_unknown_reals=[ ... ],\n)\n\n# create validation dataset using the same normalization techniques as for the training dataset\nvalidation = TimeSeriesDataSet.from_dataset(training, data, min_prediction_idx=training.index.time.max() + 1, stop_randomization=True)\n\n# convert datasets to dataloaders for training\nbatch_size = 128\ntrain_dataloader = training.to_dataloader(train=True, batch_size=batch_size, num_workers=2)\nval_dataloader = validation.to_dataloader(train=False, batch_size=batch_size, num_workers=2)\n\n# create PyTorch Lighning Trainer with early stopping\nearly_stop_callback = EarlyStopping(monitor="val_loss", min_delta=1e-4, patience=1, verbose=False, mode="min")\nlr_logger = LearningRateMonitor()\ntrainer = pl.Trainer(\n    max_epochs=100,\n    gpus=0,  # run on CPU, if on multiple GPUs, use accelerator="ddp"\n    gradient_clip_val=0.1,\n    limit_train_batches=30,  # 30 batches per epoch\n    callbacks=[lr_logger, early_stop_callback],\n    logger=TensorBoardLogger("lightning_logs")\n)\n\n# define network to train - the architecture is mostly inferred from the dataset, so that only a few hyperparameters have to be set by the user\ntft = TemporalFusionTransformer.from_dataset(\n    # dataset\n    training,\n    # architecture hyperparameters\n    hidden_size=32,\n    attention_head_size=1,\n    dropout=0.1,\n    hidden_continuous_size=16,\n    # loss metric to optimize\n    loss=QuantileLoss(),\n    # logging frequency\n    log_interval=2,\n    # optimizer parameters\n    learning_rate=0.03,\n    reduce_on_plateau_patience=4\n)\nprint(f"Number of parameters in network: {tft.size()/1e3:.1f}k")\n\n# find the optimal learning rate\nres = trainer.lr_find(\n    tft, train_dataloader=train_dataloader, val_dataloaders=val_dataloader, early_stop_threshold=1000.0, max_lr=0.3,\n)\n# and plot the result - always visually confirm that the suggested learning rate makes sense\nprint(f"suggested learning rate: {res.suggestion()}")\nfig = res.plot(show=True, suggest=True)\nfig.show()\n\n# fit the model on the data - redefine the model with the correct learning rate if necessary\ntrainer.fit(\n    tft, train_dataloader=train_dataloader, val_dataloaders=val_dataloader,\n)\n```\n',
-    'author': 'Jan Beitner',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://pytorch-forecasting.readthedocs.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
```

