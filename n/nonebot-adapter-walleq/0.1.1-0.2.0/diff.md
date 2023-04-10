# Comparing `tmp/nonebot_adapter_walleq-0.1.1.tar.gz` & `tmp/nonebot_adapter_walleq-0.2.0.tar.gz`

## Comparing `nonebot_adapter_walleq-0.1.1.tar` & `nonebot_adapter_walleq-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 nonebot_adapter_walleq-0.1.1/Cargo.toml
--rw-r--r--   0        0        0       73 2023-04-03 12:36:46.000000 nonebot_adapter_walleq-0.1.1/.gitignore
--rw-r--r--   0        0        0    34521 2023-04-03 12:47:51.000000 nonebot_adapter_walleq-0.1.1/LICENSE
--rw-r--r--   0        0        0     1047 2023-04-04 11:13:38.000000 nonebot_adapter_walleq-0.1.1/README.md
--rw-r--r--   0        0        0      100 2023-04-04 11:14:23.000000 nonebot_adapter_walleq-0.1.1/examples/wqtest/.env.prod
--rw-r--r--   0        0        0      202 2023-04-03 07:08:51.000000 nonebot_adapter_walleq-0.1.1/examples/wqtest/README.md
--rw-r--r--   0        0        0      363 2023-04-03 12:42:14.000000 nonebot_adapter_walleq-0.1.1/examples/wqtest/pyproject.toml
--rw-r--r--   0        0        0     4998 2023-04-04 11:07:32.000000 nonebot_adapter_walleq-0.1.1/nonebot_adapter_walleq/__init__.py
--rw-r--r--   0        0        0      233 2023-04-04 11:07:21.000000 nonebot_adapter_walleq-0.1.1/nonebot_adapter_walleq/nonebot_adapter_walleq.pyi
--rw-r--r--   0        0        0      647 2023-04-04 11:15:14.000000 nonebot_adapter_walleq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        7 2023-04-03 05:19:33.000000 nonebot_adapter_walleq-0.1.1/rust-toolchain
--rw-r--r--   0        0        0     4111 2023-04-04 11:06:55.000000 nonebot_adapter_walleq-0.1.1/src/lib.rs
--rw-r--r--   0        0        0    74424 2023-04-04 11:15:20.000000 nonebot_adapter_walleq-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 nonebot_adapter_walleq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 nonebot_adapter_walleq-0.2.0/Cargo.toml
+-rw-r--r--   0        0        0       73 2023-04-03 12:36:46.000000 nonebot_adapter_walleq-0.2.0/.gitignore
+-rw-r--r--   0        0        0    34521 2023-04-03 12:47:51.000000 nonebot_adapter_walleq-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1119 2023-04-10 04:38:17.000000 nonebot_adapter_walleq-0.2.0/README.md
+-rw-r--r--   0        0        0      100 2023-04-08 14:01:09.000000 nonebot_adapter_walleq-0.2.0/examples/wqtest/.env.prod
+-rw-r--r--   0        0        0      202 2023-04-03 07:08:51.000000 nonebot_adapter_walleq-0.2.0/examples/wqtest/README.md
+-rw-r--r--   0        0        0      391 2023-04-09 02:09:48.000000 nonebot_adapter_walleq-0.2.0/examples/wqtest/pyproject.toml
+-rw-r--r--   0        0        0     7057 2023-04-08 13:56:24.000000 nonebot_adapter_walleq-0.2.0/nonebot_adapter_walleq/__init__.py
+-rw-r--r--   0        0        0      284 2023-04-08 09:46:59.000000 nonebot_adapter_walleq-0.2.0/nonebot_adapter_walleq/nonebot_adapter_walleq.pyi
+-rw-r--r--   0        0        0      697 2023-04-10 04:36:45.000000 nonebot_adapter_walleq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        7 2023-04-03 05:19:33.000000 nonebot_adapter_walleq-0.2.0/rust-toolchain
+-rw-r--r--   0        0        0     4330 2023-04-08 10:58:21.000000 nonebot_adapter_walleq-0.2.0/src/lib.rs
+-rw-r--r--   0        0        0    74562 2023-04-08 13:51:58.000000 nonebot_adapter_walleq-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0     1762 1970-01-01 00:00:00.000000 nonebot_adapter_walleq-0.2.0/PKG-INFO
```

### Comparing `nonebot_adapter_walleq-0.1.1/Cargo.toml` & `nonebot_adapter_walleq-0.2.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_walleq-0.1.1/LICENSE` & `nonebot_adapter_walleq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_walleq-0.1.1/README.md` & `nonebot_adapter_walleq-0.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "0": {             //密码登录时必须为 qq 号
       "protocol": 2,   // watch
       "password": null // 留空则使用扫码登录
     }
   }
   ```
 - walle_q_leveldb: bool 是否启用 leveldb
-- walle_q_sled： bool 是否启用 sled
+- walle_q_sled：bool 是否启用 sled
+- walle_q_data_path: str 数据存储路径，默认将使用localstore
 
 ## 特别鸣谢
 
 [Nonebot2](https://github.com/nonebot/nonebot2)：跨平台 PYTHON 异步机器人框架
 
 [Walle-Q](https://github.com/onebot-walle/walle-q)：Onebot 12 QQ 协议实现（我谢我自己）
```

