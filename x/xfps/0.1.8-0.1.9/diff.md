# Comparing `tmp/xfps-0.1.8.tar.gz` & `tmp/xfps-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfps-0.1.8.tar", last modified: Sun Apr  2 22:48:39 2023, max compression
+gzip compressed data, was "xfps-0.1.9.tar", last modified: Mon Apr 10 14:27:06 2023, max compression
```

## Comparing `xfps-0.1.8.tar` & `xfps-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-02 22:48:39.348803 xfps-0.1.8/
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1062 2023-03-29 22:02:05.000000 xfps-0.1.8/LICENSE
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      419 2023-04-02 22:48:39.348668 xfps-0.1.8/PKG-INFO
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      137 2023-04-02 13:17:47.000000 xfps-0.1.8/README.md
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       38 2023-04-02 22:48:39.348849 xfps-0.1.8/setup.cfg
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      599 2023-04-02 22:47:53.000000 xfps-0.1.8/setup.py
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-02 22:48:39.346655 xfps-0.1.8/src/
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-02 22:48:39.347730 xfps-0.1.8/src/xfps/
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       55 2023-03-29 23:05:44.000000 xfps-0.1.8/src/xfps/__init__.py
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1311 2023-03-31 14:22:14.000000 xfps-0.1.8/src/xfps/effects.py
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     8964 2023-04-02 22:47:26.000000 xfps-0.1.8/src/xfps/particle_system.py
-drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-02 22:48:39.348446 xfps-0.1.8/src/xfps.egg-info/
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      419 2023-04-02 22:48:39.000000 xfps-0.1.8/src/xfps.egg-info/PKG-INFO
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      254 2023-04-02 22:48:39.000000 xfps-0.1.8/src/xfps.egg-info/SOURCES.txt
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        1 2023-04-02 22:48:39.000000 xfps-0.1.8/src/xfps.egg-info/dependency_links.txt
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       10 2023-04-02 22:48:39.000000 xfps-0.1.8/src/xfps.egg-info/requires.txt
--rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        5 2023-04-02 22:48:39.000000 xfps-0.1.8/src/xfps.egg-info/top_level.txt
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-10 14:27:06.182160 xfps-0.1.9/
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1062 2023-03-29 22:02:05.000000 xfps-0.1.9/LICENSE
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      419 2023-04-10 14:27:06.182021 xfps-0.1.9/PKG-INFO
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      137 2023-04-02 13:17:47.000000 xfps-0.1.9/README.md
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       38 2023-04-10 14:27:06.182206 xfps-0.1.9/setup.cfg
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      599 2023-04-10 14:24:55.000000 xfps-0.1.9/setup.py
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-10 14:27:06.179770 xfps-0.1.9/src/
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-10 14:27:06.181009 xfps-0.1.9/src/xfps/
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       55 2023-03-29 23:05:44.000000 xfps-0.1.9/src/xfps/__init__.py
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     1311 2023-03-31 14:22:14.000000 xfps-0.1.9/src/xfps/effects.py
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)     9947 2023-04-10 14:24:11.000000 xfps-0.1.9/src/xfps/particle_system.py
+drwxr-xr-x   0 rudolfvrbensky   (501) staff       (20)        0 2023-04-10 14:27:06.181811 xfps-0.1.9/src/xfps.egg-info/
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      419 2023-04-10 14:27:06.000000 xfps-0.1.9/src/xfps.egg-info/PKG-INFO
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)      254 2023-04-10 14:27:06.000000 xfps-0.1.9/src/xfps.egg-info/SOURCES.txt
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        1 2023-04-10 14:27:06.000000 xfps-0.1.9/src/xfps.egg-info/dependency_links.txt
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)       10 2023-04-10 14:27:06.000000 xfps-0.1.9/src/xfps.egg-info/requires.txt
+-rw-r--r--   0 rudolfvrbensky   (501) staff       (20)        5 2023-04-10 14:27:06.000000 xfps-0.1.9/src/xfps.egg-info/top_level.txt
```

### Comparing `xfps-0.1.8/LICENSE` & `xfps-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xfps-0.1.8/setup.py` & `xfps-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xfps',
-    version='0.1.8',
+    version='0.1.9',
     description='A particle system and effects library for Pygame',
     author='XFajk',
     author_email='ertyperty24@gmail.com',
     url='https://github.com/XFajk/xfps/tree/main',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `xfps-0.1.8/src/xfps/effects.py` & `xfps-0.1.9/src/xfps/effects.py`

 * *Files identical despite different names*

### Comparing `xfps-0.1.8/src/xfps/particle_system.py` & `xfps-0.1.9/src/xfps/particle_system.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,73 +8,81 @@
         self.shape_type = shape_type
         self.gravity = gravity
         self.objects = []
 
     def add(self, loc: list | pygame.Vector2, angle: float, speed: float, size: float, color: tuple | pygame.Color,
             dis_amount: float):
         vel = [math.cos(math.radians(angle)) * speed, math.sin(math.radians(angle)) * speed]
