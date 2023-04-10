# Comparing `tmp/rewards-0.1.0.tar.gz` & `tmp/rewards-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rewards-0.1.0.tar", max compression
+gzip compressed data, was "rewards-0.1.1.tar", max compression
```

## Comparing `rewards-0.1.0.tar` & `rewards-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0    16281 2023-04-07 11:06:54.658349 rewards-0.1.0/README.md
--rw-r--r--   0        0        0      473 2023-04-08 14:02:32.679739 rewards-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        5 2023-04-08 10:26:58.739678 rewards-0.1.0/rewards/VERSION
--rw-r--r--   0        0        0      247 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/__init__.py
--rw-r--r--   0        0        0     3828 2023-04-07 10:49:49.552985 rewards-0.1.0/rewards/agent.py
--rw-r--r--   0        0        0       18 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/assets/CarRace/__init__.py
--rw-r--r--   0        0        0    79384 2023-03-31 17:19:59.957981 rewards-0.1.0/rewards/assets/CarRace/car.png
--rw-r--r--   0        0        0    60297 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/assets/CarRace/track-1.png
--rw-r--r--   0        0        0    42293 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/assets/CarRace/track-2.png
--rw-r--r--   0        0        0    49467 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/assets/CarRace/track-3.png
--rw-r--r--   0        0        0       18 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/assets/__init__.py
--rw-r--r--   0        0        0        0 2023-04-02 06:50:32.365576 rewards-0.1.0/rewards/envs/__init__.py
--rw-r--r--   0        0        0    15306 2023-04-06 14:35:37.602050 rewards-0.1.0/rewards/envs/car.py
--rw-r--r--   0        0        0     5175 2023-04-08 10:35:27.177576 rewards-0.1.0/rewards/models.py
--rw-r--r--   0        0        0     5845 2023-04-08 13:38:08.747967 rewards-0.1.0/rewards/trainer.py
--rw-r--r--   0        0        0     6227 2023-04-08 13:58:58.268032 rewards-0.1.0/rewards/workflow.py
--rw-r--r--   0        0        0    17159 1970-01-01 00:00:00.000000 rewards-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16042 2023-04-10 07:26:34.829243 rewards-0.1.1/README.md
+-rw-r--r--   0        0        0      454 2023-04-10 07:30:00.709535 rewards-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        5 2023-04-10 07:30:13.797553 rewards-0.1.1/rewards/VERSION
+-rw-r--r--   0        0        0      247 2023-04-06 14:35:37.602050 rewards-0.1.1/rewards/__init__.py
+-rw-r--r--   0        0        0     3800 2023-04-09 23:33:00.544889 rewards-0.1.1/rewards/agent.py
+-rw-r--r--   0        0        0       18 2023-04-06 14:35:37.602050 rewards-0.1.1/rewards/assets/CarRace/__init__.py
+-rw-r--r--   0        0        0    79384 2023-03-31 17:19:59.957981 rewards-0.1.1/rewards/assets/CarRace/car.png
+-rw-r--r--   0        0        0    86212 2023-04-09 19:15:07.601577 rewards-0.1.1/rewards/assets/CarRace/evaluation/track-1.png
+-rw-r--r--   0        0        0    60297 2023-04-06 14:35:37.602050 rewards-0.1.1/rewards/assets/CarRace/training/track-1.png
+-rw-r--r--   0        0        0    42293 2023-04-06 14:35:37.602050 rewards-0.1.1/rewards/assets/CarRace/training/track-2.png
+-rw-r--r--   0        0        0    49467 2023-04-06 14:35:37.602050 rewards-0.1.1/rewards/assets/CarRace/training/track-3.png
+-rw-r--r--   0        0        0       18 2023-04-06 14:35:37.602050 rewards-0.1.1/rewards/assets/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-02 06:50:32.365576 rewards-0.1.1/rewards/envs/__init__.py
+-rw-r--r--   0        0        0    15740 2023-04-10 07:04:33.071374 rewards-0.1.1/rewards/envs/c.py
+-rw-r--r--   0        0        0    17030 2023-04-10 00:10:25.051719 rewards-0.1.1/rewards/envs/car.py
+-rw-r--r--   0        0        0     5262 2023-04-09 22:53:21.460200 rewards-0.1.1/rewards/models.py
+-rw-r--r--   0        0        0     6153 2023-04-09 23:46:27.999270 rewards-0.1.1/rewards/trainer.py
+-rw-r--r--   0        0        0     5347 2023-04-10 00:12:48.092137 rewards-0.1.1/rewards/workflow.py
+-rw-r--r--   0        0        0    16880 1970-01-01 00:00:00.000000 rewards-0.1.1/PKG-INFO
```

### Comparing `rewards-0.1.0/README.md` & `rewards-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -119,25 +119,14 @@
 | LAYER_CONFIG       | `List[List[int]]` | This expects a list of list. Where the inner list will have only two values [input neurons, output neurons]. This configuration will help us to build the neural network for our agent. The first value for the current environment must be 3. | [[5, 64], [64, 3]] | Here user can add more values but the values `5` in the first and `3` in the last must be fixed for this current environment that we are supporting. Example: <br> `[[5, ...], [..., ...], ...., [..., 3]]`, <br> Where `...` can be any value. We recommend to keep it between (1 - 256) |
 | CHECKPOINT_FOLDER_PATH    | `str`             | The model checkpoint path from where it should be loaded. This can be either `None` then it will auto create a checkpoint path and store all the checkpoints there else it will save the models on the folder mentioned if exists.                                                                                                                                                                                      | `./saved_models`                                                                                                 | User's choice                                                                                                                                                                                                                                                                         |
 | CHECKPOINT_MODEL_NAME    | `str`             | The name of the model name. This can be either named by the user or by default it will create the model name as `model_{<latest_date_and_time>}_.pth`.                                                                                                                                                                                       | `model_2023-04-07 16:10:36.366395_.pth` (This is just an example)                                                                                                 | User's choice                                                                                                                                                                                                                                                                         |
 | REWARD_FUNCTION    | `Callable`        | Users are expected to write some reward function (`Callable`) and then have to use this reward function for agent's training.|  ```def default_reward_function(props): if props["isAlive"]: return 1 return 0 ```| User's choice <br> **some important parameters** <br><br> `isAlive` represents whether the car is alive or not. So on that basis we can penalize our agent. <br><br> `obs` The car's radar's oberservations values. (more on documentation) <br> <br>`rotationVel` Car's rotational velocity value (more on documentation)        |
 
 
 So above is a quick overview of how to use different reward configurations. Now once configuration part is done, load those configuration to `RLWorkFlow()` and run for a single episodes. 
