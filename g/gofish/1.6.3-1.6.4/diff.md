# Comparing `tmp/gofish-1.6.3.tar.gz` & `tmp/gofish-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gofish-1.6.3.tar", last modified: Mon Mar 20 18:37:49 2023, max compression
+gzip compressed data, was "gofish-1.6.4.tar", last modified: Mon Apr 10 00:11:52 2023, max compression
```

## Comparing `gofish-1.6.3.tar` & `gofish-1.6.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-20 18:37:49.439871 gofish-1.6.3/
--rw-r--r--   0 richardteague   (501) staff       (20)    35149 2022-07-28 17:00:43.000000 gofish-1.6.3/LICENSE.md
--rw-r--r--   0 richardteague   (501) staff       (20)      392 2023-03-20 18:37:49.439773 gofish-1.6.3/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)     2778 2022-07-28 17:00:43.000000 gofish-1.6.3/README.md
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-20 18:37:49.439090 gofish-1.6.3/gofish/
--rw-r--r--   0 richardteague   (501) staff       (20)      104 2022-07-28 17:00:43.000000 gofish-1.6.3/gofish/__init__.py
--rw-r--r--   0 richardteague   (501) staff       (20)    45398 2022-07-28 17:00:43.000000 gofish-1.6.3/gofish/annulus.py
--rw-r--r--   0 richardteague   (501) staff       (20)   188844 2023-03-20 18:37:00.000000 gofish-1.6.3/gofish/gofish.py
-drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-03-20 18:37:49.439638 gofish-1.6.3/gofish.egg-info/
--rw-r--r--   0 richardteague   (501) staff       (20)      392 2023-03-20 18:37:49.000000 gofish-1.6.3/gofish.egg-info/PKG-INFO
--rw-r--r--   0 richardteague   (501) staff       (20)      232 2023-03-20 18:37:49.000000 gofish-1.6.3/gofish.egg-info/SOURCES.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-03-20 18:37:49.000000 gofish-1.6.3/gofish.egg-info/dependency_links.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-03-20 18:37:49.000000 gofish-1.6.3/gofish.egg-info/requires.txt
--rw-r--r--   0 richardteague   (501) staff       (20)        7 2023-03-20 18:37:49.000000 gofish-1.6.3/gofish.egg-info/top_level.txt
--rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-03-20 18:37:49.439907 gofish-1.6.3/setup.cfg
--rw-r--r--   0 richardteague   (501) staff       (20)      593 2023-03-20 18:37:06.000000 gofish-1.6.3/setup.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-10 00:11:52.405613 gofish-1.6.4/
+-rw-r--r--   0 richardteague   (501) staff       (20)    35149 2023-03-27 18:30:37.000000 gofish-1.6.4/LICENSE.md
+-rw-r--r--   0 richardteague   (501) staff       (20)      392 2023-04-10 00:11:52.405493 gofish-1.6.4/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)     2778 2023-03-27 18:30:37.000000 gofish-1.6.4/README.md
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-10 00:11:52.404680 gofish-1.6.4/gofish/
+-rw-r--r--   0 richardteague   (501) staff       (20)      104 2023-03-27 18:30:38.000000 gofish-1.6.4/gofish/__init__.py
+-rw-r--r--   0 richardteague   (501) staff       (20)    45466 2023-04-09 23:58:51.000000 gofish-1.6.4/gofish/annulus.py
+-rw-r--r--   0 richardteague   (501) staff       (20)   190217 2023-04-10 00:09:47.000000 gofish-1.6.4/gofish/gofish.py
+drwxr-xr-x   0 richardteague   (501) staff       (20)        0 2023-04-10 00:11:52.405338 gofish-1.6.4/gofish.egg-info/
+-rw-r--r--   0 richardteague   (501) staff       (20)      392 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/PKG-INFO
+-rw-r--r--   0 richardteague   (501) staff       (20)      232 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/SOURCES.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        1 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/dependency_links.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/requires.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)        7 2023-04-10 00:11:52.000000 gofish-1.6.4/gofish.egg-info/top_level.txt
+-rw-r--r--   0 richardteague   (501) staff       (20)       38 2023-04-10 00:11:52.405652 gofish-1.6.4/setup.cfg
+-rw-r--r--   0 richardteague   (501) staff       (20)      593 2023-04-09 23:58:37.000000 gofish-1.6.4/setup.py
```

### Comparing `gofish-1.6.3/LICENSE.md` & `gofish-1.6.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gofish-1.6.3/README.md` & `gofish-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `gofish-1.6.3/gofish/annulus.py` & `gofish-1.6.4/gofish/annulus.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,25 +712,26 @@
         return A * np.cos(x) + B * np.sin(x) + y0
 
     # -- Deprojection Functions -- #
 
     def calc_vlos(self, vrot, vrad=0.0):
         """
         Calculate the line of sight velocity for each spectrum given the
-        rotational and radial velocities at the attached polar angles.
+        rotational and radial velocities at the attached polar angles. Here
+        positive `vrad` values are away from the disk center.
 
         Args:
             vrot (float): Projected rotation velocity in [m/s].
             vrad (optional[float]): Projected radial velocity in [m/s].
 
         Returns
             Array of projected line of sight velocities at each polar angle.
         """
         _vrot = vrot * np.cos(self.theta)
-        _vrad = vrad * np.sin(self.theta)
+        _vrad = -vrad * np.sin(self.theta)
         return _vrot + _vrad
 
     def _deprojected_spectra(self, vrot, vrad=0.0):
         """Returns all deprojected points as an ensemble."""
         vlos = self.calc_vlos(vrot=vrot, vrad=vrad)
         return np.array([np.interp(self.velax, self.velax - dv, spectra)
                          for dv, spectra in zip(vlos, self.spectra)])
```

