# Comparing `tmp/rescupybs-0.0.1.3.1-py3-none-any.whl.zip` & `tmp/rescupybs-0.0.1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8365 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx       31 b- defN 23-Mar-30 19:51 rescupybs/__init__.py
--rwxrwxrwx  2.0 unx     8199 b- defN 23-Mar-30 05:50 rescupybs/functions.py
--rwxrwxrwx  2.0 unx     6759 b- defN 23-Mar-30 19:51 rescupybs/plots.py
+Zip file size: 8382 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx       31 b- defN 23-Mar-31 04:02 rescupybs/__init__.py
+-rwxrwxrwx  2.0 unx     8230 b- defN 23-Apr-04 03:16 rescupybs/functions.py
+-rwxrwxrwx  2.0 unx     6786 b- defN 23-Mar-31 04:58 rescupybs/plots.py
 -rwxrwxrwx  2.0 unx    10461 b- defN 23-Mar-30 05:33 rescupybs/wrapper.py
--rwxrwxrwx  2.0 unx     1060 b- defN 23-Mar-30 20:03 rescupybs-0.0.1.3.1.dist-info/LICENSE
--rwxrwxrwx  2.0 unx     1858 b- defN 23-Mar-30 20:03 rescupybs-0.0.1.3.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Mar-30 20:03 rescupybs-0.0.1.3.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       53 b- defN 23-Mar-30 20:03 rescupybs-0.0.1.3.1.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       10 b- defN 23-Mar-30 20:03 rescupybs-0.0.1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      825 b- defN 23-Mar-30 20:03 rescupybs-0.0.1.3.1.dist-info/RECORD
-10 files, 29348 bytes uncompressed, 6951 bytes compressed:  76.3%
+-rwxrwxrwx  2.0 unx     1060 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/LICENSE
+-rwxrwxrwx  2.0 unx     1858 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       53 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      825 b- defN 23-Apr-09 23:16 rescupybs-0.0.1.3.2.dist-info/RECORD
+10 files, 29406 bytes uncompressed, 6968 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: rescupybs/plots.py
 Comment: 
 
 Filename: rescupybs/wrapper.py
 Comment: 
 
-Filename: rescupybs-0.0.1.3.1.dist-info/LICENSE
+Filename: rescupybs-0.0.1.3.2.dist-info/LICENSE
 Comment: 
 
-Filename: rescupybs-0.0.1.3.1.dist-info/METADATA
+Filename: rescupybs-0.0.1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: rescupybs-0.0.1.3.1.dist-info/WHEEL
+Filename: rescupybs-0.0.1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: rescupybs-0.0.1.3.1.dist-info/entry_points.txt
+Filename: rescupybs-0.0.1.3.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.3.1.dist-info/top_level.txt
+Filename: rescupybs-0.0.1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: rescupybs-0.0.1.3.1.dist-info/RECORD
+Filename: rescupybs-0.0.1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rescupybs/__init__.py

```diff
@@ -1,3 +1,3 @@
 
-__version__ = "0.0.1.3.1"
+__version__ = "0.0.1.3.2"
```

## rescupybs/functions.py

