# Comparing `tmp/basic-pitch-0.2.3.tar.gz` & `tmp/basic-pitch-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basic-pitch-0.2.3.tar", last modified: Tue Feb 28 15:36:37 2023, max compression
+gzip compressed data, was "basic-pitch-0.2.4.tar", last modified: Mon Apr 10 16:04:35 2023, max compression
```

## Comparing `basic-pitch-0.2.3.tar` & `basic-pitch-0.2.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.691347 basic-pitch-0.2.3/
--rw-r--r--   0 jgao       (501) staff       (20)     7365 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 jgao       (501) staff       (20)     3559 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 jgao       (501) staff       (20)    11384 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/LICENSE
--rw-r--r--   0 jgao       (501) staff       (20)      241 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/MANIFEST.in
--rw-r--r--   0 jgao       (501) staff       (20)     1034 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/NOTICE
--rw-r--r--   0 jgao       (501) staff       (20)     1110 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/OWNERS.md
--rw-r--r--   0 jgao       (501) staff       (20)     1160 2023-02-28 15:36:37.691444 basic-pitch-0.2.3/PKG-INFO
--rw-r--r--   0 jgao       (501) staff       (20)     8266 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/README.md
--rw-r--r--   0 jgao       (501) staff       (20)      970 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/SECURITY.md
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.645141 basic-pitch-0.2.3/basic_pitch/
--rw-r--r--   0 jgao       (501) staff       (20)     1009 2023-02-28 15:35:38.000000 basic-pitch-0.2.3/basic_pitch/__init__.py
--rw-r--r--   0 jgao       (501) staff       (20)     2299 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/commandline_printing.py
--rw-r--r--   0 jgao       (501) staff       (20)     2243 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/constants.py
--rw-r--r--   0 jgao       (501) staff       (20)    17170 2023-02-28 15:35:38.000000 basic-pitch-0.2.3/basic_pitch/inference.py
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.661916 basic-pitch-0.2.3/basic_pitch/layers/
--rw-r--r--   0 jgao       (501) staff       (20)        0 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/layers/__init__.py
--rw-r--r--   0 jgao       (501) staff       (20)      981 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/layers/math.py
--rw-r--r--   0 jgao       (501) staff       (20)    26142 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/layers/nnaudio.py
--rw-r--r--   0 jgao       (501) staff       (20)     7258 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/layers/signal.py
--rw-r--r--   0 jgao       (501) staff       (20)     9870 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/models.py
--rw-r--r--   0 jgao       (501) staff       (20)     3988 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/nn.py
--rw-r--r--   0 jgao       (501) staff       (20)    18920 2023-02-28 15:35:38.000000 basic-pitch-0.2.3/basic_pitch/note_creation.py
--rw-r--r--   0 jgao       (501) staff       (20)     4862 2023-02-28 15:35:38.000000 basic-pitch-0.2.3/basic_pitch/predict.py
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.587207 basic-pitch-0.2.3/basic_pitch/saved_models/
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.588271 basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.664895 basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/
--rw-r--r--   0 jgao       (501) staff       (20)  1084140 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.672269 basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/variables/
--rw-r--r--   0 jgao       (501) staff       (20)   219309 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
--rw-r--r--   0 jgao       (501) staff       (20)     4794 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.649427 basic-pitch-0.2.3/basic_pitch.egg-info/
--rw-r--r--   0 jgao       (501) staff       (20)     1160 2023-02-28 15:36:37.000000 basic-pitch-0.2.3/basic_pitch.egg-info/PKG-INFO
--rw-r--r--   0 jgao       (501) staff       (20)     1040 2023-02-28 15:36:37.000000 basic-pitch-0.2.3/basic_pitch.egg-info/SOURCES.txt
--rw-r--r--   0 jgao       (501) staff       (20)        1 2023-02-28 15:36:37.000000 basic-pitch-0.2.3/basic_pitch.egg-info/dependency_links.txt
--rw-r--r--   0 jgao       (501) staff       (20)       57 2023-02-28 15:36:37.000000 basic-pitch-0.2.3/basic_pitch.egg-info/entry_points.txt
--rw-r--r--   0 jgao       (501) staff       (20)        1 2023-02-27 16:32:34.000000 basic-pitch-0.2.3/basic_pitch.egg-info/not-zip-safe
--rw-r--r--   0 jgao       (501) staff       (20)      361 2023-02-28 15:36:37.000000 basic-pitch-0.2.3/basic_pitch.egg-info/requires.txt
--rw-r--r--   0 jgao       (501) staff       (20)       12 2023-02-28 15:36:37.000000 basic-pitch-0.2.3/basic_pitch.egg-info/top_level.txt
--rw-r--r--   0 jgao       (501) staff       (20)      115 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/catalog-info.yaml
--rw-r--r--   0 jgao       (501) staff       (20)     1749 2023-02-28 15:36:37.692454 basic-pitch-0.2.3/setup.cfg
--rw-r--r--   0 jgao       (501) staff       (20)      686 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/setup.py
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.680596 basic-pitch-0.2.3/tests/
-drwxr-xr-x   0 jgao       (501) staff       (20)        0 2023-02-28 15:36:37.688395 basic-pitch-0.2.3/tests/resources/
--rw-r--r--   0 jgao       (501) staff       (20)   802472 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/tests/resources/vocadito_10.wav
--rw-r--r--   0 jgao       (501) staff       (20)  1075892 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/tests/resources/vocadito_14.wav
--rw-r--r--   0 jgao       (501) staff       (20)     4851 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/tests/test_inference.py
--rw-r--r--   0 jgao       (501) staff       (20)     3861 2023-02-03 15:59:18.000000 basic-pitch-0.2.3/tests/test_nn.py
--rw-r--r--   0 jgao       (501) staff       (20)     2115 2023-02-23 19:08:24.000000 basic-pitch-0.2.3/tests/test_note_creation.py
--rw-r--r--   0 jgao       (501) staff       (20)     1120 2023-02-23 19:08:24.000000 basic-pitch-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/OWNERS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/commandline_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/inference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26142 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/nnaudio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/layers/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.636003 basic-pitch-0.2.4/basic_pitch/saved_models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.636003 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/
+-rw-r--r--   0 runner    (1001) docker     (123)  1084140 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)   219309 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/basic_pitch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 16:04:35.000000 basic-pitch-0.2.4/basic_pitch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/catalog-info.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.640003 basic-pitch-0.2.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:04:35.644003 basic-pitch-0.2.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   802472 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/resources/vocadito_10.wav
+-rw-r--r--   0 runner    (1001) docker     (123)  1075892 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/resources/vocadito_14.wav
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tests/test_note_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-10 16:04:21.000000 basic-pitch-0.2.4/tox.ini
```

### Comparing `basic-pitch-0.2.3/CODE_OF_CONDUCT.md` & `basic-pitch-0.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/CONTRIBUTING.md` & `basic-pitch-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/LICENSE` & `basic-pitch-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/NOTICE` & `basic-pitch-0.2.4/NOTICE`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/OWNERS.md` & `basic-pitch-0.2.4/OWNERS.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/PKG-INFO` & `basic-pitch-0.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.2.3
+Version: 0.2.4
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Home-page: https://github.com/spotify/basic-pitch
 Author: Spotify
 Author-email: basic-pitch@spotify.com
 Maintainer: Spotify
 Maintainer-email: basic-pitch@spotify.com
 License: Apache 2.0
```