### Comparing `gofish-1.6.3/gofish/gofish.py` & `gofish-1.6.4/gofish/gofish.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def average_spectrum(self, r_min, r_max, inc, PA, mstar, dist, dr=None,
         PA_min=None, PA_max=None, exclude_PA=False, abs_PA=False, x0=0.0,
         y0=0.0, z0=None, psi=None, r_cavity=None, r_taper=None, q_taper=None,
         z_func=None, resample=1, beam_spacing=False, mask_frame='disk',
         unit='Jy/beam', mask=None, skip_empty_annuli=True, shadowed=False,
         empirical_uncertainty=False, include_spectral_decorrelation=True,
-        velocity_resolution=1.0):
+        velocity_resolution=1.0, vrad_func=None):
         """
         Return the averaged spectrum over a given radial range, returning a
         spectrum in units of [Jy/beam] or [K] using the Rayleigh-Jeans
         approximation. As the Keplerian rotation of the disk needs to be
         accounted for, a stellar mass in [Msun] and distance in [pc] must be
         provided.
 
@@ -166,14 +166,17 @@
                 sigma clipping described in ``imagecube.estimate_uncertainty``.
             include_spectral_decorrlation (Optional[bool]): If ``True``, take
                 account of the spectral decorrelation when estimating
                 uncertainties on the average spectrum and return a spectral
                 correlation length too. Defaults to ``True``.
             velocity_resolution (Optional[float]): Velocity resolution of the
                 data as a fraction of the channel spacing. Defaults to ``1.0``.
+            vrad_func (Optional[callable]): Define any radial velocity component
+                here. Must return a radial velocity in [m/s] for a given radial
+                position in [arcsec].
 
         Returns:
             The velocity axis of the spectrum, ``velax``, in [m/s], the
             averaged spectrum, ``spectrum``, and the variance of the velocity
             bin, ``scatter``. The latter two are in units of either [Jy/beam]
             or [K] depending on the ``unit``.
         """
@@ -206,17 +209,25 @@
             z0=z0,
             psi=psi,
             r_cavity=r_cavity,
             r_taper=r_taper,
             q_taper=q_taper,
             z_func=z_func
             )
-
         v_kep = np.atleast_1d(v_kep)
 