-        self.objects.append([loc, vel, size, color, dis_amount])
+        self.objects.append(
+            {
+                "loc": loc,
+                "vel": vel,
+                "size": size,
+                "color": color,
+                "dis_amount": dis_amount,
+            }
+        )
 
     def use(self, surf: pygame.Surface, dt: float = 1.0, operation=lambda x, dt: x):
         if self.shape_type == "circle":
             for i, p in sorted(enumerate(self.objects), reverse=True):
-                p[0][0] += p[1][0] * dt
-                p[0][1] += p[1][1] * dt
-                p[2] -= p[4] * dt
-                p[1][1] += self.gravity * dt
+                p["loc"][0] += p["vel"][0] * dt
+                p["loc"][1] += p["vel"][1] * dt
+                p["size"] -= p["dis_amount"] * dt
+                p["vel"][1] += self.gravity * dt
                 operation(p, dt)
-                pygame.draw.circle(surf, p[3], p[0], p[2])
-                if p[2] <= 0:
+                pygame.draw.circle(surf, p["color"], p["loc"], p["size"])
+                if p["size"] <= 0:
                     self.objects.pop(i)
 
         elif self.shape_type == "rectangle":
             for i, p in sorted(enumerate(self.objects), reverse=True):
-                p[0][0] += p[1][0] * dt
-                p[0][1] += p[1][1] * dt
-                p[2] -= p[4] * dt
-                p[1][1] += self.gravity * dt
+                p["loc"][0] += p["vel"][0] * dt
+                p["loc"][1] += p["vel"][1] * dt
+                p["size"] -= p["dis_amount"] * dt
+                p["vel"][1] += self.gravity * dt
                 operation(p, dt)
-                pygame.draw.rect(surf, p[3], (p[0][0]-p[2]/2, p[0][1]-p[2]/2, p[2], p[2]))
-                if p[2] <= 0:
+                pygame.draw.rect(surf, p["color"], (p["loc"][0]-p["size"]/2, p["loc"][1]-p["size"]/2, p["size"], p["size"]))
+                if p["size"] <= 0:
                     self.objects.pop(i)
         else:
-            raise TypeError(f"{self.shape_type} is an invalid shape type")
+            raise TypeError(f"{self.shape_type} is an invalid shape type you can use circle or rectangle")
 
     def use_with_light(self, surf: pygame.Surface, dt: float, operation=lambda x, dt: x):
         if self.shape_type == "circle":
             for i, p in sorted(enumerate(self.objects), reverse=True):
-                p[0][0] += p[1][0] * dt
-                p[0][1] += p[1][1] * dt
-                p[2] -= p[4] * dt
-                p[1][1] += self.gravity * dt
+                p["loc"][0] += p["vel"][0] * dt
+                p["loc"][1] += p["vel"][1] * dt
+                p["size"] -= p["dis_amount"] * dt
+                p["vel"][1] += self.gravity * dt
                 operation(p, dt)
-                light_surf = surf_circle(p[2] * 2, (p[3][0] / 3, p[3][1] / 3, p[3][2] / 3))
+                light_surf = surf_circle(p["size"] * 2, (p["color"][0] / 3, p["color"][1] / 3, p["color"][2] / 3))
                 surf.blit(light_surf,
-                          (p[0][0] - int(light_surf.get_width() / 2), p[0][1] - int(light_surf.get_height() / 2)),
+                          (p["loc"][0] - int(light_surf.get_width() / 2), p["loc"][1] - int(light_surf.get_height() / 2)),
                           special_flags=pygame.BLEND_RGB_ADD)
-                pygame.draw.circle(surf, p[3], p[0], p[2])
-                if p[2] <= 0:
+                pygame.draw.circle(surf, p["color"], p["loc"], p["size"])
+                if p["size"] <= 0:
                     self.objects.pop(i)
 
         elif self.shape_type == "rectangle":
             for i, p in sorted(enumerate(self.objects), reverse=True):
-                p[0][0] += p[1][0] * dt
-                p[0][1] += p[1][1] * dt
-                p[2] -= p[4] * dt
-                p[1][1] += self.gravity * dt
+                p["loc"][0] += p["vel"][0] * dt
+                p["loc"][1] += p["vel"][1] * dt
+                p["size"] -= p["dis_amount"] * dt
+                p["vel"][1] += self.gravity * dt
                 operation(p, dt)
