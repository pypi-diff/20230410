# Comparing `tmp/tango_mlflow-1.0.0.tar.gz` & `tmp/tango_mlflow-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tango_mlflow-1.0.0.tar", max compression
+gzip compressed data, was "tango_mlflow-1.0.1.tar", max compression
```

## Comparing `tango_mlflow-1.0.0.tar` & `tango_mlflow-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2023-04-09 09:19:37.016393 tango_mlflow-1.0.0/LICENSE
--rw-r--r--   0        0        0     1773 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       78 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/__init__.py
--rw-r--r--   0        0        0      129 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/__main__.py
--rw-r--r--   0        0        0      569 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/commands/__init__.py
--rw-r--r--   0        0        0     3633 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/commands/subcommand.py
--rw-r--r--   0        0        0    12913 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/commands/tune.py
--rw-r--r--   0        0        0     5649 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/flax_train_callback.py
--rw-r--r--   0        0        0        0 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/py.typed
--rw-r--r--   0        0        0     1988 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/step.py
--rw-r--r--   0        0        0     6090 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/step_cache.py
--rw-r--r--   0        0        0     6692 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/torch_train_callback.py
--rw-r--r--   0        0        0    11867 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/util.py
--rw-r--r--   0        0        0    18306 2023-04-09 09:19:37.020393 tango_mlflow-1.0.0/tango_mlflow/workspace.py
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 tango_mlflow-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-10 04:52:04.195135 tango_mlflow-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1773 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/__init__.py
+-rw-r--r--   0        0        0      129 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/__main__.py
+-rw-r--r--   0        0        0      569 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/commands/__init__.py
+-rw-r--r--   0        0        0     3633 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/commands/subcommand.py
+-rw-r--r--   0        0        0    12913 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/commands/tune.py
+-rw-r--r--   0        0        0     6306 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/flax_train_callback.py
+-rw-r--r--   0        0        0        0 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/py.typed
+-rw-r--r--   0        0        0     1988 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/step.py
+-rw-r--r--   0        0        0     6090 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/step_cache.py
+-rw-r--r--   0        0        0     7535 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/torch_train_callback.py
+-rw-r--r--   0        0        0    11867 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/util.py
+-rw-r--r--   0        0        0    18306 2023-04-10 04:52:04.199135 tango_mlflow-1.0.1/tango_mlflow/workspace.py
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 tango_mlflow-1.0.1/PKG-INFO
```

### Comparing `tango_mlflow-1.0.0/LICENSE` & `tango_mlflow-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/pyproject.toml` & `tango_mlflow-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tango-mlflow"
-version = "1.0.0"
+version = "1.0.1"
 description = "MLflow integration for ai2-tango"
 authors = ["altescy <altescy@fastmail.com>"]
 
 [tool.poetry.scripts]
 tango-mlflow = "tango_mlflow.__main__:run"
 
 [tool.poetry.dependencies]
```

### Comparing `tango_mlflow-1.0.0/tango_mlflow/commands/__init__.py` & `tango_mlflow-1.0.1/tango_mlflow/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/tango_mlflow/commands/subcommand.py` & `tango_mlflow-1.0.1/tango_mlflow/commands/subcommand.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/tango_mlflow/commands/tune.py` & `tango_mlflow-1.0.1/tango_mlflow/commands/tune.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/tango_mlflow/flax_train_callback.py` & `tango_mlflow-1.0.1/tango_mlflow/flax_train_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,151 +1,154 @@
+from contextlib import suppress
 from typing import Any, Dict, Optional
 
-import jax
 import mlflow
-from flax import jax_utils
 from mlflow.entities import Metric
 from mlflow.entities import Run as MlflowRun
 from mlflow.tracking.context import registry as context_registry
 from mlflow.utils.mlflow_tags import MLFLOW_RUN_NAME
-from tango.integrations.flax.train_callback import TrainCallback
+from tango.common.exceptions import IntegrationMissingError
 
 from tango_mlflow.util import RunKind, flatten_dict, get_mlflow_run_by_tango_step, get_timestamp
 from tango_mlflow.workspace import MLFlowWorkspace
 