```diff
@@ -133,25 +133,25 @@
         str1 = lines[4].split()
         vbm_cbm = [[int(str0[0]), int(str0[2])], [int(str1[0]), int(str1[2])]]
     else:
         str = lines[3].split()
         vbm_cbm = [[int(str[0]), int(str[2])]]
     return chpts, labels, vbm_cbm
 
-def ismetal(eigenvalues):
-    issemi = np.all(eigenvalues < 0.0, axis=0)
-    issemi = np.logical_or(issemi, np.all(eigenvalues > 0.0, axis=0) )
+def ismetal(eigenvalues_s):
+    issemi = np.all(eigenvalues_s < 0.0, axis=0)
+    issemi = np.logical_or(issemi, np.all(eigenvalues_s > 0.0, axis=0) )
     return not np.all(issemi)
 
-def get_vbm_cbm(eigenvalues):
-    max = np.max(eigenvalues[eigenvalues < 0.0])
-    min = np.min(eigenvalues[eigenvalues > 0.0])
-    i, vb = np.where(eigenvalues==max)
-    i, cb = np.where(eigenvalues==min)
-    return int(vb), max, int(cb), min
+def get_vbm_cbm(eigenvalues_s):
+    max = np.max(eigenvalues_s[eigenvalues_s < 0.0])
+    min = np.min(eigenvalues_s[eigenvalues_s > 0.0])
+    i, vb = np.where(eigenvalues_s==max)
+    i, cb = np.where(eigenvalues_s==min)
+    return vb[0], max, cb[0], min
 
 def isosurfaces_wf(input, kpt, band, spin):
     calc = TotalEnergy.read(input)
     output = input.rsplit('.', 1)[0]+'_'+str(kpt)+'_'+str(band)+'_'+str(spin)+'.vasp'
     pbc = [1, 1, 1]
     positions = calc.system.atoms.positions
     cell = calc.system.cell.avec
@@ -173,12 +173,12 @@
     fld = np.asfortranarray(fld)
     fld = fld / ureg.bohr**1.5
     fld = fld[::2, :] + 1j * fld[1::2, :]
     fld.ito("angstrom ** -1.5")
     fld = fld[..., band].magnitude
     f_abs = np.abs(fld)
     f_div = np.where(np.abs(np.angle(fld)) < np.pi / 2, f_abs, -f_abs)
-    f_div = np.reshape(f_div, (3,-1), order='F').T
+    f_div = np.reshape(f_div, (f_div.shape[-1], -1), order='F').T
     with open(output, "a") as f:
         f.writelines(['\n']+[str(i)+' ' for i in grid]+['\n'])
         np.savetxt(f, f_div)
```

## rescupybs/plots.py

```diff
@@ -18,15 +18,15 @@
     plt.legend(legend, frameon=False, prop={'size':'medium'}, loc=location)
     plt.savefig(EXPORT, dpi=750, transparent=True, bbox_inches='tight')
 
 def Mnispin(EXPORT, figsize, vertical, eigenvalues, chpts, labels, vbm_cbm, linestyle, linewidth):
     plt.figure(figsize=figsize)
     VBM, CBM = vbm_cbm[0]
     org = plt.plot(eigenvalues[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    fig = plt.plot(eigenvalues[0,:,VBM-5:CBM+6], linewidth=linewidth[0]*2, linestyle='-.')
+    fig = plt.plot(eigenvalues[0,:,VBM-5:CBM+6], linewidth=linewidth[0]*1.5, linestyle=(0, (3, 1)))
     plt.xlim(chpts[0],chpts[-1])
     plt.ylim(vertical)
     plt.ylabel('Energy (eV)')
     plt.xticks(chpts,labels)
     if len(chpts) > 2:
         for i in chpts[1:-1]:
             plt.axvline(i, linewidth=0.4, linestyle='-.', c='gray')
@@ -104,17 +104,17 @@
     if len(linestyle) == 1:
         linestyle = [linestyle[0], linestyle[0]]
     if len(linewidth) == 1:
         linewidth = [linewidth[0], linewidth[0]]
     VBM_up, CBM_up = vbm_cbm[0]
     VBM_do, CBM_do = vbm_cbm[1]
     p_up_o = ax1.plot(eigenvalues[0], linewidth=linewidth[0], linestyle=linestyle[0])
-    p_up_f = ax1.plot(eigenvalues[0,:,VBM_up-5:CBM_up+6], linewidth=linewidth[0]*2, linestyle='-.')
+    p_up_f = ax1.plot(eigenvalues[0,:,VBM_up-5:CBM_up+6], linewidth=linewidth[0]*1.5, linestyle=(0, (3, 1)))
     p_do_o = ax2.plot(eigenvalues[1], linewidth=linewidth[1], linestyle=linestyle[1])
-    p_do_f = ax2.plot(eigenvalues[1,:,VBM_do-5:CBM_do+6], linewidth=linewidth[1]*2, linestyle='-.')
+    p_do_f = ax2.plot(eigenvalues[1,:,VBM_do-5:CBM_do+6], linewidth=linewidth[1]*1.5, linestyle=(0, (3, 1)))
     ax1.legend(p_up_f, range(VBM_up-5, CBM_up+6), frameon=False, prop={'size':'medium'}, alignment='left', title="up", title_fontproperties={'style':'italic', 'size':'medium'}, loc='center right')
     ax2.legend(p_do_f, range(VBM_do-5, CBM_do+6), frameon=False, prop={'size':'medium'}, alignment='left', title="down", title_fontproperties={'style':'italic', 'size':'medium'}, loc='center right')
     ax1.tick_params(axis='y', which='minor', color='gray')
     ax2.tick_params(axis='y', which='minor', color='gray')
     ax1.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.axhline(linewidth=0.4, linestyle='-.', c='gray')
     ax2.set_yticklabels([])
```