### Comparing `basic-pitch-0.2.3/README.md` & `basic-pitch-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,19 @@
 
 This library offers a command line tool interface. A basic prediction command will generate and save a MIDI file transcription of audio at the `<input-audio-path>` to the `<output-directory>`:
 
 ```bash
 basic-pitch <output-directory> <input-audio-path>
 ```
 
+For example: 
+```
+basic-pitch /output/directory/path /input/audio/path
+```
+
 To process more than one audio file at a time:
 
 ```bash
 basic-pitch <output-directory> <input-audio-path-1> <input-audio-path-2> <input-audio-path-3>
 ```
 
 Optionally, you may append any of the following flags to your prediction command to save additional formats of the prediction output to the `<output-directory>`:
@@ -82,15 +87,15 @@
 
 Import `basic-pitch` into your own Python code and run the [`predict`](basic_pitch/inference.py) functions directly, providing an `<input-audio-path>` and returning the model's prediction results:
 
 ```python
 from basic_pitch.inference import predict
 from basic_pitch import ICASSP_2022_MODEL_PATH
 
-model_output, midi_data, note_activations = predict(<input-audio-path>)
+model_output, midi_data, note_events = predict(<input-audio-path>)
 ```
 
 - `<minimum-frequency>` & `<maximum-frequency>` (*float*s) set the maximum and minimum allowed note frequency, in Hz, returned by the model. Pitch events with frequencies outside of this range will be excluded from the prediction results.
 - `model_output` is the raw model inference output
 - `midi_data` is the transcribed MIDI data derived from the `model_output`
 - `note_events` is a list of note events derived from the `model_output`
 
@@ -104,15 +109,15 @@
 from basic_pitch.inference import predict
 from basic_pitch import ICASSP_2022_MODEL_PATH
 
 basic_pitch_model = tf.saved_model.load(str(ICASSP_2022_MODEL_PATH))
 
 for x in range():
     ...