+with suppress(ModuleNotFoundError, IntegrationMissingError):
+    import jax
+    from flax import jax_utils
+    from tango.integrations.flax.train_callback import TrainCallback
+
+    @TrainCallback.register("mlflow::log_flax")
+    class MLFlowFlaxTrainCallback(TrainCallback):
+        def __init__(
+            self,
+            *args: Any,
+            experiment_name: Optional[str] = None,
+            tags: Optional[Dict[str, str]] = None,
+            tracking_uri: Optional[str] = None,
+            mlflow_config: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
+        ) -> None:
+            super().__init__(*args, **kwargs)
+
+            if isinstance(self.workspace, MLFlowWorkspace):
+                experiment_name = experiment_name or self.workspace.experiment_name
+                tracking_uri = tracking_uri or self.workspace.mlflow_tracking_uri
+
+            self.experiment_name = experiment_name
+            self.tags = tags or {}
+            self.tracking_uri = tracking_uri
+
+            self.mlflow_config = self.train_config.as_dict()
+            self.mlflow_config.pop("worker_id")
+            if mlflow_config is not None:
+                self.mlflow_config.update(mlflow_config)
+
+            self.mlflow_run: Optional[MlflowRun] = None
+
+        @property
+        def mlflow_client(self) -> mlflow.tracking.MlflowClient:
+            if isinstance(self.workspace, MLFlowWorkspace):
+                return self.workspace.mlflow_client
+            return mlflow.tracking.MlflowClient(tracking_uri=self.tracking_uri)
 
-@TrainCallback.register("mlflow::log_flax")
-class MLFlowFlaxTrainCallback(TrainCallback):
-    def __init__(
-        self,
-        *args: Any,
-        experiment_name: Optional[str] = None,
-        tags: Optional[Dict[str, str]] = None,
-        tracking_uri: Optional[str] = None,
-        mlflow_config: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
-    ) -> None:
-        super().__init__(*args, **kwargs)
-
-        if isinstance(self.workspace, MLFlowWorkspace):
-            experiment_name = experiment_name or self.workspace.experiment_name
-            tracking_uri = tracking_uri or self.workspace.mlflow_tracking_uri
-
-        self.experiment_name = experiment_name
-        self.tags = tags or {}
-        self.tracking_uri = tracking_uri
-
-        self.mlflow_config = self.train_config.as_dict()
-        self.mlflow_config.pop("worker_id")
-        if mlflow_config is not None:
-            self.mlflow_config.update(mlflow_config)
-
-        self.mlflow_run: Optional[MlflowRun] = None
-
-    @property
-    def mlflow_client(self) -> mlflow.tracking.MlflowClient:
-        if isinstance(self.workspace, MLFlowWorkspace):
-            return self.workspace.mlflow_client
-        return mlflow.tracking.MlflowClient(tracking_uri=self.tracking_uri)
-
-    def ensure_mlflow_run(self) -> MlflowRun:
-        if self.mlflow_run is None:
-            raise RuntimeError("MLFlow run not initialized")
-        return self.mlflow_run
-
-    def state_dict(self) -> Dict[str, Any]:
-        return {}
-
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        self.resume = "allow"
-
-    def pre_train_loop(self) -> None:
-        if isinstance(self.workspace, MLFlowWorkspace):
-            # Use existing MLFlow run created by the MLFlowWorkspace
-            self.mlflow_run = get_mlflow_run_by_tango_step(
-                self.mlflow_client,
-                experiment=self.experiment_name,
-                tango_step=self.step_id,
-                additional_filter_string="attributes.status = 'RUNNING'",
-            )
+        def ensure_mlflow_run(self) -> MlflowRun:
             if self.mlflow_run is None:
-                raise RuntimeError(f"Could not find a running MLFlow run for step {self.step_id}")
-        else:
-            # Create a new MLFlow run and log the config
-            self.mlflow_run = self.mlflow_client.create_run(
-                experiment_id=mlflow.get_experiment_by_name(self.experiment_name).experiment_id,
-                tags=context_registry.resolve_tags(
-                    {
-                        "job_type": RunKind.TRAIN_METRICS,
-                        "step_name": self.step_name,
-                        "step_id": self.step_id,
-                        MLFLOW_RUN_NAME: self.step_name,
-                    }.update(self.tags)
-                ),
-            )
-            for key, value in flatten_dict(self.mlflow_config).items():
-                self.mlflow_client.log_param(self.mlflow_run.info.run_id, key, value)
+                raise RuntimeError("MLFlow run not initialized")
+            return self.mlflow_run
 
-            timestamp = get_timestamp()
-            metrics = [Metric(key="epoch", value=0, timestamp=timestamp, step=0)]
-            self.mlflow_client.log_batch(self.mlflow_run.info.run_id, metrics=metrics)
+        def state_dict(self) -> Dict[str, Any]:
+            return {}
+
+        def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+            self.resume = "allow"
 
-    def post_train_loop(self, step: int, epoch: int) -> None:
-        if isinstance(self.workspace, MLFlowWorkspace):
-            # We don't need to do anything here, as the MLFlow run will be closed by the MLFlowWorkspace
-            return
-        mlflow_run = self.ensure_mlflow_run()
-        self.mlflow_client.set_terminated(mlflow_run.info.run_id)
-
-    def log_batch(self, step: int, epoch: int, train_metrics: Dict) -> None:
-        if len(jax.devices()) > 1:
-            train_metrics = jax_utils.unreplicate(train_metrics)  # type: ignore[no-untyped-call]
-        step += 1
-        timestamp = get_timestamp()
-        metrics = [
-            Metric(
-                key="train.loss",
-                value=train_metrics["loss"],
-                timestamp=timestamp,
-                step=step,
-            ),
-            Metric(
-                key="epoch",
-                value=epoch,
-                timestamp=0,
-                step=step,
-            ),
-        ]
-        mlflow_run = self.ensure_mlflow_run()
-        self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
-
-    def post_val_loop(
-        self,
-        step: int,
-        epoch: int,
-        val_metric: Optional[float],
-        best_val_metric: Optional[float],
-    ) -> None:
-        step = step + 1
-        timestamp = get_timestamp()
-        mlflow_run = self.ensure_mlflow_run()
-        metrics = [
-            Metric(
-                key="val.loss",
-                value=val_metric,
-                timestamp=timestamp,
-                step=step,
-            ),
-            Metric(
-                key=f"val.best_{self.train_config.val_metric_name}",
-                value=best_val_metric,
-                timestamp=timestamp,
-                step=step,
-            ),
-            Metric(
-                key="epoch",
-                value=epoch,
-                timestamp=timestamp,
-                step=step,
-            ),
-        ]
-        self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
+        def pre_train_loop(self) -> None:
+            if isinstance(self.workspace, MLFlowWorkspace):
+                # Use existing MLFlow run created by the MLFlowWorkspace
+                self.mlflow_run = get_mlflow_run_by_tango_step(
+                    self.mlflow_client,
+                    experiment=self.experiment_name,
+                    tango_step=self.step_id,
+                    additional_filter_string="attributes.status = 'RUNNING'",
+                )
+                if self.mlflow_run is None:
+                    raise RuntimeError(f"Could not find a running MLFlow run for step {self.step_id}")
+            else:
+                # Create a new MLFlow run and log the config
+                self.mlflow_run = self.mlflow_client.create_run(
+                    experiment_id=mlflow.get_experiment_by_name(self.experiment_name).experiment_id,
+                    tags=context_registry.resolve_tags(
+                        {
+                            "job_type": RunKind.TRAIN_METRICS,
+                            "step_name": self.step_name,
+                            "step_id": self.step_id,
+                            MLFLOW_RUN_NAME: self.step_name,
+                        }.update(self.tags)
+                    ),
+                )
+                for key, value in flatten_dict(self.mlflow_config).items():
+                    self.mlflow_client.log_param(self.mlflow_run.info.run_id, key, value)
+
+                timestamp = get_timestamp()
+                metrics = [Metric(key="epoch", value=0, timestamp=timestamp, step=0)]
+                self.mlflow_client.log_batch(self.mlflow_run.info.run_id, metrics=metrics)
+
+        def post_train_loop(self, step: int, epoch: int) -> None:
+            if isinstance(self.workspace, MLFlowWorkspace):
+                # We don't need to do anything here, as the MLFlow run will be closed by the MLFlowWorkspace
+                return
+            mlflow_run = self.ensure_mlflow_run()
+            self.mlflow_client.set_terminated(mlflow_run.info.run_id)
+
+        def log_batch(self, step: int, epoch: int, train_metrics: Dict) -> None:
+            if len(jax.devices()) > 1:
+                train_metrics = jax_utils.unreplicate(train_metrics)  # type: ignore[no-untyped-call]
+            step += 1
+            timestamp = get_timestamp()
+            metrics = [
+                Metric(
+                    key="train.loss",
+                    value=train_metrics["loss"],
+                    timestamp=timestamp,
+                    step=step,
+                ),
+                Metric(
+                    key="epoch",
+                    value=epoch,
+                    timestamp=0,
+                    step=step,
+                ),
+            ]
+            mlflow_run = self.ensure_mlflow_run()
+            self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
+
+        def post_val_loop(
+            self,
+            step: int,
+            epoch: int,
+            val_metric: Optional[float],
+            best_val_metric: Optional[float],
+        ) -> None:
+            step = step + 1
+            timestamp = get_timestamp()
+            mlflow_run = self.ensure_mlflow_run()
+            metrics = [
+                Metric(
+                    key="val.loss",
+                    value=val_metric,
+                    timestamp=timestamp,
+                    step=step,
+                ),
+                Metric(
+                    key=f"val.best_{self.train_config.val_metric_name}",
+                    value=best_val_metric,
+                    timestamp=timestamp,
+                    step=step,
+                ),
+                Metric(
+                    key="epoch",
+                    value=epoch,
+                    timestamp=timestamp,
+                    step=step,
+                ),
+            ]
+            self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
```

### Comparing `tango_mlflow-1.0.0/tango_mlflow/step.py` & `tango_mlflow-1.0.1/tango_mlflow/step.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/tango_mlflow/step_cache.py` & `tango_mlflow-1.0.1/tango_mlflow/step_cache.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/tango_mlflow/torch_train_callback.py` & `tango_mlflow-1.0.1/tango_mlflow/torch_train_callback.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,176 +1,182 @@
+from contextlib import suppress
 from typing import Any, Dict, List, Optional
 
 import mlflow