### Comparing `nonebot_adapter_walleq-0.1.1/nonebot_adapter_walleq/__init__.py` & `nonebot_adapter_walleq-0.2.0/nonebot_adapter_walleq/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,24 @@
 from nonebot.adapters.onebot.v12 import Bot, StatusUpdateMetaEvent, MetaEvent, BotEvent
 from nonebot.adapters.onebot.v12.utils import msgpack_encoder
 from nonebot.typing import overrides
 from nonebot.drivers import Driver
 from nonebot import get_driver
 from typing import Any, Optional, Dict, cast, Union, Literal
 from nonebot.utils import logger_wrapper, escape_tag
+from nonebot import require
 import msgpack
 import asyncio
 
 bots: Dict[str, Bot] = {}
 log = logger_wrapper("Walle-Q")
+require("nonebot_plugin_localstore")
+import nonebot_plugin_localstore as store
+
+data_dir = store.get_data_dir("walle_q")
 
 
 async def _call_data(data: bytes):
     driver = get_driver()
     if wq := driver._adapters.get("Walle-Q"):
         if isinstance(wq, Adapter):
             raw_data = msgpack.unpackb(data)
@@ -63,29 +68,54 @@
                     asyncio.create_task(bot.handle_event(event))
 
 
 class Adapter(V12Adapter):
     @overrides(V12Adapter)
     def __init__(self, driver: Driver, **kwargs: Any) -> None:
         self.driver = driver
-        self.wq_config = Config(**self.config.dict())
+        self._config = Config(**self.config.dict())
+        data_path: str = (
+            self._config.walle_q_data_path
+            if self._config.walle_q_data_path
+            else str(data_dir)
+        )
         self.inner: WalleQ = WalleQ(
-            self.wq_config.walle_q_leveldb, self.wq_config.walle_q_sled
+            self._config.walle_q_leveldb,
+            self._config.walle_q_sled,
+            data_path,
         )
         self.timeout: Optional[float] = driver.config.api_timeout
 
-        async def run(wq: WalleQ, config: Optional[bytes]):
-            await wq.run(config)
+        async def run(wq: WalleQ, data_path: str):
+            await wq.run(data_path, "./log")
 
         @driver.on_startup
         async def _():
-            config: Optional[bytes] = msgpack.dumps(
-                self.wq_config.walle_q, default=msgpack_encoder
-            )
-            asyncio.create_task(run(self.inner, config))
+            asyncio.create_task(run(self.inner, data_path))
+            await asyncio.sleep(0.5)
+            for id, config in self._config.walle_q.items():
+                r = LoginResp.parse_obj(
+                    await self._call_meta_api(
+                        "login",
+                        bot_id=id,
+                        protocol=config.protocol,
+                        password=config.password,
+                    )
+                )
+                if r.qrcode_str:
+                    log("INFO", f"登录 bot: {r.bot_id} 中，扫码登录：")
+                    print(r.qrcode_str)
+                elif r.url:
+                    log("INFO", f"登录 bot: {r.bot_id} 中, need captcha url: {r.url}")
+                    print(f"input ticket:", end="")
+                    ticket = input()
+                    print(ticket)
+                    await self._call_meta_api(
+                        "submit_ticket", bot_id=r.bot_id, ticket=ticket
+                    )
 
     @classmethod
     @overrides(V12Adapter)
     def get_name(cls) -> str:
         return "Walle-Q"
 
     @overrides(V12Adapter)
@@ -104,20 +134,46 @@
         else:
             raise ValueError("walle-q not running")
         try:
             return self._handle_api_result(await self._result_store.fetch(seq, timeout))
         except asyncio.TimeoutError:
             raise TimeoutError(f"Walle-Q call api {api} timeout")
 