-    model_output, midi_data, note_activations = predict(
+    model_output, midi_data, note_events = predict(
         <loop-x-input-audio-path>,
         basic_pitch_model,
     )
     ...
 ```
 
 **predict_and_save()**
@@ -124,28 +129,28 @@
 
 predict_and_save(
     <input-audio-path-list>,
     <output-directory>,
     <save-midi>,
     <sonify-midi>,
     <save-model-outputs>,
-    <save-note-events>,
+    <save-notes>,
 )
 ```
 
 where:
    - `<input-audio-path-list>` & `<output-directory>`
         - directory paths for `basic-pitch` to read from/write to.
    - `<save-midi>`
         - *bool* to control generating and saving a MIDI file to the `<output-directory>`
    - `<sonify-midi>`
         - *bool* to control saving a WAV audio rendering of the MIDI file to the `<output-directory>`
    - `<save-model-outputs>`
         - *bool* to control saving the raw model output as a NPZ file to the `<output-directory>`
-   - `<save-note-events>`
+   - `<save-notes>`
         - *bool* to control saving predicted note events as a CSV file `<output-directory>`
 
 
 
 ### Model Input
 
 **Supported Audio Codecs**
```

### Comparing `basic-pitch-0.2.3/SECURITY.md` & `basic-pitch-0.2.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/__init__.py` & `basic-pitch-0.2.4/basic_pitch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import pathlib
 
 __author__ = "Spotify"
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 __email__ = "basic-pitch@spotify.com"
 __demowebsite__ = "https://basicpitch.io"
 __description__ = "Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection."
 __url__ = "https://github.com/spotify/basic-pitch"
 
 ICASSP_2022_MODEL_PATH = pathlib.Path(__file__).parent / "saved_models/icassp_2022/nmp"
```

### Comparing `basic-pitch-0.2.3/basic_pitch/commandline_printing.py` & `basic-pitch-0.2.4/basic_pitch/commandline_printing.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/constants.py` & `basic-pitch-0.2.4/basic_pitch/constants.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/inference.py` & `basic-pitch-0.2.4/basic_pitch/inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/layers/math.py` & `basic-pitch-0.2.4/basic_pitch/layers/math.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/layers/nnaudio.py` & `basic-pitch-0.2.4/basic_pitch/layers/nnaudio.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/layers/signal.py` & `basic-pitch-0.2.4/basic_pitch/layers/signal.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/models.py` & `basic-pitch-0.2.4/basic_pitch/models.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/nn.py` & `basic-pitch-0.2.4/basic_pitch/nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/note_creation.py` & `basic-pitch-0.2.4/basic_pitch/note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/predict.py` & `basic-pitch-0.2.4/basic_pitch/predict.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb` & `basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/saved_model.pb`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001` & `basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index` & `basic-pitch-0.2.4/basic_pitch/saved_models/icassp_2022/nmp/variables/variables.index`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/basic_pitch.egg-info/PKG-INFO` & `basic-pitch-0.2.4/basic_pitch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basic-pitch
-Version: 0.2.3
+Version: 0.2.4
 Summary: Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
 Home-page: https://github.com/spotify/basic-pitch
 Author: Spotify
 Author-email: basic-pitch@spotify.com
 Maintainer: Spotify
 Maintainer-email: basic-pitch@spotify.com
 License: Apache 2.0
```

### Comparing `basic-pitch-0.2.3/basic_pitch.egg-info/SOURCES.txt` & `basic-pitch-0.2.4/basic_pitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/setup.cfg` & `basic-pitch-0.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.3
+current_version = 0.2.4
 commit = True
 tag = True
 
 [metadata]
 name = basic-pitch
 version = attr: basic_pitch.__version__
 description = Basic Pitch, a lightweight yet powerful audio-to-MIDI converter with pitch bend detection.
@@ -35,16 +35,16 @@
 install_requires = 
 	librosa>=0.8.0
 	mir_eval>=0.6
 	numpy<1.24,>=1.18
 	pretty_midi>=0.2.9
 	resampy>=0.2.2
 	scipy>=1.4.1
-	tensorflow>=2.4.1,<2.10; platform_machine != 'arm64'
-	tensorflow-macos>=2.4.1,<2.10; platform_machine == 'arm64'
+	tensorflow>=2.4.1,<2.12; platform_machine != 'arm64'
+	tensorflow-macos>=2.4.1,<2.12; platform_machine == 'arm64'
 	typing_extensions
 
 [options.entry_points]
 console_scripts = 
 	basic-pitch = basic_pitch.predict:main
 
 [options.extras_require]
```

### Comparing `basic-pitch-0.2.3/setup.py` & `basic-pitch-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/tests/resources/vocadito_10.wav` & `basic-pitch-0.2.4/tests/resources/vocadito_10.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/tests/resources/vocadito_14.wav` & `basic-pitch-0.2.4/tests/resources/vocadito_14.wav`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/tests/test_inference.py` & `basic-pitch-0.2.4/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/tests/test_nn.py` & `basic-pitch-0.2.4/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/tests/test_note_creation.py` & `basic-pitch-0.2.4/tests/test_note_creation.py`

 * *Files identical despite different names*

### Comparing `basic-pitch-0.2.3/tox.ini` & `basic-pitch-0.2.4/tox.ini`

 * *Files identical despite different names*