-import torch
 from mlflow.entities import Metric
 from mlflow.entities import Run as MlflowRun
 from mlflow.tracking.context import registry as context_registry
 from mlflow.utils.mlflow_tags import MLFLOW_RUN_NAME
-from tango.integrations.torch.train_callback import TrainCallback
-from tango.integrations.torch.util import peak_gpu_memory
+from tango.common.exceptions import IntegrationMissingError
 
 from tango_mlflow.util import RunKind, flatten_dict, get_mlflow_run_by_tango_step, get_timestamp
 from tango_mlflow.workspace import MLFlowWorkspace
 
+with suppress(ModuleNotFoundError, IntegrationMissingError):
+    import torch
+    from tango.integrations.torch.train_callback import TrainCallback
+    from tango.integrations.torch.util import peak_gpu_memory
+
+    @TrainCallback.register("mlflow::log")
+    class MLFlowTrainCallback(TrainCallback):
+        def __init__(
+            self,
+            *args: Any,
+            experiment_name: Optional[str] = None,
+            tags: Optional[Dict[str, str]] = None,
+            tracking_uri: Optional[str] = None,
+            mlflow_config: Optional[Dict[str, Any]] = None,
+            **kwargs: Any,
+        ) -> None:
+            if torch is None:
+                raise IntegrationMissingError("torch")
+
+            super().__init__(*args, **kwargs)
+
+            if isinstance(self.workspace, MLFlowWorkspace):
+                experiment_name = experiment_name or self.workspace.experiment_name
+                tracking_uri = tracking_uri or self.workspace.mlflow_tracking_uri
+
+            self.experiment_name = experiment_name
+            self.tags = tags or {}
+            self.tracking_uri = tracking_uri
+
+            self.mlflow_config = self.train_config.as_dict()
+            self.mlflow_config.pop("worker_id")
+            if mlflow_config is not None:
+                self.mlflow_config.update(mlflow_config)
+
+            self.mlflow_run: Optional[MlflowRun] = None
+
+        @property
+        def mlflow_client(self) -> mlflow.tracking.MlflowClient:
+            if isinstance(self.workspace, MLFlowWorkspace):
+                return self.workspace.mlflow_client
+            return mlflow.tracking.MlflowClient(tracking_uri=self.tracking_uri)
 
