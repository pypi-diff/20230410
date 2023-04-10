# Comparing `tmp/localthickness-0.1.1.tar.gz` & `tmp/localthickness-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localthickness-0.1.1.tar", last modified: Sat Oct 22 21:17:00 2022, max compression
+gzip compressed data, was "localthickness-0.1.2.tar", last modified: Mon Apr 10 17:52:01 2023, max compression
```

## Comparing `localthickness-0.1.1.tar` & `localthickness-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 VAND       (502) staff       (20)        0 2022-10-22 21:17:00.117716 localthickness-0.1.1/
--rw-r--r--   0 VAND       (502) staff       (20)    35149 2022-10-22 19:35:32.000000 localthickness-0.1.1/LICENSE
--rw-r--r--   0 VAND       (502) staff       (20)     1026 2022-10-22 21:17:00.117569 localthickness-0.1.1/PKG-INFO
--rw-r--r--   0 VAND       (502) staff       (20)      714 2022-10-22 20:32:06.000000 localthickness-0.1.1/README.md
-drwxr-xr-x   0 VAND       (502) staff       (20)        0 2022-10-22 21:17:00.117387 localthickness-0.1.1/localthickness.egg-info/
--rw-r--r--   0 VAND       (502) staff       (20)     1026 2022-10-22 21:16:59.000000 localthickness-0.1.1/localthickness.egg-info/PKG-INFO
--rw-r--r--   0 VAND       (502) staff       (20)      196 2022-10-22 21:17:00.000000 localthickness-0.1.1/localthickness.egg-info/SOURCES.txt
--rw-r--r--   0 VAND       (502) staff       (20)        1 2022-10-22 21:16:59.000000 localthickness-0.1.1/localthickness.egg-info/dependency_links.txt
--rw-r--r--   0 VAND       (502) staff       (20)       15 2022-10-22 21:16:59.000000 localthickness-0.1.1/localthickness.egg-info/top_level.txt
--rwx------   0 VAND       (502) staff       (20)    15088 2022-10-22 19:24:44.000000 localthickness-0.1.1/localthickness.py
--rw-r--r--   0 VAND       (502) staff       (20)       38 2022-10-22 21:17:00.117769 localthickness-0.1.1/setup.cfg
--rw-r--r--   0 VAND       (502) staff       (20)      521 2022-10-22 20:36:16.000000 localthickness-0.1.1/setup.py
+drwxr-xr-x   0 VAND       (502) staff       (20)        0 2023-04-10 17:52:01.165019 localthickness-0.1.2/
+-rw-r--r--   0 VAND       (502) staff       (20)    35149 2022-10-22 19:35:32.000000 localthickness-0.1.2/LICENSE
+-rw-r--r--   0 VAND       (502) staff       (20)     1038 2023-04-10 17:52:01.164893 localthickness-0.1.2/PKG-INFO
+-rw-r--r--   0 VAND       (502) staff       (20)      726 2023-04-10 07:35:16.000000 localthickness-0.1.2/README.md
+drwxr-xr-x   0 VAND       (502) staff       (20)        0 2023-04-10 17:52:01.164669 localthickness-0.1.2/localthickness.egg-info/
+-rw-r--r--   0 VAND       (502) staff       (20)     1038 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/PKG-INFO
+-rw-r--r--   0 VAND       (502) staff       (20)      233 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/SOURCES.txt
+-rw-r--r--   0 VAND       (502) staff       (20)        1 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/dependency_links.txt
+-rw-r--r--   0 VAND       (502) staff       (20)       10 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/requires.txt
+-rw-r--r--   0 VAND       (502) staff       (20)       15 2023-04-10 17:52:01.000000 localthickness-0.1.2/localthickness.egg-info/top_level.txt
+-rwx------   0 VAND       (502) staff       (20)    18962 2023-04-10 12:54:44.000000 localthickness-0.1.2/localthickness.py
+-rw-r--r--   0 VAND       (502) staff       (20)       38 2023-04-10 17:52:01.165069 localthickness-0.1.2/setup.cfg
+-rw-r--r--   0 VAND       (502) staff       (20)      579 2023-03-05 23:22:51.000000 localthickness-0.1.2/setup.py
```

### Comparing `localthickness-0.1.1/LICENSE` & `localthickness-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `localthickness-0.1.1/PKG-INFO` & `localthickness-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localthickness
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fast local thickness in 3D and 2D.
 Home-page: https://github.com/vedranaa/local-thickness
 Author: VA Dahl and AB Dahl
 Author-email: vand@dtu.dk, abda@dtu.dk
 License: GPL-3.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,23 +15,24 @@
 ## Installation
 Install the module using ```pip install localthickness``` or clone the repository.
 
 ## Use
 ``` python
 import localthickness as lt
 
