# Comparing `tmp/pytpu-14.6.7.tar.gz` & `tmp/pytpu-14.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytpu-14.6.7.tar", last modified: Tue Mar  7 16:36:05 2023, max compression
+gzip compressed data, was "dist/pytpu-14.6.8.tar", last modified: Mon Apr 10 16:10:29 2023, max compression
```

## Comparing `pytpu-14.6.7.tar` & `pytpu-14.6.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:36:05.878873 pytpu-14.6.7/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-03-07 16:35:19.000000 pytpu-14.6.7/MANIFEST.in
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-03-07 16:36:05.878873 pytpu-14.6.7/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3131 2023-03-07 16:35:19.000000 pytpu-14.6.7/README.md
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:36:05.874873 pytpu-14.6.7/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      600 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/__init__.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:36:05.874873 pytpu-14.6.7/pytpu/pytpu/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      695 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/pytpu/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    11758 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/pytpu/libtpu_bindings.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:36:05.874873 pytpu-14.6.7/pytpu/scripts/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/scripts/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2258 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/scripts/pyrun_tpu_cli.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      810 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/scripts/run_get_fps.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:36:05.878873 pytpu-14.6.7/pytpu/tools/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      119 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/tools/__init__.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5134 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/tools/get_fps.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6860 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/tools/helpers.py
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7381 2023-03-07 16:35:19.000000 pytpu-14.6.7/pytpu/tools/tpu_runner.py
-drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-03-07 16:36:05.874873 pytpu-14.6.7/pytpu.egg-info/
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      489 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/entry_points.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/not-zip-safe
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      197 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/requires.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-03-07 16:36:05.000000 pytpu-14.6.7/pytpu.egg-info/top_level.txt
--rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-03-07 16:36:05.878873 pytpu-14.6.7/setup.cfg
--rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)     1531 2023-03-07 16:36:05.000000 pytpu-14.6.7/setup.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       41 2023-04-10 16:09:07.000000 pytpu-14.6.8/MANIFEST.in
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-10 16:10:29.590434 pytpu-14.6.8/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     3131 2023-04-10 16:09:07.000000 pytpu-14.6.8/README.md
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      600 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/__init__.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/pytpu/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      695 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/pytpu/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)    12138 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/pytpu/libtpu_bindings.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/scripts/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/scripts/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     2258 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/scripts/pyrun_tpu_cli.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      810 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/scripts/run_get_fps.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu/tools/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      119 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/__init__.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     5134 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/get_fps.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     6860 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/helpers.py
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     7808 2023-04-10 16:09:07.000000 pytpu-14.6.8/pytpu/tools/tpu_runner.py
+drwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)        0 2023-04-10 16:10:29.590434 pytpu-14.6.8/pytpu.egg-info/
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)     4262 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/PKG-INFO
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      489 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      109 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/entry_points.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        1 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/not-zip-safe
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)      197 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/requires.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)        6 2023-04-10 16:10:29.000000 pytpu-14.6.8/pytpu.egg-info/top_level.txt
+-rw-r--r--   0 gitlab-runner  (1001) gitlab-runner  (1001)       38 2023-04-10 16:10:29.590434 pytpu-14.6.8/setup.cfg
+-rwxr-xr-x   0 gitlab-runner  (1001) gitlab-runner  (1001)     1531 2023-04-10 16:10:29.000000 pytpu-14.6.8/setup.py
```

### Comparing `pytpu-14.6.7/PKG-INFO` & `pytpu-14.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 14.6.7
+Version: 14.6.8
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
 Author: Alexey Antipin
 Author-email: a.antipin@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