-@TrainCallback.register("mlflow::log")
-class MLFlowTrainCallback(TrainCallback):
-    def __init__(
-        self,
-        *args: Any,
-        experiment_name: Optional[str] = None,
-        tags: Optional[Dict[str, str]] = None,
-        tracking_uri: Optional[str] = None,
-        mlflow_config: Optional[Dict[str, Any]] = None,
-        **kwargs: Any,
-    ) -> None:
-        super().__init__(*args, **kwargs)
-
-        if isinstance(self.workspace, MLFlowWorkspace):
-            experiment_name = experiment_name or self.workspace.experiment_name
-            tracking_uri = tracking_uri or self.workspace.mlflow_tracking_uri
-
-        self.experiment_name = experiment_name
-        self.tags = tags or {}
-        self.tracking_uri = tracking_uri
-
-        self.mlflow_config = self.train_config.as_dict()
-        self.mlflow_config.pop("worker_id")
-        if mlflow_config is not None:
-            self.mlflow_config.update(mlflow_config)
-
-        self.mlflow_run: Optional[MlflowRun] = None
-
-    @property
-    def mlflow_client(self) -> mlflow.tracking.MlflowClient:
-        if isinstance(self.workspace, MLFlowWorkspace):
-            return self.workspace.mlflow_client
-        return mlflow.tracking.MlflowClient(tracking_uri=self.tracking_uri)
-
-    def ensure_mlflow_run(self) -> MlflowRun:
-        if self.mlflow_run is None:
-            raise RuntimeError("MLFlow run not initialized")
-        return self.mlflow_run
-
-    def state_dict(self) -> Dict[str, Any]:
-        return {}
-
-    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
-        pass
-
-    def pre_train_loop(self) -> None:
-        if isinstance(self.workspace, MLFlowWorkspace):
-            # Use existing MLFlow run created by the MLFlowWorkspace
-            self.mlflow_run = get_mlflow_run_by_tango_step(
-                self.mlflow_client,
-                experiment=self.experiment_name,
-                tango_step=self.step_id,
-                additional_filter_string="attributes.status = 'RUNNING'",
-            )
+        def ensure_mlflow_run(self) -> MlflowRun:
             if self.mlflow_run is None:
-                raise RuntimeError(f"Could not find a running MLFlow run for step {self.step_id}")
-        else:
-            # Create a new MLFlow run and log the config
-            self.mlflow_run = self.mlflow_client.create_run(
-                experiment_id=mlflow.get_experiment_by_name(self.experiment_name).experiment_id,
-                tags=context_registry.resolve_tags(
-                    {
-                        "job_type": RunKind.TRAIN_METRICS,
-                        "step_name": self.step_name,
-                        "step_id": self.step_id,
-                        MLFLOW_RUN_NAME: self.step_name,
-                    }.update(self.tags)
-                ),
-            )
-            for key, value in flatten_dict(self.mlflow_config).items():
-                self.mlflow_client.log_param(self.mlflow_run.info.run_id, key, value)
-
-        if torch.cuda.is_available():
-            torch.cuda.reset_peak_memory_stats()
-        peak_gpu_mbs = peak_gpu_memory()
-        if self.is_local_main_process:
-            timestamp = self.mlflow_run.info.start_time
-            metrics = [
-                Metric(key=f"sys.worker{rank}_peak_gpu_mem", value=mbs, timestamp=timestamp, step=0)
-                for rank, mbs in peak_gpu_mbs.items()
-            ]
-            metrics.append(Metric(key="epoch", value=0, timestamp=timestamp, step=0))
-            self.mlflow_client.log_batch(self.mlflow_run.info.run_id, metrics=metrics)
-
-    def post_train_loop(self, step: int, epoch: int) -> None:
-        if isinstance(self.workspace, MLFlowWorkspace):
-            # We don't need to do anything here, as the MLFlow run will be closed by the MLFlowWorkspace
-            return
-        if self.is_local_main_process:
-            mlflow_run = self.ensure_mlflow_run()
-            self.mlflow_client.set_terminated(mlflow_run.info.run_id)
-
-    def log_batch(
-        self,
-        step: int,
-        epoch: int,
-        batch_loss: float,
-        batch_outputs: List[Dict[str, Any]],
-    ) -> None:
-        step = step + 1
-        timestamp = get_timestamp()
-        peak_gpu_mbs = peak_gpu_memory()
-        if self.is_local_main_process:
-            mlflow_run = self.ensure_mlflow_run()
-            metrics = [
-                Metric(
-                    key="train.loss",
-                    value=batch_loss,
-                    timestamp=timestamp,
-                    step=step,
-                ),
-                Metric(
-                    key="train.lr",
-                    value=self.training_engine.optimizer.param_groups[0]["lr"],
-                    timestamp=timestamp,
-                    step=step,
-                ),
-                Metric(
-                    key="epoch",
-                    value=epoch,
-                    timestamp=0,
-                    step=step,
-                ),
-            ] + [
-                Metric(key=f"sys.worker{rank}_peak_gpu_mem", value=mbs, timestamp=timestamp, step=step)
-                for rank, mbs in peak_gpu_mbs.items()
-            ]
-            self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
-
-    def post_val_loop(
-        self,
-        step: int,
-        epoch: int,
-        val_metric: float,
-        best_val_metric: float,
-    ) -> None:
-        step = step + 1
-        timestamp = get_timestamp()
-        if self.is_local_main_process:
-            mlflow_run = self.ensure_mlflow_run()
-            metrics = [
-                Metric(
-                    key="val.loss",
-                    value=val_metric,
-                    timestamp=timestamp,
-                    step=step,
-                ),
-                Metric(
-                    key=f"val.best_{self.train_config.val_metric_name}",
-                    value=best_val_metric,
-                    timestamp=timestamp,
-                    step=step,
-                ),
-                Metric(
-                    key="epoch",
-                    value=epoch,
-                    timestamp=timestamp,
-                    step=step,
-                ),
-            ]
-            self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
+                raise RuntimeError("MLFlow run not initialized")
+            return self.mlflow_run
+
+        def state_dict(self) -> Dict[str, Any]:
+            return {}
+
+        def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+            pass
+
+        def pre_train_loop(self) -> None:
+            if isinstance(self.workspace, MLFlowWorkspace):
+                # Use existing MLFlow run created by the MLFlowWorkspace
+                self.mlflow_run = get_mlflow_run_by_tango_step(
+                    self.mlflow_client,
+                    experiment=self.experiment_name,
+                    tango_step=self.step_id,
+                    additional_filter_string="attributes.status = 'RUNNING'",
+                )
+                if self.mlflow_run is None:
+                    raise RuntimeError(f"Could not find a running MLFlow run for step {self.step_id}")
+            else:
+                # Create a new MLFlow run and log the config
+                self.mlflow_run = self.mlflow_client.create_run(
+                    experiment_id=mlflow.get_experiment_by_name(self.experiment_name).experiment_id,
+                    tags=context_registry.resolve_tags(
+                        {
+                            "job_type": RunKind.TRAIN_METRICS,
+                            "step_name": self.step_name,
+                            "step_id": self.step_id,
+                            MLFLOW_RUN_NAME: self.step_name,
+                        }.update(self.tags)
+                    ),
+                )
+                for key, value in flatten_dict(self.mlflow_config).items():
+                    self.mlflow_client.log_param(self.mlflow_run.info.run_id, key, value)
+
+            if torch.cuda.is_available():
+                torch.cuda.reset_peak_memory_stats()
+            peak_gpu_mbs = peak_gpu_memory()
+            if self.is_local_main_process:
+                timestamp = self.mlflow_run.info.start_time
+                metrics = [
+                    Metric(key=f"sys.worker{rank}_peak_gpu_mem", value=mbs, timestamp=timestamp, step=0)
+                    for rank, mbs in peak_gpu_mbs.items()
+                ]
+                metrics.append(Metric(key="epoch", value=0, timestamp=timestamp, step=0))
+                self.mlflow_client.log_batch(self.mlflow_run.info.run_id, metrics=metrics)
+
+        def post_train_loop(self, step: int, epoch: int) -> None:
+            if isinstance(self.workspace, MLFlowWorkspace):
+                # We don't need to do anything here, as the MLFlow run will be closed by the MLFlowWorkspace
+                return
+            if self.is_local_main_process:
+                mlflow_run = self.ensure_mlflow_run()
+                self.mlflow_client.set_terminated(mlflow_run.info.run_id)
+
+        def log_batch(
+            self,
+            step: int,
+            epoch: int,
+            batch_loss: float,
+            batch_outputs: List[Dict[str, Any]],
+        ) -> None:
+            step = step + 1
+            timestamp = get_timestamp()
+            peak_gpu_mbs = peak_gpu_memory()
+            if self.is_local_main_process:
+                mlflow_run = self.ensure_mlflow_run()
+                metrics = [
+                    Metric(
+                        key="train.loss",
+                        value=batch_loss,
+                        timestamp=timestamp,
+                        step=step,
+                    ),
+                    Metric(
+                        key="train.lr",
+                        value=self.training_engine.optimizer.param_groups[0]["lr"],
+                        timestamp=timestamp,
+                        step=step,
+                    ),
+                    Metric(
+                        key="epoch",
+                        value=epoch,
+                        timestamp=0,
+                        step=step,
+                    ),
+                ] + [
+                    Metric(key=f"sys.worker{rank}_peak_gpu_mem", value=mbs, timestamp=timestamp, step=step)
+                    for rank, mbs in peak_gpu_mbs.items()
+                ]
+                self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
+
+        def post_val_loop(
+            self,
+            step: int,
+            epoch: int,
+            val_metric: float,
+            best_val_metric: float,
+        ) -> None:
+            step = step + 1
+            timestamp = get_timestamp()
+            if self.is_local_main_process:
+                mlflow_run = self.ensure_mlflow_run()
+                metrics = [
+                    Metric(
+                        key="val.loss",
+                        value=val_metric,
+                        timestamp=timestamp,
+                        step=step,
+                    ),
+                    Metric(
+                        key=f"val.best_{self.train_config.val_metric_name}",
+                        value=best_val_metric,
+                        timestamp=timestamp,
+                        step=step,
+                    ),
+                    Metric(
+                        key="epoch",
+                        value=epoch,
+                        timestamp=timestamp,
+                        step=step,
+                    ),
+                ]
+                self.mlflow_client.log_batch(mlflow_run.info.run_id, metrics=metrics)
```

### Comparing `tango_mlflow-1.0.0/tango_mlflow/util.py` & `tango_mlflow-1.0.1/tango_mlflow/util.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/tango_mlflow/workspace.py` & `tango_mlflow-1.0.1/tango_mlflow/workspace.py`

 * *Files identical despite different names*

### Comparing `tango_mlflow-1.0.0/PKG-INFO` & `tango_mlflow-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tango-mlflow
-Version: 1.0.0
+Version: 1.0.1
 Summary: MLflow integration for ai2-tango
 Author: altescy
 Author-email: altescy@fastmail.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