-**NOTE:** Make sure you have `weights and biases` installed. You can install that using:
-
-```bash
-pip install wandb
-```
-
-After this log in / create a new account. Then authorize it inside the command line by typing
-
-```bash
-wandb auth
-```
 
 After this you are ready to run the above code:
 
 ```python 
 from rewards import workflow
 
 configs = workflow.WorkFlowConfigurations(
```

### Comparing `rewards-0.1.0/rewards/agent.py` & `rewards-0.1.1/rewards/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import numpy as np
 import torch
 
-# TODO:
-# - Use Hydra for configuration management
-
-
 @dataclass
 class AgentConf:
     MAX_MEMORY: int = 100000
     BATCH_SIZE: int = 1000
     PARENT_PATH: str = str(Path(__file__).parent.parent)
     DEVICE: str = "cpu"
 
@@ -95,15 +91,15 @@
         """
         Args:
             state (_type_): _description_
 
         Returns:
             _type_: _description_
         """
-        self.epsilon = 25
+        self.epsilon = 25 # self.epsilon (WHY NOT)
         final_move = [
             0,
             0,
             0,
         ]  # TODO: need to make a general array of zeros which matches with the length of action
 
         if random.randint(0, 100) < self.epsilon:
```

### Comparing `rewards-0.1.0/rewards/assets/CarRace/car.png` & `rewards-0.1.1/rewards/assets/CarRace/car.png`

 * *Files identical despite different names*

### Comparing `rewards-0.1.0/rewards/assets/CarRace/track-1.png` & `rewards-0.1.1/rewards/assets/CarRace/training/track-1.png`

 * *Files identical despite different names*

### Comparing `rewards-0.1.0/rewards/assets/CarRace/track-2.png` & `rewards-0.1.1/rewards/assets/CarRace/training/track-2.png`

 * *Files identical despite different names*

### Comparing `rewards-0.1.0/rewards/assets/CarRace/track-3.png` & `rewards-0.1.1/rewards/assets/CarRace/training/track-3.png`

 * *Files identical despite different names*

### Comparing `rewards-0.1.0/rewards/envs/car.py` & `rewards-0.1.1/rewards/envs/c.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,18 @@
         self.CAR_RECT_SIZE: Tuple[int, int] = (200, 50)
         self.CAR_VELOCITY_VECTOR: Tuple[float, float] = (0.8, 0.0)
         self.CAR_ROTATION_VELOCITY: Union[int, float] = 15
         self.CAR_DIRECTION: Union[int, float] = 0
         self.CAR_IS_ALIVE: bool = True
         self.CAR_REWARD: int = (0,)
         self.CAR_RADAR: List[Union[int, float]] = [0, 0, 0, 0, 0]