```

### Comparing `pytpu-14.6.7/README.md` & `pytpu-14.6.8/README.md`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/__init__.py` & `pytpu-14.6.8/pytpu/__init__.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/pytpu/__init__.py` & `pytpu-14.6.8/pytpu/pytpu/__init__.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/pytpu/libtpu_bindings.py` & `pytpu-14.6.8/pytpu/pytpu/libtpu_bindings.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,151 +26,151 @@
     'get_inference',
     'submit_inference',
 ]
 
 
 
 class TPUDevice(Structure):
-    
+
     _fields_ = []
 
     def __init__(self, dev_name):
-        # self.pointer = libtpu.create_device(c_int(dev_no))
-        self.pointer = libtpu.create_device(c_char_p(dev_name))
+        # self.pointer = libtpu.tpu_create_device(c_int(dev_no))
+        self.pointer = libtpu.tpu_create_device(c_char_p(dev_name))
 
     def __del__(self):
-        return libtpu.destroy_device(self.pointer)
+        return libtpu.tpu_destroy_device(self.pointer)
 
     def is_valid(self):
-        return libtpu.is_device_valid(self.pointer)
+        return libtpu.tpu_is_device_valid(self.pointer)
 
     def init(self):
-        return libtpu.init_device(self.pointer)
+        return libtpu.tpu_init_device(self.pointer)
 
     def get_error(self):
-        return libtpu.get_device_error_message(self.pointer)
+        return libtpu.tpu_get_device_error_message(self.pointer)
 
     def info(self):
-        return libtpu.get_device_info(self.pointer)
+        return libtpu.tpu_get_device_info(self.pointer)
 
     def load_program(self, program):
-        return libtpu.load_program(self.pointer, program.pointer)
+        return libtpu.tpu_load_program(self.pointer, program.pointer)
 
     def run_inference(self, inference, mode):
-        return libtpu.run_inference(self.pointer, inference.pointer, mode)
+        return libtpu.tpu_run_inference(self.pointer, inference.pointer, mode)
 
     def submit_inference(self, inference, mode, callback_fn, context):
-        return libtpu.submit_inference(self.pointer, inference.pointer, mode, callback_fn, context)
+        return libtpu.tpu_submit_inference(self.pointer, inference.pointer, mode, callback_fn, context)
 
 
 class TPUProgram(Structure):
 
     _fields_ = []
 
     def __init__(self, program_path):
-        self.pointer = libtpu.create_program(c_char_p(program_path))
+        self.pointer = libtpu.tpu_create_program(c_char_p(program_path))
 
     def __del__(self):
-        return libtpu.destroy_program(self.pointer)
+        return libtpu.tpu_destroy_program(self.pointer)
 
     def is_valid(self):
-        return libtpu.is_program_valid(self.pointer)
+        return libtpu.tpu_is_program_valid(self.pointer)
 
     def info(self):
-        return libtpu.get_program_info(self.pointer)
+        return libtpu.tpu_get_program_info(self.pointer)
 
     def get_error(self):
-        return libtpu.get_program_error_message(self.pointer)
+        return libtpu.tpu_get_program_error_message(self.pointer)
 
     def get_batch_size(self):
-        return libtpu.get_batch_size(self.pointer)
+        return libtpu.tpu_get_batch_size(self.pointer)
 
     def get_input_count(self):
-        return libtpu.get_input_count(self.pointer)
+        return libtpu.tpu_get_input_count(self.pointer)
 
     def get_input_size(self, n, raw):
-        return libtpu.get_input_size(self.pointer, c_size_t(n), c_bool(raw))
+        return libtpu.tpu_get_input_size(self.pointer, c_size_t(n), c_bool(raw))
 
     def get_output_count(self):
-        return libtpu.get_output_count(self.pointer)
+        return libtpu.tpu_get_output_count(self.pointer)
 
     def get_output_size(self, n, raw):
-        return libtpu.get_output_size(self.pointer, c_size_t(n), c_bool(raw))
+        return libtpu.tpu_get_output_size(self.pointer, c_size_t(n), c_bool(raw))
 
 
 class TPUTensorBufferObject(Structure):
 
     _fields_ = []
 
     def __init__(self, prog, Type):
-        self.pointer = libtpu.create_tensor_buffer_object(prog.pointer, Type)
+        self.pointer = libtpu.tpu_create_tensor_buffer_object(prog.pointer, Type)
 
     def __del__(self):
-        return libtpu.destroy_tensor_buffer_object(self.pointer)
+        return libtpu.tpu_destroy_tensor_buffer_object(self.pointer)
 
     def process_tensor_buffers(self):
-        return libtpu.process_tensor_buffers(self.pointer)
+        return libtpu.tpu_process_tensor_buffers(self.pointer)
 
     def get_tensor_buffer_ptr(self, n, raw):
-        return libtpu.get_tensor_buffer_ptr(self.pointer, c_size_t(n), c_bool(raw))
+        return libtpu.tpu_get_tensor_buffer_ptr(self.pointer, c_size_t(n), c_bool(raw))
 
     def set_user_tensor_buffer_ptr(self, n, ptr):
-        return libtpu.set_user_tensor_buffer_ptr(self.pointer, c_size_t(n), ptr)
+        return libtpu.tpu_set_user_tensor_buffer_ptr(self.pointer, c_size_t(n), ptr)
 
 
 class TPUInference(Structure):
 
     _fields_ = []
 
     def __init__(self, program):
-        self.pointer = libtpu.create_inference(program.pointer)
+        self.pointer = libtpu.tpu_create_inference(program.pointer)
 
     def __del__(self):
-        return libtpu.destroy_inference(self.pointer)
+        return libtpu.tpu_destroy_inference(self.pointer)
 
     def get_program(self):
-        return libtpu.get_inference_program(self.pointer)
+        return libtpu.tpu_get_inference_program(self.pointer)
 
     def get_inputs(self):
-        return libtpu.get_inference_inputs(self.pointer)
+        return libtpu.tpu_get_inference_inputs(self.pointer)
 
     def set_inputs(self, buf_obj):
-        return libtpu.set_inference_inputs(self.pointer, buf_obj.pointer)
+        return libtpu.tpu_set_inference_inputs(self.pointer, buf_obj.pointer)
 
     def set_outputs(self, buf_obj):
-        return libtpu.set_inference_outputs(self.pointer, buf_obj.pointer)
+        return libtpu.tpu_set_inference_outputs(self.pointer, buf_obj.pointer)
 
     def get_outputs(self):
-        return libtpu.get_inference_outputs(self.pointer)
+        return libtpu.tpu_get_inference_outputs(self.pointer)
 
     def get_status(self):
-        return libtpu.get_inference_status(self.pointer)
+        return libtpu.tpu_get_inference_status(self.pointer)
 
     def get_error(self):
-        return libtpu.get_inference_error_message(self.pointer)
+        return libtpu.tpu_get_inference_error_message(self.pointer)
 
 CB_POINTER = CFUNCTYPE(None, POINTER(TPUInference), c_int, c_void_p)
 
 
 def load_inference(data, program, mode=False):
     in_meta = input_metadata(program)
     out_meta = output_metadata(program)
 
     if not isinstance(data, dict):
         data_ = {}
         for k, d_ in zip(in_meta, (data, )):
             data_.update({k: d_})
         data = data_
-    
+
     tpu_input = TPUTensorBufferObject(program, TPUTensorBufferType.kInputs.value)
     for i, (k, data) in enumerate(data.items()):
         in_tensor = bytearray(data)
         p_in_tensor = (c_uint8 * program.get_input_size(i, mode)).from_buffer(in_tensor)
         tpu_input.set_user_tensor_buffer_ptr(i, cast(p_in_tensor, POINTER(c_uint8)))
-    
+
     out_ctx = []
     tpu_output = TPUTensorBufferObject(program, TPUTensorBufferType.kOutputs.value)
     for o, k in enumerate(out_meta):
         out_tensor = bytearray(np.empty((program.get_output_size(o, mode), ), dtype=np.uint8))
         p_out_tensor = (c_uint8 * program.get_output_size(o, mode)).from_buffer(out_tensor)
         c_out_ptr = cast(p_out_tensor, POINTER(c_uint8))
         out_ctx.append(c_out_ptr)
@@ -189,34 +189,34 @@
 
 async def submit_inference_(device, program, inference, output_buffer, mode):
     finish_flag = asyncio.Event()
     finish_flag_p = cast(pointer(py_object(finish_flag)), c_void_p)
     # print(f'Flag status before: {finish_flag.is_set()}')
     status = device.submit_inference(inference, mode, inference_cb, finish_flag_p)
     await POINTER(py_object).from_address(addressof(finish_flag_p)).contents.value.wait()
-    
+
     # print(f'Flag status after: {POINTER(py_object).from_address(addressof(finish_flag_p)).contents.value.is_set()}')
     assert status == 0
 
 
 async def submit_inference(device, program, inference, output_buffer, mode):
     finish_flag = False
     finish_flag_p = cast(pointer(py_object(finish_flag)), c_void_p)
     # print(f'Flag status before: {finish_flag}')
     status = device.submit_inference(inference, mode, inference_cb, finish_flag_p)
     while not POINTER(py_object).from_address(addressof(finish_flag_p)).contents.value:
         await asyncio.sleep(0)
-    
+
     # print(f'Flag status after: {POINTER(py_object).from_address(addressof(finish_flag_p)).contents.value}')
     assert status == 0, 'Inference did not start!'
 
 def get_inference(program, output_buffer, out_ctx, as_dict=True, mode=False):
     out_meta = output_metadata(program)
     collected_data = dict() if as_dict else list()
-    
+
     for i, k in enumerate(out_meta):
         data = np.ctypeslib.as_array(out_ctx[i], shape = (program.get_output_size(i, mode), ))
         data = convert_from_uint8_to_user_dtype(data, out_meta[k]['user_dtype'])
         data = data.reshape(out_meta[k]['user_shape'])
         if as_dict:
             collected_data.update({k: data})
         else:
@@ -236,109 +236,109 @@
 class TPUInferenceStatus(Enum):
     kOk = 0
     kError = 1
     kDevError = 2
 
 
 # TPUDevice
-libtpu.create_device.restype = POINTER(TPUDevice)
-# libtpu.create_device.argtypes = [c_int]
-libtpu.create_device.argtypes = [c_char_p]
+libtpu.tpu_create_device.restype = POINTER(TPUDevice)
+# libtpu.tpu_create_device.argtypes = [c_int]
+libtpu.tpu_create_device.argtypes = [c_char_p]
 
-libtpu.destroy_device.restype = c_void_p
-libtpu.destroy_device.argtypes = [POINTER(TPUDevice)]
+libtpu.tpu_destroy_device.restype = c_void_p
+libtpu.tpu_destroy_device.argtypes = [POINTER(TPUDevice)]
 
-libtpu.is_device_valid.restype = c_int
-libtpu.is_device_valid.argtypes = [POINTER(TPUDevice)]
+libtpu.tpu_is_device_valid.restype = c_int
+libtpu.tpu_is_device_valid.argtypes = [POINTER(TPUDevice)]
 
-libtpu.init_device.restype = c_int
-libtpu.init_device.argtypes = [POINTER(TPUDevice)]
+libtpu.tpu_init_device.restype = c_int
+libtpu.tpu_init_device.argtypes = [POINTER(TPUDevice)]
 
-libtpu.get_device_error_message.restype = c_char_p
-libtpu.get_device_error_message.argtypes = [POINTER(TPUDevice)]
+libtpu.tpu_get_device_error_message.restype = c_char_p
+libtpu.tpu_get_device_error_message.argtypes = [POINTER(TPUDevice)]
 
-libtpu.get_device_info.restype = c_char_p
-libtpu.get_device_info.argtypes = [POINTER(TPUDevice)]
+libtpu.tpu_get_device_info.restype = c_char_p
+libtpu.tpu_get_device_info.argtypes = [POINTER(TPUDevice)]
 
-libtpu.load_program.restype = c_int
-libtpu.load_program.argtypes = [POINTER(TPUDevice), POINTER(TPUProgram)]
+libtpu.tpu_load_program.restype = c_int
+libtpu.tpu_load_program.argtypes = [POINTER(TPUDevice), POINTER(TPUProgram)]
 
-libtpu.run_inference.restype = c_int
-libtpu.run_inference.argtypes = [POINTER(TPUDevice), POINTER(TPUInference), c_int]
+libtpu.tpu_run_inference.restype = c_int
+libtpu.tpu_run_inference.argtypes = [POINTER(TPUDevice), POINTER(TPUInference), c_int]
 
-libtpu.submit_inference.restype = c_int
-libtpu.submit_inference.argtypes = [POINTER(TPUDevice), POINTER(TPUInference), c_int, CB_POINTER, c_void_p]
+libtpu.tpu_submit_inference.restype = c_int
+libtpu.tpu_submit_inference.argtypes = [POINTER(TPUDevice), POINTER(TPUInference), c_int, CB_POINTER, c_void_p]
 
 # TPUProgram
-libtpu.create_program.restype = POINTER(TPUProgram)
-libtpu.create_program.argtypes = [POINTER(c_char)]
+libtpu.tpu_create_program.restype = POINTER(TPUProgram)
+libtpu.tpu_create_program.argtypes = [POINTER(c_char)]
 
-libtpu.destroy_program.restype = c_void_p
-libtpu.destroy_program.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_destroy_program.restype = c_void_p
+libtpu.tpu_destroy_program.argtypes = [POINTER(TPUProgram)]
 
-libtpu.is_program_valid.restype = c_int
-libtpu.is_program_valid.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_is_program_valid.restype = c_int
+libtpu.tpu_is_program_valid.argtypes = [POINTER(TPUProgram)]
 
-libtpu.get_program_info.restype = c_char_p
-libtpu.get_program_info.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_get_program_info.restype = c_char_p
+libtpu.tpu_get_program_info.argtypes = [POINTER(TPUProgram)]
 
-libtpu.get_program_error_message.restype = c_char_p
-libtpu.get_program_error_message.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_get_program_error_message.restype = c_char_p
+libtpu.tpu_get_program_error_message.argtypes = [POINTER(TPUProgram)]
 
-libtpu.get_batch_size.restype = c_size_t
-libtpu.get_batch_size.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_get_batch_size.restype = c_size_t
+libtpu.tpu_get_batch_size.argtypes = [POINTER(TPUProgram)]
 
-libtpu.get_input_count.restype = c_size_t
-libtpu.get_input_count.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_get_input_count.restype = c_size_t
+libtpu.tpu_get_input_count.argtypes = [POINTER(TPUProgram)]
 
-libtpu.get_input_size.restype = c_size_t
-libtpu.get_input_size.argtypes = [POINTER(TPUProgram), c_size_t, c_bool]
+libtpu.tpu_get_input_size.restype = c_size_t
+libtpu.tpu_get_input_size.argtypes = [POINTER(TPUProgram), c_size_t, c_bool]
 
-libtpu.get_output_count.restype = c_size_t
-libtpu.get_output_count.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_get_output_count.restype = c_size_t
+libtpu.tpu_get_output_count.argtypes = [POINTER(TPUProgram)]
 
-libtpu.get_output_size.restype = c_size_t
-libtpu.get_output_size.argtypes = [POINTER(TPUProgram), c_size_t, c_bool]
+libtpu.tpu_get_output_size.restype = c_size_t
+libtpu.tpu_get_output_size.argtypes = [POINTER(TPUProgram), c_size_t, c_bool]
 
 # TPUTensorBufferObject
-libtpu.create_tensor_buffer_object.restype = POINTER(TPUTensorBufferObject)
-libtpu.create_tensor_buffer_object.argtypes = [POINTER(TPUProgram), c_int]
+libtpu.tpu_create_tensor_buffer_object.restype = POINTER(TPUTensorBufferObject)
+libtpu.tpu_create_tensor_buffer_object.argtypes = [POINTER(TPUProgram), c_int]
 
-libtpu.destroy_tensor_buffer_object.restype = c_void_p
-libtpu.destroy_tensor_buffer_object.argtypes = [POINTER(TPUTensorBufferObject)]
+libtpu.tpu_destroy_tensor_buffer_object.restype = c_void_p
+libtpu.tpu_destroy_tensor_buffer_object.argtypes = [POINTER(TPUTensorBufferObject)]
 
-libtpu.process_tensor_buffers.restype = c_void_p
-libtpu.process_tensor_buffers.argtypes = [POINTER(TPUTensorBufferObject)]
+libtpu.tpu_process_tensor_buffers.restype = c_void_p
+libtpu.tpu_process_tensor_buffers.argtypes = [POINTER(TPUTensorBufferObject)]
 
-libtpu.get_tensor_buffer_ptr.restype = POINTER(c_uint8)
-libtpu.get_tensor_buffer_ptr.argtypes = [POINTER(TPUTensorBufferObject), c_size_t, c_bool]
+libtpu.tpu_get_tensor_buffer_ptr.restype = POINTER(c_uint8)
+libtpu.tpu_get_tensor_buffer_ptr.argtypes = [POINTER(TPUTensorBufferObject), c_size_t, c_bool]
 
-libtpu.set_user_tensor_buffer_ptr.restype = POINTER(c_uint8)
-libtpu.set_user_tensor_buffer_ptr.argtypes = [POINTER(TPUTensorBufferObject), c_size_t, POINTER(c_uint8)]
+libtpu.tpu_set_user_tensor_buffer_ptr.restype = POINTER(c_uint8)
+libtpu.tpu_set_user_tensor_buffer_ptr.argtypes = [POINTER(TPUTensorBufferObject), c_size_t, POINTER(c_uint8)]
 
 # TPUInference
-libtpu.create_inference.restype = POINTER(TPUInference)
-libtpu.create_inference.argtypes = [POINTER(TPUProgram)]
+libtpu.tpu_create_inference.restype = POINTER(TPUInference)
+libtpu.tpu_create_inference.argtypes = [POINTER(TPUProgram)]
 
-libtpu.destroy_inference.restype = c_void_p
-libtpu.destroy_inference.argtypes = [POINTER(TPUInference)]
+libtpu.tpu_destroy_inference.restype = c_void_p
+libtpu.tpu_destroy_inference.argtypes = [POINTER(TPUInference)]
 
-libtpu.get_inference_program.restype = POINTER(TPUProgram)
-libtpu.get_inference_program.argtypes = [POINTER(TPUInference)]
+libtpu.tpu_get_inference_program.restype = POINTER(TPUProgram)
+libtpu.tpu_get_inference_program.argtypes = [POINTER(TPUInference)]
 
-libtpu.get_inference_inputs.restype = POINTER(TPUTensorBufferObject)
-libtpu.get_inference_inputs.argtypes = [POINTER(TPUInference)]
+libtpu.tpu_get_inference_inputs.restype = POINTER(TPUTensorBufferObject)
+libtpu.tpu_get_inference_inputs.argtypes = [POINTER(TPUInference)]
 
-libtpu.set_inference_inputs.restype = POINTER(TPUTensorBufferObject)
-libtpu.set_inference_inputs.argtypes = [POINTER(TPUInference), POINTER(TPUTensorBufferObject)]
+libtpu.tpu_set_inference_inputs.restype = POINTER(TPUTensorBufferObject)
+libtpu.tpu_set_inference_inputs.argtypes = [POINTER(TPUInference), POINTER(TPUTensorBufferObject)]
 
-libtpu.get_inference_outputs.restype = POINTER(TPUTensorBufferObject)
-libtpu.get_inference_outputs.argtypes = [POINTER(TPUInference)]
+libtpu.tpu_get_inference_outputs.restype = POINTER(TPUTensorBufferObject)
+libtpu.tpu_get_inference_outputs.argtypes = [POINTER(TPUInference)]
 
-libtpu.set_inference_outputs.restype = POINTER(TPUTensorBufferObject)
-libtpu.set_inference_outputs.argtypes = [POINTER(TPUInference), POINTER(TPUTensorBufferObject)]
+libtpu.tpu_set_inference_outputs.restype = POINTER(TPUTensorBufferObject)
+libtpu.tpu_set_inference_outputs.argtypes = [POINTER(TPUInference), POINTER(TPUTensorBufferObject)]
 
-libtpu.get_inference_status.restype = c_int
-libtpu.get_inference_status.argtypes = [POINTER(TPUInference)]
+libtpu.tpu_get_inference_status.restype = c_int
+libtpu.tpu_get_inference_status.argtypes = [POINTER(TPUInference)]
 
-libtpu.get_inference_error_message.restype = c_char_p
-libtpu.get_inference_error_message.argtypes = [POINTER(TPUInference)]
+libtpu.tpu_get_inference_error_message.restype = c_char_p
+libtpu.tpu_get_inference_error_message.argtypes = [POINTER(TPUInference)]
```