-                light_surf = surf_rect(p[2] * 2, p[2] * 2, (p[3][0] / 3, p[3][1] / 3, p[3][2] / 3))
+                light_surf = surf_rect(p["size"] * 2, p["size"] * 2, (p["color"][0] / 3,p["color"][1] / 3, p["color"][2] / 3))
                 surf.blit(light_surf,
-                          (p[0][0] - int(light_surf.get_width() / 4)-p[2]/2, p[0][1] - int(light_surf.get_height() / 4)-p[2]/2),
+                          (p["loc"][0] - int(light_surf.get_width() / 4)-p["size"]/2, p["loc"][1] - int(light_surf.get_height() / 4)-p["size"]/2),
                           special_flags=pygame.BLEND_RGB_ADD)
-                pygame.draw.rect(surf, p[3], (p[0][0]-p[2]/2, p[0][1]-p[2]/2, p[2], p[2]))
-                if p[2] <= 0:
+                pygame.draw.rect(surf, p["color"], (p["loc"][0]-p["size"]/2, p["loc"][1]-p["size"]/2, p["size"], p["size"]))
+                if p["size"] <= 0:
                     self.objects.pop(i)
         else:
-            raise TypeError(f"{self.shape_type} is an invalid shape type")
+            raise TypeError(f"{self.shape_type} is an invalid shape type you can use circle or rectangle")
 
 
 class SparkParticles:
     def __init__(self, gravity: float = 0.0):
         self.gravity = gravity
         self.objects = []
 
@@ -115,41 +123,52 @@
 
             surf.blit(light_surf, (s.loc[0] - new_loc[0], s.loc[1] - new_loc[1]), special_flags=pygame.BLEND_RGB_ADD)
             if not s.alive:
                 self.objects.pop(i)
 
 
 class ImgParticles:
-    def __init__(self, img: pygame.Surface, gravity: float = 0.0, color_key: tuple | pygame.Color = (0, 0, 0)):
+    def __init__(self, img: pygame.Surface, gravity: float = 0.0, give_color_key: bool = False, color_key: tuple | pygame.Color = (0, 0, 0)):
         self.img = img
-        self.img.set_colorkey(color_key)
+        if give_color_key:
+            self.img.set_colorkey(color_key)
         self.gravity = gravity
         self.objects = []
 
     def add(self, loc: list | pygame.Vector2, angle: float, speed: float, size: float, color: tuple | pygame.Color,
             dis_amount: float, rot_amount_deg: float = 0.0):
         vel = [math.cos(math.radians(angle)) * speed, math.sin(math.radians(angle)) * speed]
-        self.objects.append([loc, vel, size, color, dis_amount, 0, rot_amount_deg])
+        self.objects.append(
+            {
+                "loc": loc,
+                "vel": vel,
+                "size": size,
+                "color": color,
+                "dis_amount": dis_amount,
+                "rot_amount_deg": rot_amount_deg,
+                "rotation": 0
+            }
+        )
 
     def use(self, surf: pygame.Surface, dt: float, operation=lambda x, dt: x):
         for i, p in sorted(enumerate(self.objects), reverse=True):
-            p[0][0] += p[1][0] * dt
-            p[0][1] += p[1][1] * dt
-            p[2] -= p[4] * dt
-            p[1][1] += self.gravity * dt
+            p["loc"][0] += p["vel"][0] * dt
+            p["loc"][1] += p["vel"][1] * dt
+            p["size"] -= p["dis_amount"] * dt
+            p["vel"][1] += self.gravity * dt
             operation(p, dt)
-            p_img = pygame.transform.scale(self.img, (p[2], p[2]))
-            if p[6] > 0:
-                p[5] += p[6]
-                p_img_rot = pygame.transform.rotate(p_img, p[5])
-                surf.blit(p_img_rot, (p[0][0] - int(p_img_rot.get_width() / 2) + p[2] / 2,
-                                      p[0][1] - int(p_img_rot.get_height() / 2) + p[2] / 2))
+            p_img = pygame.transform.scale(self.img, (p["size"], p["size"]))
+            if p["rot_amount_deg"] > 0:
+                p["rotation"] += p["rot_amount_deg"]
+                p_img_rot = pygame.transform.rotate(p_img, p["rotation"])
+                surf.blit(p_img_rot, (p["loc"][0] - int(p_img_rot.get_width() / 2) + p["size"] / 2,
+                                      p["loc"][1] - int(p_img_rot.get_height() / 2) + p["size"] / 2))
             else:
-                surf.blit(p_img, (p[0][0] - p[2] / 2, p[0][1] - p[2] / 2))
-            if p[2] <= 0:
+                surf.blit(p_img, (p["loc"][0] - p["size"] / 2, p["loc"][1] - p["size"] / 2))
+            if p["size"] <= 0:
                 self.objects.pop(i)
 
 
 class Spark:
     def __init__(self, loc: list | tuple | pygame.Vector2, angle: float, speed: float, color: tuple = (255, 255, 255),
                  scale: float = 1,
                  dis_amount: float = 0.25):
```