## Comparing `rescupybs-0.0.1.3.1.dist-info/LICENSE` & `rescupybs-0.0.1.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rescupybs-0.0.1.3.1.dist-info/METADATA` & `rescupybs-0.0.1.3.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rescupybs
-Version: 0.0.1.3.1
+Version: 0.0.1.3.2
 Summary: Band structure plot from rescuplus json file.
 Home-page: https://github.com/lkccrr/rescupybs
 Author: kan
 Author-email: luokan@hrbeu.edu.cn
 License: MIT
 Keywords: DFT rescuplus band plot
 Platform: Unix
```

## Comparing `rescupybs-0.0.1.3.1.dist-info/RECORD` & `rescupybs-0.0.1.3.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-rescupybs/__init__.py,sha256=18qASy8ivN34SNr7JlZc5xfEVMSzoxX0tX5xupezVUY,31
-rescupybs/functions.py,sha256=kYdO-bf2wXsQAbiqnfOKWhyyfs1ER9CcriS4xADOSl8,8199
-rescupybs/plots.py,sha256=kkuTLsWFiaO-fR_DlIsjfS7BpJBSoWJs5He5S5gUQIE,6759
+rescupybs/__init__.py,sha256=cTmFF1WqPMbeqRNUHztB-QeJOqsFzpIP7dbrWJwHEPE,31
+rescupybs/functions.py,sha256=70LXS_a3LjzIfxYNgFokskikZOIIdm_FIPsyr0rJIfk,8230
+rescupybs/plots.py,sha256=5_7__zep7lgbxNqw-UZ_Nm2h4uSbtjCbeqB9g3FHLoM,6786
 rescupybs/wrapper.py,sha256=275oEos1nyUX-A9PgTXw6ruOmXELpaF7w-qSEKOzweE,10461
-rescupybs-0.0.1.3.1.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
-rescupybs-0.0.1.3.1.dist-info/METADATA,sha256=bfepRdsdc-5eymdrshdQv1Co4FEQkzodT98WT2RA9s8,1858
-rescupybs-0.0.1.3.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rescupybs-0.0.1.3.1.dist-info/entry_points.txt,sha256=DUGWHtRnZ-6RuS6H2KaXmmQzv_teO2Ddmrq5Nq20e3g,53
-rescupybs-0.0.1.3.1.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
-rescupybs-0.0.1.3.1.dist-info/RECORD,,
+rescupybs-0.0.1.3.2.dist-info/LICENSE,sha256=aWH1yhtukPX_iihAaz4foL04PJNxgsrRPqp_iwxlTr0,1060
+rescupybs-0.0.1.3.2.dist-info/METADATA,sha256=tY37RnJLnI7GdMvebMgT1wnrNqp2zNcxCz8UqHU4TvE,1858
+rescupybs-0.0.1.3.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rescupybs-0.0.1.3.2.dist-info/entry_points.txt,sha256=DUGWHtRnZ-6RuS6H2KaXmmQzv_teO2Ddmrq5Nq20e3g,53
+rescupybs-0.0.1.3.2.dist-info/top_level.txt,sha256=w6nJZTS0VDiS0Ij6-ub0Pukls7j8IAjyKwWgA8JHPS4,10
+rescupybs-0.0.1.3.2.dist-info/RECORD,,
```