### Comparing `pytpu-14.6.7/pytpu/scripts/pyrun_tpu_cli.py` & `pytpu-14.6.8/pytpu/scripts/pyrun_tpu_cli.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/scripts/run_get_fps.py` & `pytpu-14.6.8/pytpu/scripts/run_get_fps.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/tools/get_fps.py` & `pytpu-14.6.8/pytpu/tools/get_fps.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/tools/helpers.py` & `pytpu-14.6.8/pytpu/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `pytpu-14.6.7/pytpu/tools/tpu_runner.py` & `pytpu-14.6.8/pytpu/tools/tpu_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,28 +89,35 @@
 
     return node_tensor
 
 
 class TpuRunner:
     """Runner for IVA TPU."""
 
-    def __init__(self, program_path: str, loop: Any = None, sync: bool = False, pyprocessing: bool = False) -> None:
+    def __init__(self, program_path: str, device_name: str = None, loop: Any = None, sync: bool = False, pyprocessing: bool = False) -> None:
 
         LOGGER.debug(f'Init TpuRunner with program: {program_path}')
 
         self._pyprocessing = pyprocessing
         self._sync = sync
         self._loop = loop if loop else asyncio.get_event_loop()
 
         tpu_devices = get_tpu_devices()
         if len(tpu_devices) < 1:
             raise EnvironmentError('No TPU devices found')
         