+    async def _call_meta_api(self, api: str, **data: Any) -> Any:
+        timeout: float = data.get("_timeout", self.timeout)
+        seq = self._result_store.get_seq()
+        action_data = {
+            "action": api,
+            "params": data,
+            "echo": str(seq),
+        }
+        b: Optional[bytes] = msgpack.packb(action_data, default=msgpack_encoder)
+        if self.inner:
+            self.inner.call_api(b)
+        else:
+            raise ValueError("walle-q not running")
+        try:
+            return self._handle_api_result(await self._result_store.fetch(seq, timeout))
+        except asyncio.TimeoutError:
+            raise TimeoutError(f"Walle-Q call api {api} timeout")
+
 
 from pydantic import BaseModel
 
 
 class QQConfig(BaseModel):
     password: Optional[str]
     protocol: Optional[int]
 
 
 class Config(BaseModel):
     walle_q: Dict[str, QQConfig]
     walle_q_leveldb: Optional[bool]
     walle_q_sled: Optional[bool]
+    walle_q_data_path: Optional[str]
+
+
+class LoginResp(BaseModel):
+    bot_id: str
+    url: Optional[str]
+    qrcode: Optional[bytes]
+    qrcode_str: Optional[str]
```

### Comparing `nonebot_adapter_walleq-0.1.1/src/lib.rs` & `nonebot_adapter_walleq-0.2.0/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -8,61 +8,62 @@
 
 use std::sync::Arc;
 
 use pyo3::types::PyBytes;
 use pyo3::{PyAny, PyResult, Python};
 use tokio::sync::broadcast::{channel, Sender as BTx};
 use walle_core::OneBot;
-use walle_q::config::QQConfig;
 use walle_q::database::WQDatabase;
 use walle_q::init;
 use walle_q::multi::MultiAH;
 
 #[pyo3::pyclass]
 pub struct WalleQ {
     ob: Arc<OneBot<MultiAH, PyoHandler>>,
     action_tx: BTx<Vec<u8>>,
     event_tx: BTx<Vec<u8>>,
 }
 
