# Comparing `tmp/donatellopyzza-1.6.1.tar.gz` & `tmp/donatellopyzza-1.6.2.tar.gz`

## Comparing `donatellopyzza-1.6.1.tar` & `donatellopyzza-1.6.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/__init__.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/assessor.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/envBuilder.py
--rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/game.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/main.py
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/mazeGenerator.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/turtleAgent.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/environments/assessment_maze.png
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/environments/assessment_maze.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/environments/hard_maze.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/environments/maze.txt
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/environments/test.png
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/environments/test.txt
--rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/images/pizza.png
--rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/images/turtle.png
--rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/data/images/turtle_small.png
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/agent.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/careTaker.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/constants.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/grid.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/gui.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/map.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/memento.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/orientation.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/originator.py
--rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/parser.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/square.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/donatellopyzza/grid/turn.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/LICENSE
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/README.md
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 donatellopyzza-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/__init__.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/assessor.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/envBuilder.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/game.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/main.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/mazeGenerator.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/turtleAgent.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/environments/assessment_maze.png
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/environments/assessment_maze.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/environments/hard_maze.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/environments/maze.txt
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/environments/test.png
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/environments/test.txt
+-rw-r--r--   0        0        0    40100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/images/pizza.png
+-rw-r--r--   0        0        0     8849 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/images/turtle.png
+-rw-r--r--   0        0        0    22725 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/data/images/turtle_small.png
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/agent.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/careTaker.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/constants.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/grid.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/gui.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/map.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/memento.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/orientation.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/originator.py
+-rw-r--r--   0        0        0     4213 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/parser.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/square.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/donatellopyzza/grid/turn.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/LICENSE
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/README.md
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 donatellopyzza-1.6.2/PKG-INFO
```

### Comparing `donatellopyzza-1.6.1/donatellopyzza/assessor.py` & `donatellopyzza-1.6.2/donatellopyzza/assessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,18 +34,16 @@
 
         success = 0
         failure = 0
         startTime = time.time()
         totalActions = 0
         for i in tqdm(range(self.nruns)):
             r, c = randint(self.minrows, self.maxrows), randint(self.mincolumns, self.maxcolumns)
-            deviation = (abs(c-(r+c)/2)/2)
-            a = int(min(r, c) + deviation)
-            b = int(max(r, c) - deviation)
-            maze = self.generator.create_maze(a, b, self.complexity)
+
+            maze = self.generator.create_maze(r, c, self.complexity)
             filepath = "assessment_maze"
             maze.save(maze, filename=filepath)       
             game = Game(filepath, False)
             # returns a turtle that execute actions on its environment
             turtle = game.start()
             feedback = Feedback.NO_FEEDBACK
             cnt = 0
```

### Comparing `donatellopyzza-1.6.1/donatellopyzza/envBuilder.py` & `donatellopyzza-1.6.2/donatellopyzza/envBuilder.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/game.py` & `donatellopyzza-1.6.2/donatellopyzza/game.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/main.py` & `donatellopyzza-1.6.2/donatellopyzza/main.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/mazeGenerator.py` & `donatellopyzza-1.6.2/donatellopyzza/mazeGenerator.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,20 @@
 class MazeGenerator():
     def create_maze(self, nrows, ncolumns, complexity=0, seed=None):
         if nrows <= 9 and ncolumns <= 9:
             print("WARNING: make a maze that have at least 10 rows and 10 columns. "
                 "The generated maze has been sized at 10x10")
             nrows = 10
             ncolumns = 10