+        # import ipdb; ipdb.set_trace()
+        if device_name is None:
         # device_num = int(list(filter(str.isdigit, tpu_devices[0]))[0])
-        self._device = TPUDevice(tpu_devices[0].encode('utf-8'))
+            self._device = TPUDevice(tpu_devices[0].encode('utf-8'))
+        else:
+            full_name = [name for name in tpu_devices if device_name in name]
+            assert len(full_name) == 1, f'More than one device selected: {full_name}'
+            assert full_name[0] in tpu_devices, f'No such device: {device_name}'
+            self._device = TPUDevice(full_name[0].encode('utf-8'))
         
         if self._device.init() != 0:
             print('\n\nDevice error: {}\n'.format(self._device.get_error().decode('utf-8')))
 
         if pyprocessing:
             with tempfile.TemporaryDirectory() as tempdir:
                 with ZipFile(program_path, 'r') as zip_obj:
```

### Comparing `pytpu-14.6.7/pytpu.egg-info/PKG-INFO` & `pytpu-14.6.8/pytpu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytpu
-Version: 14.6.7
+Version: 14.6.8
 Summary: TPU Python API
 Home-page: http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk
 Author: Alexey Antipin
 Author-email: a.antipin@iva-tech.ru
 License: UNKNOWN
 Description: # IVA TPU Python API
         ## Main entities
```

### Comparing `pytpu-14.6.7/setup.py` & `pytpu-14.6.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #     print(f'Install version: {VERSION}')
 
 setup(
     name='pytpu',
     packages=['pytpu', 'pytpu.tools', 'pytpu.pytpu', 'pytpu.scripts'],
     # packages=find_packages(),
     # version=VERSION,
-    version="14.6.7",
+    version="14.6.8",
     author="Alexey Antipin",
     author_email="a.antipin@iva-tech.ru",
     description="TPU Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.mmp.iva-tech.ru/tpu_sw/iva_tpu_sdk",
     install_requires=[
```