-
 #[pyo3::pymethods]
 impl WalleQ {
     #[new]
-    fn new(level_db: Option<bool>, sled_db: Option<bool>) -> Self {
+    fn new(level_db: Option<bool>, sled_db: Option<bool>, data_path: Option<String>) -> Self {
         let (action_tx, _) = channel(64);
         let (event_tx, _) = channel(64);
-        let mut databse = WQDatabase::default();
+        let data_path = Arc::new(data_path.unwrap_or(walle_q::DATA_PATH.to_owned()));
+        let mut databse = WQDatabase::new(&data_path);
         if let Some(true) = level_db {
             databse = databse.add_level();
         }
         if let Some(true) = sled_db {
             databse = databse.add_sled();
         }
         Self {
             ob: Arc::new(OneBot::new(
-                MultiAH::new(None, 10, Arc::new(databse)),
+                MultiAH::new(None, 10, Arc::new(databse), data_path),
                 PyoHandler {
                     action_tx: action_tx.clone(),
                     event_tx: event_tx.clone(),
                 },
             )),
             action_tx,
             event_tx,
         }
     }
 
-    fn run<'a>(&self, config: Vec<u8>, py: Python<'a>) -> PyResult<&'a PyAny> {
-        let config: std::collections::HashMap<String, QQConfig> =
-            rmp_serde::from_slice(&config).unwrap();
+    fn run<'a>(&self, data_path: String, log_path: String, py: Python<'a>) -> PyResult<&'a PyAny> {
+        // let config: std::collections::HashMap<String, QQConfig> =
+        //     rmp_serde::from_slice(&config).unwrap();
         let ob = self.ob.clone();
         let mut event_rx = self.event_tx.subscribe();
         pyo3_asyncio::tokio::future_into_py(py, async move {
-            init().await;
-            ob.start(config, (), true).await.unwrap(); //todo()
+            init(Some(data_path), Some(log_path)).await;
+            ob.start(std::collections::HashMap::default(), (), true)
+                .await
+                .unwrap(); //todo()
             while let Ok(data) = event_rx.recv().await {
                 let f = Python::with_gil(|py| {
                     pyo3_asyncio::tokio::into_future(
                         py.import("nonebot_adapter_walleq")
                             .unwrap()
                             .call_method1("_call_data", (PyBytes::new(py, &data),))
                             .unwrap(),
```

### Comparing `nonebot_adapter_walleq-0.1.1/Cargo.lock` & `nonebot_adapter_walleq-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -566,21 +566,21 @@
  "errno-dragonfly",
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "errno"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d6a0976c999d473fe89ad888d5a284e55366d9dc9038b1ba2aa15128c4afa0"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -810,17 +810,17 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
@@ -1090,33 +1090,33 @@
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.6"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "256017f749ab3117e93acb91063009e1f1bb56d03965b14c2c8df4eb02c524d8"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -1271,15 +1271,15 @@
 
 [[package]]
 name = "nanorand"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -1768,15 +1768,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.8",
+ "getrandom 0.2.9",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -1839,17 +1839,16 @@
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "ricq"
-version = "0.1.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44588852775d7416accd9044e1ff3837ca93403064f646b2067d2f77fc48f0"
+version = "0.1.20"
+source = "git+https://github.com/lz1998/ricq.git#5c5a5901bc6951fd2186f841a394f5d3fcd41ad7"
 dependencies = [
  "async-trait",
  "bytes",
  "cached 0.35.0",
  "derivative",
  "flate2",
  "futures-util",
@@ -1862,17 +1861,16 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "ricq-core"
-version = "0.1.19"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9921e29625c65fab984c532382e8954b5de34f83139dfd371aeb59ccb9f3a310"
+version = "0.1.20"
+source = "git+https://github.com/lz1998/ricq.git#5c5a5901bc6951fd2186f841a394f5d3fcd41ad7"
 dependencies = [
  "byteorder",
  "bytes",
  "derivative",
  "flate2",
  "generic-array",
  "jcers",
@@ -1906,24 +1904,24 @@
  "byteorder",
  "rmp",
  "serde",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.7"
+version = "0.37.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aae838e49b3d63e9274e1c01833cc8139d3fec468c3b84688c628f44b1ae11d"
+checksum = "85597d61f83914ddeba6a47b3b8ffe7365107221c2e557ed94426489fefb5f77"
 dependencies = [
  "bitflags",
- "errno 0.3.0",
+ "errno 0.3.1",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rusty-leveldb"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04c67700d4731d7c35c914a844dba95ae6689a419a576433c745b76757a555db"
@@ -2593,17 +2591,17 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walle-core"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7bb70f392de9b8308f5e0d7b93804c636e08bed587f5f98d86e239e077a4c261"
+checksum = "637bb74074a93867d2eafca363bf8b9bf37afd8e4e3c1aeb15a77649357e18c5"
 dependencies = [
  "async-trait",
  "base64 0.13.1",
  "colored",
  "dashmap",
  "futures-util",
  "hex",
@@ -2628,16 +2626,16 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "walle-q"
-version = "0.2.5-fix2"
-source = "git+https://github.com/onebot-walle/walle-q.git#11e0ca4424af82ffe3003bf8bf188460db232430"
+version = "0.3.0-a1"
+source = "git+https://github.com/onebot-walle/walle-q.git#6e40fd80286b0f238f4ff5a3c3a8068cbab7bc76"
 dependencies = [
  "async-recursion",
  "async-trait",
  "base64 0.21.0",
  "bytes",
  "cached 0.42.0",
  "chrono",
@@ -2831,14 +2829,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
  "windows-targets 0.42.2",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
```

### Comparing `nonebot_adapter_walleq-0.1.1/PKG-INFO` & `nonebot_adapter_walleq-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-walleq
-Version: 0.1.1
+Version: 0.2.0
 Requires-Dist: nonebot-adapter-onebot~=2.2.2
+Requires-Dist: nonebot-plugin-localstore>=0.4.1
 License-File: LICENSE
 Summary: Just run walle-q in nonebot2
 Keywords: nonebot,nonebot2,bot,walleq
 Author-email: AbrahumLink <307887491@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: hongpage, https://github.com/onebot-walle/nonebot_adapter_walleq
 Project-URL: documentation, https://github.com/onebot-walle/nonebot_adapter_walleq#readme
+Project-URL: hongpage, https://github.com/onebot-walle/nonebot_adapter_walleq
 Project-URL: repository, https://github.com/onebot-walle/nonebot_adapter_walleq
 
 # nonebot-adapter-walleq
 
 <img alt="PyPI" src="https://img.shields.io/pypi/v/nonebot-adapter-walleq"> <img alt="GitHub" src="https://img.shields.io/github/license/onebot-walle/nonebot_adapter_walleq">
 
 直接在你的 [Nonebot2](https://github.com/nonebot/nonebot2) 内置 [Walle-Q](https://github.com/onebot-walle/walle-q) ，他甚至不需要通过 Onebot Connect！
@@ -28,14 +29,15 @@
     "0": {             //密码登录时必须为 qq 号
       "protocol": 2,   // watch
       "password": null // 留空则使用扫码登录
     }
   }
   ```
 - walle_q_leveldb: bool 是否启用 leveldb
-- walle_q_sled： bool 是否启用 sled
+- walle_q_sled：bool 是否启用 sled
+- walle_q_data_path: str 数据存储路径，默认将使用localstore
 
 ## 特别鸣谢
 
 [Nonebot2](https://github.com/nonebot/nonebot2)：跨平台 PYTHON 异步机器人框架
 
 [Walle-Q](https://github.com/onebot-walle/walle-q)：Onebot 12 QQ 协议实现（我谢我自己）
```