-#  Make test volume.
+#  Make a binary test volume. 
 B = lt.create_test_volume((100, 500, 400), sigma=15, boundary=0.001)
 
-# Compute thickness and separation
+# Compute thickness and separation.
 thickness = lt.local_thickness(B, scale=0.5)
 separation = lt.local_thickness(~B, scale=0.5)
 
 # Visualize.
 import matplotlib.pyplot as plt
 fig, ax = plt.subplots(1, 3, figsize=(10, 5))
 ax[0].imshow(B[10])
 ax[1].imshow(thickness[10], cmap=lt.black_plasma())
 ax[2].imshow(separation[10], cmap=lt.white_viridis())
+
 ```
 
 ![](https://github.com/vedranaa/local-thickness/raw/main/mwe_figure.png)
```

### Comparing `localthickness-0.1.1/README.md` & `localthickness-0.1.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 ## Installation
 Install the module using ```pip install localthickness``` or clone the repository.
 
 ## Use
 ``` python
 import localthickness as lt
 
-#  Make test volume.
+#  Make a binary test volume. 
 B = lt.create_test_volume((100, 500, 400), sigma=15, boundary=0.001)
 
-# Compute thickness and separation
+# Compute thickness and separation.
 thickness = lt.local_thickness(B, scale=0.5)
 separation = lt.local_thickness(~B, scale=0.5)
 
 # Visualize.
 import matplotlib.pyplot as plt
 fig, ax = plt.subplots(1, 3, figsize=(10, 5))
 ax[0].imshow(B[10])
 ax[1].imshow(thickness[10], cmap=lt.black_plasma())
 ax[2].imshow(separation[10], cmap=lt.white_viridis())
+
 ```
 
 ![](https://github.com/vedranaa/local-thickness/raw/main/mwe_figure.png)
```

### Comparing `localthickness-0.1.1/localthickness.egg-info/PKG-INFO` & `localthickness-0.1.2/localthickness.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localthickness
-Version: 0.1.1
+Version: 0.1.2
 Summary: Fast local thickness in 3D and 2D.
 Home-page: https://github.com/vedranaa/local-thickness
 Author: VA Dahl and AB Dahl
 Author-email: vand@dtu.dk, abda@dtu.dk
 License: GPL-3.0 license
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,23 +15,24 @@
 ## Installation
 Install the module using ```pip install localthickness``` or clone the repository.
 
 ## Use
 ``` python
 import localthickness as lt
 
-#  Make test volume.
+#  Make a binary test volume. 
 B = lt.create_test_volume((100, 500, 400), sigma=15, boundary=0.001)
 
-# Compute thickness and separation
+# Compute thickness and separation.
 thickness = lt.local_thickness(B, scale=0.5)
 separation = lt.local_thickness(~B, scale=0.5)
 
 # Visualize.
 import matplotlib.pyplot as plt
 fig, ax = plt.subplots(1, 3, figsize=(10, 5))
 ax[0].imshow(B[10])
 ax[1].imshow(thickness[10], cmap=lt.black_plasma())
 ax[2].imshow(separation[10], cmap=lt.white_viridis())
+
 ```
 
 ![](https://github.com/vedranaa/local-thickness/raw/main/mwe_figure.png)
```

### Comparing `localthickness-0.1.1/localthickness.py` & `localthickness-0.1.2/localthickness.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,72 +21,74 @@
     
     if scale==1:
         return local_thickness_basic(B, mask)
     else:
         return local_thickness_scaled(B, scale, mask)
         
 
-def local_thickness_basic(B, mask=None):
+def local_thickness_basic(B, mask=None, given_dist=False):
     """
     Computes local thickness in 2D or 3D (without scaling).
     """
     
-    if B.ndim==2:
-        dilate = dilate2d
-    elif B.ndim==3:
-        dilate = dilate3d
-    else:
-        return
+    dilate = {2: dilate2d, 3: dilate3d}[B.ndim]
       
-    # distance field
-    out = edt.edt(B)
+    # distance field, if not already given distances
+    if not given_dist:
+        out = edt.edt(B)
+    else:
+        out = B
+    
     if mask is not None:
         out = out * mask
-     
+        
     # iteratively dilate the distance field starting with max value
     for r in range(0, int(out.max())):
         temp = dilate(out)
         change = out > r
-        out[change] = temp[change]
+        np.copyto(out, temp, where=change)
     return out
 
 
 def local_thickness_scaled(B, scale=0.5, mask=None):
     """
     Computes local thickness in 2D or 3D using scaled approach.
     """
     
-    if B.ndim==2:
-        dilate = dilate2d
-    elif B.ndim==3:
-        dilate = dilate3d
-    else:
-        return
+    dilate = {2: dilate2d, 3: dilate3d}[B.ndim]
     
     dim = B.shape  # original image dimension
     dim_s = tuple(int(scale*d) for d in dim)  # dowscaled image dimension
     c = coords(dim, dim_s)
+
+    dist = edt.edt(B)
     
-    # downscaling the volumes, order=0 is nearest-neighbor
+    # downscale (order=0 is nearest-neighbor) and masking
     if mask is None:
         mask_s = None
     else: 
+        dist = dist * mask
         mask_s = scipy.ndimage.map_coordinates(mask, c, order=0)
-    B_s = scipy.ndimage.map_coordinates(B, c, order=0)
+        
+    dist_s = scipy.ndimage.map_coordinates(dist, c, order=0) * scale
     
-    # computing local thickness for downscaled
-    out = local_thickness(B_s, mask=mask_s)
+    # compute local thickness for downscaled
+    out = local_thickness_basic(dist_s, mask=mask_s, given_dist=True)
     
+    # free up some memery (does this make difference?)
+    del dist_s
+    del mask_s
+
     # flow-over boundary to avoid blend across boundary, will mask later
+    B_s = scipy.ndimage.map_coordinates(B, c, order=0)
     temp = dilate(out)
     out[~B_s] = temp[~B_s]
     
     # free up some memery (does this make difference?)
     del B_s
-    del mask_s
 
     # upscale, order=1 is bi-linear
     out = scipy.ndimage.map_coordinates(out, coords(dim_s, dim), order=1)
     out *= (1/scale) 
     out *= B    
     
     # mask output
@@ -97,20 +99,25 @@
 
 def coords(old, new):
     '''Query coordinates when rescaling the image of shape old to shape new.
        Made to be used with ndimage.map_coordianges for rescaling images.
     '''
 
     if len(old)==3:
-        c = np.mgrid[0:old[0]-1:new[0]*1j, 0:old[1]-1:new[1]*1j, 0:old[2]-1:new[2]*1j]
+        c = np.mgrid[0 : old[0]-1 : new[0] * 1j, 0 : old[1]-1 : new[1] * 1j, 
+                     0 : old[2]-1 : new[2] * 1j]
     elif len(old)==2:
-        c = np.mgrid[0:old[0]-1:new[0]*1j, 0:old[1]-1:new[1]*1j]
+        c = np.mgrid[0: old[0]-1 : new[0] * 1j, 0 : old[1]-1 : new[1] * 1j]
     else:
         return
     
+    # we had numerical problems so I make sure that we stay inside the image
+    for i in range(len(c)):
+        c[i] = np.clip(c[i], 0, old[i] - 1)
+
     return c
 
 
 def dilate3d(vol):
     ''' Dilation with 1-sphere approximated with small kernels.'''
     
     IDX = [None] * 3
@@ -220,50 +227,76 @@
     
     # image that will be updated
     out = np.copy(df) 
     
     # iteratively dilate the distance field starting with max value
     for r in range(1, int(df.max()) + 1):
         if verbose:
-            print(f'Dilating with radius {r}/{int(np.max(df))}')
+            print(f'Dilating with radius {r} of {int(np.max(df))}')
         if B.ndim==2:
             selem = skimage.morphology.disk(r)
         elif B.ndim==3:
             selem = skimage.morphology.ball(r)
-        temp = skimage.morphology.dilation(df * (df>=r), footprint=selem)
-        change = temp > r    
-        out[change] = temp[change]
+        df[df < r] = 0
+        temp = skimage.morphology.dilation(df, footprint=selem)
+        out = np.maximum(out, temp)    
     out *= B
     if mask is not None:
         out *= mask
     return out       
 
 
 
 #%% VISUALIZATION FUNCTIONS
 
-def black_plasma():
+
+def mixed_colors(N, bg=0.5, bg_alpha=0.5):
+    '''Colormap with permuted jet colors.'''
+    rng = np.random.default_rng(2022)
+    colors = plt.cm.jet(np.linspace(0, 1, N))
+    colors = rng.permutation(colors)
+    colors = np.vstack((np.array([bg] * 3 + [bg_alpha]), colors))
+    cmap = matplotlib.colors.ListedColormap(colors)
+    return cmap
+
+
+def black_plasma(bg=0, bg_alpha=1):
+    ''' Matplotlib colormap often used for local thickness.
+        bg: background color (default black).
+        bg_alpha: background alpha value (default opaque).
+    '''
     colors = plt.cm.plasma(np.linspace(0, 1, 256))
-    colors[:1, :] = np.array([0, 0, 0, 1])
+    colors[:1, :] = np.array([bg] * 3 + [bg_alpha])
     cmap = matplotlib.colors.ListedColormap(colors)
     return cmap
 
+
 def white_viridis():
+    '''Another colormap useful for showing both thickness and separation.'''
     colors = np.flip(plt.cm.viridis(np.linspace(0, 1, 256)), axis=0)
     colors[:1, :] = np.array([1, 1, 1, 1])
     cmap = matplotlib.colors.ListedColormap(colors)
     return cmap
 
+
 def pl_black_plasma():
-    c = black_plasma()(np.linspace(0, 1, 256))[:,0:3]
+    '''Colormap in plotly format'''
+    c = black_plasma()(np.linspace(0, 1, 256))[:, 0:3]
     pl_colorscale = []
     for i in range(256):
         pl_colorscale.append([i/255, f'rgb({c[i,0]},{c[i,1]},{c[i,2]})'])
     return pl_colorscale
- 
+
+
+def view_thickness_slice(z, T, vmax):
+    plt.imshow(T[z], cmap=black_plasma(), vmin=0, vmax=vmax, interpolation='nearest')
+    plt.title(f'slice z={z}')
+    plt.show()
+
+
 def arrow_navigation(event, z, Z):
     if event.key == "up" or event.key.lower()=='w':
         z = min(z+1, Z-1)
     elif event.key == 'down' or event.key.lower()=='z':
         z = max(z-1, 0)
     elif event.key == 'right' or event.key.lower()=='d':
         z = min(z+10, Z-1)
@@ -271,17 +304,19 @@
         z = max(z-10, 0)
     elif event.key == 'pagedown' or event.key.lower()=='x':
         z = min(z+50, Z-1)
     elif event.key == 'pageup' or event.key.lower()=='e':
         z = max(z-50, 0)
     return z
 
-def show_vol(V, cmap=plt.cm.gray, vmin = None, vmax = None): 
+
+def show_vol(V, cmap=plt.cm.gray, vmin=None, vmax=None): 
     """
-    Shows volumetric data for interactive inspection.
+    Shows volumetric data for interactive inspection. 
+    Whether it works depends on matplotlib backend.
     @author: vand at dtu dot dk
     """
     def update_drawing():
         ax.images[0].set_array(V[z])
         ax.set_title(f'slice z={z}')
         fig.canvas.draw()
  
@@ -293,17 +328,20 @@
     Z = V.shape[0]
     z = (Z-1)//2
     fig, ax = plt.subplots()
     if vmin is None: 
         vmin = np.min(V)
     if vmax is None: 
         vmax = np.max(V)
+    
     ax.imshow(V[z], cmap=cmap, vmin=vmin, vmax=vmax)
     ax.set_title(f'slice z={z}')
     fig.canvas.mpl_connect('key_press_event', key_press)
+    plt.show()
+
 
 #%% HELPING FUNCTIONS
 
 def create_test_volume(dim, sigma=7, threshold=0, boundary=0, frame = True, seed = None):
     """ Creates test volume for local thickness and porosity analysis.
     Arguments:
         dim: tuple giving the size of the volume
@@ -337,14 +375,80 @@
     if frame:
         V[[0,-1]] = False
         V[:, [0,-1]] = False
         if len(dim)==3:
             V[:, :, [0,-1]] = False
     return V
 
+
+#%% 
+def prepare_for_saving(thickness, options):
+
+    factor = options.get('factor', 1)
+    pad = options.get('pad', True)
+    blend = options.get('blend', True)
+    dilate = options.get('dilate', True)
+    maxval = options.get('maxval', thickness.max())
+
+    if factor>1:
+        Z, Y, X = thickness.shape
+        thickness = thickness[Z%factor//2::factor, Y%factor//2::factor, 
+                              X%factor//2::factor]
+    if pad:
+        thickness = np.pad(thickness, ((1, 1), ) * 3, constant_values=0)
+
+    # Grayscale volume which will be saved for shape
+    gray = ~(thickness>0)  
+    if blend:
+        gray = edt.edt(gray) - edt.edt(~gray) - gray + 0.5
+        gray = np.clip(gray, -25, 25)
+        gray = np.exp(0.1 * gray)
+        gray = gray / (gray + 1)  # values between 0 and 1 with 0.5 at interface
+    
+    if dilate:
+        thickness = dilate3d(thickness)
+
+    return thickness, gray, maxval
+
+
+
+def save_thickness_volumes(thickness, filename_root, **options):
+    '''Saves results of local thickness analysis in two volumes suitable for
+    visualization in paraview.
+    Inputs:
+        thickness: local thickness volume, a 3D numpy array, where 0 is 
+            bacground and positive values are thickness.
+        filename_root: root of the filename, sufixes will be added 
+        factor: int, downscaling factor. Default 1 does not downscale.
+        pad: bool, whether to pad with background to ensure closed surfaces.
+        dilate: bool, whether to dilate colored object 1px to ensure color on 
+            surface.
+        blend: whether to blend binary values of object representation for a
+            smoother surface.
+        maxval: thickness which will be shown with last color in cmap.
+        paraview_alpha: whether to invert alpha values as paraview expects.
+    '''
+    import tifffile
+
+    paraview_alpha = options.get('paraview_alpha', True)
+    thickness, gray, maxval = prepare_for_saving(thickness, options)
+
+    cmap = black_plasma(bg=0, bg_alpha=1)  # set bg=1 for white which might blend nicer
+    
+    with (tifffile.TiffWriter(filename_root + '_gray.tif') as gr, 
+            tifffile.TiffWriter(filename_root + '_rgba.tif') as rgba):
+        for g, t in zip(gray, thickness):
+            gr.write((255 * g).astype(np.uint8))
+            t_rgba = cmap(t/maxval)
+            if paraview_alpha:
+                t_rgba[:, :, 3] = 1 - t_rgba[:, :, 3]  # flipping opacity to work with paraview
+            rgba.write((255*t_rgba).astype(np.uint8), photometric='rgb', extrasamples = 'ASSOCALPHA') 
+            # rgb.write((255*t_rgba[:, :, :3]).astype(np.uint8), photometric='rgb')
+    
+
 #%% VTK WRITE FUNCTIONS
 
 def save_gray2vtk(volume, filename, filetype='ASCII', origin=(0,0,0),
                   spacing=(1,1,1), dataname='gray'):
     ''' Writes a vtk file with grayscace volume data.
     Arguments:
        volume: a grayscale volume, values will be saved as floats
@@ -409,35 +513,31 @@
             rgba.byteswap(True) # Paraview expects big-endian 
             rgba.tofile(f)
     else: # ASCII
         with open(filename, 'a') as f:
             np.savetxt(f,rgba.ravel(),fmt='%.5g', newline= ' ')   
 
 
-def save_thickness2vtk(B, thickness, filename, colormap = black_plasma(), 
-                  maxval = None, dilate = True, filetype='ASCII', origin=(0,0,0),
-                  spacing=(1,1,1)):
+def save_thickness2vtk(thickness, filename, **options):
     ''' Writes a vtk file with results of local thickness analysis.
     Author:vand@dtu.dk, 2019
     '''
-    
-    g = edt.edt(B) - edt.edt(~B) - B + 0.5
-    g = np.exp(0.1*g)
-    g = g/(g+1)
-    
-    save_gray2vtk(g, filename, filetype=filetype, origin=origin, spacing = spacing)
-    
-    if maxval is None: 
-        maxval = np.max(thickness)
-    
-    if dilate:
-        thickness = dilate3d(thickness)
-   
-    rgba = colormap(thickness.ravel()/maxval)
 
+    filetype = options.get('filetype', 'ASCII')
+    origin = options.get('origin', (0, 0, 0))
+    spacing = options.get('spacing', (1, 1, 1))
+    
+    thickness, gray, maxval = prepare_for_saving(thickness, options)
+
+    cmap = black_plasma(bg=0, bg_alpha=0.1)  
+    rgba = cmap(thickness.ravel()/maxval)
+
+    # Now saving
+    save_gray2vtk(gray, filename, filetype=filetype, origin=origin, spacing=spacing)
+       
     with open(filename, 'a') as f:
         f.write('COLOR_SCALARS rgba 4\n')
     
     # writing color data
     if filetype.upper()=='BINARY':
         with open(filename, 'ab') as f:
             rgba = (255*rgba).astype('ubyte') # Pareview expects unsigned char
```

### Comparing `localthickness-0.1.1/setup.py` & `localthickness-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1 +1,18 @@
-from setuptools import setupwith open("README.md", "r") as fh:    long_description = fh.read()setup(    name = 'localthickness',    version = '0.1.1',    description = 'Fast local thickness in 3D and 2D.',    long_description = long_description,    long_description_content_type = "text/markdown",    url = 'https://github.com/vedranaa/local-thickness',    author = 'VA Dahl and AB Dahl',    author_email = 'vand@dtu.dk, abda@dtu.dk',    license ='GPL-3.0 license',    py_modules = ['localthickness']    )
+from setuptools import setup
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name = 'localthickness',
+    version = '0.1.2',
+    description = 'Fast local thickness in 3D and 2D.',
+    long_description = long_description,
+    long_description_content_type = "text/markdown",
+    url = 'https://github.com/vedranaa/local-thickness',
+    author = 'VA Dahl and AB Dahl',
+    author_email = 'vand@dtu.dk, abda@dtu.dk',
+    license ='GPL-3.0 license',
+    py_modules = ['localthickness'],
+    install_requires = ['edt', 'numpy']
+    )
```