+        
+        # pygame screen type 
+        # there are two options ("surface", display)
+        self.PYGAME_SCREEN_TYPE : str = "display"
 
 
 ######################### Track Class #########################
 
 
 class Track(CarConfig):
     def __init__(self, track_num: int = 0):
@@ -65,15 +69,15 @@
 
         print(self.ASSET_PATH)
         print(self.CAR_ANGLE)
         print(self.CAR_VELOCITY_VECTOR)
         print(self.CAR_TRACKS)
 
         self.track_image_path = os.path.join(
-            self.ASSET_PATH, self.CAR_TRACKS[track_num]
+            self.ASSET_PATH, "training", self.CAR_TRACKS[track_num]
         ).replace(os.sep, '/')
 
         self.car_image_path = os.path.join(self.ASSET_PATH, self.CAR_IMAGE)
 
         self.track_image = pygame.image.load(self.track_image_path)
         self.car_image = pygame.transform.scale(
             pygame.image.load(self.car_image_path),
@@ -89,15 +93,14 @@
 
 ####################### CarGame #########################
 
 
 class CarGame(Track):
     def __init__(
         self,
-        frame: Optional[Any] = None,
         track_num: Optional[int] = 0,
         reward_func: Optional[Union[str, Callable]] = None,
     ) -> None:
         """### CarGame Environment:
 
         This is the reward's CarGame environment. There are mainly 4 main types of operations under which this environment operates.
         Those are as follows:
@@ -111,32 +114,36 @@
         Although it does not make the agent learn anything. So we expect users to use their custom reward function to make the
         car agent to gain max reward and make it go brumm brummm !!
 
         Rewards has three different training environments to make the agent learn. It also has 2 Test environments for testing.
         In the future version we will let user to make/design their own car training environment and train their agents their.
 
         Args:
-            frame (Optional[Any], optional): The current pygame frame. Defaults to None.
             track_num (Optional[int], optional): The . Defaults to 0.
             reward_func (Optional[Union[str, Callable]], optional): The reward function. Defaults to None.
         """
 
         # we need to also keep in track with the track's default asset parent folder path and it's other paths
         # we also need to design a way where user can make their own environment asset and use them by sucessfully integrating them to rewards
 
         super(CarGame, self).__init__(track_num=track_num)
 
-        self.screen = pygame.display.set_mode(self.SCREEN_SIZE)
+        if self.PYGAME_SCREEN_TYPE == "display":
+            self.screen = pygame.display.set_mode(self.SCREEN_SIZE)
+        else:
+            self.screen = pygame.Surface(self.SCREEN_SIZE) 
+            
         self.screen.fill((0, 0, 0))
         self.params = {
             "is_alive": None,
             "observation": None,
             "direction": None,
             "rotational_velocity": None,
         }
+        
 
         # TODO: Change this (car_image, original_image, image confusion and make proper usage and naming of the variables)
 
         self.angle = self.CAR_ANGLE
         self.original_image = self.car_image
         self.image = pygame.transform.rotozoom(
             self.original_image, self.angle, 0.1
@@ -151,17 +158,15 @@
         self.reward = 0
         self.radars = self.CAR_RADAR
 
         self.clock = pygame.time.Clock()
         self.track = self.track_image
         self.FPS = self.CAR_FPS
         self.iterations = 0
-        self.reward_func = (
-            self._default_reward_func
-        )  # (self._default_reward_func if reward_func is None else reward_func)
+        self.reward_func = self._default_reward_func if reward_func is None else reward_func
 
     def initialize(self) -> None:
         """Initializes the game state from where it had started"""
         # The below needs to change as this will do those flikering stuffs
         # self.screen = pygame.display.set_mode(self.SCREEN_SIZE)
 
         self.angle = self.CAR_ANGLE
@@ -193,14 +198,16 @@
 
         Args:
             props (Dict[str, Any]): properties as arguments containing a dict of parameter
 
         Returns:
             int: The reward
         """
+        # TODO: Change the default reward function, this is the actual reward function 
+        
         reward = 0
         if props["isAlive"]:
             reward = 1
         obs = props["obs"]
         if obs[0] < obs[-1] and props["dir"] == -1:
             reward += 1
             if props["rotationVel"] == 7 or props["rotationVel"] == 10:
@@ -417,8 +424,13 @@
             0,
         ]  # TODO: We have already initialised radars before, is there any need to initialize it here.
         self._drive()
 
         current_state_params = self.get_current_state(action=action)
         current_reward = self.reward_func(current_state_params)
         self.reward += current_reward
-        return current_reward, not self.alive, self.reward
+        
+        if self.PYGAME_SCREEN_TYPE == "surface":
+            pixel_data = pygame.surfarray.array3d(self.screen)
+            return current_reward, not self.alive, self.reward, pixel_data
+        else:
+            return current_reward, not self.alive, self.reward
```

### Comparing `rewards-0.1.0/rewards/models.py` & `rewards-0.1.1/rewards/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 
 
-DEFAULT_MODEL_PATH = './saved_models'
+DEFAULT_MODEL_PATH = './saved_models/'
 
 class DeepNet(nn.Module):
     """
     Base Class for all the models that will be added from here and inherited from this class.
     """
 
     def __init__(self) -> None:
@@ -59,15 +59,15 @@
         """Loads the model in a robust file structure and setting 
 
         Args:
             checkpoint_folder_path (Optional[str], optional): The model checkpoint folder where all the checkpoints are been saved. Defaults to None.
             model_name (Optional[str], optional): The name of the model to save. Defaults to None.
         """
         if checkpoint_folder_path and len(os.listdir(checkpoint_folder_path)) > 0:
-            
+            print(checkpoint_folder_path, self._get_file_list_mod_by_date(checkpoint_folder_path))
             _model_name = self._get_file_list_mod_by_date(checkpoint_folder_path)[0] if model_name is None else model_name 
             model_path = os.path.join(checkpoint_folder_path, _model_name)
             try:
                 self.load_state_dict(
                     torch.load(
                         model_path,
                         map_location=device,
```

### Comparing `rewards-0.1.0/rewards/trainer.py` & `rewards-0.1.1/rewards/trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.optim as optim
 
 from .agent import Agent
+from .envs.car import CarGame
 
 # TODO:
 # - Move RMSE, MAE to utils module
 
 
 class RootMeanSquaredError(torch.nn.Module):
     def __init__(self):
@@ -126,15 +127,15 @@
         self.optimizer.zero_grad()
         loss = self.criterion(state_target, state_prediction)
         loss.backward()
         self.optimizer.step()
 
     def train_long_memory(self) -> None:
         """Trains the agent for a longer step saving state-actions to the memory
-
+     print("stepping")
         Returns:
             None
         """
         if len(self.memory) > self.BATCH_SIZE:
             mini_sample = random.sample(self.memory, self.BATCH_SIZE)
         else:
             mini_sample = self.memory
@@ -153,28 +154,34 @@
             done (function): _description_
 
         Returns:
             _type_: _description_
         """
         return self.step(state, action, reward, next_state, done)
 
-    def train_step(self, game: Any) -> List[Union[int, float, bool]]:
+    def train_step(self, game: CarGame) -> List[Union[int, float, bool]]:
         """
         Defines a single train step for an agent where the agent performs
         some action in a given state to get next state, current rewards, and
         its status of completion
 
         Args:
             game (Any): The game environment
 
         Returns:
             (List[Union[int, float], bool, Union[int, float]]) : [current_reward, done, score]
         """
 
         state_old = self.get_state(game)
         final_move = self.get_action(state_old)
-        reward, done, score = game.play_step(final_move)
+        
+        if game.PYGAME_SCREEN_TYPE == "surface":
+            reward, done, score, pixel_data = game.play_step(final_move)
+        
+        else:
+            reward, done, score = game.play_step(final_move)
+            
         state_new = self.get_state(game)
         self.train_short_memory(state_old, final_move, reward, state_new, done)
         self.remember(state_old, final_move, reward, state_new, done)
 
-        return reward, done, score
+        return [reward, done, score, pixel_data] if game.PYGAME_SCREEN_TYPE == "surface" else [reward, done, score]
```

### Comparing `rewards-0.1.0/rewards/workflow.py` & `rewards-0.1.1/rewards/workflow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,22 @@
+import cv2 
 import sys 
 import time 
 import inspect
 from dataclasses import dataclass
 from typing import Callable, List, Optional, Tuple, Union
 
-import pandas as pd
+import pandas as pdsys
 import pygame
 import torch
-import wandb
 
 from .envs.car import CarGame
 from .models import LinearQNet
 from .trainer import QTrainer
 
-# TODO: Make a video recording feature (that will record and upload to W&B dashboard once training is complete)
-# TODO: Things that is to be tracked in wandb
-
-# - Live metrics of the plots
-# - CPU usages (default)
-# - All the configurations
-# - Once experiment is complete then upload the recorded pygame environment
-
-
-def default_reward_function(props):
-    if props["isAlive"]:
-        return 1
-    return 0
-
 
 @dataclass(kw_only=True)
 class WorkFlowConfigurations:
     # wandb experiment
     DEVICE : str = "cpu"
     # Environment configuration
 
@@ -57,105 +43,96 @@
 
     CHECKPOINT_FOLDER_PATH: Optional[str] = None
     CHECKPOINT_MODEL_NAME: Optional[str] = None
     REWARD_FUNCTION: Callable = None # required 
 
     # Tracking configuration 
     ENABLE_WANDB : bool = False 
+    
+    # Newly added 
+    
+    MODE : str = "training"
+    PYGAME_WINDOW_TYPE : str = "display"
 
 class RLWorkFlow:
     def __init__(
-        self, experiment_configuration: Optional[WorkFlowConfigurations] = None
-    ) -> None:
+        self, experiment_configuration: Optional[WorkFlowConfigurations] = None) -> None:
         """
         **RLWorkFlow** is the module which ables us to run complete RL experiments
         """
 
         self.config = (
             WorkFlowConfigurations()
             if experiment_configuration is None
             else experiment_configuration
         )
 
         # Build model
         if isinstance(self.config.LAYER_CONFIG, torch.nn.Module):
             self.model = self.config.LAYER_CONFIG
         else:
-            self.model = LinearQNet(self.config.LAYER_CONFIG) if self.config.LAYER_CONFIG is not None else LinearQNet([[5, 64], [64, 3]])
+            self.model = LinearQNet(
+                self.config.LAYER_CONFIG) if self.config.LAYER_CONFIG is not None else LinearQNet([[5, 64], [64, 3]])
 
         # Build Agent
         self.agent = QTrainer(
             lr=self.config.LR,
             gamma=self.config.GAMMA,
             epsilon=self.config.EPSILON,
             model=self.model,
             loss=self.config.LOSS,
             optimizer=self.config.OPTIMIZER,
             checkpoint_folder_path=self.config.CHECKPOINT_FOLDER_PATH,
             model_name = self.config.CHECKPOINT_MODEL_NAME
         )
 
-        # Once everything is done then upload all configurations to wandb
-        
-        if self.config.ENABLE_WANDB:
-            wandb_config = self.config.__dict__.copy()
-            wandb_config["REWARD_FUNCTION"] = inspect.getsource(
-                self.config.REWARD_FUNCTION if self.config.REWARD_FUNCTION is not None else default_reward_function
-            )
-
-            if isinstance(self.model, torch.nn.Module):
-                wandb_config.pop("LAYER_CONFIG")
-                # Also upload the model to wandb artifact 
-                
-            wandb_config.pop("CHECKPOINT_FOLDER_PATH")
-
-            self.run = wandb.init(
-                project=self.config.EXPERIMENT_NAME, config=wandb_config
-            )
-            
-        if self.config.ENABLE_WANDB:
-            config_dataframe = pd.DataFrame(
-                data={
-                    "configuration name": list(wandb_config.keys()),
-                    "configuration": [
-                        str(ele) for ele in list(wandb_config.values())
-                    ],
-                }
-            )
-        
-            config_table = wandb.Table(dataframe=config_dataframe)
-            config_table_artifact = wandb.Artifact(
-                "configuration_artifact", type="dataset"
-            )
-            config_table_artifact.add(config_table, "configuration_table")
-
-            self.run.log({"Configuration": config_table})
-            self.run.log_artifact(config_table_artifact)
-
-        
-        self.reward_func = self.config.REWARD_FUNCTION if self.config.REWARD_FUNCTION is not None else default_reward_function
+        self.reward_func = self.config.REWARD_FUNCTION if self.config.REWARD_FUNCTION is not None else None 
+        print("=> All configs done and saved")
 
-    def stop_game(self):
-        for event in pygame.event.get():
-            if event.type == pygame.QUIT:
-                pygame.quit()
-    
-    def run_episodes(self):
-        # Build PyGame
-        self.screen = pygame.display.set_mode(
-            self.config.SCREEN_SIZE, pygame.HIDDEN
-        )
-        
         self.game = CarGame(
-            frame=self.screen,
-            track_num=self.config.ENVIRONMENT_WORLD,
-            reward_func=self.reward_func,
+            mode=self.config.MODE, 
+            track_num=self.config.ENVIRONMENT_WORLD, 
+            reward_function=self.reward_func, 
+            display_type=self.config.PYGAME_WINDOW_TYPE, 
+            screen_size=self.config.SCREEN_SIZE
         )
+    
+    
+    def stream_single_episode(self):
+        done = False 
+        while not done and self.config.PYGAME_WINDOW_TYPE == "surface":
+            _, done, score, pixel_data = self.agent.train_step(self.game)
+            yield {
+                'data' : pixel_data, 
+                'score' : score,
+            }
+                
+    def stream_multi_episodes(self):
+        for episode in range(1, self.config.NUM_EPISODES + 1):
+            self.game.initialize()
+            self.game.FPS = self.config.CAR_SPEED
+            total_score, record = 0, 0
+            
+            for streamed_responses in self.stream_single_episode():
+                cv2.imshow('Frame', streamed_responses['data'])
+                if cv2.waitKey(20) & 0xFF == ord('q'):
+                    sys.exit() 
+            
+            score = streamed_responses['score']
+            if score > record:
+                    self.agent.model.save(
+                        self.config.CHECKPOINT_FOLDER_PATH, 
+                        self.config.CHECKPOINT_MODEL_NAME, self.config.DEVICE
+                    )
+                    record = score 
+            total_score += score 
+        print("=> Process finished")
+        cv2.destroyAllWindows()
         
-        
+    def run_episodes(self):
         for episode in range(1, self.config.NUM_EPISODES + 1):
             self.game.initialize() # change it to env.reset() 
             self.game.FPS = self.config.CAR_SPEED
             total_score, record = 0, 0
             done = False 
             
             try:
@@ -174,16 +151,12 @@
                 total_score += score 
                 
                 episode_response = {
                     "episode_num" : episode, 
                     "episode score": score,
                     "mean score": total_score / self.agent.n_games
                 }
-                
-                if self.agent.n_games != 0 and self.config.ENABLE_WANDB:
-                    self.run.log(episode_response)
-                yield episode_response
             
             except pygame.error:
                 pygame.quit() 
                 break 
         print("=> Process finished")
```

### Comparing `rewards-0.1.0/PKG-INFO` & `rewards-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rewards
-Version: 0.1.0
+Version: 0.1.1
 Summary: Start learning about RL and make model and envs in minutes in just few lines of code
 License: MIT
 Author: rewards.ai
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pygame (>=2.3.0,<3.0.0)
 Requires-Dist: torch (>=2.0.0,<3.0.0)
-Requires-Dist: wandb (>=0.14.1,<0.15.0)
 Description-Content-Type: text/markdown
 
 # **rewards** 
 ### A low code sdk for crearing custom environments and deep RL agents. 
 
 
 <br>
@@ -142,25 +141,14 @@
 | LAYER_CONFIG       | `List[List[int]]` | This expects a list of list. Where the inner list will have only two values [input neurons, output neurons]. This configuration will help us to build the neural network for our agent. The first value for the current environment must be 3. | [[5, 64], [64, 3]] | Here user can add more values but the values `5` in the first and `3` in the last must be fixed for this current environment that we are supporting. Example: <br> `[[5, ...], [..., ...], ...., [..., 3]]`, <br> Where `...` can be any value. We recommend to keep it between (1 - 256) |
 | CHECKPOINT_FOLDER_PATH    | `str`             | The model checkpoint path from where it should be loaded. This can be either `None` then it will auto create a checkpoint path and store all the checkpoints there else it will save the models on the folder mentioned if exists.                                                                                                                                                                                      | `./saved_models`                                                                                                 | User's choice                                                                                                                                                                                                                                                                         |
 | CHECKPOINT_MODEL_NAME    | `str`             | The name of the model name. This can be either named by the user or by default it will create the model name as `model_{<latest_date_and_time>}_.pth`.                                                                                                                                                                                       | `model_2023-04-07 16:10:36.366395_.pth` (This is just an example)                                                                                                 | User's choice                                                                                                                                                                                                                                                                         |
 | REWARD_FUNCTION    | `Callable`        | Users are expected to write some reward function (`Callable`) and then have to use this reward function for agent's training.|  ```def default_reward_function(props): if props["isAlive"]: return 1 return 0 ```| User's choice <br> **some important parameters** <br><br> `isAlive` represents whether the car is alive or not. So on that basis we can penalize our agent. <br><br> `obs` The car's radar's oberservations values. (more on documentation) <br> <br>`rotationVel` Car's rotational velocity value (more on documentation)        |
 
 
 So above is a quick overview of how to use different reward configurations. Now once configuration part is done, load those configuration to `RLWorkFlow()` and run for a single episodes. 
-**NOTE:** Make sure you have `weights and biases` installed. You can install that using:
-
-```bash
-pip install wandb
-```
-
-After this log in / create a new account. Then authorize it inside the command line by typing
-
-```bash
-wandb auth
-```
 
 After this you are ready to run the above code:
 
 ```python 
 from rewards import workflow
 
 configs = workflow.WorkFlowConfigurations(
```