+        # Radial velocity at the annulus centers. Note that positive v_rad are
+        # moving away from the disk center.
+
+        if vrad_func is None:
+            v_rad = np.zeros(v_kep.shape)
+        else:
+            v_rad = vrad_func(rvals)
+        assert v_rad.shape == v_kep.shape
+
         # Output unit.
 
         unit = unit.lower()
         if unit not in ['mjy/beam', 'jy/beam', 'mk', 'k']:
             raise ValueError("Unknown `unit`.")
         if resample < 1.0 and self.verbose:
             print('WARNING: `resample < 1`, are you sure you want channels '
@@ -242,14 +253,15 @@
             user_mask = np.ones(self.data[0].shape)
 
         # Calculate the number of independent samples for each pixel after
         # accounting for the spectral deprojection of the data. This is based
         # on a similar approach to Yen et al. (2016), but performed
         # numerically such that we can a) take account of any masks and b)
         # estimate the introduced spectral correlation.
+        # TODO: Include the vrad component here.
 
         if include_spectral_decorrelation and not empirical_uncertainty:
             v0_map = self.keplerian(
                 inc=inc,
                 PA=PA,
                 mstar=mstar,
                 dist=dist,
@@ -327,14 +339,15 @@
             # The try / except loop is that when masking, the spectrum values
             # are converted to NaNs which look like pixels in the calculation
             # of the annulus, but then cannot be binned.
             # TODO: See if there's a better way to combine these two checks.
 
             try:
                 x, y, dy = annulus.deprojected_spectrum(vrot=v_kep[ridx],
+                                                        vrad=v_rad[ridx],
                                                         resample=resample,
                                                         scatter=True)
             except ValueError:
                 msg = "No finite pixels found between"
                 msg += " {:.2f} and".format(rbins[ridx])
                 msg += " {:.2f} arcsec.".format(rbins[ridx+1])
                 if not skip_empty_annuli:
@@ -762,15 +775,15 @@
         return std
 
     def integrated_spectrum(self, r_min, r_max, inc, PA, mstar=None, dist=None,
         dr=None, x0=0.0, y0=0.0, z0=None, psi=None, r_cavity=None, r_taper=None,
         q_taper=None, z_func=None, resample=1, beam_spacing=False, PA_min=None,
         PA_max=None, exclude_PA=False, abs_PA=False, mask=None,
         mask_frame='disk', empirical_uncertainty=False, skip_empty_annuli=True,
-        shadowed=False, velocity_resolution=1.0,
+        shadowed=False, velocity_resolution=1.0, vrad_func=None,
         include_spectral_decorrelation=True):
         """
         Return the integrated spectrum over a given radial range, returning a
         spectrum in units of [Jy]. If a stellar mass and distance are specified
         then this will split the data into concentric annuli, correcting each
         annulus for the Keplerian rotation of the disk to generate a more
         precise measurement. If no stellar mass or distance are given then a
@@ -841,14 +854,17 @@
                 which are stacked as correlated, by default this is
                 ``True``. If ``False``, the uncertainty will be estimated using
                 Poisson statistics, otherwise the uncertainty is just the
                 standard deviation of each velocity bin.
             skip_empty_annuli (Optional[bool]): If ``True``, skip any annuli
                 which are empty (i.e. their masks have zero pixels in). If
                 ``False``, any empty masks will raise a ``ValueError``.
+            vrad_func (Optional[callable]): Define any radial velocity component
+                here. Must return a radial velocity in [m/s] for a given radial
+                position in [arcsec].
 
         Returns:
             The velocity axis of the spectrum, ``velax``, in [m/s], the
             integrated spectrum, ``spectrum``, and the variance of the velocity
             bin, ``scatter``. The latter two are in units of [Jy].
 
         """
@@ -856,14 +872,18 @@
 
         self._test_2D()
 
         # Check to see if a shift-and-stack approach is required. If so, check
         # that both `mstar` and `dist` have been provided.
 
         if mstar is None:
+
+            if vrad_func is not None:
+                raise ValueError("Must specify `mstar` to use `vrad_func`.")
+
             return self._integrated_spectrum_basic(
                 r_min=r_min,
                 r_max=r_max,
                 x0=x0,
                 y0=y0,
                 inc=inc,
                 PA=PA,
@@ -912,14 +932,15 @@
             mask=mask,
             mask_frame=mask_frame,
             skip_empty_annuli=skip_empty_annuli,
             empirical_uncertainty=empirical_uncertainty,
             velocity_resolution=velocity_resolution,
             include_spectral_decorrelation=include_spectral_decorrelation,
             shadowed=shadowed,
+            vrad_func=vrad_func,
             )
 
         # Calculate the area of the integration region.
 
         if mask is not None:
             if mask.shape != self.data.shape:
                 if mask.shape != self.data.shape[1:]:
@@ -1053,15 +1074,15 @@
 
     def radial_spectra(self, rvals=None, rbins=None, dr=None, x0=0.0, y0=0.0,
         inc=0.0, PA=0.0, z0=None, psi=None, r_cavity=None, r_taper=None,
         q_taper=None, z_func=None, mstar=1.0, dist=100., resample=1,
         beam_spacing=False, r_min=None, r_max=None, PA_min=None, PA_max=None,
         exclude_PA=None, abs_PA=False, mask_frame='disk', mask=None,
         unit='Jy/beam', shadowed=False, skip_empty_annuli=True,
-        empirical_uncertainty=False):
+        empirical_uncertainty=False, vrad_func=None):
         """
         Return shifted and stacked spectra, over a given spatial region in the
         disk. The averaged spectra can be rescaled by using the ``unit``
         argument for which the possible units are:
 
             - ``'mJy/beam'``
             - ``'Jy/beam'``
@@ -1193,17 +1214,25 @@
             z0=z0,
             psi=psi,
             r_cavity=r_cavity,
             r_taper=r_taper,
             q_taper=q_taper,
             z_func=z_func
             )
-
         v_kep = np.atleast_1d(v_kep)
 
+        # Radial velocity at the annulus centers. Note that positive v_rad are
+        # moving away from the disk center.
+
+        if vrad_func is None:
+            v_rad = np.zeros(v_kep.shape)
+        else:
+            v_rad = vrad_func(rvals)
+        assert v_rad.shape == v_kep.shape
+
         # Output unit.
 
         unit = unit.lower()
         if unit not in ['mjy/beam', 'jy/beam', 'jy', 'mjy', 'mk', 'k']:
             raise ValueError("Unknown `unit`.")
         if resample < 1.0 and self.verbose:
             print('WARNING: `resample < 1`, are you sure you want channels '
@@ -1250,14 +1279,15 @@
                     abs_PA=abs_PA,
                     mask_frame=mask_frame,
                     shadowed=shadowed
                     )
 
                 x, y, dy = annulus.deprojected_spectrum(
                     vrot=v_kep[ridx],
+                    vrad=v_rad[ridx],
                     resample=resample,
                     scatter=True
                     )
 
             # Complain if no spectra are found in the annulus.
 
             except ValueError:
@@ -2859,15 +2889,15 @@
         elif coord_type_out.lower() == 'cylindrical':
             return np.hypot(x_disk, y_disk), np.arctan2(y_disk, x_disk)
         else:
             message = "`coord_type_out` must be 'cartesian' or 'cylindrical'."
             raise ValueError(message)
 
     def disk_to_sky(self, coords, inc, PA, x0=0.0, y0=0.0,
-                    coord_type='cartesian', return_idx=False):
+                    coord_type='cylindrical', return_idx=False):
         """
         Project disk-frame coordinates onto the sky plane. Can return either
         the coordinates (the default return), useful for plotting, or the
         pixel indices (if ``return_idx=True``) which can be used to extract a
         spectrum at a particular location.
 
         Args:
@@ -3874,15 +3904,15 @@
     def plot_teardrop(self, inc, PA, mstar, dist, ax=None, rvals=None,
                       rbins=None, dr=None, x0=0.0, y0=0.0, z0=None, psi=None,
                       r_cavity=None, r_taper=None, q_taper=None, z_func=None,
                       resample=1, beam_spacing=False,
                       r_min=None, r_max=None, PA_min=None, PA_max=None,
                       exclude_PA=False, abs_PA=False, mask_frame='disk',
                       mask=None, unit='Jy/beam', pcolormesh_kwargs=None,
-                      shadowed=False):
+                      shadowed=False, vrad_func=None):
         """
         Make a `teardrop` plot. For argument descriptions see
         ``radial_spectra``. For all properties related to ``pcolormesh``,
         include them in ``pcolormesh_kwargs`` as a dictionary, e.g.
 
             pcolormesh_kwargs = dict(cmap='inferno', vmin=0.0, vmax=1.0)
 
@@ -3895,15 +3925,15 @@
                                   r_cavity=r_cavity, r_taper=r_taper,
                                   q_taper=q_taper, z_func=z_func, mstar=mstar,
                                   dist=dist, resample=resample,
                                   beam_spacing=beam_spacing, r_min=r_min,
                                   r_max=r_max, PA_min=PA_min, PA_max=PA_max,
                                   exclude_PA=exclude_PA, abs_PA=abs_PA,
                                   mask_frame=mask_frame, mask=mask, unit=unit,
-                                  shadowed=shadowed)
+                                  shadowed=shadowe, vrad_func=vrad_func)
         rvals, velax, spectra, scatter = out
 
         # Generate the axes.
         if ax is None:
             fig, ax = plt.subplots()
 
         # Plot the figure.
```

### Comparing `gofish-1.6.3/setup.py` & `gofish-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="gofish",
-    version="1.6.3",
+    version="1.6.4",
     author="Richard Teague",
     author_email="rteague@mit.edu",
     description="Fishing for molecular line emission in protoplanetary disks.",
     url="https://github.com/richteague/gofish",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