+        r = nrows
+        c = ncolumns
+        deviation = (abs(c-(r+c)/2)/2)
+        nrows = int(min(r, c) + deviation)
+        ncolumns = int(max(r, c) - deviation)
+
         startPosition = 1
         pizzaPosition = 1
 
         rows = (nrows // 2) * 2 + 1
         columns = (ncolumns // 2) * 2 + 1
 
         if seed is not None:
```

### Comparing `donatellopyzza-1.6.1/donatellopyzza/data/environments/assessment_maze.png` & `donatellopyzza-1.6.2/donatellopyzza/data/environments/assessment_maze.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/data/environments/test.png` & `donatellopyzza-1.6.2/donatellopyzza/data/environments/test.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/data/images/pizza.png` & `donatellopyzza-1.6.2/donatellopyzza/data/images/pizza.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/data/images/turtle.png` & `donatellopyzza-1.6.2/donatellopyzza/data/images/turtle.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/data/images/turtle_small.png` & `donatellopyzza-1.6.2/donatellopyzza/data/images/turtle_small.png`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/grid/agent.py` & `donatellopyzza-1.6.2/donatellopyzza/grid/agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,13 +39,14 @@
 
     def getLastPosition(self):
         return self.caretaker.getLast().getState()
 
     def getCurrentPosition(self):
         return self.position
 
-    def draw(self, screen, xy):
+    def draw(self, screen, xy, scale):
         cste_angle = 90
         new_angle = cste_angle * self.orientation.value
+        self.turtle = pygame.transform.scale(self.turtle, (scale, scale))
         self.turtle = pygame.transform.rotate(self.turtle, new_angle - self.angle)
         self.angle = new_angle
         screen.blit(self.turtle, xy)
```

### Comparing `donatellopyzza-1.6.1/donatellopyzza/grid/grid.py` & `donatellopyzza-1.6.2/donatellopyzza/grid/grid.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/grid/gui.py` & `donatellopyzza-1.6.2/donatellopyzza/grid/gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from random import randint
 import sys, pygame
 import pkg_resources
+import math
 
 class GUI:
     def __init__(self, height, width):
         pygame.init()
         self.squareToDisplay = []
         self.agentToDisplay = []
         self.height = height
@@ -20,42 +21,47 @@
             g = randint(0, 160)
             b = randint(0, 255)
             sr = r - 15
             self.colors.append(pygame.Color(r, g, b, 255))
             self.shadeColors.append(pygame.Color(sr, g, b, 255))
         self.endCt = 0
 
+    def scale(self, value):
+        res = int(1 / (math.sqrt(value) + 1) * 1000)
+        print(1 / (math.sqrt(value) + 1))
+        return res
+
     '''
     Objectif : Mettre a jour l'image
     Param : map - la grille
     '''
     def update(self, map):
+        self.squareWidth = self.scale(len(self.squareToDisplay))
         self.squareToDisplay = []
         self.agentToDisplay = []
         for square in map.squares:
-            self.square(square.end, square.color, square._char, (square.x * self.squareWidth) - 75, (square.y * self.squareWidth) - 75, square.touched)
+            self.square(square.end, square.color, square._char, (square.x * self.squareWidth) - self.squareWidth, (square.y * self.squareWidth) - self.squareWidth, square.touched)
             for ag in square._filled:
                 self.agent(square, ag)
 
     '''
     Objectif : Ajoute un carre a la liste d'affichage
     Param : Int, Int, Int - w, le type de case (mur ou pas), x, y, les coordonnees de la case
     '''
     def square(self, end, color, w, x, y, touched):
         width = self.squareWidth
-        wallWidth = 7
 
         col = -1
         if end:
             col = color
             
         if touched:
-            self.touchedSquare(x, y, 74, 74)
+            self.touchedSquare(x, y, self.squareWidth - 1, self.squareWidth - 1)
         elif w == "B":
-            self.wall(x, y, 74, 74)
+            self.wall(x, y, self.squareWidth - 1, self.squareWidth - 1)
         else:
             self.squareToDisplay.append([col, (x ,y, width, width)])
 
     '''
     Objectif : Change le design de la case lorsque c'est un mur
     Param : Int, Int, Int, Int - x, y, les coordonnees de la case, width, height, les dimensions de la case
     '''
@@ -69,25 +75,27 @@
 
     '''
     Objectif : Ajout un agent a la liste d'affichage
     Param : Square - la case sur laquelle dessiner l'agent
     '''
     def agent(self, square, agent):
         marge = 0
-        self.agentToDisplay.append([agent, (marge + (square.x * self.squareWidth) - 75, marge + (square.y * self.squareWidth) - 75 )])
+        self.agentToDisplay.append([agent, (marge + (square.x * self.squareWidth) - self.squareWidth, marge + (square.y * self.squareWidth) - self.squareWidth)])
 
     '''
     Objectif : Afficher les donnees presentent dans les listes d'affichages (cases et agents)
     '''
     def display(self):
+        squareWidth = self.scale(len(self.squareToDisplay))
         self.endCt = 0
         if not self.disp:
-            size = width, height = self.height * 75, self.width * 75
+            print(self.height)
+            size = width, height = self.height * squareWidth, self.width * squareWidth
             self.screen = pygame.display.set_mode(size)
-            pygame.display.set_caption("Grid world")
+            pygame.display.set_caption("DonatelloPyzza")
             self.disp = True
         black = 0, 0, 0
         green = pygame.Color(0, 180, 0, 255)
         self.screen.fill(black)
         for i in range(len(self.squareToDisplay)):
             color = pygame.Color(0, 180, 0, 255)
             if not self.squareToDisplay[i][0] is None:
@@ -95,11 +103,12 @@
                     color = self.shadeColors[self.squareToDisplay[i][0]]
                 elif self.squareToDisplay[i][0] == -2:
                     color = pygame.Color(255, 255, 255, 255)
                 elif self.squareToDisplay[i][0] == -3:
                     color = pygame.Color(0, 0, 200, 255)
             pygame.draw.rect(self.screen,  color, self.squareToDisplay[i][1], 0)
             if self.squareToDisplay[i][0] is None:
+                self.pizza = pygame.transform.scale(self.pizza, (squareWidth, squareWidth))
                 self.screen.blit(self.pizza, self.squareToDisplay[i][1])
         for i in range(len(self.agentToDisplay)):
-            self.agentToDisplay[i][0].draw(self.screen, self.agentToDisplay[i][1])
+            self.agentToDisplay[i][0].draw(self.screen, self.agentToDisplay[i][1], squareWidth)
         pygame.display.flip()
```

### Comparing `donatellopyzza-1.6.1/donatellopyzza/grid/map.py` & `donatellopyzza-1.6.2/donatellopyzza/grid/map.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/grid/parser.py` & `donatellopyzza-1.6.2/donatellopyzza/grid/parser.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/donatellopyzza/grid/square.py` & `donatellopyzza-1.6.2/donatellopyzza/grid/square.py`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/LICENSE` & `donatellopyzza-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/README.md` & `donatellopyzza-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `donatellopyzza-1.6.1/pyproject.toml` & `donatellopyzza-1.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "DonatelloPyzza"
-version = "1.6.1"
+version = "1.6.2"
 authors = [
   { name="Mickaël Bettinelli", email="mickael.bettinelli@univ-smb.fr" },
 ]
 description = "A simple grid environment to learn Python"
 readme = "README.md"
 requires-python = ">=3.1"
 classifiers = [
```

### Comparing `donatellopyzza-1.6.1/PKG-INFO` & `donatellopyzza-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DonatelloPyzza
-Version: 1.6.1
+Version: 1.6.2
 Summary: A simple grid environment to learn Python
 Project-URL: Homepage, https://github.com/MilowB/Donatello
 Project-URL: Bug Tracker, https://github.com/MilowB/Donatello/pulls
 Author-email: Mickaël Bettinelli <mickael.bettinelli@univ-smb.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

